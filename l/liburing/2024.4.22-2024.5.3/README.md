# Comparing `tmp/liburing-2024.4.22.tar.gz` & `tmp/liburing-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liburing-2024.4.22.tar", last modified: Mon Apr 22 17:23:22 2024, max compression
+gzip compressed data, was "liburing-2024.5.3.tar", last modified: Fri May  3 16:42:14 2024, max compression
```

## Comparing `liburing-2024.4.22.tar` & `liburing-2024.5.3.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.724832 liburing-2024.4.22/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     7048 2020-02-25 13:24:03.000000 liburing-2024.4.22/LICENSE.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)      470 2024-04-07 19:00:27.000000 liburing-2024.4.22/MANIFEST.in
--rw-r--r--   0 stealth   (1000) stealth   (1000)    14847 2024-04-22 17:23:22.724832 liburing-2024.4.22/PKG-INFO
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5966 2024-04-22 17:22:42.000000 liburing-2024.4.22/README.rst
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.698166 liburing-2024.4.22/example/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2545 2024-02-13 18:58:50.000000 liburing-2024.4.22/example/open_write_read_close.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       55 2024-02-13 04:08:10.000000 liburing-2024.4.22/example/probe.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.694832 liburing-2024.4.22/libs/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.698166 liburing-2024.4.22/libs/liburing/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1050 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/LICENSE
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2727 2024-04-09 21:18:47.000000 liburing-2024.4.22/libs/liburing/Makefile
--rw-r--r--   0 stealth   (1000) stealth   (1000)      309 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/Makefile.common
--rw-r--r--   0 stealth   (1000) stealth   (1000)      237 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/Makefile.quiet
--rwxr-xr-x   0 stealth   (1000) stealth   (1000)    14335 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/configure
--rw-r--r--   0 stealth   (1000) stealth   (1000)      242 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/liburing-ffi.pc.in
--rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/liburing.pc.in
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1743 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/liburing.spec
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.701499 liburing-2024.4.22/libs/liburing/src/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4297 2024-04-09 21:18:47.000000 liburing-2024.4.22/libs/liburing/src/Makefile
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.701499 liburing-2024.4.22/libs/liburing/src/arch/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/arch/aarch64/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      734 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/aarch64/lib.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2857 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/aarch64/syscall.h
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/arch/generic/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      316 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/generic/lib.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2451 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/generic/syscall.h
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/arch/riscv64/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      756 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/riscv64/lib.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3082 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/riscv64/syscall.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2425 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/syscall-defs.h
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/arch/x86/
--rw-r--r--   0 stealth   (1000) stealth   (1000)      204 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/x86/lib.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     7227 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/arch/x86/syscall.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)      397 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/ffi.c
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/include/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.704832 liburing-2024.4.22/libs/liburing/src/include/liburing/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2495 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/include/liburing/barrier.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)    19614 2024-04-07 19:55:29.000000 liburing-2024.4.22/libs/liburing/src/include/liburing/io_uring.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)    45194 2024-04-18 06:05:05.000000 liburing-2024.4.22/libs/liburing/src/include/liburing.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)      183 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/int_flags.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1301 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/lib.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5039 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/liburing-ffi.map
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2070 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/liburing.map
--rw-r--r--   0 stealth   (1000) stealth   (1000)      987 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/nolibc.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)    10858 2024-04-09 21:18:47.000000 liburing-2024.4.22/libs/liburing/src/queue.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)     8698 2024-04-18 06:05:05.000000 liburing-2024.4.22/libs/liburing/src/register.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)    17820 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/setup.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/setup.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)      804 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/syscall.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1134 2024-03-31 00:15:28.000000 liburing-2024.4.22/libs/liburing/src/syscall.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)      414 2024-04-09 21:18:47.000000 liburing-2024.4.22/libs/liburing/src/version.c
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1872 2024-04-22 17:20:48.000000 liburing-2024.4.22/pyproject.toml
--rw-r--r--   0 stealth   (1000) stealth   (1000)       38 2024-04-22 17:23:22.724832 liburing-2024.4.22/setup.cfg
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2906 2024-04-22 17:20:20.000000 liburing-2024.4.22/setup.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.694832 liburing-2024.4.22/src/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.714832 liburing-2024.4.22/src/liburing/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-02-24 22:43:25.000000 liburing-2024.4.22/src/liburing/__init__.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)      495 2024-04-22 07:59:14.000000 liburing-2024.4.22/src/liburing/__init__.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       48 2024-04-18 09:30:08.000000 liburing-2024.4.22/src/liburing/_test.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1109 2024-04-21 08:19:46.000000 liburing-2024.4.22/src/liburing/_test.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4951 2024-04-12 01:25:52.000000 liburing-2024.4.22/src/liburing/common.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4083 2024-04-12 01:25:55.000000 liburing-2024.4.22/src/liburing/common.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)      272 2024-04-05 23:39:01.000000 liburing-2024.4.22/src/liburing/error.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1447 2024-04-05 23:39:38.000000 liburing-2024.4.22/src/liburing/error.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5761 2024-04-12 01:25:58.000000 liburing-2024.4.22/src/liburing/file.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     9068 2024-04-12 01:26:02.000000 liburing-2024.4.22/src/liburing/file.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2103 2024-04-09 06:51:42.000000 liburing-2024.4.22/src/liburing/futex.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5125 2024-04-09 06:51:39.000000 liburing-2024.4.22/src/liburing/futex.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)      181 2024-04-12 08:25:42.000000 liburing-2024.4.22/src/liburing/helper.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2102 2024-04-16 04:33:13.000000 liburing-2024.4.22/src/liburing/helper.pyx
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.714832 liburing-2024.4.22/src/liburing/include/
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.714832 liburing-2024.4.22/src/liburing/include/liburing/
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:04:01.000000 liburing-2024.4.22/src/liburing/include/liburing/barrier.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:04:00.000000 liburing-2024.4.22/src/liburing/include/liburing/compat.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:03:57.000000 liburing-2024.4.22/src/liburing/include/liburing/io_uring.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:03:59.000000 liburing-2024.4.22/src/liburing/include/liburing/io_uring_version.h
--rw-r--r--   0 stealth   (1000) stealth   (1000)      341 2024-04-22 17:04:02.000000 liburing-2024.4.22/src/liburing/include/liburing.h
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.718165 liburing-2024.4.22/src/liburing/lib/
--rw-r--r--   0 stealth   (1000) stealth   (1000)       63 2024-02-23 03:27:25.000000 liburing-2024.4.22/src/liburing/lib/__init__.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2161 2024-04-03 06:01:55.000000 liburing-2024.4.22/src/liburing/lib/file.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2276 2024-04-03 06:29:26.000000 liburing-2024.4.22/src/liburing/lib/futex.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)    24713 2024-04-12 08:39:32.000000 liburing-2024.4.22/src/liburing/lib/io_uring.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)      351 2024-03-26 22:05:44.000000 liburing-2024.4.22/src/liburing/lib/poll.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)    12270 2024-03-27 23:28:03.000000 liburing-2024.4.22/src/liburing/lib/socket.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5860 2024-03-26 22:30:12.000000 liburing-2024.4.22/src/liburing/lib/statx.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3979 2024-04-03 08:31:10.000000 liburing-2024.4.22/src/liburing/lib/type.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)    53874 2024-04-18 09:33:10.000000 liburing-2024.4.22/src/liburing/lib/uring.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3541 2024-03-28 04:31:56.000000 liburing-2024.4.22/src/liburing/os.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5656 2024-03-26 23:41:50.000000 liburing-2024.4.22/src/liburing/os.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2755 2024-03-28 05:43:54.000000 liburing-2024.4.22/src/liburing/other.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3635 2024-04-16 04:32:30.000000 liburing-2024.4.22/src/liburing/other.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1076 2024-03-16 01:03:17.000000 liburing-2024.4.22/src/liburing/poll.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1569 2024-03-16 01:06:50.000000 liburing-2024.4.22/src/liburing/poll.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)      504 2024-03-28 05:14:47.000000 liburing-2024.4.22/src/liburing/probe.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)      650 2024-03-01 06:44:03.000000 liburing-2024.4.22/src/liburing/probe.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1403 2024-04-16 04:32:30.000000 liburing-2024.4.22/src/liburing/probe.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     7267 2024-04-22 13:50:05.000000 liburing-2024.4.22/src/liburing/queue.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)    17056 2024-04-22 13:24:11.000000 liburing-2024.4.22/src/liburing/queue.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4041 2024-03-28 05:15:17.000000 liburing-2024.4.22/src/liburing/register.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     6633 2024-04-16 04:32:30.000000 liburing-2024.4.22/src/liburing/register.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)    10711 2024-04-12 01:28:38.000000 liburing-2024.4.22/src/liburing/socket.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)    20082 2024-04-12 01:28:43.000000 liburing-2024.4.22/src/liburing/socket.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1015 2024-03-28 05:16:50.000000 liburing-2024.4.22/src/liburing/socket_extra.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4388 2024-03-28 05:16:58.000000 liburing-2024.4.22/src/liburing/socket_extra.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2216 2024-03-28 05:17:18.000000 liburing-2024.4.22/src/liburing/statx.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     6674 2024-03-28 05:17:23.000000 liburing-2024.4.22/src/liburing/statx.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     6905 2024-04-12 01:28:46.000000 liburing-2024.4.22/src/liburing/syscall.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1151 2024-04-12 01:28:49.000000 liburing-2024.4.22/src/liburing/syscall.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1597 2024-04-22 12:23:18.000000 liburing-2024.4.22/src/liburing/time.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2492 2024-04-22 12:23:19.000000 liburing-2024.4.22/src/liburing/time.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)      340 2024-04-03 08:28:15.000000 liburing-2024.4.22/src/liburing/version.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1192 2024-04-03 08:29:45.000000 liburing-2024.4.22/src/liburing/version.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      544 2024-04-03 08:28:16.000000 liburing-2024.4.22/src/liburing/version.pyx
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1367 2024-03-03 06:46:36.000000 liburing-2024.4.22/src/liburing/xattr.pxd
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1598 2024-03-03 07:14:04.000000 liburing-2024.4.22/src/liburing/xattr.pyx
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.724832 liburing-2024.4.22/src/liburing.egg-info/
--rw-r--r--   0 stealth   (1000) stealth   (1000)    14847 2024-04-22 17:23:22.000000 liburing-2024.4.22/src/liburing.egg-info/PKG-INFO
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3620 2024-04-22 17:23:22.000000 liburing-2024.4.22/src/liburing.egg-info/SOURCES.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)        1 2024-04-22 17:23:22.000000 liburing-2024.4.22/src/liburing.egg-info/dependency_links.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)       30 2024-04-22 17:23:22.000000 liburing-2024.4.22/src/liburing.egg-info/requires.txt
--rw-r--r--   0 stealth   (1000) stealth   (1000)        9 2024-04-22 17:23:22.000000 liburing-2024.4.22/src/liburing.egg-info/top_level.txt
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.721499 liburing-2024.4.22/test/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2370 2024-04-03 08:36:54.000000 liburing-2024.4.22/test/conftest.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1103 2024-03-14 16:24:01.000000 liburing-2024.4.22/test/error_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.721499 liburing-2024.4.22/test/file/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5225 2024-03-23 23:11:53.000000 liburing-2024.4.22/test/file/file_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4385 2024-03-07 13:50:23.000000 liburing-2024.4.22/test/file/open_close_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      428 2024-02-09 00:25:55.000000 liburing-2024.4.22/test/file/open_how_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     5188 2024-04-03 08:18:47.000000 liburing-2024.4.22/test/futex_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.721499 liburing-2024.4.22/test/helper/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1168 2024-04-19 06:00:23.000000 liburing-2024.4.22/test/helper/io_uring_put_sqe_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1430 2024-02-24 00:07:21.000000 liburing-2024.4.22/test/iovec_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.721499 liburing-2024.4.22/test/lib/
--rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-03-26 21:50:01.000000 liburing-2024.4.22/test/lib/file_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1584 2024-04-03 08:18:20.000000 liburing-2024.4.22/test/lib/futex_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)    12004 2024-04-03 06:35:48.000000 liburing-2024.4.22/test/lib/io_uring_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)       77 2024-03-26 22:06:30.000000 liburing-2024.4.22/test/lib/poll_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4180 2024-03-26 23:30:17.000000 liburing-2024.4.22/test/lib/socket_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2390 2024-03-26 22:10:51.000000 liburing-2024.4.22/test/lib/statx_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1093 2024-04-03 08:38:15.000000 liburing-2024.4.22/test/lib/type_define_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      111 2024-03-28 03:58:21.000000 liburing-2024.4.22/test/lib/uring_define_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.721499 liburing-2024.4.22/test/os/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1387 2024-03-23 22:30:21.000000 liburing-2024.4.22/test/os/splice_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3528 2024-03-06 09:51:18.000000 liburing-2024.4.22/test/os/unlink_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      879 2024-02-29 00:01:02.000000 liburing-2024.4.22/test/probe_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.724832 liburing-2024.4.22/test/queue/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     2741 2024-04-20 02:21:55.000000 liburing-2024.4.22/test/queue/init_exit_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1834 2024-04-19 06:01:18.000000 liburing-2024.4.22/test/queue/macro_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1761 2024-04-21 08:07:48.000000 liburing-2024.4.22/test/queue/sqe_cqe_test.py
-drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-04-22 17:23:22.724832 liburing-2024.4.22/test/socket/
--rw-r--r--   0 stealth   (1000) stealth   (1000)     4514 2024-03-12 19:49:40.000000 liburing-2024.4.22/test/socket/cmd_sock_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      708 2024-03-15 17:59:06.000000 liburing-2024.4.22/test/socket/getaddinfo_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      698 2024-03-14 19:27:18.000000 liburing-2024.4.22/test/socket/getnameinfo_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1490 2024-03-14 18:29:13.000000 liburing-2024.4.22/test/socket/getsockname_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     3914 2024-04-22 17:08:26.000000 liburing-2024.4.22/test/socket/socket_connect_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1181 2024-04-10 09:02:07.000000 liburing-2024.4.22/test/statx_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      119 2024-03-01 08:26:52.000000 liburing-2024.4.22/test/syscall_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)      405 2024-03-26 22:03:19.000000 liburing-2024.4.22/test/time_test.py
--rw-r--r--   0 stealth   (1000) stealth   (1000)     1071 2024-04-04 00:17:53.000000 liburing-2024.4.22/test/version_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.576114 liburing-2024.5.3/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     7048 2020-02-25 13:24:03.000000 liburing-2024.5.3/LICENSE.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      470 2024-04-22 20:51:12.000000 liburing-2024.5.3/MANIFEST.in
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    14846 2024-05-03 16:42:14.576114 liburing-2024.5.3/PKG-INFO
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5966 2024-04-30 20:50:21.000000 liburing-2024.5.3/README.rst
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.546115 liburing-2024.5.3/example/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2545 2024-02-13 18:58:50.000000 liburing-2024.5.3/example/open_write_read_close.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       55 2024-02-13 04:08:10.000000 liburing-2024.5.3/example/probe.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.542782 liburing-2024.5.3/libs/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.549448 liburing-2024.5.3/libs/liburing/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1050 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/LICENSE
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2727 2024-04-09 21:18:47.000000 liburing-2024.5.3/libs/liburing/Makefile
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      309 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/Makefile.common
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      237 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/Makefile.quiet
+-rwxr-xr-x   0 stealth   (1000) stealth   (1000)    14326 2024-04-26 16:58:29.000000 liburing-2024.5.3/libs/liburing/configure
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      242 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/liburing-ffi.pc.in
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/liburing.pc.in
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1743 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/liburing.spec
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4297 2024-04-09 21:18:47.000000 liburing-2024.5.3/libs/liburing/src/Makefile
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/arch/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/arch/aarch64/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      734 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/aarch64/lib.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2857 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/aarch64/syscall.h
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/arch/generic/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      316 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/generic/lib.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2451 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/generic/syscall.h
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/arch/riscv64/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      756 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/riscv64/lib.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3082 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/riscv64/syscall.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2425 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/syscall-defs.h
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/arch/x86/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      204 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/x86/lib.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     7227 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/arch/x86/syscall.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      397 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/ffi.c
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/include/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.552781 liburing-2024.5.3/libs/liburing/src/include/liburing/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2495 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/include/liburing/barrier.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    19614 2024-04-07 19:55:29.000000 liburing-2024.5.3/libs/liburing/src/include/liburing/io_uring.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    45194 2024-04-18 06:05:05.000000 liburing-2024.5.3/libs/liburing/src/include/liburing.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      183 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/int_flags.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1301 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/lib.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5039 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/liburing-ffi.map
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2070 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/liburing.map
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      987 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/nolibc.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    10858 2024-04-09 21:18:47.000000 liburing-2024.5.3/libs/liburing/src/queue.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     8698 2024-04-18 06:05:05.000000 liburing-2024.5.3/libs/liburing/src/register.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    17820 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/setup.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      234 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/setup.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      804 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/syscall.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1134 2024-03-31 00:15:28.000000 liburing-2024.5.3/libs/liburing/src/syscall.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      414 2024-04-09 21:18:47.000000 liburing-2024.5.3/libs/liburing/src/version.c
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1872 2024-05-03 16:37:45.000000 liburing-2024.5.3/pyproject.toml
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       38 2024-05-03 16:42:14.576114 liburing-2024.5.3/setup.cfg
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3012 2024-05-02 16:56:12.000000 liburing-2024.5.3/setup.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.542782 liburing-2024.5.3/src/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.562781 liburing-2024.5.3/src/liburing/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       60 2024-02-24 22:43:25.000000 liburing-2024.5.3/src/liburing/__init__.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      494 2024-05-03 16:36:00.000000 liburing-2024.5.3/src/liburing/__init__.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       48 2024-04-18 09:30:08.000000 liburing-2024.5.3/src/liburing/_test.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1109 2024-04-21 08:19:46.000000 liburing-2024.5.3/src/liburing/_test.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4951 2024-05-03 16:34:00.000000 liburing-2024.5.3/src/liburing/common.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4284 2024-05-03 16:33:57.000000 liburing-2024.5.3/src/liburing/common.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      272 2024-04-05 23:39:01.000000 liburing-2024.5.3/src/liburing/error.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1447 2024-04-05 23:39:38.000000 liburing-2024.5.3/src/liburing/error.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5763 2024-05-03 16:33:54.000000 liburing-2024.5.3/src/liburing/file.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     9315 2024-05-03 16:33:50.000000 liburing-2024.5.3/src/liburing/file.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2103 2024-05-03 16:33:47.000000 liburing-2024.5.3/src/liburing/futex.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5125 2024-05-03 16:33:44.000000 liburing-2024.5.3/src/liburing/futex.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      181 2024-04-12 08:25:42.000000 liburing-2024.5.3/src/liburing/helper.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2102 2024-04-16 04:33:13.000000 liburing-2024.5.3/src/liburing/helper.pyx
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.566115 liburing-2024.5.3/src/liburing/include/
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.566115 liburing-2024.5.3/src/liburing/include/liburing/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:33:34.000000 liburing-2024.5.3/src/liburing/include/liburing/barrier.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:33:32.000000 liburing-2024.5.3/src/liburing/include/liburing/compat.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:33:31.000000 liburing-2024.5.3/src/liburing/include/liburing/io_uring.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:33:30.000000 liburing-2024.5.3/src/liburing/include/liburing/io_uring_version.h
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      341 2024-05-03 16:33:35.000000 liburing-2024.5.3/src/liburing/include/liburing.h
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.566115 liburing-2024.5.3/src/liburing/lib/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       63 2024-02-23 03:27:25.000000 liburing-2024.5.3/src/liburing/lib/__init__.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2161 2024-04-03 06:01:55.000000 liburing-2024.5.3/src/liburing/lib/file.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2276 2024-04-03 06:29:26.000000 liburing-2024.5.3/src/liburing/lib/futex.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    24713 2024-04-12 08:39:32.000000 liburing-2024.5.3/src/liburing/lib/io_uring.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      351 2024-03-26 22:05:44.000000 liburing-2024.5.3/src/liburing/lib/poll.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    12270 2024-03-27 23:28:03.000000 liburing-2024.5.3/src/liburing/lib/socket.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5860 2024-03-26 22:30:12.000000 liburing-2024.5.3/src/liburing/lib/statx.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3979 2024-04-03 08:31:10.000000 liburing-2024.5.3/src/liburing/lib/type.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    53874 2024-05-03 16:39:29.000000 liburing-2024.5.3/src/liburing/lib/uring.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3541 2024-03-28 04:31:56.000000 liburing-2024.5.3/src/liburing/os.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5656 2024-03-26 23:41:50.000000 liburing-2024.5.3/src/liburing/os.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2755 2024-03-28 05:43:54.000000 liburing-2024.5.3/src/liburing/other.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3635 2024-04-16 04:32:30.000000 liburing-2024.5.3/src/liburing/other.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1076 2024-03-16 01:03:17.000000 liburing-2024.5.3/src/liburing/poll.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1569 2024-03-16 01:06:50.000000 liburing-2024.5.3/src/liburing/poll.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      504 2024-05-03 16:33:24.000000 liburing-2024.5.3/src/liburing/probe.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      650 2024-03-01 06:44:03.000000 liburing-2024.5.3/src/liburing/probe.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1403 2024-05-03 16:33:21.000000 liburing-2024.5.3/src/liburing/probe.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     7267 2024-05-03 16:33:18.000000 liburing-2024.5.3/src/liburing/queue.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    17085 2024-05-03 16:33:16.000000 liburing-2024.5.3/src/liburing/queue.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4041 2024-03-28 05:15:17.000000 liburing-2024.5.3/src/liburing/register.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     6633 2024-04-16 04:32:30.000000 liburing-2024.5.3/src/liburing/register.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    10711 2024-05-03 16:33:08.000000 liburing-2024.5.3/src/liburing/socket.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    20082 2024-05-03 16:33:04.000000 liburing-2024.5.3/src/liburing/socket.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1015 2024-03-28 05:16:50.000000 liburing-2024.5.3/src/liburing/socket_extra.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4388 2024-03-28 05:16:58.000000 liburing-2024.5.3/src/liburing/socket_extra.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2216 2024-05-03 16:32:46.000000 liburing-2024.5.3/src/liburing/statx.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     6665 2024-05-03 16:32:30.000000 liburing-2024.5.3/src/liburing/statx.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     6905 2024-04-12 01:28:46.000000 liburing-2024.5.3/src/liburing/syscall.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1151 2024-04-12 01:28:49.000000 liburing-2024.5.3/src/liburing/syscall.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1597 2024-05-03 16:32:34.000000 liburing-2024.5.3/src/liburing/time.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2492 2024-05-03 16:32:39.000000 liburing-2024.5.3/src/liburing/time.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      340 2024-04-03 08:28:15.000000 liburing-2024.5.3/src/liburing/version.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1192 2024-04-03 08:29:45.000000 liburing-2024.5.3/src/liburing/version.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      544 2024-04-03 08:28:16.000000 liburing-2024.5.3/src/liburing/version.pyx
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1367 2024-03-03 06:46:36.000000 liburing-2024.5.3/src/liburing/xattr.pxd
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1598 2024-03-03 07:14:04.000000 liburing-2024.5.3/src/liburing/xattr.pyx
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.576114 liburing-2024.5.3/src/liburing.egg-info/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    14846 2024-05-03 16:42:14.000000 liburing-2024.5.3/src/liburing.egg-info/PKG-INFO
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3620 2024-05-03 16:42:14.000000 liburing-2024.5.3/src/liburing.egg-info/SOURCES.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        1 2024-05-03 16:42:14.000000 liburing-2024.5.3/src/liburing.egg-info/dependency_links.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       30 2024-05-03 16:42:14.000000 liburing-2024.5.3/src/liburing.egg-info/requires.txt
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        9 2024-05-03 16:42:14.000000 liburing-2024.5.3/src/liburing.egg-info/top_level.txt
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.569448 liburing-2024.5.3/test/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2370 2024-04-03 08:36:54.000000 liburing-2024.5.3/test/conftest.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1103 2024-03-14 16:24:01.000000 liburing-2024.5.3/test/error_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.569448 liburing-2024.5.3/test/file/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5225 2024-03-23 23:11:53.000000 liburing-2024.5.3/test/file/file_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4385 2024-03-07 13:50:23.000000 liburing-2024.5.3/test/file/open_close_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      505 2024-04-25 09:02:44.000000 liburing-2024.5.3/test/file/open_how_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     5188 2024-04-03 08:18:47.000000 liburing-2024.5.3/test/futex_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.569448 liburing-2024.5.3/test/helper/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1168 2024-04-19 06:00:23.000000 liburing-2024.5.3/test/helper/io_uring_put_sqe_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1543 2024-04-27 23:56:45.000000 liburing-2024.5.3/test/iovec_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.572781 liburing-2024.5.3/test/lib/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)        0 2024-03-26 21:50:01.000000 liburing-2024.5.3/test/lib/file_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1584 2024-04-03 08:18:20.000000 liburing-2024.5.3/test/lib/futex_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)    12004 2024-04-27 22:12:38.000000 liburing-2024.5.3/test/lib/io_uring_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)       77 2024-03-26 22:06:30.000000 liburing-2024.5.3/test/lib/poll_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4180 2024-03-26 23:30:17.000000 liburing-2024.5.3/test/lib/socket_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2390 2024-03-26 22:10:51.000000 liburing-2024.5.3/test/lib/statx_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1093 2024-04-03 08:38:15.000000 liburing-2024.5.3/test/lib/type_define_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      111 2024-03-28 03:58:21.000000 liburing-2024.5.3/test/lib/uring_define_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.572781 liburing-2024.5.3/test/os/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1387 2024-03-23 22:30:21.000000 liburing-2024.5.3/test/os/splice_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3528 2024-03-06 09:51:18.000000 liburing-2024.5.3/test/os/unlink_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      879 2024-02-29 00:01:02.000000 liburing-2024.5.3/test/probe_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.572781 liburing-2024.5.3/test/queue/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     2741 2024-04-20 02:21:55.000000 liburing-2024.5.3/test/queue/init_exit_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1834 2024-04-19 06:01:18.000000 liburing-2024.5.3/test/queue/macro_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1761 2024-04-21 08:07:48.000000 liburing-2024.5.3/test/queue/sqe_cqe_test.py
+drwxr-xr-x   0 stealth   (1000) stealth   (1000)        0 2024-05-03 16:42:14.572781 liburing-2024.5.3/test/socket/
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     4514 2024-03-12 19:49:40.000000 liburing-2024.5.3/test/socket/cmd_sock_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      708 2024-03-15 17:59:06.000000 liburing-2024.5.3/test/socket/getaddinfo_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      698 2024-03-14 19:27:18.000000 liburing-2024.5.3/test/socket/getnameinfo_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1490 2024-03-14 18:29:13.000000 liburing-2024.5.3/test/socket/getsockname_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     3914 2024-04-22 17:08:26.000000 liburing-2024.5.3/test/socket/socket_connect_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1181 2024-04-10 09:02:07.000000 liburing-2024.5.3/test/statx_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      119 2024-03-01 08:26:52.000000 liburing-2024.5.3/test/syscall_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)      405 2024-03-26 22:03:19.000000 liburing-2024.5.3/test/time_test.py
+-rw-r--r--   0 stealth   (1000) stealth   (1000)     1071 2024-04-04 00:17:53.000000 liburing-2024.5.3/test/version_test.py
```

### Comparing `liburing-2024.4.22/LICENSE.txt` & `liburing-2024.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/PKG-INFO` & `liburing-2024.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liburing
-Version: 2024.4.22
+Version: 2024.5.3
 Summary: ...
 Author: Ritesh
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -166,15 +166,15 @@
     - Linux 6.1+ (6.7+ recommended)
     - Python 3.8+
 
 
 Includes (battery)
 ------------------
 
