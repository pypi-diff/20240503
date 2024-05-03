# Comparing `tmp/libluksde-python-20240114.tar.gz` & `tmp/libluksde-python-20240503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libluksde-python-20240114.tar", last modified: Sun Jan 14 19:07:49 2024, max compression
+gzip compressed data, was "libluksde-python-20240503.tar", last modified: Fri May  3 04:23:55 2024, max compression
```

## Comparing `libluksde-python-20240114.tar` & `libluksde-python-20240503.tar`

### file list

```diff
@@ -1,811 +1,811 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      790 2024-01-14 17:30:57.000000 libluksde-20240114/libluksde.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-14 17:30:57.000000 libluksde-20240114/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-14 18:51:04.000000 libluksde-20240114/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 17:30:57.000000 libluksde-20240114/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-14 18:51:04.000000 libluksde-20240114/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_tweaked_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30048 2024-01-14 18:51:04.000000 libluksde-20240114/libcaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-01-14 18:50:38.000000 libluksde-20240114/libcaes/libcaes_tweaked_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29743 2024-01-14 18:51:04.000000 libluksde-20240114/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-14 18:50:51.000000 libluksde-20240114/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:56.000000 libluksde-20240114/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:56.000000 libluksde-20240114/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:56.000000 libluksde-20240114/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7287 2024-01-14 17:33:39.000000 libluksde-20240114/m4/libfcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:56.000000 libluksde-20240114/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:56.000000 libluksde-20240114/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:10:56.000000 libluksde-20240114/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-14 18:50:59.000000 libluksde-20240114/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-14 18:50:59.000000 libluksde-20240114/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:56.000000 libluksde-20240114/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-14 18:50:59.000000 libluksde-20240114/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:56.000000 libluksde-20240114/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:56.000000 libluksde-20240114/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-14 18:50:59.000000 libluksde-20240114/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:56.000000 libluksde-20240114/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:56.000000 libluksde-20240114/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-14 18:50:59.000000 libluksde-20240114/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:56.000000 libluksde-20240114/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:10:56.000000 libluksde-20240114/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:56.000000 libluksde-20240114/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:10:56.000000 libluksde-20240114/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6269 2023-12-03 09:10:56.000000 libluksde-20240114/m4/libcaes.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-01-14 17:30:57.000000 libluksde-20240114/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11148 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11148 2024-01-14 18:51:14.000000 libluksde-20240114/include/libluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28355 2024-01-14 18:51:04.000000 libluksde-20240114/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/include/libluksde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3048 2024-01-14 18:51:14.000000 libluksde-20240114/include/libluksde/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4953 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4822 2024-01-14 18:51:14.000000 libluksde-20240114/include/libluksde/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-01-14 18:51:14.000000 libluksde-20240114/include/libluksde/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-01-14 17:30:58.000000 libluksde-20240114/include/libluksde/codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-14 17:30:58.000000 libluksde-20240114/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-14 17:30:58.000000 libluksde-20240114/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-14 17:30:58.000000 libluksde-20240114/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-14 17:30:58.000000 libluksde-20240114/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-14 17:30:58.000000 libluksde-20240114/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-14 17:30:58.000000 libluksde-20240114/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-14 17:30:58.000000 libluksde-20240114/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-14 17:30:57.000000 libluksde-20240114/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-14 17:30:58.000000 libluksde-20240114/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-14 18:51:14.000000 libluksde-20240114/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19122 2024-01-14 18:51:03.000000 libluksde-20240114/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20225 2024-01-14 18:51:15.000000 libluksde-20240114/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-14 17:30:58.000000 libluksde-20240114/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-14 17:30:58.000000 libluksde-20240114/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-14 17:30:58.000000 libluksde-20240114/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25343 2024-01-14 18:51:04.000000 libluksde-20240114/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30346 2024-01-14 18:51:04.000000 libluksde-20240114/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-01-14 18:50:43.000000 libluksde-20240114/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30819 2024-01-14 18:51:04.000000 libluksde-20240114/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-01-14 18:50:49.000000 libluksde-20240114/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2415 2023-12-04 17:01:23.000000 libluksde-20240114/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2575 2024-01-14 18:51:15.000000 libluksde-20240114/libluksde.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33805 2024-01-14 18:51:04.000000 libluksde-20240114/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-01-14 18:50:36.000000 libluksde-20240114/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:10:46.000000 libluksde-20240114/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-14 18:51:04.000000 libluksde-20240114/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-01-14 17:30:59.000000 libluksde-20240114/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/libluksde.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2260 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/libluksde-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/libluksde-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-01-14 18:51:14.000000 libluksde-20240114/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-14 17:30:57.000000 libluksde-20240114/dpkg/libluksde-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-01-14 18:51:15.000000 libluksde-20240114/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-14 17:30:57.000000 libluksde-20240114/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1886893 2024-01-14 18:51:02.000000 libluksde-20240114/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-14 18:51:04.000000 libluksde-20240114/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-14 18:51:04.000000 libluksde-20240114/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksdemount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7671 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksdemount/luksdemount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6168 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_volume_header/luksde_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5730 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_notify/luksde_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_error/luksde_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_encryption_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_encryption_context/luksde_test_encryption_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcaes/libcaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6568 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_support/luksde_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1556 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_key_slot/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_key_slot/luksde_test_key_slot.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/luksde_test_tools_info_handle/luksde_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_sector_data_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/luksde_test_sector_data_vector/luksde_test_sector_data_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksdeinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksdeinfo/luksdeinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5059 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/libfcrypto/libfcrypto.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcpath/libcpath.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32434 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/libluksde.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_io_handle/luksde_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6162 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_sector_data/luksde_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23867 2024-01-14 18:51:04.000000 libluksde-20240114/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/pyluksde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7210 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/pyluksde/pyluksde.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_diffuser/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5736 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/luksde_test_diffuser/luksde_test_diffuser.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_tools_output/luksde_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/luksde_test_tools_signal/luksde_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6482 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/luksde_test_volume/luksde_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/luksde_test_password/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-01-14 17:31:37.000000 libluksde-20240114/msvscpp/luksde_test_password/luksde_test_password.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/msvscpp/libluksde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9243 2024-01-14 17:31:22.000000 libluksde-20240114/msvscpp/libluksde/libluksde.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      182 2024-01-14 17:30:58.000000 libluksde-20240114/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31110 2024-01-14 18:51:04.000000 libluksde-20240114/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-01-14 18:50:42.000000 libluksde-20240114/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2024-01-14 18:01:18.000000 libluksde-20240114/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-14 18:51:04.000000 libluksde-20240114/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32794 2024-01-14 18:51:04.000000 libluksde-20240114/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-14 18:50:39.000000 libluksde-20240114/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-14 17:30:57.000000 libluksde-20240114/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-01-14 17:30:57.000000 libluksde-20240114/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-14 18:51:04.000000 libluksde-20240114/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-14 17:30:57.000000 libluksde-20240114/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-14 17:32:04.000000 libluksde-20240114/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:10:46.000000 libluksde-20240114/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33200 2024-01-14 18:51:04.000000 libluksde-20240114/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-14 18:50:48.000000 libluksde-20240114/libcthreads/libcthreads_queue.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libfcrypto/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3331 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_blowfish_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42088 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_blowfish_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_rc4_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9130 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_rc4_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      894 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_serpent_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75716 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_serpent_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32055 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_des3_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_des3_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31222 2024-01-14 18:51:04.000000 libluksde-20240114/libfcrypto/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-14 18:50:50.000000 libluksde-20240114/libfcrypto/libfcrypto_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-14 18:51:04.000000 libluksde-20240114/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30388 2024-01-14 18:51:04.000000 libluksde-20240114/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-01-14 18:50:46.000000 libluksde-20240114/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1151 2023-12-03 09:10:46.000000 libluksde-20240114/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1738 2024-01-14 17:30:59.000000 libluksde-20240114/manuals/luksdemount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      196 2023-12-03 09:10:58.000000 libluksde-20240114/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5304 2024-01-14 17:30:59.000000 libluksde-20240114/manuals/libluksde.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-14 17:30:59.000000 libluksde-20240114/manuals/luksdeinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27351 2024-01-14 18:51:04.000000 libluksde-20240114/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21863 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_encryption_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19459 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_password.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13137 2024-01-14 17:32:04.000000 libluksde-20240114/tests/pyluksde_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42714 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3337 2024-01-14 17:30:59.000000 libluksde-20240114/tests/test_luksdeinfo.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4081 2024-01-14 17:32:04.000000 libluksde-20240114/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59939 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-14 17:31:37.000000 libluksde-20240114/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8293 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9008 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_key_slot.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_notify.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-14 17:30:59.000000 libluksde-20240114/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3837 2024-01-14 17:30:59.000000 libluksde-20240114/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17597 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-14 17:30:59.000000 libluksde-20240114/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7128 2024-01-14 17:31:37.000000 libluksde-20240114/tests/luksde_test_sector_data_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13062 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_diffuser.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14625 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64543 2024-01-14 18:51:04.000000 libluksde-20240114/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-01-14 17:30:59.000000 libluksde-20240114/tests/luksde_test_libluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3480 2024-01-14 17:32:04.000000 libluksde-20240114/tests/pyluksde_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4181 2024-01-14 17:30:59.000000 libluksde-20240114/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3607 2024-01-14 17:30:57.000000 libluksde-20240114/libluksde.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:49.000000 libluksde-20240114/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-01-14 17:30:58.000000 libluksde-20240114/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-01-14 17:30:58.000000 libluksde-20240114/ossfuzz/ossfuzz_libluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-12-03 09:10:59.000000 libluksde-20240114/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-14 17:30:58.000000 libluksde-20240114/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32604 2024-01-14 18:51:04.000000 libluksde-20240114/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-14 18:50:59.000000 libluksde-20240114/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32920 2024-01-14 18:51:04.000000 libluksde-20240114/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-01-14 18:50:53.000000 libluksde-20240114/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31168 2024-01-14 18:51:04.000000 libluksde-20240114/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-01-14 18:50:47.000000 libluksde-20240114/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:56.000000 libluksde-20240114/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:56.000000 libluksde-20240114/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:56.000000 libluksde-20240114/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:56.000000 libluksde-20240114/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:56.000000 libluksde-20240114/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:56.000000 libluksde-20240114/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:56.000000 libluksde-20240114/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:56.000000 libluksde-20240114/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:56.000000 libluksde-20240114/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-01-14 18:51:14.000000 libluksde-20240114/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:56.000000 libluksde-20240114/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:56.000000 libluksde-20240114/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53865 2024-01-14 18:51:04.000000 libluksde-20240114/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-01-14 18:50:55.000000 libluksde-20240114/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41550 2024-01-14 18:51:04.000000 libluksde-20240114/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/pyluksde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_libluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2869 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16905 2024-01-14 17:32:04.000000 libluksde-20240114/pyluksde/pyluksde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2023-12-03 09:10:58.000000 libluksde-20240114/pyluksde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1875 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_initialization_vector_modes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6668 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_hashing_methods.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7786 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_initialization_vector_modes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_encryption_methods.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_encryption_chaining_modes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38542 2024-01-14 17:32:04.000000 libluksde-20240114/pyluksde/pyluksde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48935 2024-01-14 18:51:04.000000 libluksde-20240114/pyluksde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_hashing_methods.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_encryption_chaining_modes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7774 2024-01-14 17:30:58.000000 libluksde-20240114/pyluksde/pyluksde_encryption_methods.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3858 2024-01-14 17:32:04.000000 libluksde-20240114/pyluksde/pyluksde_volume.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/luksdetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3003 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26475 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3074 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_input.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19010 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2513 2023-12-03 09:10:57.000000 libluksde-20240114/luksdetools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20786 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24750 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3632 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6321 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_input.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libluksde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3344 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24428 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35002 2024-01-14 18:51:04.000000 libluksde-20240114/luksdetools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3957 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/luksdetools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7571 2024-01-14 18:46:05.000000 libluksde-20240114/luksdetools/luksdeinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2768 2024-01-14 17:30:59.000000 libluksde-20240114/luksdetools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17142 2024-01-14 17:32:04.000000 libluksde-20240114/luksdetools/luksdemount.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30222 2024-01-14 18:51:04.000000 libluksde-20240114/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-14 18:50:45.000000 libluksde-20240114/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:47.000000 libluksde-20240114/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-14 18:50:40.000000 libluksde-20240114/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29735 2024-01-14 18:51:04.000000 libluksde-20240114/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56881 2024-01-14 18:51:01.000000 libluksde-20240114/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8853 2024-01-14 17:34:03.000000 libluksde-20240114/configure.ac
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-14 19:07:48.000000 libluksde-20240114/libluksde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1110 2024-01-14 18:51:15.000000 libluksde-20240114/libluksde/libluksde.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3487 2024-01-14 17:34:52.000000 libluksde-20240114/libluksde/libluksde_encryption_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3609 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7452 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7041 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_key_slot.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9214 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_sector_data_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2471 2023-12-03 09:10:57.000000 libluksde-20240114/libluksde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36678 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1583 2024-01-14 17:47:16.000000 libluksde-20240114/libluksde/libluksde_libfcrypto.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/luksde_keyslot.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_password.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11612 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_diffuser.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_password.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3825 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84497 2024-01-14 17:55:57.000000 libluksde-20240114/libluksde/libluksde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_sector_data_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3919 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/luksde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_diffuser.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_key_slot.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32205 2024-01-14 17:51:29.000000 libluksde-20240114/libluksde/libluksde_encryption_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36188 2024-01-14 18:51:04.000000 libluksde-20240114/libluksde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3962 2024-01-14 17:45:12.000000 libluksde-20240114/libluksde/libluksde_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2697 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9312 2024-01-14 17:30:58.000000 libluksde-20240114/libluksde/libluksde_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2024-01-14 18:51:14.000000 libluksde-20240114/libluksde/libluksde_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-01-14 19:07:49.738287 libluksde-20240114/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      790 2024-05-03 03:27:54.000000 libluksde-20240503/libluksde.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-03 03:27:54.000000 libluksde-20240503/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-03 04:05:43.000000 libluksde-20240503/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 03:27:54.000000 libluksde-20240503/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-03 04:05:44.000000 libluksde-20240503/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:53.000000 libluksde-20240503/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_tweaked_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30345 2024-05-03 04:05:43.000000 libluksde-20240503/libcaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-05-03 04:05:11.000000 libluksde-20240503/libcaes/libcaes_tweaked_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29996 2024-05-03 04:05:43.000000 libluksde-20240503/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-03 04:05:28.000000 libluksde-20240503/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:56.000000 libluksde-20240503/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:56.000000 libluksde-20240503/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:56.000000 libluksde-20240503/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5887 2024-05-03 03:28:01.000000 libluksde-20240503/m4/libfcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:56.000000 libluksde-20240503/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:56.000000 libluksde-20240503/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-03 03:28:00.000000 libluksde-20240503/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-03 04:05:38.000000 libluksde-20240503/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-03 04:05:37.000000 libluksde-20240503/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:56.000000 libluksde-20240503/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-03 03:28:01.000000 libluksde-20240503/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-03 04:05:37.000000 libluksde-20240503/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:56.000000 libluksde-20240503/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:56.000000 libluksde-20240503/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-03 04:05:38.000000 libluksde-20240503/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:56.000000 libluksde-20240503/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:56.000000 libluksde-20240503/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-03 04:05:37.000000 libluksde-20240503/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:56.000000 libluksde-20240503/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-03 03:28:00.000000 libluksde-20240503/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:56.000000 libluksde-20240503/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-03 03:28:00.000000 libluksde-20240503/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6500 2024-05-03 03:28:00.000000 libluksde-20240503/m4/libcaes.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      440 2024-05-03 03:33:50.000000 libluksde-20240503/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11148 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11148 2024-05-03 04:06:03.000000 libluksde-20240503/include/libluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28391 2024-05-03 04:05:43.000000 libluksde-20240503/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/include/libluksde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3048 2024-05-03 04:06:03.000000 libluksde-20240503/include/libluksde/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4953 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4822 2024-05-03 04:06:03.000000 libluksde-20240503/include/libluksde/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-05-03 04:06:03.000000 libluksde-20240503/include/libluksde/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-05-03 03:27:57.000000 libluksde-20240503/include/libluksde/codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-03 03:27:57.000000 libluksde-20240503/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-03 03:27:57.000000 libluksde-20240503/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-03 03:27:57.000000 libluksde-20240503/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-03 03:27:57.000000 libluksde-20240503/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-03 03:27:57.000000 libluksde-20240503/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-03 03:27:57.000000 libluksde-20240503/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-03 03:27:57.000000 libluksde-20240503/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-03 03:33:50.000000 libluksde-20240503/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-03 03:27:57.000000 libluksde-20240503/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-03 04:06:04.000000 libluksde-20240503/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19205 2024-05-03 04:05:42.000000 libluksde-20240503/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20314 2024-05-03 04:06:04.000000 libluksde-20240503/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-03 03:27:57.000000 libluksde-20240503/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-03 03:27:57.000000 libluksde-20240503/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-03 03:27:57.000000 libluksde-20240503/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25406 2024-05-03 04:05:43.000000 libluksde-20240503/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30604 2024-05-03 04:05:43.000000 libluksde-20240503/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-03 04:05:17.000000 libluksde-20240503/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31113 2024-05-03 04:05:43.000000 libluksde-20240503/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-03 04:05:25.000000 libluksde-20240503/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2223 2024-05-03 03:36:43.000000 libluksde-20240503/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2577 2024-05-03 04:06:04.000000 libluksde-20240503/libluksde.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34456 2024-05-03 04:05:43.000000 libluksde-20240503/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-03 04:05:09.000000 libluksde-20240503/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:10:46.000000 libluksde-20240503/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-03 04:05:43.000000 libluksde-20240503/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-05-03 03:28:00.000000 libluksde-20240503/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:50.000000 libluksde-20240503/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/libluksde.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2260 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/libluksde-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/libluksde-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-05-03 04:06:04.000000 libluksde-20240503/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-03 03:27:54.000000 libluksde-20240503/dpkg/libluksde-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-05-03 04:06:04.000000 libluksde-20240503/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-03 03:27:54.000000 libluksde-20240503/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1880730 2024-05-03 04:05:41.000000 libluksde-20240503/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-03 04:05:43.000000 libluksde-20240503/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-03 04:05:43.000000 libluksde-20240503/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksdemount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7671 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksdemount/luksdemount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6168 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_volume_header/luksde_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5730 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_notify/luksde_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_error/luksde_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_encryption_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_encryption_context/luksde_test_encryption_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcaes/libcaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6568 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_support/luksde_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-05-03 03:34:03.000000 libluksde-20240503/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_key_slot/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_key_slot/luksde_test_key_slot.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/luksde_test_tools_info_handle/luksde_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_sector_data_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/luksde_test_sector_data_vector/luksde_test_sector_data_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksdeinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksdeinfo/luksdeinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5059 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/libfcrypto/libfcrypto.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcpath/libcpath.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32434 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/libluksde.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_io_handle/luksde_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6162 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_sector_data/luksde_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23923 2024-05-03 04:05:44.000000 libluksde-20240503/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/pyluksde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7210 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/pyluksde/pyluksde.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_diffuser/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5736 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/luksde_test_diffuser/luksde_test_diffuser.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_tools_output/luksde_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/luksde_test_tools_signal/luksde_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6482 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/luksde_test_volume/luksde_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/luksde_test_password/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2024-05-03 03:30:41.000000 libluksde-20240503/msvscpp/luksde_test_password/luksde_test_password.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/msvscpp/libluksde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9243 2024-05-03 03:29:03.000000 libluksde-20240503/msvscpp/libluksde/libluksde.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      182 2024-05-03 03:27:56.000000 libluksde-20240503/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31437 2024-05-03 04:05:43.000000 libluksde-20240503/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-03 04:05:16.000000 libluksde-20240503/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2024-05-03 03:32:32.000000 libluksde-20240503/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-03 04:05:43.000000 libluksde-20240503/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33350 2024-05-03 04:05:43.000000 libluksde-20240503/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-03 04:05:13.000000 libluksde-20240503/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-03 03:27:54.000000 libluksde-20240503/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-05-03 03:27:54.000000 libluksde-20240503/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-03 04:05:43.000000 libluksde-20240503/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-03 03:27:54.000000 libluksde-20240503/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-03 03:37:27.000000 libluksde-20240503/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:10:46.000000 libluksde-20240503/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33789 2024-05-03 04:05:43.000000 libluksde-20240503/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-03 04:05:23.000000 libluksde-20240503/libcthreads/libcthreads_queue.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:53.000000 libluksde-20240503/libfcrypto/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3331 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_blowfish_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42088 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_blowfish_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_rc4_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9130 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_rc4_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      890 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_serpent_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75716 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_serpent_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32055 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_des3_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_des3_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31586 2024-05-03 04:05:43.000000 libluksde-20240503/libfcrypto/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-03 04:05:26.000000 libluksde-20240503/libfcrypto/libfcrypto_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-03 04:05:44.000000 libluksde-20240503/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-03 04:05:21.000000 libluksde-20240503/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-03 04:05:21.000000 libluksde-20240503/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30635 2024-05-03 04:05:43.000000 libluksde-20240503/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-03 04:05:20.000000 libluksde-20240503/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1151 2023-12-03 09:10:46.000000 libluksde-20240503/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1738 2024-05-03 03:28:00.000000 libluksde-20240503/manuals/luksdemount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      167 2024-05-03 03:34:18.000000 libluksde-20240503/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5304 2024-05-03 03:28:00.000000 libluksde-20240503/manuals/libluksde.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-03 03:28:00.000000 libluksde-20240503/manuals/luksdeinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27407 2024-05-03 04:05:44.000000 libluksde-20240503/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21863 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_encryption_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19459 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_password.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13137 2024-05-03 03:32:32.000000 libluksde-20240503/tests/pyluksde_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42714 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-05-03 03:28:00.000000 libluksde-20240503/tests/test_luksdeinfo.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4050 2024-05-03 03:33:29.000000 libluksde-20240503/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59939 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7417 2024-05-03 03:35:44.000000 libluksde-20240503/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8293 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9008 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_key_slot.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_notify.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-03 03:28:00.000000 libluksde-20240503/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4419 2024-05-03 03:28:00.000000 libluksde-20240503/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17597 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-03 03:28:00.000000 libluksde-20240503/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7128 2024-05-03 03:30:41.000000 libluksde-20240503/tests/luksde_test_sector_data_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13062 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_diffuser.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14625 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65685 2024-05-03 04:05:44.000000 libluksde-20240503/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-03 03:28:00.000000 libluksde-20240503/tests/luksde_test_libluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3480 2024-05-03 03:32:32.000000 libluksde-20240503/tests/pyluksde_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4150 2024-05-03 03:28:00.000000 libluksde-20240503/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3607 2024-05-03 03:27:54.000000 libluksde-20240503/libluksde.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-05-03 03:27:58.000000 libluksde-20240503/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-05-03 03:27:58.000000 libluksde-20240503/ossfuzz/ossfuzz_libluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      903 2024-05-03 03:34:51.000000 libluksde-20240503/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-03 03:27:58.000000 libluksde-20240503/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32723 2024-05-03 04:05:44.000000 libluksde-20240503/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-03 04:05:37.000000 libluksde-20240503/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33500 2024-05-03 04:05:43.000000 libluksde-20240503/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-03 04:05:29.000000 libluksde-20240503/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31532 2024-05-03 04:05:43.000000 libluksde-20240503/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-03 04:05:22.000000 libluksde-20240503/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:54.000000 libluksde-20240503/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:56.000000 libluksde-20240503/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:56.000000 libluksde-20240503/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:56.000000 libluksde-20240503/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:56.000000 libluksde-20240503/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:56.000000 libluksde-20240503/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:56.000000 libluksde-20240503/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:56.000000 libluksde-20240503/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:56.000000 libluksde-20240503/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:56.000000 libluksde-20240503/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-05-03 04:06:03.000000 libluksde-20240503/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:56.000000 libluksde-20240503/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:56.000000 libluksde-20240503/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:52.000000 libluksde-20240503/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57116 2024-05-03 04:05:43.000000 libluksde-20240503/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-03 04:05:32.000000 libluksde-20240503/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41488 2024-05-03 04:05:43.000000 libluksde-20240503/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:53.000000 libluksde-20240503/pyluksde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_libluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2869 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16905 2024-05-03 03:32:32.000000 libluksde-20240503/pyluksde/pyluksde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-03 03:34:26.000000 libluksde-20240503/pyluksde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1875 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_initialization_vector_modes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6668 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_hashing_methods.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7786 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_initialization_vector_modes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_encryption_methods.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_encryption_chaining_modes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38515 2024-05-03 03:32:32.000000 libluksde-20240503/pyluksde/pyluksde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49604 2024-05-03 04:05:44.000000 libluksde-20240503/pyluksde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_hashing_methods.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_encryption_chaining_modes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7774 2024-05-03 03:27:58.000000 libluksde-20240503/pyluksde/pyluksde_encryption_methods.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3858 2024-05-03 03:32:32.000000 libluksde-20240503/pyluksde/pyluksde_volume.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:53.000000 libluksde-20240503/luksdetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3003 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26475 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3074 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_input.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19010 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2509 2024-05-03 03:34:43.000000 libluksde-20240503/luksdetools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20786 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24750 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3632 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6321 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_input.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libluksde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3344 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24428 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35541 2024-05-03 04:05:44.000000 libluksde-20240503/luksdetools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3957 2024-05-03 03:27:59.000000 libluksde-20240503/luksdetools/luksdetools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7571 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/luksdeinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2768 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17142 2024-05-03 03:32:32.000000 libluksde-20240503/luksdetools/luksdemount.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30473 2024-05-03 04:05:43.000000 libluksde-20240503/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-03 04:05:19.000000 libluksde-20240503/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:51.000000 libluksde-20240503/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-03 04:05:14.000000 libluksde-20240503/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29940 2024-05-03 04:05:43.000000 libluksde-20240503/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56881 2024-05-03 04:05:40.000000 libluksde-20240503/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8853 2024-05-03 03:38:37.000000 libluksde-20240503/configure.ac
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-03 04:23:53.000000 libluksde-20240503/libluksde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1110 2024-05-03 04:06:04.000000 libluksde-20240503/libluksde/libluksde.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3487 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_encryption_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3609 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7452 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1858 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7041 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_key_slot.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9214 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_sector_data_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2024-05-03 03:35:11.000000 libluksde-20240503/libluksde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36678 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1583 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libfcrypto.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/luksde_keyslot.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_password.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11612 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_diffuser.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_password.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3825 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84497 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_sector_data_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3919 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/luksde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1470 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_diffuser.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_key_slot.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32205 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_encryption_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36871 2024-05-03 04:05:43.000000 libluksde-20240503/libluksde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3962 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2697 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9312 2024-05-03 03:27:58.000000 libluksde-20240503/libluksde/libluksde_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2024-05-03 04:06:03.000000 libluksde-20240503/libluksde/libluksde_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-05-03 04:23:55.200083 libluksde-20240503/PKG-INFO
```

### Comparing `libluksde-20240114/libluksde.pc.in` & `libluksde-20240503/libluksde.pc.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/COPYING` & `libluksde-20240503/COPYING`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/install-sh` & `libluksde-20240503/install-sh`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/depcomp` & `libluksde-20240503/depcomp`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcaes/libcaes_unused.h` & `libluksde-20240503/libcaes/libcaes_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_tweaked_context.h` & `libluksde-20240503/libcaes/libcaes_tweaked_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES tweaked de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_context.h` & `libluksde-20240503/libcaes/libcaes_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_error.c` & `libluksde-20240503/libcaes/libcaes_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_context.c` & `libluksde-20240503/libcaes/libcaes_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_definitions.h` & `libluksde-20240503/libcaes/libcaes_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBCAES )
 #include <libcaes/definitions.h>
 
 /* The definitions in <libcaes/definitions.h> are copied here
  * for local use of libcaes
  */
 #else
-#define LIBCAES_VERSION				20231120
+#define LIBCAES_VERSION				20240413
 
 /* The libcaes version string
  */
-#define LIBCAES_VERSION_STRING			"20231120"
+#define LIBCAES_VERSION_STRING			"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT		= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libluksde-20240114/libcaes/Makefile.am` & `libluksde-20240503/libcaes/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 if HAVE_LOCAL_LIBCAES
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
-	@LIBCERROR_CPPFLAGS@ 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
+	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcaes.la
 
 libcaes_la_SOURCES = \
 	libcaes_context.c libcaes_context.h \
 	libcaes_definitions.h \
 	libcaes_extern.h \
@@ -14,19 +15,17 @@
 	libcaes_libcerror.h \
 	libcaes_support.c libcaes_support.h \
 	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 	libcaes_types.h \
 	libcaes_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
```

