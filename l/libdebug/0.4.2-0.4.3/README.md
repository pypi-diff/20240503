# Comparing `tmp/libdebug-0.4.2.tar.gz` & `tmp/libdebug-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdebug-0.4.2.tar", last modified: Tue Apr 30 22:01:29 2024, max compression
+gzip compressed data, was "libdebug-0.4.3.tar", last modified: Fri May  3 14:07:45 2024, max compression
```

## Comparing `libdebug-0.4.2.tar` & `libdebug-0.4.3.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.381147 libdebug-0.4.2/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1139 2024-04-18 06:52:12.000000 libdebug-0.4.2/LICENSE
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       43 2024-04-30 21:27:42.000000 libdebug-0.4.2/MANIFEST.in
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13690 2024-04-30 22:01:29.381147 libdebug-0.4.2/PKG-INFO
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10817 2024-04-30 21:25:54.000000 libdebug-0.4.2/README.md
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       72 2024-04-30 21:25:45.000000 libdebug-0.4.2/libdebug/__init__.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/architectures/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/__init__.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/architectures/amd64/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/amd64/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5227 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5107 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/architectures/amd64/amd64_ptrace_register_holder.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1573 2024-04-28 13:25:27.000000 libdebug-0.4.2/libdebug/architectures/amd64/amd64_stack_unwinder.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1668 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/ptrace_hardware_breakpoint_manager.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1196 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/ptrace_hardware_breakpoint_provider.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      612 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/ptrace_software_breakpoint_patcher.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1014 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/register_helper.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      629 2024-04-28 13:25:27.000000 libdebug-0.4.2/libdebug/architectures/stack_unwinding_manager.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      930 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/architectures/stack_unwinding_provider.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/builtin/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      147 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/builtin/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1754 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/builtin/antidebug_syscall_hook.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1959 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/builtin/pretty_print_syscall_hook.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/cffi/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1253 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_build.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1229 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_build_legacy.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11861 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_source.c
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11447 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_source_legacy.c
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      739 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/cffi/personality_cffi_build.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4006 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/cffi/ptrace_cffi_build.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14356 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/cffi/ptrace_cffi_source.c
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/data/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/data/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2621 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/data/breakpoint.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2178 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/data/memory_map.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5728 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/data/memory_view.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1870 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/data/register_holder.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1857 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/data/syscall_hook.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/interfaces/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/interfaces/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4639 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/interfaces/debugging_interface.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      370 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/interfaces/gdb_interface.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      873 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/interfaces/interface_helper.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      325 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/interfaces/interfaces.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    17683 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/interfaces/ptrace_interface.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    27309 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/libdebug.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4190 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/liblog.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/ptrace/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/ptrace/__init__.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/ptrace/jumpstart/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/ptrace/jumpstart/__init__.py
--rwxrwxr-x   0 gabriele  (1000) gabriele  (1000)    16080 2024-04-30 22:00:56.000000 libdebug-0.4.2/libdebug/ptrace/jumpstart/jumpstart
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      473 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/ptrace/jumpstart/jumpstart.c
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1937 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/ptrace/ptrace_constants.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8426 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/ptrace/ptrace_status_handler.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.377147 libdebug-0.4.2/libdebug/state/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/state/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10532 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/state/debugging_context.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3619 2024-04-30 21:25:45.000000 libdebug-0.4.2/libdebug/state/thread_context.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.381147 libdebug-0.4.2/libdebug/utils/
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/__init__.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3956 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/debugging_utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8540 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/elf_utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      728 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/gdb.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6267 2024-04-30 21:25:45.000000 libdebug-0.4.2/libdebug/utils/libcontext.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    13882 2024-04-30 21:25:45.000000 libdebug-0.4.2/libdebug/utils/pipe_manager.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      997 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/posix_spawn.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1804 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/process_utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1389 2024-04-18 06:52:12.000000 libdebug-0.4.2/libdebug/utils/register_utils.py
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2806 2024-04-30 21:25:54.000000 libdebug-0.4.2/libdebug/utils/syscall_utils.py
-drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-04-30 22:01:29.381147 libdebug-0.4.2/libdebug.egg-info/
--rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13690 2024-04-30 22:01:29.000000 libdebug-0.4.2/libdebug.egg-info/PKG-INFO
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2279 2024-04-30 22:01:29.000000 libdebug-0.4.2/libdebug.egg-info/SOURCES.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        1 2024-04-30 22:01:29.000000 libdebug-0.4.2/libdebug.egg-info/dependency_links.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       53 2024-04-30 22:01:29.000000 libdebug-0.4.2/libdebug.egg-info/requires.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        9 2024-04-30 22:01:29.000000 libdebug-0.4.2/libdebug.egg-info/top_level.txt
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1736 2024-04-30 21:33:27.000000 libdebug-0.4.2/pyproject.toml
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       38 2024-04-30 22:01:29.381147 libdebug-0.4.2/setup.cfg
--rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2747 2024-04-30 22:01:21.000000 libdebug-0.4.2/setup.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1139 2024-05-01 23:50:33.000000 libdebug-0.4.3/LICENSE
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       43 2024-05-03 14:06:24.000000 libdebug-0.4.3/MANIFEST.in
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13654 2024-05-03 14:07:45.668930 libdebug-0.4.3/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10781 2024-05-03 14:06:31.000000 libdebug-0.4.3/README.md
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.664930 libdebug-0.4.3/libdebug/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       72 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.664930 libdebug-0.4.3/libdebug/architectures/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.664930 libdebug-0.4.3/libdebug/architectures/amd64/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/amd64/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5227 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5107 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/amd64/amd64_ptrace_register_holder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1573 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/architectures/amd64/amd64_stack_unwinder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1668 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/architectures/ptrace_hardware_breakpoint_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1196 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/ptrace_hardware_breakpoint_provider.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      612 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/ptrace_software_breakpoint_patcher.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1014 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/register_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      629 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/architectures/stack_unwinding_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      930 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/architectures/stack_unwinding_provider.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.664930 libdebug-0.4.3/libdebug/builtin/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      147 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/builtin/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1754 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/builtin/antidebug_syscall_hook.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1959 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/builtin/pretty_print_syscall_hook.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.664930 libdebug-0.4.3/libdebug/cffi/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1253 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_build.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1229 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_build_legacy.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11861 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_source.c
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    11447 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_source_legacy.c
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      739 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/cffi/personality_cffi_build.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4006 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/cffi/ptrace_cffi_build.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    14353 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/cffi/ptrace_cffi_source.c
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/data/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/data/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2621 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/data/breakpoint.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2178 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/data/memory_map.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     5728 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/data/memory_view.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1870 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/data/register_holder.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1857 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/data/syscall_hook.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/interfaces/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/interfaces/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4639 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/interfaces/debugging_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      370 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/interfaces/gdb_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      873 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/interfaces/interface_helper.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      325 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/interfaces/interfaces.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    17683 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/interfaces/ptrace_interface.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    27309 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/libdebug.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     4190 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/liblog.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/ptrace/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/ptrace/__init__.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/ptrace/jumpstart/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/ptrace/jumpstart/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      473 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/ptrace/jumpstart/jumpstart.c
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1937 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/ptrace/ptrace_constants.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8426 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/ptrace/ptrace_status_handler.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/state/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/state/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    10532 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/state/debugging_context.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3619 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/state/thread_context.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug/utils/
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        0 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/__init__.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     3956 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/debugging_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     8540 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/elf_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      728 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/gdb.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     6267 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/utils/libcontext.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)    13882 2024-05-03 14:06:31.000000 libdebug-0.4.3/libdebug/utils/pipe_manager.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)      997 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/posix_spawn.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1804 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/process_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1389 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/register_utils.py
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2806 2024-05-01 23:50:33.000000 libdebug-0.4.3/libdebug/utils/syscall_utils.py
+drwxrwxr-x   0 gabriele  (1000) gabriele  (1000)        0 2024-05-03 14:07:45.668930 libdebug-0.4.3/libdebug.egg-info/
+-rw-r--r--   0 gabriele  (1000) gabriele  (1000)    13654 2024-05-03 14:07:45.000000 libdebug-0.4.3/libdebug.egg-info/PKG-INFO
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2243 2024-05-03 14:07:45.000000 libdebug-0.4.3/libdebug.egg-info/SOURCES.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        1 2024-05-03 14:07:45.000000 libdebug-0.4.3/libdebug.egg-info/dependency_links.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       53 2024-05-03 14:07:45.000000 libdebug-0.4.3/libdebug.egg-info/requires.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)        9 2024-05-03 14:07:45.000000 libdebug-0.4.3/libdebug.egg-info/top_level.txt
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     1736 2024-05-03 14:06:31.000000 libdebug-0.4.3/pyproject.toml
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)       38 2024-05-03 14:07:45.668930 libdebug-0.4.3/setup.cfg
+-rw-rw-r--   0 gabriele  (1000) gabriele  (1000)     2747 2024-05-03 14:06:31.000000 libdebug-0.4.3/setup.py
```

### Comparing `libdebug-0.4.2/LICENSE` & `libdebug-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/PKG-INFO` & `libdebug-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdebug
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python library for the debugging of binary executables.
 Author: JinBlack, Io_no, MrIndeciso, Frank01001, MarcoDige
 License: MIT License
         
         Copyright (c) 2023 - 2024 Mario Polino, Gabriele Digregorio, Roberto Bertolini, 
         Francesco Panebianco.
         