-    - C liburing 2.5+
+    - C liburing 2.6+
 
 
 Install, update & uninstall (Alpha)
 -----------------------------------
 
 Use `pip`_ to install, upgrade & uninstall Python wrapper:
```

### Comparing `liburing-2024.4.22/README.rst` & `liburing-2024.5.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     - Linux 6.1+ (6.7+ recommended)
     - Python 3.8+
 
 
 Includes (battery)
 ------------------
 
-    - C liburing 2.5+
+    - C liburing 2.6+
 
 
 Install, update & uninstall (Alpha)
 -----------------------------------
 
 Use `pip`_ to install, upgrade & uninstall Python wrapper:
```

### Comparing `liburing-2024.4.22/example/open_write_read_close.py` & `liburing-2024.5.3/example/open_write_read_close.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/LICENSE` & `liburing-2024.5.3/libs/liburing/LICENSE`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/Makefile` & `liburing-2024.5.3/libs/liburing/Makefile`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/configure` & `liburing-2024.5.3/libs/liburing/configure`

 * *Files 1% similar despite different names*

```diff
@@ -515,17 +515,17 @@
 print_config "CC" "$cc"
 echo "CXX=$cxx" >> $config_host_mak
 print_config "CXX" "$cxx"
 
 # generate io_uring_version.h
 # Reset MAKEFLAGS
 MAKEFLAGS=