### Comparing `libluksde-20240114/libcaes/libcaes_error.h` & `libluksde-20240503/libcaes/libcaes_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_types.h` & `libluksde-20240503/libcaes/libcaes_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_extern.h` & `libluksde-20240503/libcaes/libcaes_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_support.h` & `libluksde-20240503/libcaes/libcaes_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_libcerror.h` & `libluksde-20240503/libcaes/libcaes_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/libcaes_support.c` & `libluksde-20240503/libcaes/libcaes_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcaes/Makefile.in` & `libluksde-20240503/libcaes/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,31 +531,33 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCAES_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/common \
-@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ 
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../common -I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCRYPTO_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCAES_TRUE@noinst_LTLIBRARIES = libcaes.la
 @HAVE_LOCAL_LIBCAES_TRUE@libcaes_la_SOURCES = \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_context.c libcaes_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_definitions.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_extern.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_error.c libcaes_error.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_libcerror.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_support.c libcaes_support.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_types.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -756,24 +760,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcaes_context.Plo
+	-rm -f ./$(DEPDIR)/libcaes_error.Plo
+	-rm -f ./$(DEPDIR)/libcaes_support.Plo
+	-rm -f ./$(DEPDIR)/libcaes_tweaked_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,17 +870,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcaes/libcaes_tweaked_context.c` & `libluksde-20240503/libcaes/libcaes_tweaked_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES encryption functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_error.c` & `libluksde-20240503/libfguid/libfguid_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_support.h` & `libluksde-20240503/libfguid/libfguid_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_identifier.h` & `libluksde-20240503/libfguid/libfguid_identifier.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Global (or Universal) Unique Identifier (GUID/UUID) functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_libcerror.h` & `libluksde-20240503/libfguid/libfguid_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/Makefile.am` & `libluksde-20240503/libfguid/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,17 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libluksde-20240114/libfguid/libfguid_unused.h` & `libluksde-20240503/libfguid/libfguid_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_extern.h` & `libluksde-20240503/libfguid/libfguid_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_types.h` & `libluksde-20240503/libfguid/libfguid_types.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_identifier.c` & `libluksde-20240503/libfguid/libfguid_identifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * GUID functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_support.c` & `libluksde-20240503/libfguid/libfguid_support.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libfguid/libfguid_definitions.h` & `libluksde-20240503/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20220113
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20220113"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libluksde-20240114/libfguid/Makefile.in` & `libluksde-20240503/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,30 +531,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -754,24 +757,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -831,14 +839,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -849,23 +859,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/libfguid/libfguid_error.h` & `libluksde-20240503/libfguid/libfguid_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/m4/libcfile.m4` & `libluksde-20240503/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/tests.m4` & `libluksde-20240503/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libcpath.m4` & `libluksde-20240503/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/lib-prefix.m4` & `libluksde-20240503/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/progtest.m4` & `libluksde-20240503/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libfcrypto.m4` & `libluksde-20240503/m4/libfcrypto.m4`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for libfcrypto required headers and functions
 dnl