@@ -59,15 +59,15 @@
 Requires-Dist: rich; extra == "dev"
 
 # libdebug
 libdebug is a Python library to automate the debugging of a binary executable.
 
 ## Installation
 ```bash
-python3 -m pip install git+https://github.com/libdebug/libdebug.git
+python3 -m pip install libdebug
 ```
 PyPy3 is supported but not recommended, as it performs worse on most of our tests.
 
 ### Installation Requirements:
 Ubuntu: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Debian: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Fedora: `sudo dnf install -y python3 python3-devel kernel-devel binutils-devel libdwarf-devel`
```

### Comparing `libdebug-0.4.2/README.md` & `libdebug-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # libdebug
 libdebug is a Python library to automate the debugging of a binary executable.
 
 ## Installation
 ```bash
-python3 -m pip install git+https://github.com/libdebug/libdebug.git
+python3 -m pip install libdebug
 ```
 PyPy3 is supported but not recommended, as it performs worse on most of our tests.
 
 ### Installation Requirements:
 Ubuntu: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Debian: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Fedora: `sudo dnf install -y python3 python3-devel kernel-devel binutils-devel libdwarf-devel`
```

### Comparing `libdebug-0.4.2/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py` & `libdebug-0.4.3/libdebug/architectures/amd64/amd64_ptrace_hw_bp_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/amd64/amd64_ptrace_register_holder.py` & `libdebug-0.4.3/libdebug/architectures/amd64/amd64_ptrace_register_holder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/amd64/amd64_stack_unwinder.py` & `libdebug-0.4.3/libdebug/architectures/amd64/amd64_stack_unwinder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/ptrace_hardware_breakpoint_manager.py` & `libdebug-0.4.3/libdebug/architectures/ptrace_hardware_breakpoint_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/ptrace_hardware_breakpoint_provider.py` & `libdebug-0.4.3/libdebug/architectures/ptrace_hardware_breakpoint_provider.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/ptrace_software_breakpoint_patcher.py` & `libdebug-0.4.3/libdebug/architectures/ptrace_software_breakpoint_patcher.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/register_helper.py` & `libdebug-0.4.3/libdebug/architectures/register_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/stack_unwinding_manager.py` & `libdebug-0.4.3/libdebug/architectures/stack_unwinding_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/architectures/stack_unwinding_provider.py` & `libdebug-0.4.3/libdebug/architectures/stack_unwinding_provider.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/builtin/antidebug_syscall_hook.py` & `libdebug-0.4.3/libdebug/builtin/antidebug_syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/builtin/pretty_print_syscall_hook.py` & `libdebug-0.4.3/libdebug/builtin/pretty_print_syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_build.py` & `libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_build_legacy.py` & `libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_build_legacy.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_source.c` & `libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_source.c`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/debug_sym_cffi_source_legacy.c` & `libdebug-0.4.3/libdebug/cffi/debug_sym_cffi_source_legacy.c`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/personality_cffi_build.py` & `libdebug-0.4.3/libdebug/cffi/personality_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/ptrace_cffi_build.py` & `libdebug-0.4.3/libdebug/cffi/ptrace_cffi_build.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/cffi/ptrace_cffi_source.c` & `libdebug-0.4.3/libdebug/cffi/ptrace_cffi_source.c`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         if (t->tid != head->tid) {
             // If GETREGS succeeds, the thread is already stopped, so we must
             // not "stop" it again
             if (ptrace(PTRACE_GETREGS, t->tid, NULL, &t->regs) == -1) {
                 // Stop the thread with a SIGSTOP
                 tgkill(pid, t->tid, SIGSTOP);
                 // Wait for the thread to stop
-                temp_tid = waitpid(t->tid, &temp_status, NULL);
+                temp_tid = waitpid(t->tid, &temp_status, 0);
 
                 // Register the status of the thread, as it might contain useful
                 // information
                 struct thread_status *ts = malloc(sizeof(struct thread_status));
                 ts->tid = temp_tid;
                 ts->status = temp_status;
                 ts->next = head;
```