-MAKE_PRINT_VARS="include Makefile.common\nprint-%: ; @echo \$(\$*)\n"
-VERSION_MAJOR=$(env echo -e "$MAKE_PRINT_VARS" | make -s --no-print-directory -f - print-VERSION_MAJOR)
-VERSION_MINOR=$(env echo -e "$MAKE_PRINT_VARS" | make -s --no-print-directory -f - print-VERSION_MINOR)
+MAKE_PRINT_VARS="include Makefile.common\nprint-%%: ; @echo \$(\$*)\n"
+VERSION_MAJOR=$(printf "$MAKE_PRINT_VARS" | make -s --no-print-directory -f - print-VERSION_MAJOR)
+VERSION_MINOR=$(printf "$MAKE_PRINT_VARS" | make -s --no-print-directory -f - print-VERSION_MINOR)
 io_uring_version_h="src/include/liburing/io_uring_version.h"
 cat > $io_uring_version_h << EOF
 /* SPDX-License-Identifier: MIT */
 #ifndef LIBURING_VERSION_H
 #define LIBURING_VERSION_H
 
 #define IO_URING_VERSION_MAJOR $VERSION_MAJOR
```

### Comparing `liburing-2024.4.22/libs/liburing/liburing.spec` & `liburing-2024.5.3/libs/liburing/liburing.spec`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/Makefile` & `liburing-2024.5.3/libs/liburing/src/Makefile`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/aarch64/lib.h` & `liburing-2024.5.3/libs/liburing/src/arch/aarch64/lib.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/aarch64/syscall.h` & `liburing-2024.5.3/libs/liburing/src/arch/aarch64/syscall.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/generic/syscall.h` & `liburing-2024.5.3/libs/liburing/src/arch/generic/syscall.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/riscv64/lib.h` & `liburing-2024.5.3/libs/liburing/src/arch/riscv64/lib.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/riscv64/syscall.h` & `liburing-2024.5.3/libs/liburing/src/arch/riscv64/syscall.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/syscall-defs.h` & `liburing-2024.5.3/libs/liburing/src/arch/syscall-defs.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/arch/x86/syscall.h` & `liburing-2024.5.3/libs/liburing/src/arch/x86/syscall.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/include/liburing/barrier.h` & `liburing-2024.5.3/libs/liburing/src/include/liburing/barrier.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/include/liburing/io_uring.h` & `liburing-2024.5.3/libs/liburing/src/include/liburing/io_uring.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/include/liburing.h` & `liburing-2024.5.3/libs/liburing/src/include/liburing.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/lib.h` & `liburing-2024.5.3/libs/liburing/src/lib.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/liburing-ffi.map` & `liburing-2024.5.3/libs/liburing/src/liburing-ffi.map`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/liburing.map` & `liburing-2024.5.3/libs/liburing/src/liburing.map`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/nolibc.c` & `liburing-2024.5.3/libs/liburing/src/nolibc.c`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/queue.c` & `liburing-2024.5.3/libs/liburing/src/queue.c`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/register.c` & `liburing-2024.5.3/libs/liburing/src/register.c`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/setup.c` & `liburing-2024.5.3/libs/liburing/src/setup.c`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/syscall.c` & `liburing-2024.5.3/libs/liburing/src/syscall.c`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/libs/liburing/src/syscall.h` & `liburing-2024.5.3/libs/liburing/src/syscall.h`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/pyproject.toml` & `liburing-2024.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/setup.py` & `liburing-2024.5.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os import cpu_count
-from shutil import copy2, copytree, rmtree
+from shutil import copy2, copytree
 from os.path import join