-dnl Version: 20240114
+dnl Version: 20240413
 
 dnl Function to detect if libfcrypto is available
 dnl ac_libfcrypto_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcrypto" = xno],
     [ac_cv_libfcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcrypto which returns "yes" and --with-libfcrypto= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect],
+      [test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_with_libfcrypto" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcrypto"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcrypto}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcrypto}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcrypto],
           [1])
@@ -48,72 +50,14 @@
 
         AC_CHECK_LIB(
           fcrypto,
           libfcrypto_get_version,
           [ac_cv_libfcrypto_dummy=yes],
           [ac_cv_libfcrypto=no])
 
-        dnl Blowfish context functions
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_blowfish_context_initialize,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_blowfish_context_free,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_blowfish_context_set_key,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_blowfish_crypt_cbc,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_blowfish_crypt_ecb,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
-        dnl DES3 context functions
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_des3_context_initialize,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_des3_context_free,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_des3_context_set_key,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_des3_crypt_cbc,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-        AC_CHECK_LIB(
-          fcrypto,
-          libfcrypto_des3_crypt_ecb,
-          [ac_cv_libfcrypto_dummy=yes],
-          [ac_cv_libfcrypto=no])
-
         dnl RC4 context functions
         AC_CHECK_LIB(
           fcrypto,
           libfcrypto_rc4_context_initialize,
           [ac_cv_libfcrypto_dummy=yes],
           [ac_cv_libfcrypto=no])
         AC_CHECK_LIB(
@@ -161,16 +105,17 @@
           fcrypto,
           libfcrypto_serpent_crypt_ecb,
           [ac_cv_libfcrypto_dummy=yes],
           [ac_cv_libfcrypto=no])
 
         ac_cv_libfcrypto_LIBADD="-lfcrypto"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_libfcrypto" != xyes],
+      [test "x$ac_cv_libfcrypto" != xyes && test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_with_libfcrypto" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcrypto in directory: $ac_cv_with_libfcrypto],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfcrypto dependencies are available
 AC_DEFUN([AX_LIBFCRYPTO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfcrypto_CPPFLAGS="-I../libfcrypto";
+  ac_cv_libfcrypto_CPPFLAGS="-I../libfcrypto -I\$(top_srcdir)/libfcrypto";
   ac_cv_libfcrypto_LIBADD="../libfcrypto/libfcrypto.la";
 
   ac_cv_libfcrypto=local
   ])
 
 dnl Function to detect how to enable libfcrypto
 AC_DEFUN([AX_LIBFCRYPTO_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libuna.m4` & `libluksde-20240503/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/gettext.m4` & `libluksde-20240503/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/lib-ld.m4` & `libluksde-20240503/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libclocale.m4` & `libluksde-20240503/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libcdata.m4` & `libluksde-20240503/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libcsplit.m4` & `libluksde-20240503/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/common.m4` & `libluksde-20240503/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libluksde-20240114/m4/libcthreads.m4` & `libluksde-20240503/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libluksde-20240114/m4/ltversion.m4` & `libluksde-20240503/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/ltsugar.m4` & `libluksde-20240503/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/host-cpu-c-abi.m4` & `libluksde-20240503/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libfuse.m4` & `libluksde-20240503/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libluksde-20240114/m4/libtool.m4` & `libluksde-20240503/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/po.m4` & `libluksde-20240503/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libcerror.m4` & `libluksde-20240503/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libcnotify.m4` & `libluksde-20240503/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libfguid.m4` & `libluksde-20240503/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libluksde-20240114/m4/libbfio.m4` & `libluksde-20240503/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/libhmac.m4` & `libluksde-20240503/m4/libhmac.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libhmac required headers and functions
 dnl
-dnl Version: 20200104
+dnl Version: 20240413
 
 dnl Function to detect if libhmac is available
 dnl ac_libhmac_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBHMAC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno],
     [ac_cv_libhmac=no],
     [ac_cv_libhmac=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libhmac which returns "yes" and --with-libhmac= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect],
+      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libhmac"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libhmac],
           [1])
@@ -161,16 +163,17 @@
           hmac,
           libhmac_sha512_free,
           [ac_cv_libhmac_dummy=yes],
           [ac_cv_libhmac=no])
 
         ac_cv_libhmac_LIBADD="-lhmac"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes],
+      [test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libhmac in directory: $ac_cv_with_libhmac],
         [1])
       ])
     ])
 
   AS_IF(
@@ -240,15 +243,15 @@
     [ac_cv_libhmac_sha256=$ac_cv_libcrypto_sha256])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno],
     [ac_cv_libhmac_sha512=local],
     [ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512])
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
   ])
 
 dnl Function to detect how to enable libhmac
 AC_DEFUN([AX_LIBHMAC_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/intlmacosx.m4` & `libluksde-20240503/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/lt~obsolete.m4` & `libluksde-20240503/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/lib-link.m4` & `libluksde-20240503/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/iconv.m4` & `libluksde-20240503/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/ltoptions.m4` & `libluksde-20240503/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/nls.m4` & `libluksde-20240503/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/python.m4` & `libluksde-20240503/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libluksde-20240114/m4/libcrypto.m4` & `libluksde-20240503/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libluksde-20240114/m4/types.m4` & `libluksde-20240503/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/m4/libfcache.m4` & `libluksde-20240503/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/m4/pthread.m4` & `libluksde-20240503/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libluksde-20240114/m4/libcaes.m4` & `libluksde-20240503/m4/libcaes.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcaes required headers and functions
 dnl
-dnl Version: 20220529
+dnl Version: 20240413
 
 dnl Function to detect if libcaes is available
 dnl ac_libcaes_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCAES_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno],
     [ac_cv_libcaes=no],
     [ac_cv_libcaes=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcaes which returns "yes" and --with-libcaes= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect],
+      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcaes"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcaes],
           [1])
@@ -107,16 +109,17 @@
           caes,
           libcaes_crypt_xts,
           [ac_cv_libcaes_dummy=yes],
           [ac_cv_libcaes=no])
 
         ac_cv_libcaes_LIBADD="-lcaes"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes],
+      [test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcaes in directory: $ac_cv_with_libcaes],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +168,15 @@
     [ac_cv_libcaes_aes_ecb=$ac_cv_libcrypto_aes_ecb])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno],
     [ac_cv_libcaes_aes_xts=local],
     [ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts])
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
   ])
 
 dnl Function to detect how to enable libcaes
 AC_DEFUN([AX_LIBCAES_CHECK_ENABLE],
```

### Comparing `libluksde-20240114/include/libluksde.h.in` & `libluksde-20240503/include/libluksde.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde.h` & `libluksde-20240503/include/libluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/Makefile.in` & `libluksde-20240503/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -535,15 +537,20 @@
 
 EXTRA_DIST = \
 	libluksde.h.in \
 	libluksde/definitions.h.in \
 	libluksde/features.h.in \
 	libluksde/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libluksde.h \
+	libluksde/definitions.h \
+	libluksde/features.h \
+	libluksde/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -740,23 +747,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -838,17 +847,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libluksde.h
-	-rm -f libluksde/definitions.h
-	-rm -f libluksde/features.h
-	-rm -f libluksde/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/include/libluksde/definitions.h.in` & `libluksde-20240503/include/libluksde/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/definitions.h` & `libluksde-20240503/include/libluksde/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBLUKSDE_DEFINITIONS_H )
 #define _LIBLUKSDE_DEFINITIONS_H
 
 #include <libluksde/types.h>
 
-#define LIBLUKSDE_VERSION		20240114
+#define LIBLUKSDE_VERSION		20240503
 
 /* The version string
  */
-#define LIBLUKSDE_VERSION_STRING	"20240114"
+#define LIBLUKSDE_VERSION_STRING	"20240503"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBLUKSDE_ACCESS_FLAGS
```

### Comparing `libluksde-20240114/include/libluksde/types.h.in` & `libluksde-20240503/include/libluksde/types.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/types.h` & `libluksde-20240503/include/libluksde/types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/features.h.in` & `libluksde-20240503/include/libluksde/features.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/error.h` & `libluksde-20240503/include/libluksde/error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/extern.h` & `libluksde-20240503/include/libluksde/extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/features.h` & `libluksde-20240503/include/libluksde/features.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/include/libluksde/codepage.h` & `libluksde-20240503/include/libluksde/codepage.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/config_borlandc.h` & `libluksde-20240503/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/file_stream.h` & `libluksde-20240503/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/memory.h` & `libluksde-20240503/common/memory.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/byte_stream.h` & `libluksde-20240503/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/common.h` & `libluksde-20240503/common/common.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/config_winapi.h` & `libluksde-20240503/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/system_string.h` & `libluksde-20240503/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/types.h.in` & `libluksde-20240503/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/types.h` & `libluksde-20240503/common/types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/config.h.in` & `libluksde-20240503/common/config.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,17 @@
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 #undef HAVE_LIBFGUID_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `hmac' library (-lhmac). */
 #undef HAVE_LIBHMAC
 
 /* Define to 1 if you have the <libhmac.h> header file. */
 #undef HAVE_LIBHMAC_H
 
 /* Define to 1 if you have the <libintl.h> header file. */