### Comparing `libdebug-0.4.2/libdebug/data/breakpoint.py` & `libdebug-0.4.3/libdebug/data/breakpoint.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/data/memory_map.py` & `libdebug-0.4.3/libdebug/data/memory_map.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/data/memory_view.py` & `libdebug-0.4.3/libdebug/data/memory_view.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/data/register_holder.py` & `libdebug-0.4.3/libdebug/data/register_holder.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/data/syscall_hook.py` & `libdebug-0.4.3/libdebug/data/syscall_hook.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/interfaces/debugging_interface.py` & `libdebug-0.4.3/libdebug/interfaces/debugging_interface.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/interfaces/interface_helper.py` & `libdebug-0.4.3/libdebug/interfaces/interface_helper.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/interfaces/ptrace_interface.py` & `libdebug-0.4.3/libdebug/interfaces/ptrace_interface.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/libdebug.py` & `libdebug-0.4.3/libdebug/libdebug.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/liblog.py` & `libdebug-0.4.3/libdebug/liblog.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/ptrace/ptrace_constants.py` & `libdebug-0.4.3/libdebug/ptrace/ptrace_constants.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/ptrace/ptrace_status_handler.py` & `libdebug-0.4.3/libdebug/ptrace/ptrace_status_handler.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/state/debugging_context.py` & `libdebug-0.4.3/libdebug/state/debugging_context.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/state/thread_context.py` & `libdebug-0.4.3/libdebug/state/thread_context.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/debugging_utils.py` & `libdebug-0.4.3/libdebug/utils/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/elf_utils.py` & `libdebug-0.4.3/libdebug/utils/elf_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/gdb.py` & `libdebug-0.4.3/libdebug/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/libcontext.py` & `libdebug-0.4.3/libdebug/utils/libcontext.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/pipe_manager.py` & `libdebug-0.4.3/libdebug/utils/pipe_manager.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/posix_spawn.py` & `libdebug-0.4.3/libdebug/utils/posix_spawn.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/process_utils.py` & `libdebug-0.4.3/libdebug/utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/register_utils.py` & `libdebug-0.4.3/libdebug/utils/register_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug/utils/syscall_utils.py` & `libdebug-0.4.3/libdebug/utils/syscall_utils.py`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/libdebug.egg-info/PKG-INFO` & `libdebug-0.4.3/libdebug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdebug
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python library for the debugging of binary executables.
 Author: JinBlack, Io_no, MrIndeciso, Frank01001, MarcoDige
 License: MIT License
         
         Copyright (c) 2023 - 2024 Mario Polino, Gabriele Digregorio, Roberto Bertolini, 
         Francesco Panebianco.
         