-from tempfile import mkdtemp
+from tempfile import TemporaryDirectory
 from subprocess import run as sub_process_run
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
 from Cython.Build import cythonize
 from Cython.Compiler import Options
 from Cython.Distutils import Extension
 
@@ -23,50 +23,47 @@
                     'libs/liburing/liburing.pc.in',
                     'libs/liburing/liburing.spec',
                     'libs/liburing/Makefile',
                     'libs/liburing/Makefile.common',
                     'libs/liburing/Makefile.quiet'):
             copy2(src, join(tmpdir, src))
 
-        # sub_process_run(['./configure', '--use-libc'], cwd=lib, capture_output=True, check=True)
+        # note: just runs `configure` & `make`, does not `install`.
         sub_process_run(['./configure'], cwd=lib, capture_output=True, check=True)
         sub_process_run(['make', f'--jobs={threads}'], cwd=lib, capture_output=True)
-        # note: just runs `configure` & `make`, does not `install`.
 
         # replace `include` placeholder files with actual content.
         copytree(libinc, 'src/liburing/include', dirs_exist_ok=True)
+        # have to replace `include` in `build_lib` e.g.'build/lib.linux-x86_64-cpython-313'
+        # as well since installer copies over the files before `BuildExt` is called. 
+        copytree(libinc, join(self.build_lib, 'liburing/include'), dirs_exist_ok=True)
         super().build_extensions()
 
 
 if __name__ == '__main__':