```

### Comparing `libluksde-20240114/common/config.h` & `libluksde-20240503/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,18 @@
 /* Define to 1 if you have the `fguid' library (-lfguid). */
 /* #undef HAVE_LIBFGUID */
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 /* #undef HAVE_LIBFGUID_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `hmac' library (-lhmac). */
 /* #undef HAVE_LIBHMAC */
 
 /* Define to 1 if you have the <libhmac.h> header file. */
 /* #undef HAVE_LIBHMAC_H */
 
@@ -631,24 +634,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libluksde"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libluksde 20240114"
+#define PACKAGE_STRING "libluksde 20240503"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libluksde"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240114"
+#define PACKAGE_VERSION "20240503"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -669,15 +672,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240114"
+#define VERSION "20240503"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libluksde-20240114/common/wide_string.h` & `libluksde-20240503/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/narrow_string.h` & `libluksde-20240503/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/config_msc.h` & `libluksde-20240503/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/common/Makefile.in` & `libluksde-20240503/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -488,15 +490,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -504,15 +508,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -680,23 +687,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -776,15 +785,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/libclocale/libclocale_wide_string.c` & `libluksde-20240503/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_support.h` & `libluksde-20240503/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/Makefile.am` & `libluksde-20240503/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libluksde-20240114/libclocale/libclocale_definitions.h` & `libluksde-20240503/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libluksde-20240114/libclocale/libclocale_unused.h` & `libluksde-20240503/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_libcerror.h` & `libluksde-20240503/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_locale.h` & `libluksde-20240503/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_support.c` & `libluksde-20240503/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_codepage.c` & `libluksde-20240503/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_locale.c` & `libluksde-20240503/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/Makefile.in` & `libluksde-20240503/libclocale/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -465,14 +465,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -534,30 +536,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -760,24 +763,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -864,17 +873,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libclocale/libclocale_extern.h` & `libluksde-20240503/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_wide_string.h` & `libluksde-20240503/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libclocale/libclocale_codepage.h` & `libluksde-20240503/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_libcdata.h` & `libluksde-20240503/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_types.h` & `libluksde-20240503/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_cache_value.c` & `libluksde-20240503/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_unused.h` & `libluksde-20240503/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/Makefile.am` & `libluksde-20240503/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libluksde-20240114/libfcache/libfcache_support.h` & `libluksde-20240503/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_error.h` & `libluksde-20240503/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_support.c` & `libluksde-20240503/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_cache.h` & `libluksde-20240503/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_error.c` & `libluksde-20240503/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_libcerror.h` & `libluksde-20240503/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_date_time.c` & `libluksde-20240503/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_extern.h` & `libluksde-20240503/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_cache_value.h` & `libluksde-20240503/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/Makefile.in` & `libluksde-20240503/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -557,15 +559,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -769,24 +772,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -874,17 +884,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libfcache/libfcache_date_time.h` & `libluksde-20240503/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcache/libfcache_definitions.h` & `libluksde-20240503/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libluksde-20240114/libfcache/libfcache_cache.c` & `libluksde-20240503/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/Makefile.am` & `libluksde-20240503/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libluksde.pc \
+	libluksde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libluksde.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -94,19 +101,7 @@
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcrypto && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libluksde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libluksde.pc
-	-rm -f libluksde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libluksde-20240114/libluksde.spec` & `libluksde-20240503/libluksde.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libluksde
-Version: 20240114
+Version: 20240503
 Release: 1
 Summary: Library to access the Linux Unified Key Setup (LUKS) Disk Encryption format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libluksde
 Requires:         openssl       
@@ -36,16 +36,16 @@
 
 %description -n libluksde-python3
 Python 3 bindings for libluksde
 
 %package -n libluksde-tools
 Summary: Several tools for reading Linux Unified Key Setup (LUKS) Disk Encryption volumes
 Group: Applications/System
-Requires: libluksde = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libluksde = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libluksde-tools
 Several tools for reading Linux Unified Key Setup (LUKS) Disk Encryption volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libluksde-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sun Jan 14 2024 Joachim Metz <joachim.metz@gmail.com> 20240114-1
+* Fri May  3 2024 Joachim Metz <joachim.metz@gmail.com> 20240503-1
 - Auto-generated
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_range.h` & `libluksde-20240503/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_range_io_handle.c` & `libluksde-20240503/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_support.c` & `libluksde-20240503/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libcpath.h` & `libluksde-20240503/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_error.h` & `libluksde-20240503/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libclocale.h` & `libluksde-20240503/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_error.c` & `libluksde-20240503/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libuna.h` & `libluksde-20240503/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_io_handle.h` & `libluksde-20240503/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_pool.h` & `libluksde-20240503/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_range.c` & `libluksde-20240503/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_types.h` & `libluksde-20240503/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_unused.h` & `libluksde-20240503/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libcdata.h` & `libluksde-20240503/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file.h` & `libluksde-20240503/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/Makefile.am` & `libluksde-20240503/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libluksde-20240114/libbfio/libbfio_libcfile.h` & `libluksde-20240503/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_definitions.h` & `libluksde-20240503/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libluksde-20240114/libbfio/libbfio_codepage.h` & `libluksde-20240503/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_io_handle.c` & `libluksde-20240503/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_support.h` & `libluksde-20240503/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_memory_range.h` & `libluksde-20240503/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_pool.c` & `libluksde-20240503/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file_range_io_handle.h` & `libluksde-20240503/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libcthreads.h` & `libluksde-20240503/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_system_string.h` & `libluksde-20240503/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_memory_range_io_handle.c` & `libluksde-20240503/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_handle.c` & `libluksde-20240503/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_file.c` & `libluksde-20240503/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_handle.h` & `libluksde-20240503/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_memory_range.c` & `libluksde-20240503/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_pool.c` & `libluksde-20240503/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_libcerror.h` & `libluksde-20240503/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/Makefile.in` & `libluksde-20240503/libbfio/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -486,14 +486,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -554,16 +556,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -594,15 +596,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -813,24 +816,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -899,14 +916,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -917,23 +936,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/libbfio/libbfio_system_string.c` & `libluksde-20240503/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_memory_range_io_handle.h` & `libluksde-20240503/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_extern.h` & `libluksde-20240503/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libbfio/libbfio_pool.h` & `libluksde-20240503/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/config.guess` & `libluksde-20240503/config.guess`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/dpkg/copyright` & `libluksde-20240503/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/dpkg/control` & `libluksde-20240503/dpkg/control`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/dpkg/rules` & `libluksde-20240503/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/COPYING.LESSER` & `libluksde-20240503/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/configure` & `libluksde-20240503/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libluksde 20240114.
+# Generated by GNU Autoconf 2.71 for libluksde 20240503.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libluksde'
 PACKAGE_TARNAME='libluksde'
-PACKAGE_VERSION='20240114'
-PACKAGE_STRING='libluksde 20240114'
+PACKAGE_VERSION='20240503'
+PACKAGE_STRING='libluksde 20240503'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libluksde.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1129,14 +1131,16 @@
 libhmac_LIBS
 openssl_CFLAGS
 openssl_LIBS
 libcaes_CFLAGS
 libcaes_LIBS
 libfcrypto_CFLAGS
 libfcrypto_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1679,15 +1683,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libluksde 20240114 to adapt to many kinds of systems.