@@ -59,15 +59,15 @@
 Requires-Dist: rich; extra == "dev"
 
 # libdebug
 libdebug is a Python library to automate the debugging of a binary executable.
 
 ## Installation
 ```bash
-python3 -m pip install git+https://github.com/libdebug/libdebug.git
+python3 -m pip install libdebug
 ```
 PyPy3 is supported but not recommended, as it performs worse on most of our tests.
 
 ### Installation Requirements:
 Ubuntu: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Debian: `sudo apt install -y python3 python3-dev libdwarf-dev libelf-dev libiberty-dev linux-headers-generic libc6-dbg`
 Fedora: `sudo dnf install -y python3 python3-devel kernel-devel binutils-devel libdwarf-devel`
```

### Comparing `libdebug-0.4.2/libdebug.egg-info/SOURCES.txt` & `libdebug-0.4.3/libdebug.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 libdebug/interfaces/interface_helper.py
 libdebug/interfaces/interfaces.py
 libdebug/interfaces/ptrace_interface.py
 libdebug/ptrace/__init__.py
 libdebug/ptrace/ptrace_constants.py
 libdebug/ptrace/ptrace_status_handler.py
 libdebug/ptrace/jumpstart/__init__.py
-libdebug/ptrace/jumpstart/jumpstart
 libdebug/ptrace/jumpstart/jumpstart.c
 libdebug/state/__init__.py
 libdebug/state/debugging_context.py
 libdebug/state/thread_context.py
 libdebug/utils/__init__.py
 libdebug/utils/debugging_utils.py
 libdebug/utils/elf_utils.py
```

### Comparing `libdebug-0.4.2/pyproject.toml` & `libdebug-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdebug-0.4.2/setup.py` & `libdebug-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         outputs = build.get_outputs(self)
         outputs.append("libdebug/ptrace/jumpstart/jumpstart")
         return outputs
 
 
 setup(
     name="libdebug",
-    version="0.4.2",
+    version="0.4.3",
     description="A library to debug binary programs",
     packages=find_packages(include=["libdebug", "libdebug.*"]),
     install_requires=["capstone", "pyelftools", "cffi", "requests", "psutil"],
     setup_requires=["cffi"],
     cffi_modules=[
         "./libdebug/cffi/ptrace_cffi_build.py:ffibuilder",
         "./libdebug/cffi/personality_cffi_build.py:ffibuilder",
```