-    # uring = 'uring'
-    uring = 'uring-ffi'
-    tmpdir = mkdtemp()
-    threads = cpu_count()
     # compiler options
     Options.annotate = False
     Options.fast_fail = True
     Options.docstrings = True
     Options.warning_errors = False
 
-    try:
+    with TemporaryDirectory() as tmpdir:
         lib = join(tmpdir, 'libs/liburing')
         libsrc = join(lib, 'src')
         libinc = join(libsrc, 'include')
+        threads = cpu_count()
         extension = [Extension(name='liburing.*',  # where the `.so` will be saved.
                                sources=['src/liburing/*.pyx'],
                                language='c',
-                               libraries=[uring],
+                               libraries=['uring-ffi'],
                                library_dirs=[libsrc],
                                include_dirs=[libinc],
                                # optimize & remove debug symbols + data.
                                extra_compile_args=['-O3', '-g0'])]
         # install
         setup(cmdclass={'build_ext': BuildExt},
               ext_modules=cythonize(extension,
                                     nthreads=threads,
-                                    compiler_directives={'embedsignature': True,  # show `__doc__`
+                                    compiler_directives={'language_level': 3,
+                                                         'embedsignature': True,  # show `__doc__`
                                                          'boundscheck': False,
-                                                         'wraparound': False,
-                                                         'language_level': 3}))
-    finally:
-        rmtree(tmpdir)
+                                                         'wraparound': False}))
```

### Comparing `liburing-2024.4.22/src/liburing/_test.pyx` & `liburing-2024.5.3/src/liburing/_test.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/common.pxd` & `liburing-2024.5.3/src/liburing/common.pxd`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from cpython.mem cimport PyMem_RawCalloc, PyMem_RawFree
 from posix.unistd cimport _SC_IOV_MAX
+from cpython.mem cimport PyMem_RawCalloc, PyMem_RawFree
 from .lib.uring cimport *
 from .error cimport memory_error, index_error
 from .queue cimport io_uring_sqe
 
 
 cdef class iovec:
     cdef:
```