+\`configure' configures libluksde 20240503 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1750,15 +1754,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libluksde 20240114:";;
+     short | recursive ) echo "Configuration of libluksde 20240503:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1948,14 +1952,17 @@
               C compiler flags for libcaes, overriding pkg-config
   libcaes_LIBS
               linker flags for libcaes, overriding pkg-config
   libfcrypto_CFLAGS
               C compiler flags for libfcrypto, overriding pkg-config
   libfcrypto_LIBS
               linker flags for libfcrypto, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -2018,15 +2025,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libluksde configure 20240114
+libluksde configure 20240503
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2739,15 +2746,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libluksde $as_me 20240114, which was
+It was created by libluksde $as_me 20240503, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4228,15 +4235,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libluksde'
- VERSION='20240114'
+ VERSION='20240503'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23823,15 +23830,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24322,15 +24329,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24472,15 +24480,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24574,15 +24582,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26214,15 +26222,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26276,47 +26284,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26350,15 +26363,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26392,15 +26405,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26435,15 +26448,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26477,15 +26490,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26519,15 +26532,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26561,15 +26574,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26603,15 +26616,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26646,15 +26659,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26688,15 +26701,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26730,15 +26743,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26772,15 +26785,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26814,15 +26827,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26857,15 +26870,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26899,15 +26912,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26941,15 +26954,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26983,15 +26996,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27025,15 +27038,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27068,67 +27081,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27216,15 +27238,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30995,15 +31017,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31028,15 +31051,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31106,15 +31129,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31661,15 +31684,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31825,15 +31849,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31903,15 +31927,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32361,15 +32385,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32424,15 +32449,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32502,15 +32527,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33225,15 +33250,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33258,15 +33284,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33336,15 +33362,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40546,15 +40572,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40579,15 +40606,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40657,15 +40684,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41846,15 +41873,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42168,15 +42196,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42246,15 +42274,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43051,15 +43079,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43249,15 +43278,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43327,15 +43356,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45445,15 +45474,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45478,15 +45508,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45556,15 +45586,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46476,15 +46506,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46577,15 +46608,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46655,15 +46686,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -47237,15 +47268,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -47270,15 +47302,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -47348,15 +47380,15 @@
 printf "%s\n" "$ac_cv_with_libhmac" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno
 then :
   ac_cv_libhmac=no
 else $as_nop
   ac_cv_libhmac=check
-        if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect
+                if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   if test -d "$ac_cv_with_libhmac"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48354,15 +48386,16 @@
 fi
 
 
         ac_cv_libhmac_LIBADD="-lhmac"
 fi
 
 fi
-    if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes
+
+    if test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libhmac in directory: $ac_cv_with_libhmac
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -48468,15 +48501,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -52654,15 +52687,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno
 then :
   ac_cv_libhmac_sha512=local
 else $as_nop
   ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512
 fi
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBHMAC 1" >>confdefs.h
@@ -52732,15 +52765,15 @@
 printf "%s\n" "$ac_cv_with_libcaes" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno
 then :
   ac_cv_libcaes=no
 else $as_nop
   ac_cv_libcaes=check
-        if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect
+                if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   if test -d "$ac_cv_with_libcaes"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53316,15 +53349,16 @@
 fi
 
 
         ac_cv_libcaes_LIBADD="-lcaes"
 fi
 
 fi
-    if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes
+
+    if test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcaes in directory: $ac_cv_with_libcaes
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53422,15 +53456,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56257,15 +56291,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno
 then :
   ac_cv_libcaes_aes_xts=local
 else $as_nop
   ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts
 fi
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCAES 1" >>confdefs.h
@@ -56334,15 +56368,15 @@
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfcrypto" >&5
 printf "%s\n" "$ac_cv_with_libfcrypto" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcrypto" = xno
 then :
   ac_cv_libfcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect
+              if test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_with_libfcrypto" != xyes
 then :
   if test -d "$ac_cv_with_libfcrypto"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcrypto}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcrypto}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56491,440 +56525,14 @@
 then :
   ac_cv_libfcrypto_dummy=yes
 else $as_nop
   ac_cv_libfcrypto=no
 fi
 
 
-                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_blowfish_context_initialize in -lfcrypto" >&5
-printf %s "checking for libfcrypto_blowfish_context_initialize in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_blowfish_context_initialize ();
-int
-main (void)
-{
-return libfcrypto_blowfish_context_initialize ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_initialize" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_blowfish_context_free in -lfcrypto" >&5
-printf %s "checking for libfcrypto_blowfish_context_free in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_blowfish_context_free ();
-int
-main (void)
-{
-return libfcrypto_blowfish_context_free ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_free" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_blowfish_context_set_key in -lfcrypto" >&5
-printf %s "checking for libfcrypto_blowfish_context_set_key in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_blowfish_context_set_key ();
-int
-main (void)
-{
-return libfcrypto_blowfish_context_set_key ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_blowfish_context_set_key" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_blowfish_crypt_cbc in -lfcrypto" >&5
-printf %s "checking for libfcrypto_blowfish_crypt_cbc in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_blowfish_crypt_cbc ();
-int
-main (void)
-{
-return libfcrypto_blowfish_crypt_cbc ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_cbc" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_blowfish_crypt_ecb in -lfcrypto" >&5
-printf %s "checking for libfcrypto_blowfish_crypt_ecb in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_blowfish_crypt_ecb ();
-int
-main (void)
-{
-return libfcrypto_blowfish_crypt_ecb ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_blowfish_crypt_ecb" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
-                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_des3_context_initialize in -lfcrypto" >&5
-printf %s "checking for libfcrypto_des3_context_initialize in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_des3_context_initialize ();
-int
-main (void)
-{
-return libfcrypto_des3_context_initialize ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_des3_context_initialize" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_des3_context_free in -lfcrypto" >&5
-printf %s "checking for libfcrypto_des3_context_free in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_des3_context_free+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_des3_context_free ();
-int
-main (void)
-{
-return libfcrypto_des3_context_free ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_free=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_free=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_des3_context_free" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_des3_context_free" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_des3_context_free" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_des3_context_set_key in -lfcrypto" >&5
-printf %s "checking for libfcrypto_des3_context_set_key in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_des3_context_set_key ();
-int
-main (void)
-{
-return libfcrypto_des3_context_set_key ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_des3_context_set_key" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_des3_crypt_cbc in -lfcrypto" >&5
-printf %s "checking for libfcrypto_des3_crypt_cbc in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_des3_crypt_cbc ();
-int
-main (void)
-{
-return libfcrypto_des3_crypt_cbc ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_des3_crypt_cbc" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_des3_crypt_ecb in -lfcrypto" >&5
-printf %s "checking for libfcrypto_des3_crypt_ecb in -lfcrypto... " >&6; }
-if test ${ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb+y}
-then :
-  printf %s "(cached) " >&6
-else $as_nop
-  ac_check_lib_save_LIBS=$LIBS
-LIBS="-lfcrypto  $LIBS"
-cat confdefs.h - <<_ACEOF >conftest.$ac_ext
-/* end confdefs.h.  */
-
-/* Override any GCC internal prototype to avoid an error.
-   Use char because int might match the return type of a GCC
-   builtin and then its argument prototype would still apply.  */
-char libfcrypto_des3_crypt_ecb ();
-int
-main (void)
-{
-return libfcrypto_des3_crypt_ecb ();
-  ;
-  return 0;
-}
-_ACEOF
-if ac_fn_c_try_link "$LINENO"
-then :
-  ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb=yes
-else $as_nop
-  ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb=no
-fi
-rm -f core conftest.err conftest.$ac_objext conftest.beam \
-    conftest$ac_exeext conftest.$ac_ext
-LIBS=$ac_check_lib_save_LIBS
-fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb" >&5
-printf "%s\n" "$ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb" >&6; }
-if test "x$ac_cv_lib_fcrypto_libfcrypto_des3_crypt_ecb" = xyes
-then :
-  ac_cv_libfcrypto_dummy=yes
-else $as_nop
-  ac_cv_libfcrypto=no
-fi
-
-
                 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfcrypto_rc4_context_initialize in -lfcrypto" >&5
 printf %s "checking for libfcrypto_rc4_context_initialize in -lfcrypto... " >&6; }
 if test ${ac_cv_lib_fcrypto_libfcrypto_rc4_context_initialize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -57305,15 +56913,16 @@
 fi
 
 
         ac_cv_libfcrypto_LIBADD="-lfcrypto"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_libfcrypto" != xyes
+
+    if test "x$ac_cv_libfcrypto" != xyes && test "x$ac_cv_with_libfcrypto" != x && test "x$ac_cv_with_libfcrypto" != xauto-detect && test "x$ac_cv_with_libfcrypto" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcrypto in directory: $ac_cv_with_libfcrypto
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -57338,15 +56947,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfcrypto" != xyes
 then :
 
-  ac_cv_libfcrypto_CPPFLAGS="-I../libfcrypto";
+  ac_cv_libfcrypto_CPPFLAGS="-I../libfcrypto -I\$(top_srcdir)/libfcrypto";
   ac_cv_libfcrypto_LIBADD="../libfcrypto/libfcrypto.la";
 
   ac_cv_libfcrypto=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCRYPTO 1" >>confdefs.h
@@ -57657,16 +57266,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -57824,33 +57437,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -57918,51 +57605,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -58125,45 +57871,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -58331,29 +58070,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -58384,14 +58143,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -58399,14 +58164,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -59364,15 +59137,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libluksde $as_me 20240114, which was
+This file was extended by libluksde $as_me 20240503, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -59432,15 +59205,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libluksde config.status 20240114
+libluksde config.status 20240503
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libluksde-20240114/compile` & `libluksde-20240503/compile`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/missing` & `libluksde-20240503/missing`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksdemount/luksdemount.vcproj` & `libluksde-20240503/msvscpp/luksdemount/luksdemount.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_volume_header/luksde_test_volume_header.vcproj` & `libluksde-20240503/msvscpp/luksde_test_volume_header/luksde_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_notify/luksde_test_notify.vcproj` & `libluksde-20240503/msvscpp/luksde_test_notify/luksde_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_error/luksde_test_error.vcproj` & `libluksde-20240503/msvscpp/luksde_test_error/luksde_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_encryption_context/luksde_test_encryption_context.vcproj` & `libluksde-20240503/msvscpp/luksde_test_encryption_context/luksde_test_encryption_context.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcaes/libcaes.vcproj` & `libluksde-20240503/msvscpp/libcaes/libcaes.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_support/luksde_test_support.vcproj` & `libluksde-20240503/msvscpp/luksde_test_support/luksde_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libfguid/libfguid.vcproj` & `libluksde-20240503/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libclocale/libclocale.vcproj` & `libluksde-20240503/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libfcache/libfcache.vcproj` & `libluksde-20240503/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/Makefile.am` & `libluksde-20240503/msvscpp/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,11 @@
 	luksdemount/luksdemount.vcproj \
 	pyluksde/pyluksde.vcproj \
 	libluksde.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libluksde-20240114/msvscpp/libbfio/libbfio.vcproj` & `libluksde-20240503/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_key_slot/luksde_test_key_slot.vcproj` & `libluksde-20240503/msvscpp/luksde_test_key_slot/luksde_test_key_slot.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcfile/libcfile.vcproj` & `libluksde-20240503/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcdata/libcdata.vcproj` & `libluksde-20240503/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_tools_info_handle/luksde_test_tools_info_handle.vcproj` & `libluksde-20240503/msvscpp/luksde_test_tools_info_handle/luksde_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_sector_data_vector/luksde_test_sector_data_vector.vcproj` & `libluksde-20240503/msvscpp/luksde_test_sector_data_vector/luksde_test_sector_data_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksdeinfo/luksdeinfo.vcproj` & `libluksde-20240503/msvscpp/luksdeinfo/luksdeinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcthreads/libcthreads.vcproj` & `libluksde-20240503/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libfcrypto/libfcrypto.vcproj` & `libluksde-20240503/msvscpp/libfcrypto/libfcrypto.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcpath/libcpath.vcproj` & `libluksde-20240503/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libluksde.sln` & `libluksde-20240503/msvscpp/libluksde.sln`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libhmac/libhmac.vcproj` & `libluksde-20240503/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_io_handle/luksde_test_io_handle.vcproj` & `libluksde-20240503/msvscpp/luksde_test_io_handle/luksde_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_sector_data/luksde_test_sector_data.vcproj` & `libluksde-20240503/msvscpp/luksde_test_sector_data/luksde_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcsplit/libcsplit.vcproj` & `libluksde-20240503/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libuna/libuna.vcproj` & `libluksde-20240503/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/Makefile.in` & `libluksde-20240503/msvscpp/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -403,14 +403,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -510,15 +512,16 @@
 	luksdemount/luksdemount.vcproj \
 	pyluksde/pyluksde.vcproj \
 	libluksde.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -622,23 +625,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -717,13 +722,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/msvscpp/pyluksde/pyluksde.vcproj` & `libluksde-20240503/msvscpp/pyluksde/pyluksde.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_diffuser/luksde_test_diffuser.vcproj` & `libluksde-20240503/msvscpp/luksde_test_diffuser/luksde_test_diffuser.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_tools_output/luksde_test_tools_output.vcproj` & `libluksde-20240503/msvscpp/luksde_test_tools_output/luksde_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_tools_signal/luksde_test_tools_signal.vcproj` & `libluksde-20240503/msvscpp/luksde_test_tools_signal/luksde_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcnotify/libcnotify.vcproj` & `libluksde-20240503/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libcerror/libcerror.vcproj` & `libluksde-20240503/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_volume/luksde_test_volume.vcproj` & `libluksde-20240503/msvscpp/luksde_test_volume/luksde_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/luksde_test_password/luksde_test_password.vcproj` & `libluksde-20240503/msvscpp/luksde_test_password/luksde_test_password.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/msvscpp/libluksde/libluksde.vcproj` & `libluksde-20240503/msvscpp/libluksde/libluksde.vcproj`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_extern.h` & `libluksde-20240503/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_support.h` & `libluksde-20240503/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_unused.h` & `libluksde-20240503/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_notify.h` & `libluksde-20240503/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_support.c` & `libluksde-20240503/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_types.h` & `libluksde-20240503/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/Makefile.am` & `libluksde-20240503/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libluksde-20240114/libcfile/libcfile_notify.c` & `libluksde-20240503/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_system_string.h` & `libluksde-20240503/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_file.h` & `libluksde-20240503/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_libcnotify.h` & `libluksde-20240503/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_system_string.c` & `libluksde-20240503/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_error.h` & `libluksde-20240503/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_libcerror.h` & `libluksde-20240503/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_file.c` & `libluksde-20240503/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_libclocale.h` & `libluksde-20240503/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_winapi.h` & `libluksde-20240503/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/Makefile.in` & `libluksde-20240503/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -560,15 +562,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -773,24 +776,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -879,17 +890,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcfile/libcfile_error.c` & `libluksde-20240503/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_libuna.h` & `libluksde-20240503/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_winapi.c` & `libluksde-20240503/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcfile/libcfile_definitions.h` & `libluksde-20240503/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libluksde-20240114/README` & `libluksde-20240503/README`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/INSTALL` & `libluksde-20240503/INSTALL`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_list_element.h` & `libluksde-20240503/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_array.h` & `libluksde-20240503/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_definitions.h` & `libluksde-20240503/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libluksde-20240114/libcdata/libcdata_libcerror.h` & `libluksde-20240503/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_unused.h` & `libluksde-20240503/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_btree.h` & `libluksde-20240503/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_btree.c` & `libluksde-20240503/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_support.c` & `libluksde-20240503/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_list.c` & `libluksde-20240503/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_extern.h` & `libluksde-20240503/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_list.h` & `libluksde-20240503/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_btree_values_list.h` & `libluksde-20240503/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/Makefile.am` & `libluksde-20240503/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libluksde-20240114/libcdata/libcdata_btree_node.h` & `libluksde-20240503/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_range_list_value.h` & `libluksde-20240503/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_range_list.h` & `libluksde-20240503/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_range_list.c` & `libluksde-20240503/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_array.c` & `libluksde-20240503/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_list_element.c` & `libluksde-20240503/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_libcthreads.h` & `libluksde-20240503/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_tree_node.h` & `libluksde-20240503/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_error.h` & `libluksde-20240503/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_types.h` & `libluksde-20240503/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_btree_node.c` & `libluksde-20240503/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_tree_node.c` & `libluksde-20240503/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_support.h` & `libluksde-20240503/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/Makefile.in` & `libluksde-20240503/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -482,14 +482,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -550,16 +552,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -576,15 +578,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -794,24 +797,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -905,17 +921,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcdata/libcdata_range_list_value.c` & `libluksde-20240503/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_btree_values_list.c` & `libluksde-20240503/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcdata/libcdata_error.c` & `libluksde-20240503/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/config.sub` & `libluksde-20240503/config.sub`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/setup.py` & `libluksde-20240503/setup.py`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/acinclude.m4` & `libluksde-20240503/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/config.rpath` & `libluksde-20240503/config.rpath`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread.h` & `libluksde-20240503/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_read_write_lock.h` & `libluksde-20240503/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread.c` & `libluksde-20240503/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread_pool.h` & `libluksde-20240503/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_support.h` & `libluksde-20240503/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_lock.h` & `libluksde-20240503/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_unused.h` & `libluksde-20240503/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_lock.c` & `libluksde-20240503/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_condition.h` & `libluksde-20240503/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_repeating_thread.h` & `libluksde-20240503/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/Makefile.am` & `libluksde-20240503/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libluksde-20240114/libcthreads/libcthreads_support.c` & `libluksde-20240503/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_mutex.c` & `libluksde-20240503/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_queue.c` & `libluksde-20240503/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_mutex.h` & `libluksde-20240503/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_types.h` & `libluksde-20240503/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread_attributes.h` & `libluksde-20240503/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_condition.c` & `libluksde-20240503/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_error.c` & `libluksde-20240503/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_read_write_lock.c` & `libluksde-20240503/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_libcerror.h` & `libluksde-20240503/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_definitions.h` & `libluksde-20240503/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread_pool.c` & `libluksde-20240503/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_error.h` & `libluksde-20240503/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_thread_attributes.c` & `libluksde-20240503/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_extern.h` & `libluksde-20240503/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/libcthreads_repeating_thread.c` & `libluksde-20240503/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcthreads/Makefile.in` & `libluksde-20240503/libcthreads/Makefile.in`

 * *Files 11% similar despite different names*

```diff
@@ -486,14 +486,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -554,16 +556,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -578,15 +580,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -796,24 +799,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -907,17 +923,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcthreads/libcthreads_queue.h` & `libluksde-20240503/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_blowfish_context.h` & `libluksde-20240503/libfcrypto/libfcrypto_blowfish_context.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_extern.h` & `libluksde-20240503/libfcrypto/libfcrypto_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_blowfish_context.c` & `libluksde-20240503/libfcrypto/libfcrypto_blowfish_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_types.h` & `libluksde-20240503/libfcrypto/libfcrypto_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_rc4_context.h` & `libluksde-20240503/libfcrypto/libfcrypto_rc4_context.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_support.c` & `libluksde-20240503/libfcrypto/libfcrypto_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_definitions.h` & `libluksde-20240503/libfcrypto/libfcrypto_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfcrypto/definitions.h> are copied here
  * for local use of libfcrypto
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFCRYPTO_VERSION			20240114
+#define LIBFCRYPTO_VERSION			20240414
 
 /* The version string
  */
-#define LIBFCRYPTO_VERSION_STRING		"20240114"
+#define LIBFCRYPTO_VERSION_STRING		"20240414"
 
 /* The crypt modes
  */
 enum LIBFCRYPTO_CRYPT_MODES
 {
 	LIBFCRYPTO_CRYPT_MODE_DECRYPT		= 0,
 	LIBFCRYPTO_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_rc4_context.c` & `libluksde-20240503/libfcrypto/libfcrypto_rc4_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/Makefile.am` & `libluksde-20240503/libfcrypto/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCRYPTO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcrypto.la
 
 libfcrypto_la_SOURCES = \
 	libfcrypto_blowfish_context.c libfcrypto_blowfish_context.h \
 	libfcrypto_definitions.h \
@@ -16,19 +16,17 @@
 	libfcrypto_rc4_context.c libfcrypto_rc4_context.h \
 	libfcrypto_serpent_context.c libfcrypto_serpent_context.h \
 	libfcrypto_support.c libfcrypto_support.h \
 	libfcrypto_types.h \
 	libfcrypto_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcrypto ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcrypto_la_SOURCES)