### Comparing `liburing-2024.4.22/src/liburing/common.pyx` & `liburing-2024.5.3/src/liburing/common.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,17 @@
                 >>> io_uring_prep_readv(sqe, fd, iov_write, ...)
 
             Note
                 - Make sure to hold on to variable you are passing into `iovec` so it does not get
                 garbage collected before you get the chance to use it!
         '''
         cdef:
-            unsigned int index
-            str error
-            const unsigned char[:] buffer
+            str                     error
+            unsigned int            index, length
+            const unsigned char[:]  buffer
 
         if buffers:
             self.ref = []  # reference holder
             if isinstance(buffers, (bytes, bytearray, memoryview)):
                 self.ref.append(buffers)
             elif isinstance(buffers, Iterable):
                 self.ref.extend(buffers)
@@ -58,38 +58,40 @@
 
             self.ptr = <__iovec*>PyMem_RawCalloc(self.len, sizeof(__iovec))
             if self.ptr is NULL:
                 memory_error(self)
 
             for index in range(self.len):
                 buffer = self.ref[index]
+                if not (length := len(self.ref[index])):
+                    raise ValueError(f'`{self.__class__.__name__}()` can not be length of `0`')
                 self.ptr[index].iov_base = <void*>&buffer[0]  # starting address
-                self.ptr[index].iov_len = len(self.ref[index])
+                self.ptr[index].iov_len = length
 
     def __dealloc__(self):
         if self.ptr is not NULL:
             PyMem_RawFree(self.ptr)
             self.ptr = NULL
 
     def __bool__(self):
         return self.ptr is not NULL
 
     def __len__(self):
         return self.len
 
-    @boundscheck(True)
     def __getitem__(self, unsigned int index):
         cdef iovec iov
-        if index:
+        if index == 0:
+            return self
+        elif self.len and index < self.len:
             iov = iovec()
             iov.ptr = &self.ptr[index]
-            if iov.ptr is not NULL:
+            if iov.ptr.iov_len:
                 return iov
-            index_error(self, index)
-        return self
+        index_error(self, index)
 
     @property
     def iov_base(self):
         return self.ref[0]
 
     @property
     def iov_len(self):
```

### Comparing `liburing-2024.4.22/src/liburing/error.pyx` & `liburing-2024.5.3/src/liburing/error.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/file.pxd` & `liburing-2024.5.3/src/liburing/file.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                                         open_how how,
                                         unsigned int file_index=?,
                                         int dfd=?) noexcept nogil
 cpdef void io_uring_prep_read(io_uring_sqe sqe,
                               int fd,
                               unsigned char[:] buf,  # `void *buf`
                               unsigned int nbytes,
-                              __u64 offset) noexcept nogil
+                              __u64 offset=?) noexcept nogil
 cpdef void io_uring_prep_read_multishot(io_uring_sqe sqe,
                                         int fd,
                                         unsigned int nbytes,
                                         __u64 offset,
                                         int buf_group) noexcept nogil
 cpdef void io_uring_prep_write(io_uring_sqe sqe,
                                int fd,
```

### Comparing `liburing-2024.4.22/src/liburing/file.pyx` & `liburing-2024.5.3/src/liburing/file.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,20 @@
             self.ptr.resolve = resolve
 
     def __dealloc__(self):
         if self.ptr is not NULL:
             PyMem_RawFree(self.ptr)
             self.ptr = NULL
 
+    def __repr__(self):
+        if self.ptr is not NULL:
+            return f'{self.__class__.__name__}(flags={self.ptr.flags!r}, ' \
+                   f'mode={self.ptr.mode!r}, resolve={self.ptr.resolve!r})'
+        return super().__repr__()
+
     @property
     def mode(self):
         return self.ptr.mode
 
     @mode.setter
     def mode(self, __u64 mode):
         self.ptr.mode = mode
@@ -185,15 +191,15 @@
     '''
     __io_uring_prep_openat2_direct(sqe.ptr, dfd, path, how.ptr, file_index)
 
 cpdef inline void io_uring_prep_read(io_uring_sqe sqe,
                                      int fd,
                                      unsigned char[:] buf,  # `void *buf`
                                      unsigned int nbytes,
-                                     __u64 offset) noexcept nogil:
+                                     __u64 offset=0) noexcept nogil:
     __io_uring_prep_read(sqe.ptr, fd, &buf[0], nbytes, offset)
 
 cpdef inline void io_uring_prep_read_multishot(io_uring_sqe sqe,
                                                int fd,
                                                unsigned int nbytes,
                                                __u64 offset,
                                                int buf_group) noexcept nogil:
```

### Comparing `liburing-2024.4.22/src/liburing/futex.pxd` & `liburing-2024.5.3/src/liburing/futex.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/futex.pyx` & `liburing-2024.5.3/src/liburing/futex.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/helper.pyx` & `liburing-2024.5.3/src/liburing/helper.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/file.pxd` & `liburing-2024.5.3/src/liburing/lib/file.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/futex.pxd` & `liburing-2024.5.3/src/liburing/lib/futex.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/io_uring.pxd` & `liburing-2024.5.3/src/liburing/lib/io_uring.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/socket.pxd` & `liburing-2024.5.3/src/liburing/lib/socket.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/statx.pxd` & `liburing-2024.5.3/src/liburing/lib/statx.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/type.pxd` & `liburing-2024.5.3/src/liburing/lib/type.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/lib/uring.pxd` & `liburing-2024.5.3/src/liburing/lib/uring.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/os.pxd` & `liburing-2024.5.3/src/liburing/os.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/os.pyx` & `liburing-2024.5.3/src/liburing/os.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/other.pxd` & `liburing-2024.5.3/src/liburing/other.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/other.pyx` & `liburing-2024.5.3/src/liburing/other.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/poll.pxd` & `liburing-2024.5.3/src/liburing/poll.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/poll.pyx` & `liburing-2024.5.3/src/liburing/poll.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/probe.py` & `liburing-2024.5.3/src/liburing/probe.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/probe.pyx` & `liburing-2024.5.3/src/liburing/probe.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/queue.pxd` & `liburing-2024.5.3/src/liburing/queue.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/queue.pyx` & `liburing-2024.5.3/src/liburing/queue.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             - `io_uring_sqe` is not the same as `io_uring_get_sqe()`.
             - This class has dual usage:
                 1. It works as a base class for `io_uring_get_sqe()` return.
                 2. It can also be used as `sqe = io_uring_sqe(<int>)`, rather than "get" sqe(s)
                 you are going to "put" pre-made sqe(s) into the ring later. Refer to
                 `help(io_uring_put_sqe)` to see more detail.
     '''
-    def __cinit__(self, __u16 num=1):
+    def __cinit__(self, __u16 num=1, *args, **kwargs):
         cdef str msg
         if num:
             if num > 1024:
                 msg = f'`{self.__class__.__name__}(num)` is limited to 1024, received {num!r}'
                 raise ValueError(msg)
             self.ptr = <__io_uring_sqe*>PyMem_RawCalloc(num, sizeof(__io_uring_sqe))
             if self.ptr is NULL:
@@ -103,19 +103,19 @@
                 sqe = io_uring_sqe(0)  # `0` is set to indicated `ptr` memory is not managed
                 sqe.ptr = &self.ptr[index]
                 self.ref[index-1] = sqe  # cache sqe as this class attribute
                 return sqe
         index_error(self, index, 'out of `sqe`')
 
     @property
-    def flags(self) -> __u8:
+    def flags(self) -> unsigned:
         return self.ptr.flags
 
     @flags.setter
-    def flags(self, __u8 flags):
+    def flags(self, unsigned int flags):
         __io_uring_sqe_set_flags(self.ptr, flags)
 
     @property
     def user_data(self) -> __u64:
         return self.ptr.user_data
 
     @user_data.setter
```

### Comparing `liburing-2024.4.22/src/liburing/register.pxd` & `liburing-2024.5.3/src/liburing/register.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/register.pyx` & `liburing-2024.5.3/src/liburing/register.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/socket.pxd` & `liburing-2024.5.3/src/liburing/socket.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/socket.pyx` & `liburing-2024.5.3/src/liburing/socket.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/socket_extra.pxd` & `liburing-2024.5.3/src/liburing/socket_extra.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/socket_extra.pyx` & `liburing-2024.5.3/src/liburing/socket_extra.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/statx.pxd` & `liburing-2024.5.3/src/liburing/statx.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/statx.pyx` & `liburing-2024.5.3/src/liburing/statx.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     @property
     def stx_gid(self):
         return self.ptr.stx_gid
 
     @property
     def stx_mode(self):
-        return self.ptr.stx_mode & 0o7777
+        return self.ptr.stx_mode
 
     @property
     def stx_ino(self):
         return self.ptr.stx_ino
 
     @property
     def stx_size(self):
```

### Comparing `liburing-2024.4.22/src/liburing/syscall.pxd` & `liburing-2024.5.3/src/liburing/syscall.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/syscall.pyx` & `liburing-2024.5.3/src/liburing/syscall.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/time.pxd` & `liburing-2024.5.3/src/liburing/time.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/time.pyx` & `liburing-2024.5.3/src/liburing/time.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/version.py` & `liburing-2024.5.3/src/liburing/version.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/version.pyx` & `liburing-2024.5.3/src/liburing/version.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/xattr.pxd` & `liburing-2024.5.3/src/liburing/xattr.pxd`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing/xattr.pyx` & `liburing-2024.5.3/src/liburing/xattr.pyx`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/src/liburing.egg-info/PKG-INFO` & `liburing-2024.5.3/src/liburing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liburing
-Version: 2024.4.22
+Version: 2024.5.3
 Summary: ...
 Author: Ritesh
 License: Creative Commons Legal Code
         
         CC0 1.0 Universal
         
             CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
@@ -166,15 +166,15 @@
     - Linux 6.1+ (6.7+ recommended)
     - Python 3.8+
 
 
 Includes (battery)
 ------------------
 
-    - C liburing 2.5+
+    - C liburing 2.6+
 
 
 Install, update & uninstall (Alpha)
 -----------------------------------
 
 Use `pip`_ to install, upgrade & uninstall Python wrapper:
```

### Comparing `liburing-2024.4.22/src/liburing.egg-info/SOURCES.txt` & `liburing-2024.5.3/src/liburing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/conftest.py` & `liburing-2024.5.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/error_test.py` & `liburing-2024.5.3/test/error_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/file/file_test.py` & `liburing-2024.5.3/test/file/file_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/file/open_close_test.py` & `liburing-2024.5.3/test/file/open_close_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/futex_test.py` & `liburing-2024.5.3/test/futex_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/helper/io_uring_put_sqe_test.py` & `liburing-2024.5.3/test/helper/io_uring_put_sqe_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/iovec_test.py` & `liburing-2024.5.3/test/iovec_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,7 +39,10 @@
     assert iovec(write_memoryview).iov_base == b'ccc'
 
     iov_max = SC_IOV_MAX + 1
     buffers = [bytes(1)] * iov_max
     error = re.escape(f"`iovec()` - `buffers` length of {iov_max} exceeds `SC_IOV_MAX` limit set by OS of {SC_IOV_MAX}")
     with pytest.raises(OverflowError, match=error):
         iovec(buffers)
+
+    with pytest.raises(ValueError, match=re.escape('`iovec()` can not be length of `0`')):
+        iovec([b''])
```

### Comparing `liburing-2024.4.22/test/lib/futex_define_test.py` & `liburing-2024.5.3/test/lib/futex_define_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/lib/io_uring_define_test.py` & `liburing-2024.5.3/test/lib/io_uring_define_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/lib/socket_define_test.py` & `liburing-2024.5.3/test/lib/socket_define_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/lib/statx_define_test.py` & `liburing-2024.5.3/test/lib/statx_define_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/lib/type_define_test.py` & `liburing-2024.5.3/test/lib/type_define_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/os/splice_test.py` & `liburing-2024.5.3/test/os/splice_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/os/unlink_test.py` & `liburing-2024.5.3/test/os/unlink_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/probe_test.py` & `liburing-2024.5.3/test/probe_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/queue/init_exit_test.py` & `liburing-2024.5.3/test/queue/init_exit_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/queue/macro_test.py` & `liburing-2024.5.3/test/queue/macro_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/queue/sqe_cqe_test.py` & `liburing-2024.5.3/test/queue/sqe_cqe_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/socket/cmd_sock_test.py` & `liburing-2024.5.3/test/socket/cmd_sock_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/socket/getaddinfo_test.py` & `liburing-2024.5.3/test/socket/getaddinfo_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/socket/getnameinfo_test.py` & `liburing-2024.5.3/test/socket/getnameinfo_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/socket/getsockname_test.py` & `liburing-2024.5.3/test/socket/getsockname_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/socket/socket_connect_test.py` & `liburing-2024.5.3/test/socket/socket_connect_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/statx_test.py` & `liburing-2024.5.3/test/statx_test.py`

 * *Files identical despite different names*

### Comparing `liburing-2024.4.22/test/version_test.py` & `liburing-2024.5.3/test/version_test.py`

 * *Files identical despite different names*