```

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_serpent_context.h` & `libluksde-20240503/libfcrypto/libfcrypto_serpent_context.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_serpent_context.c` & `libluksde-20240503/libfcrypto/libfcrypto_serpent_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_des3_context.c` & `libluksde-20240503/libfcrypto/libfcrypto_des3_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_des3_context.h` & `libluksde-20240503/libfcrypto/libfcrypto_des3_context.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_error.c` & `libluksde-20240503/libfcrypto/libfcrypto_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_support.h` & `libluksde-20240503/libfcrypto/libfcrypto_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_error.h` & `libluksde-20240503/libfcrypto/libfcrypto_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_libcerror.h` & `libluksde-20240503/libfcrypto/libfcrypto_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libfcrypto/Makefile.in` & `libluksde-20240503/libfcrypto/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -539,16 +541,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCRYPTO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCRYPTO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCRYPTO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCRYPTO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@noinst_LTLIBRARIES = libfcrypto.la
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@libfcrypto_la_SOURCES = \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_blowfish_context.c libfcrypto_blowfish_context.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_definitions.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_des3_context.c libfcrypto_des3_context.h \
@@ -557,15 +559,16 @@
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_libcerror.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_rc4_context.c libfcrypto_rc4_context.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_serpent_context.c libfcrypto_serpent_context.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_support.c libfcrypto_support.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_types.h \
 @HAVE_LOCAL_LIBFCRYPTO_TRUE@	libfcrypto_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -770,24 +773,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcrypto_blowfish_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_des3_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_error.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_rc4_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_serpent_context.Plo
+	-rm -f ./$(DEPDIR)/libfcrypto_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -876,17 +887,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcrypto ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcrypto_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libfcrypto/libfcrypto_unused.h` & `libluksde-20240503/libfcrypto/libfcrypto_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/test-driver` & `libluksde-20240503/test-driver`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_support.c` & `libluksde-20240503/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_libcerror.h` & `libluksde-20240503/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_definitions.h` & `libluksde-20240503/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libluksde-20240114/libcpath/Makefile.am` & `libluksde-20240503/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libluksde-20240114/libcpath/libcpath_error.c` & `libluksde-20240503/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_extern.h` & `libluksde-20240503/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_system_string.h` & `libluksde-20240503/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_support.h` & `libluksde-20240503/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_libcsplit.h` & `libluksde-20240503/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_system_string.c` & `libluksde-20240503/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_libclocale.h` & `libluksde-20240503/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_error.h` & `libluksde-20240503/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/Makefile.in` & `libluksde-20240503/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -462,14 +462,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -530,16 +532,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -551,15 +553,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +765,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -866,17 +875,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcpath/libcpath_libuna.h` & `libluksde-20240503/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_unused.h` & `libluksde-20240503/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_path.c` & `libluksde-20240503/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcpath/libcpath_path.h` & `libluksde-20240503/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/ChangeLog` & `libluksde-20240503/ChangeLog`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/manuals/luksdemount.1` & `libluksde-20240503/manuals/luksdemount.1`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/manuals/libluksde.3` & `libluksde-20240503/manuals/libluksde.3`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/manuals/luksdeinfo.1` & `libluksde-20240503/manuals/luksdeinfo.1`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/manuals/Makefile.in` & `libluksde-20240503/manuals/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,15 +514,16 @@
 	libluksde.3
 
 EXTRA_DIST = \
 	luksdeinfo.1 \
 	luksdemount.1 \
 	libluksde.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -713,23 +716,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -811,13 +816,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/tests/luksde_test_encryption_context.c` & `libluksde-20240503/tests/luksde_test_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_password.c` & `libluksde-20240503/tests/luksde_test_password.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_tools_signal.c` & `libluksde-20240503/tests/luksde_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/pyluksde_test_volume.py` & `libluksde-20240503/tests/pyluksde_test_volume.py`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_libcnotify.h` & `libluksde-20240503/tests/luksde_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_volume_header.c` & `libluksde-20240503/tests/luksde_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_libuna.h` & `libluksde-20240503/tests/luksde_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_memory.h` & `libluksde-20240503/tests/luksde_test_memory.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/test_luksdeinfo.sh` & `libluksde-20240503/tests/test_luksdeinfo.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("luksdeinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libluksde-20240114/tests/test_tools.sh` & `libluksde-20240503/tests/test_tools.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libluksde-20240114/tests/luksde_test_tools_output.c` & `libluksde-20240503/tests/luksde_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_libbfio.h` & `libluksde-20240503/tests/luksde_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_volume.c` & `libluksde-20240503/tests/luksde_test_volume.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/Makefile.am` & `libluksde-20240503/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -300,13 +300,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libluksde/libluksde.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libluksde-20240114/tests/luksde_test_memory.c` & `libluksde-20240503/tests/luksde_test_memory.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_io_handle.c` & `libluksde-20240503/tests/luksde_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_getopt.h` & `libluksde-20240503/tests/luksde_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_macros.h` & `libluksde-20240503/tests/luksde_test_macros.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_key_slot.c` & `libluksde-20240503/tests/luksde_test_key_slot.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_notify.c` & `libluksde-20240503/tests/luksde_test_notify.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/test_python_module.sh` & `libluksde-20240503/tests/test_python_module.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="volume";
 OPTION_SETS=("password");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libluksde";
+PYTHON_MODULE="pyluksde";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyluksde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyluksde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -45,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyluksde");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -120,38 +124,47 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +177,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libluksde-20240114/tests/luksde_test_libclocale.h` & `libluksde-20240503/tests/luksde_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_libcerror.h` & `libluksde-20240503/tests/luksde_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_error.c` & `libluksde-20240503/tests/luksde_test_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_functions.h` & `libluksde-20240503/tests/luksde_test_functions.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_getopt.c` & `libluksde-20240503/tests/luksde_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_unused.h` & `libluksde-20240503/tests/luksde_test_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_sector_data.c` & `libluksde-20240503/tests/luksde_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/test_runner.sh` & `libluksde-20240503/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_functions.c` & `libluksde-20240503/tests/luksde_test_functions.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_sector_data_vector.c` & `libluksde-20240503/tests/luksde_test_sector_data_vector.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_diffuser.c` & `libluksde-20240503/tests/luksde_test_diffuser.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_tools_info_handle.c` & `libluksde-20240503/tests/luksde_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/luksde_test_support.c` & `libluksde-20240503/tests/luksde_test_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/Makefile.in` & `libluksde-20240503/tests/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -786,14 +786,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -855,16 +857,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1139,16 +1141,18 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libluksde/libluksde.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1635,24 +1639,48 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../luksdetools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../luksdetools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../luksdetools/$(DEPDIR)/info_handle.Po
+	-rm -f ../luksdetools/$(DEPDIR)/luksdetools_input.Po
+	-rm -f ../luksdetools/$(DEPDIR)/luksdetools_output.Po
+	-rm -f ../luksdetools/$(DEPDIR)/luksdetools_signal.Po
+	-rm -f ./$(DEPDIR)/luksde_test_diffuser.Po
+	-rm -f ./$(DEPDIR)/luksde_test_encryption_context.Po
+	-rm -f ./$(DEPDIR)/luksde_test_error.Po
+	-rm -f ./$(DEPDIR)/luksde_test_functions.Po
+	-rm -f ./$(DEPDIR)/luksde_test_getopt.Po
+	-rm -f ./$(DEPDIR)/luksde_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/luksde_test_key_slot.Po
+	-rm -f ./$(DEPDIR)/luksde_test_memory.Po
+	-rm -f ./$(DEPDIR)/luksde_test_notify.Po
+	-rm -f ./$(DEPDIR)/luksde_test_password.Po
+	-rm -f ./$(DEPDIR)/luksde_test_sector_data.Po
+	-rm -f ./$(DEPDIR)/luksde_test_sector_data_vector.Po
+	-rm -f ./$(DEPDIR)/luksde_test_support.Po
+	-rm -f ./$(DEPDIR)/luksde_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/luksde_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/luksde_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/luksde_test_volume.Po
+	-rm -f ./$(DEPDIR)/luksde_test_volume_header.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1757,13 +1785,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/tests/luksde_test_libluksde.h` & `libluksde-20240503/tests/luksde_test_libluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/pyluksde_test_support.py` & `libluksde-20240503/tests/pyluksde_test_support.py`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/tests/test_library.sh` & `libluksde-20240503/tests/test_library.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="diffuser encryption_context error io_handle key_slot notify password sector_data sector_data_vector volume_header";
 LIBRARY_TESTS_WITH_INPUT="support volume";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libluksde-20240114/libluksde.spec.in` & `libluksde-20240503/libluksde.spec.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/ossfuzz/volume_fuzzer.cc` & `libluksde-20240503/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/ossfuzz/ossfuzz_libluksde.h` & `libluksde-20240503/ossfuzz/ossfuzz_libluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/ossfuzz/Makefile.am` & `libluksde-20240503/ossfuzz/Makefile.am`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libluksde/libluksde.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libluksde-20240114/ossfuzz/ossfuzz_libbfio.h` & `libluksde-20240503/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/ossfuzz/Makefile.in` & `libluksde-20240503/ossfuzz/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -475,14 +475,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -543,16 +545,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -572,15 +574,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libluksde/libluksde.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -822,23 +825,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -922,17 +928,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/ltmain.sh` & `libluksde-20240503/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libhmac/libhmac_sha1_context.c` & `libluksde-20240503/libhmac/libhmac_sha1_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha224.h` & `libluksde-20240503/libhmac/libhmac_sha224.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha512_context.c` & `libluksde-20240503/libhmac/libhmac_sha512_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_extern.h` & `libluksde-20240503/libhmac/libhmac_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_md5.c` & `libluksde-20240503/libhmac/libhmac_md5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_md5.h` & `libluksde-20240503/libhmac/libhmac_md5.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_error.h` & `libluksde-20240503/libhmac/libhmac_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_types.h` & `libluksde-20240503/libhmac/libhmac_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_byte_stream.h` & `libluksde-20240503/libhmac/libhmac_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha512.c` & `libluksde-20240503/libhmac/libhmac_sha512.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha256_context.c` & `libluksde-20240503/libhmac/libhmac_sha256_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha224.c` & `libluksde-20240503/libhmac/libhmac_sha224.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_definitions.h` & `libluksde-20240503/libhmac/libhmac_definitions.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20231127
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20231127"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libluksde-20240114/libhmac/libhmac_unused.h` & `libluksde-20240503/libhmac/libhmac_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha1.h` & `libluksde-20240503/libhmac/libhmac_sha1.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha256_context.h` & `libluksde-20240503/libhmac/libhmac_sha256_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/Makefile.am` & `libluksde-20240503/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBHMAC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libhmac.la
 
 libhmac_la_SOURCES = \
@@ -25,19 +25,17 @@
 	libhmac_sha512.c libhmac_sha512.h \
 	libhmac_sha512_context.c libhmac_sha512_context.h \
 	libhmac_support.c libhmac_support.h \
 	libhmac_types.h \
 	libhmac_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha224_context.c` & `libluksde-20240503/libhmac/libhmac_sha224_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_md5_context.h` & `libluksde-20240503/libhmac/libhmac_md5_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha256.c` & `libluksde-20240503/libhmac/libhmac_sha256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha1_context.h` & `libluksde-20240503/libhmac/libhmac_sha1_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_libcerror.h` & `libluksde-20240503/pyluksde/pyluksde_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBHMAC_LIBCERROR_H )
-#define _LIBHMAC_LIBCERROR_H
+#if !defined( _PYLUKSDE_LIBCERROR_H )
+#define _PYLUKSDE_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
+#endif /* !defined( _PYLUKSDE_LIBCERROR_H ) */
```

### Comparing `libluksde-20240114/libhmac/libhmac_error.c` & `libluksde-20240503/libhmac/libhmac_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_support.h` & `libluksde-20240503/libhmac/libhmac_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/Makefile.in` & `libluksde-20240503/libhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -485,14 +485,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -553,16 +555,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBHMAC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCRYPTO_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBHMAC_TRUE@noinst_LTLIBRARIES = libhmac.la
 @HAVE_LOCAL_LIBHMAC_TRUE@libhmac_la_SOURCES = \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_byte_stream.h \
@@ -580,15 +582,16 @@
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha256_context.c libhmac_sha256_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512.c libhmac_sha512.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512_context.c libhmac_sha512_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_support.c libhmac_support.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_types.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -799,24 +802,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -911,17 +928,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha256.h` & `libluksde-20240503/libhmac/libhmac_sha256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha224_context.h` & `libluksde-20240503/libhmac/libhmac_sha224_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha512_context.h` & `libluksde-20240503/libhmac/libhmac_sha512_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha512.h` & `libluksde-20240503/libhmac/libhmac_sha512.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_support.c` & `libluksde-20240503/libuna/libuna_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libhmac_definitions.h"
-#include "libhmac_support.h"
+#include "libuna_definitions.h"
+#include "libuna_support.h"
 
-#if !defined( HAVE_LOCAL_LIBHMAC )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
 /* Returns the library version as a string
  */
-const char *libhmac_get_version(
+const char *libuna_get_version(
              void )
 {
-	return( (const char *) LIBHMAC_VERSION_STRING );
+	return( (const char *) LIBUNA_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
```

### Comparing `libluksde-20240114/libhmac/libhmac_sha1.c` & `libluksde-20240503/libhmac/libhmac_sha1.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libhmac/libhmac_md5_context.c` & `libluksde-20240503/libhmac/libhmac_md5_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libcsplit/libcsplit_narrow_string.c` & `libluksde-20240503/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_definitions.h` & `libluksde-20240503/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libluksde-20240114/libcsplit/libcsplit_types.h` & `libluksde-20240503/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_wide_split_string.c` & `libluksde-20240503/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_support.h` & `libluksde-20240503/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/Makefile.am` & `libluksde-20240503/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libluksde-20240114/libcsplit/libcsplit_libcerror.h` & `libluksde-20240503/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_wide_string.c` & `libluksde-20240503/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_unused.h` & `libluksde-20240503/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_wide_split_string.h` & `libluksde-20240503/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_error.c` & `libluksde-20240503/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_narrow_split_string.c` & `libluksde-20240503/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_extern.h` & `libluksde-20240503/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_error.h` & `libluksde-20240503/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_support.c` & `libluksde-20240503/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_wide_string.h` & `libluksde-20240503/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/Makefile.in` & `libluksde-20240503/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -540,16 +542,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -558,15 +560,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -771,24 +774,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -877,17 +888,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcsplit/libcsplit_narrow_split_string.h` & `libluksde-20240503/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcsplit/libcsplit_narrow_string.h` & `libluksde-20240503/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/remove-potcdate.sin` & `libluksde-20240503/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/Makefile.in.in` & `libluksde-20240503/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/en@quot.header` & `libluksde-20240503/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/en@boldquot.header` & `libluksde-20240503/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/insert-header.sin` & `libluksde-20240503/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/Makevars` & `libluksde-20240503/po/Makevars`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/Makevars.in` & `libluksde-20240503/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/po/Rules-quot` & `libluksde-20240503/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1251.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1251.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf16_string.c` & `libluksde-20240503/libuna/libuna_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base16_stream.c` & `libluksde-20240503/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf8_stream.h` & `libluksde-20240503/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_2.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_932.c` & `libluksde-20240503/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_dingbats.h` & `libluksde-20240503/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf8_string.c` & `libluksde-20240503/libuna/libuna_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base64_stream.c` & `libluksde-20240503/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_error.h` & `libluksde-20240503/libuna/libuna_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_turkish.h` & `libluksde-20240503/libuna/libuna_codepage_mac_turkish.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_unicode_character.c` & `libluksde-20240503/libuna/libuna_unicode_character.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_gaelic.c` & `libluksde-20240503/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_arabic.h` & `libluksde-20240503/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_thai.c` & `libluksde-20240503/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_874.h` & `libluksde-20240503/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_15.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-15 codepage (Latin 9) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_15_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_utf8_string.h` & `libluksde-20240503/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_16.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1255.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf7_stream.c` & `libluksde-20240503/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_byte_stream.h` & `libluksde-20240503/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_koi8_u.c` & `libluksde-20240503/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_unused.h` & `libluksde-20240503/libuna/libuna_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_6.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_14.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base64_stream.h` & `libluksde-20240503/libuna/libuna_base64_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_error.c` & `libluksde-20240503/libuna/libuna_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_centraleurroman.h` & `libluksde-20240503/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_romanian.c` & `libluksde-20240503/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_6.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_9.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_russian.h` & `libluksde-20240503/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_dingbats.c` & `libluksde-20240503/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_15.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_936.c` & `libluksde-20240503/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_croatian.h` & `libluksde-20240503/libuna/libuna_codepage_mac_croatian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_scsu.h` & `libluksde-20240503/libuna/libuna_scsu.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/Makefile.am` & `libluksde-20240503/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,17 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libluksde-20240114/libuna/libuna_utf32_stream.c` & `libluksde-20240503/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_936.h` & `libluksde-20240503/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_10.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_roman.c` & `libluksde-20240503/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf7_stream.h` & `libluksde-20240503/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_3.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_thai.h` & `libluksde-20240503/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_farsi.h` & `libluksde-20240503/libuna/libuna_codepage_mac_farsi.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_ukrainian.c` & `libluksde-20240503/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_inuit.c` & `libluksde-20240503/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_932.h` & `libluksde-20240503/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_874.c` & `libluksde-20240503/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_5.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_10.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_definitions.h` & `libluksde-20240503/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20230710
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20230710"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libluksde-20240114/libuna/libuna_url_stream.h` & `libluksde-20240503/libuna/libuna_url_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_icelandic.h` & `libluksde-20240503/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_koi8_u.h` & `libluksde-20240503/libuna/libuna_codepage_koi8_u.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf16_stream.c` & `libluksde-20240503/libuna/libuna_utf16_stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1253.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_4.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_greek.c` & `libluksde-20240503/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_libcerror.h` & `libluksde-20240503/libuna/libuna_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_centraleurroman.c` & `libluksde-20240503/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1254.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_13.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_7.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1255.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1251.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1255 codepage (Hebrew) functions
+ * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1255_copy_from_byte_stream(
+int libuna_codepage_windows_1251_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1255_copy_to_byte_stream(
+int libuna_codepage_windows_1251_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_unicode_character.h` & `libluksde-20240503/libuna/libuna_unicode_character.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_8.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_13.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_949.h` & `libluksde-20240503/libuna/libuna_codepage_windows_949.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_cyrillic.c` & `libluksde-20240503/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_celtic.c` & `libluksde-20240503/libuna/libuna_codepage_mac_celtic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_support.h` & `libluksde-20240503/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_4.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_949.c` & `libluksde-20240503/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf16_stream.h` & `libluksde-20240503/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_symbol.c` & `libluksde-20240503/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_roman.h` & `libluksde-20240503/libuna/libuna_codepage_mac_roman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1257.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1254.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1254.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_950.c` & `libluksde-20240503/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_extern.h` & `libluksde-20240503/libuna/libuna_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1256.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_types.h` & `libluksde-20240503/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base32_stream.h` & `libluksde-20240503/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1253.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_16.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf8_stream.c` & `libluksde-20240503/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1250.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1250.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_2.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_support.c` & `libluksde-20240503/libcerror/libcerror_support.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libuna_definitions.h"
-#include "libuna_support.h"
+#include "libcerror_definitions.h"
+#include "libcerror_support.h"
 
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBCERROR )
 
 /* Returns the library version as a string
  */
-const char *libuna_get_version(
+const char *libcerror_get_version(
              void )
 {
-	return( (const char *) LIBUNA_VERSION_STRING );
+	return( (const char *) LIBCERROR_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_koi8_r.c` & `libluksde-20240503/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_5.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_15_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_utf16_string.h` & `libluksde-20240503/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf32_string.c` & `libluksde-20240503/libuna/libuna_utf32_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_icelandic.c` & `libluksde-20240503/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1256.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_utf32_string.h` & `libluksde-20240503/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_romanian.h` & `libluksde-20240503/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
+#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_8.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_koi8_r.h` & `libluksde-20240503/libuna/libuna_codepage_koi8_r.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_cyrillic.h` & `libluksde-20240503/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCyrillic codepage functions
+ * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
-#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
+#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
+int libuna_codepage_mac_gaelic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
+int libuna_codepage_mac_gaelic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_arabic.c` & `libluksde-20240503/libuna/libuna_codepage_mac_arabic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_croatian.c` & `libluksde-20240503/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_9.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_greek.h` & `libluksde-20240503/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1258.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1258.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_7.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/Makefile.in` & `libluksde-20240503/libuna/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -640,14 +640,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -708,16 +710,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -783,15 +785,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1053,24 +1056,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1190,14 +1258,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -1208,23 +1278,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_3.c` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1250.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_scsu.c` & `libluksde-20240503/libuna/libuna_scsu.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1252.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1252.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_turkish.c` & `libluksde-20240503/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_ukrainian.h` & `libluksde-20240503/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_russian.c` & `libluksde-20240503/libuna/libuna_codepage_mac_russian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1258.c` & `libluksde-20240503/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_celtic.h` & `libluksde-20240503/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_byte_stream.c` & `libluksde-20240503/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_gaelic.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1257.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacGaelic codepage functions
+ * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
-#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_gaelic_copy_from_byte_stream(
+int libuna_codepage_windows_1257_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_gaelic_copy_to_byte_stream(
+int libuna_codepage_windows_1257_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_utf32_stream.h` & `libluksde-20240503/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_symbol.h` & `libluksde-20240503/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1257.h` & `libluksde-20240503/libuna/libuna_codepage_mac_inuit.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1257 codepage (Baltic) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1257_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1257_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_inuit.h` & `libluksde-20240503/libuna/libuna_codepage_mac_romanian.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacInuit codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_mac_farsi.c` & `libluksde-20240503/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_950.h` & `libluksde-20240503/libuna/libuna_codepage_windows_950.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_url_stream.c` & `libluksde-20240503/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1251.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1255.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1251 codepage (Cyrillic) functions
+ * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1251_copy_from_byte_stream(
+int libuna_codepage_windows_1255_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1251_copy_to_byte_stream(
+int libuna_codepage_windows_1255_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_windows_1252.h` & `libluksde-20240503/libuna/libuna_codepage_windows_1252.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_codepage_iso_8859_14.h` & `libluksde-20240503/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base16_stream.h` & `libluksde-20240503/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/libuna/libuna_base32_stream.c` & `libluksde-20240503/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libluksde-20240114/Makefile.in` & `libluksde-20240503/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -522,14 +522,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -654,16 +656,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libluksde.pc \
+	libluksde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libluksde.pc
 
 all: all-recursive
 
@@ -1080,23 +1089,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1209,22 +1221,10 @@
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcrypto && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libluksde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libluksde.pc
-	-rm -f libluksde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/pyluksde/pyluksde_libluksde.h` & `libluksde-20240503/pyluksde/pyluksde_libluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_libfguid.h` & `libluksde-20240503/pyluksde/pyluksde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_python.h` & `libluksde-20240503/pyluksde/pyluksde_python.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_guid.c` & `libluksde-20240503/pyluksde/pyluksde_guid.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde.c` & `libluksde-20240503/pyluksde/pyluksde.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_guid.h` & `libluksde-20240503/pyluksde/pyluksde_guid.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/Makefile.am` & `libluksde-20240503/pyluksde/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -47,13 +47,11 @@
 	@LIBFGUID_LIBADD@
 
 pyluksde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyluksde_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libluksde-20240114/pyluksde/pyluksde_initialization_vector_modes.h` & `libluksde-20240503/pyluksde/pyluksde_initialization_vector_modes.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_libclocale.h` & `libluksde-20240503/pyluksde/pyluksde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_error.c` & `libluksde-20240503/pyluksde/pyluksde_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde.h` & `libluksde-20240503/pyluksde/pyluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_libcerror.h` & `libluksde-20240503/libluksde/libluksde_libcerror.h`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _PYLUKSDE_LIBCERROR_H )
-#define _PYLUKSDE_LIBCERROR_H
+#if !defined( _LIBLUKSDE_LIBCERROR_H )
+#define _LIBLUKSDE_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _PYLUKSDE_LIBCERROR_H ) */
+#endif /* !defined( _LIBLUKSDE_LIBCERROR_H ) */
```

### Comparing `libluksde-20240114/pyluksde/pyluksde_file_object_io_handle.c` & `libluksde-20240503/pyluksde/pyluksde_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_hashing_methods.c` & `libluksde-20240503/pyluksde/pyluksde_hashing_methods.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_initialization_vector_modes.c` & `libluksde-20240503/pyluksde/pyluksde_initialization_vector_modes.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_encryption_methods.h` & `libluksde-20240503/pyluksde/pyluksde_encryption_methods.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_file_object_io_handle.h` & `libluksde-20240503/pyluksde/pyluksde_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_integer.h` & `libluksde-20240503/pyluksde/pyluksde_integer.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_error.h` & `libluksde-20240503/pyluksde/pyluksde_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_encryption_chaining_modes.c` & `libluksde-20240503/pyluksde/pyluksde_encryption_chaining_modes.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_volume.c` & `libluksde-20240503/pyluksde/pyluksde_volume.c`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,22 @@
 	  "unlock() -> Boolean\n"
 	  "\n"
 	  "Unlocks the volume." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyluksde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyluksde_volume_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyluksde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -120,15 +120,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset within the data." },
 
 	{ "read",
 	  (PyCFunction) pyluksde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyluksde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libluksde-20240114/pyluksde/Makefile.in` & `libluksde-20240503/pyluksde/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -517,14 +517,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -585,16 +587,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -632,15 +634,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyluksde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyluksde_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -946,24 +949,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_encryption_chaining_modes.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_encryption_methods.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_error.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_guid.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_hashing_methods.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_initialization_vector_modes.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_integer.Plo
+	-rm -f ./$(DEPDIR)/pyluksde_la-pyluksde_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1057,13 +1072,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libluksde-20240114/pyluksde/pyluksde_hashing_methods.h` & `libluksde-20240503/pyluksde/pyluksde_hashing_methods.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_integer.c` & `libluksde-20240503/pyluksde/pyluksde_integer.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_unused.h` & `libluksde-20240503/pyluksde/pyluksde_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_encryption_chaining_modes.h` & `libluksde-20240503/pyluksde/pyluksde_encryption_chaining_modes.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_libbfio.h` & `libluksde-20240503/pyluksde/pyluksde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_encryption_methods.c` & `libluksde-20240503/pyluksde/pyluksde_encryption_methods.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/pyluksde/pyluksde_volume.h` & `libluksde-20240503/pyluksde/pyluksde_volume.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libcpath.h` & `libluksde-20240503/luksdetools/luksdetools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_unused.h` & `libluksde-20240503/luksdetools/luksdetools_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_dokan.c` & `libluksde-20240503/luksdetools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_file_system.h` & `libluksde-20240503/luksdetools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_signal.h` & `libluksde-20240503/luksdetools/luksdetools_signal.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libfguid.h` & `libluksde-20240503/luksdetools/luksdetools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_fuse.c` & `libluksde-20240503/luksdetools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/info_handle.h` & `libluksde-20240503/luksdetools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_dokan.h` & `libluksde-20240503/luksdetools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_input.h` & `libluksde-20240503/luksdetools/luksdetools_input.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libcdata.h` & `libluksde-20240503/luksdetools/luksdetools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_file_system.c` & `libluksde-20240503/luksdetools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_output.h` & `libluksde-20240503/luksdetools/luksdetools_output.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/Makefile.am` & `libluksde-20240503/luksdetools/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -84,19 +84,17 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libluksde/libluksde.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on luksdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(luksdeinfo_SOURCES)
 	@echo "Running splint on luksdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(luksdemount_SOURCES)
```

### Comparing `libluksde-20240114/luksdetools/mount_file_entry.c` & `libluksde-20240503/luksdetools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/info_handle.c` & `libluksde-20240503/luksdetools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_file_entry.h` & `libluksde-20240503/luksdetools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_input.c` & `libluksde-20240503/luksdetools/luksdetools_input.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libcsplit.h` & `libluksde-20240503/luksdetools/luksdetools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libcnotify.h` & `libluksde-20240503/luksdetools/luksdetools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_signal.c` & `libluksde-20240503/luksdetools/luksdetools_signal.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libluksde.h` & `libluksde-20240503/luksdetools/luksdetools_libluksde.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libcerror.h` & `libluksde-20240503/luksdetools/luksdetools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_handle.h` & `libluksde-20240503/luksdetools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libbfio.h` & `libluksde-20240503/luksdetools/luksdetools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_i18n.h` & `libluksde-20240503/luksdetools/luksdetools_i18n.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libuna.h` & `libluksde-20240503/luksdetools/luksdetools_libuna.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_libclocale.h` & `libluksde-20240503/luksdetools/luksdetools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_getopt.c` & `libluksde-20240503/luksdetools/luksdetools_getopt.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_handle.c` & `libluksde-20240503/luksdetools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/Makefile.in` & `libluksde-20240503/luksdetools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -539,16 +541,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -623,15 +625,16 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libluksde/libluksde.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -888,23 +891,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/luksdeinfo.Po
+	-rm -f ./$(DEPDIR)/luksdemount.Po
+	-rm -f ./$(DEPDIR)/luksdetools_getopt.Po
+	-rm -f ./$(DEPDIR)/luksdetools_input.Po
+	-rm -f ./$(DEPDIR)/luksdetools_output.Po
+	-rm -f ./$(DEPDIR)/luksdetools_signal.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -999,17 +1016,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on luksdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(luksdeinfo_SOURCES)
 	@echo "Running splint on luksdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(luksdemount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/luksdetools/luksdetools_getopt.h` & `libluksde-20240503/luksdetools/luksdetools_getopt.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdetools_output.c` & `libluksde-20240503/luksdetools/luksdetools_output.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdeinfo.c` & `libluksde-20240503/luksdetools/luksdeinfo.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/mount_fuse.h` & `libluksde-20240503/luksdetools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/luksdetools/luksdemount.c` & `libluksde-20240503/luksdetools/luksdemount.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_definitions.h` & `libluksde-20240503/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libluksde-20240114/libcnotify/libcnotify_extern.h` & `libluksde-20240503/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_support.c` & `libluksde-20240503/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_stream.h` & `libluksde-20240503/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/Makefile.am` & `libluksde-20240503/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libluksde-20240114/libcnotify/libcnotify_unused.h` & `libluksde-20240503/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_verbose.h` & `libluksde-20240503/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_print.h` & `libluksde-20240503/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_stream.c` & `libluksde-20240503/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_support.h` & `libluksde-20240503/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_verbose.c` & `libluksde-20240503/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/Makefile.in` & `libluksde-20240503/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -464,14 +464,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -532,30 +534,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -758,24 +761,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -862,17 +871,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libcnotify/libcnotify_libcerror.h` & `libluksde-20240503/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcnotify/libcnotify_print.c` & `libluksde-20240503/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_system.c` & `libluksde-20240503/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_error.c` & `libluksde-20240503/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_extern.h` & `libluksde-20240503/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/Makefile.am` & `libluksde-20240503/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libluksde-20240114/libcerror/libcerror_types.h` & `libluksde-20240503/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_support.h` & `libluksde-20240503/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_error.h` & `libluksde-20240503/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_system.h` & `libluksde-20240503/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/libcerror_definitions.h` & `libluksde-20240503/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libluksde-20240114/libcerror/libcerror_support.c` & `libluksde-20240503/libluksde/libluksde_libcnotify.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Support functions
+ * The libcnotify header wrapper
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,25 +15,36 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
+#if !defined( _LIBLUKSDE_LIBCNOTIFY_H )
+#define _LIBLUKSDE_LIBCNOTIFY_H
+
 #include <common.h>
-#include <types.h>
 
-#include "libcerror_definitions.h"
-#include "libcerror_support.h"
+/* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
+ */
+#if defined( HAVE_LOCAL_LIBCNOTIFY )
+
+#include <libcnotify_definitions.h>
+#include <libcnotify_print.h>
+#include <libcnotify_stream.h>
+#include <libcnotify_verbose.h>
 
-#if !defined( HAVE_LOCAL_LIBCERROR )
+#else
 
-/* Returns the library version as a string
+/* If libtool DLL support is enabled set LIBCNOTIFY_DLL_IMPORT
+ * before including libcnotify.h
  */
-const char *libcerror_get_version(
-             void )
-{
-	return( (const char *) LIBCERROR_VERSION_STRING );
-}
+#if defined( _WIN32 ) && defined( DLL_IMPORT )
+#define LIBCNOTIFY_DLL_IMPORT
+#endif
+
+#include <libcnotify.h>
+
+#endif /* defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
+#endif /* !defined( _LIBLUKSDE_LIBCNOTIFY_H ) */
```

### Comparing `libluksde-20240114/libcerror/libcerror_unused.h` & `libluksde-20240503/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libcerror/Makefile.in` & `libluksde-20240503/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,28 +531,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -752,24 +755,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -855,17 +863,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/aclocal.m4` & `libluksde-20240503/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/configure.ac` & `libluksde-20240503/configure.ac`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libluksde],
- [20240114],
+ [20240503],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libluksde.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

### Comparing `libluksde-20240114/libluksde/libluksde.rc` & `libluksde-20240503/libluksde/libluksde.rc`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Linux Unified Key Setup (LUKS) Disk Encryption format\0"
-      VALUE "FileVersion",		"20240114" "\0"
+      VALUE "FileVersion",		"20240503" "\0"
       VALUE "InternalName",		"libluksde.dll\0"
       VALUE "LegalCopyright",		"(C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libluksde.dll\0"
       VALUE "ProductName",		"libluksde\0"
-      VALUE "ProductVersion",		"20240114" "\0"
+      VALUE "ProductVersion",		"20240503" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libluksde/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libluksde-20240114/libluksde/libluksde_debug.c` & `libluksde-20240503/libluksde/libluksde_debug.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libhmac.h` & `libluksde-20240503/libluksde/libluksde_libhmac.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libclocale.h` & `libluksde-20240503/libluksde/libluksde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libcdata.h` & `libluksde-20240503/libluksde/libluksde_libcdata.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde.rc.in` & `libluksde-20240503/libluksde/libluksde.rc.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_debug.h` & `libluksde-20240503/libluksde/libluksde_debug.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_encryption_context.h` & `libluksde-20240503/libluksde/libluksde_encryption_context.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_volume_header.h` & `libluksde-20240503/libluksde/libluksde_volume_header.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_sector_data.c` & `libluksde-20240503/libluksde/libluksde_sector_data.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_error.c` & `libluksde-20240503/libluksde/libluksde_error.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_support.h` & `libluksde-20240503/libluksde/libluksde_support.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde.c` & `libluksde-20240503/libluksde/libluksde.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libcaes.h` & `libluksde-20240503/libluksde/libluksde_libcaes.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_io_handle.h` & `libluksde-20240503/libluksde/libluksde_io_handle.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_error.h` & `libluksde-20240503/libluksde/libluksde_error.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_volume.h` & `libluksde-20240503/libluksde/libluksde_volume.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_notify.h` & `libluksde-20240503/libluksde/libluksde_notify.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_key_slot.c` & `libluksde-20240503/libluksde/libluksde_key_slot.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_sector_data_vector.c` & `libluksde-20240503/libluksde/libluksde_sector_data_vector.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/Makefile.am` & `libluksde-20240503/libluksde/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -79,21 +79,19 @@
 libluksde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libluksde_definitions.h.in \
 	libluksde.rc \
 	libluksde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libluksde_definitions.h \
+	libluksde.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libluksde_definitions.h
-	-rm -f libluksde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libluksde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libluksde_la_SOURCES)
```

### Comparing `libluksde-20240114/libluksde/libluksde_volume_header.c` & `libluksde-20240503/libluksde/libluksde_volume_header.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libfcrypto.h` & `libluksde-20240503/libluksde/libluksde_libfcrypto.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libfguid.h` & `libluksde-20240503/libluksde/libluksde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/luksde_keyslot.h` & `libluksde-20240503/libluksde/luksde_keyslot.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_sector_data.h` & `libluksde-20240503/libluksde/libluksde_sector_data.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_password.h` & `libluksde-20240503/libluksde/libluksde_password.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_diffuser.c` & `libluksde-20240503/libluksde/libluksde_diffuser.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libfcache.h` & `libluksde-20240503/libluksde/libluksde_libfcache.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libcerror.h` & `libluksde-20240503/libhmac/libhmac_libcerror.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2013-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBLUKSDE_LIBCERROR_H )
-#define _LIBLUKSDE_LIBCERROR_H
+#if !defined( _LIBHMAC_LIBCERROR_H )
+#define _LIBHMAC_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBLUKSDE_LIBCERROR_H ) */
+#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
```

### Comparing `libluksde-20240114/libluksde/libluksde_password.c` & `libluksde-20240503/libluksde/libluksde_password.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_notify.c` & `libluksde-20240503/libluksde/libluksde_notify.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_io_handle.c` & `libluksde-20240503/libluksde/libluksde_io_handle.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_unused.h` & `libluksde-20240503/libluksde/libluksde_unused.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_volume.c` & `libluksde-20240503/libluksde/libluksde_volume.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_sector_data_vector.h` & `libluksde-20240503/libluksde/libluksde_sector_data_vector.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/luksde_volume.h` & `libluksde-20240503/libluksde/luksde_volume.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_diffuser.h` & `libluksde-20240503/libluksde/libluksde_diffuser.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_key_slot.h` & `libluksde-20240503/libluksde/libluksde_key_slot.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_extern.h` & `libluksde-20240503/libluksde/libluksde_extern.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libcthreads.h` & `libluksde-20240503/libluksde/libluksde_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_types.h` & `libluksde-20240503/libluksde/libluksde_types.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libuna.h` & `libluksde-20240503/libluksde/libluksde_libuna.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_encryption_context.c` & `libluksde-20240503/libluksde/libluksde_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_libbfio.h` & `libluksde-20240503/libluksde/libluksde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/Makefile.in` & `libluksde-20240503/libluksde/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -502,14 +502,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -570,16 +572,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -652,15 +654,18 @@
 
 libluksde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libluksde_definitions.h.in \
 	libluksde.rc \
 	libluksde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libluksde_definitions.h \
+	libluksde.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -904,24 +909,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libluksde.Plo
+	-rm -f ./$(DEPDIR)/libluksde_debug.Plo
+	-rm -f ./$(DEPDIR)/libluksde_diffuser.Plo
+	-rm -f ./$(DEPDIR)/libluksde_encryption_context.Plo
+	-rm -f ./$(DEPDIR)/libluksde_error.Plo
+	-rm -f ./$(DEPDIR)/libluksde_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libluksde_key_slot.Plo
+	-rm -f ./$(DEPDIR)/libluksde_notify.Plo
+	-rm -f ./$(DEPDIR)/libluksde_password.Plo
+	-rm -f ./$(DEPDIR)/libluksde_sector_data.Plo
+	-rm -f ./$(DEPDIR)/libluksde_sector_data_vector.Plo
+	-rm -f ./$(DEPDIR)/libluksde_support.Plo
+	-rm -f ./$(DEPDIR)/libluksde_volume.Plo
+	-rm -f ./$(DEPDIR)/libluksde_volume_header.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1018,19 +1039,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libluksde_definitions.h
-	-rm -f libluksde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libluksde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libluksde_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libluksde-20240114/libluksde/libluksde_definitions.h.in` & `libluksde-20240503/libluksde/libluksde_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_codepage.h` & `libluksde-20240503/libluksde/libluksde_codepage.h`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_support.c` & `libluksde-20240503/libluksde/libluksde_support.c`

 * *Files identical despite different names*

### Comparing `libluksde-20240114/libluksde/libluksde_definitions.h` & `libluksde-20240503/libluksde/libluksde_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBLUKSDE )
 #include <libluksde/definitions.h>
 
 /* The definitions in <libluksde/definitions.h> are copied here
  * for local use of libluksde
  */
 #else
-#define LIBLUKSDE_VERSION				20240114
+#define LIBLUKSDE_VERSION				20240503
 
 /* The version string
  */
-#define LIBLUKSDE_VERSION_STRING			"20240114"
+#define LIBLUKSDE_VERSION_STRING			"20240503"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBLUKSDE_ACCESS_FLAGS
```

