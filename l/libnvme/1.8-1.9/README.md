# Comparing `tmp/libnvme-1.8.tar.gz` & `tmp/libnvme-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libnvme-1.8.tar", last modified: Wed Feb 14 09:41:39 2024, max compression
+gzip compressed data, was "libnvme-1.9.tar", last modified: Fri May  3 12:09:45 2024, max compression
```

## Comparing `libnvme-1.8.tar` & `libnvme-1.9.tar`

### file list

```diff
@@ -1,1055 +1,1102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 09:41:33.137386 libnvme-1.8/
--rw-rw-r--   0 root         (0) root         (0)      619 2024-02-14 09:40:43.000000 libnvme-1.8/.checkpatch.conf
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/.github/
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/.github/cross/
--rw-rw-r--   0 root         (0) root         (0)      452 2024-02-14 09:40:43.000000 libnvme-1.8/.github/cross/ubuntu-cross-armhf.txt
--rw-rw-r--   0 root         (0) root         (0)      465 2024-02-14 09:40:43.000000 libnvme-1.8/.github/cross/ubuntu-cross-ppc64le.txt
--rw-rw-r--   0 root         (0) root         (0)      424 2024-02-14 09:40:43.000000 libnvme-1.8/.github/cross/ubuntu-cross-s390x.txt
--rw-rw-r--   0 root         (0) root         (0)      122 2024-02-14 09:40:43.000000 libnvme-1.8/.github/dependabot.yml
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)     2756 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/build.yml
--rw-rw-r--   0 root         (0) root         (0)      465 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/checkpatch.yml
--rw-rw-r--   0 root         (0) root         (0)      457 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/coverage.yml
--rw-rw-r--   0 root         (0) root         (0)     1955 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/release-python.yml
--rw-rw-r--   0 root         (0) root         (0)      395 2024-02-14 09:40:43.000000 libnvme-1.8/.github/workflows/release.yml
--rw-rw-r--   0 root         (0) root         (0)      130 2024-02-14 09:40:43.000000 libnvme-1.8/.gitignore
--rw-rw-r--   0 root         (0) root         (0)      420 2024-02-14 09:40:43.000000 libnvme-1.8/.readthedocs.yaml
--rw-rw-r--   0 root         (0) root         (0)    26530 2024-02-14 09:40:43.000000 libnvme-1.8/COPYING
--rw-rw-r--   0 root         (0) root         (0)     1006 2024-02-14 09:40:43.000000 libnvme-1.8/Makefile
--rw-rw-r--   0 root         (0) root         (0)     6900 2024-02-14 09:40:43.000000 libnvme-1.8/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/array_size/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.085444 libnvme-1.8/ccan/ccan/array_size/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1032 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/array_size/_info
--rw-rw-r--   0 root         (0) root         (0)      889 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/array_size/array_size.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/build_assert/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.085444 libnvme-1.8/ccan/ccan/build_assert/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1350 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/build_assert/_info
--rw-rw-r--   0 root         (0) root         (0)     1228 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/build_assert/build_assert.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/check_type/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.089444 libnvme-1.8/ccan/ccan/check_type/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)      841 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/check_type/_info
--rw-rw-r--   0 root         (0) root         (0)     2368 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/check_type/check_type.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/container_of/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.089444 libnvme-1.8/ccan/ccan/container_of/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1386 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/container_of/_info
--rw-rw-r--   0 root         (0) root         (0)     4278 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/container_of/container_of.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/endian/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.089444 libnvme-1.8/ccan/ccan/endian/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1419 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/endian/_info
--rw-rw-r--   0 root         (0) root         (0)     9656 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/endian/endian.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/list/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.089444 libnvme-1.8/ccan/ccan/list/LICENSE -> ../../licenses/BSD-MIT
--rw-rw-r--   0 root         (0) root         (0)     1519 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/list/_info
--rw-rw-r--   0 root         (0) root         (0)     1000 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/list/list.c
--rw-rw-r--   0 root         (0) root         (0)    24307 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/list/list.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/minmax/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.089444 libnvme-1.8/ccan/ccan/minmax/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1141 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/minmax/_info
--rw-rw-r--   0 root         (0) root         (0)     1266 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/minmax/minmax.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/short_types/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.093444 libnvme-1.8/ccan/ccan/short_types/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)      793 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/short_types/short_types.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.093444 libnvme-1.8/ccan/ccan/str/LICENSE -> ../../licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/_info
--rw-rw-r--   0 root         (0) root         (0)     1602 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/debug.c
--rw-rw-r--   0 root         (0) root         (0)      283 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/str.c
--rw-rw-r--   0 root         (0) root         (0)     5958 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/str.h
--rw-rw-r--   0 root         (0) root         (0)      774 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/ccan/str/str_debug.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/licenses/
--rw-rw-r--   0 root         (0) root         (0)     1023 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/licenses/BSD-MIT
--rw-rw-r--   0 root         (0) root         (0)     6383 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/licenses/CC0
--rw-rw-r--   0 root         (0) root         (0)      603 2024-02-14 09:40:43.000000 libnvme-1.8/ccan/meson.build
--rw-rw-r--   0 root         (0) root         (0)       67 2024-02-14 09:40:43.000000 libnvme-1.8/codecov.yml
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/doc/
--rw-rw-r--   0 root         (0) root         (0)      390 2024-02-14 09:40:43.000000 libnvme-1.8/doc/api.rst.in
--rw-rw-r--   0 root         (0) root         (0)     1054 2024-02-14 09:40:43.000000 libnvme-1.8/doc/conf.py
--rw-rw-r--   0 root         (0) root         (0)     1060 2024-02-14 09:40:43.000000 libnvme-1.8/doc/conf.py.in
--rw-rw-r--   0 root         (0) root         (0)     4535 2024-02-14 09:40:43.000000 libnvme-1.8/doc/config-schema.json
--rw-rw-r--   0 root         (0) root         (0)     4535 2024-02-14 09:40:43.000000 libnvme-1.8/doc/config-schema.json.in
--rw-rw-r--   0 root         (0) root         (0)      570 2024-02-14 09:40:43.000000 libnvme-1.8/doc/index.rst
--rw-rw-r--   0 root         (0) root         (0)      570 2024-02-14 09:40:43.000000 libnvme-1.8/doc/index.rst.in
--rw-rw-r--   0 root         (0) root         (0)      965 2024-02-14 09:40:43.000000 libnvme-1.8/doc/installation.rst.in
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/
--rw-rw-r--   0 root         (0) root         (0)     5415 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_control.2
--rw-rw-r--   0 root         (0) root         (0)      308 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_control_flags.2
--rw-rw-r--   0 root         (0) root         (0)     1572 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_desc_type.2
--rw-rw-r--   0 root         (0) root         (0)     2324 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_discovery.2
--rw-rw-r--   0 root         (0) root         (0)      383 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_discovery_flags.2
--rw-rw-r--   0 root         (0) root         (0)     2985 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_header.2
--rw-rw-r--   0 root         (0) root         (0)      426 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_heap_obj.2
--rw-rw-r--   0 root         (0) root         (0)     1101 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_hfi.2
--rw-rw-r--   0 root         (0) root         (0)      347 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_hfi_flags.2
--rw-rw-r--   0 root         (0) root         (0)     4751 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_hfi_info_tcp.2
--rw-rw-r--   0 root         (0) root         (0)     1035 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_hfi_info_tcp_flags.2
--rw-rw-r--   0 root         (0) root         (0)      916 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_host.2
--rw-rw-r--   0 root         (0) root         (0)     2242 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_host_flags.2
--rw-rw-r--   0 root         (0) root         (0)     1067 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info.2
--rw-rw-r--   0 root         (0) root         (0)      817 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_discovery.2
--rw-rw-r--   0 root         (0) root         (0)      600 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_hfi.2
--rw-rw-r--   0 root         (0) root         (0)     2269 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_hfi_info_tcp.2
--rw-rw-r--   0 root         (0) root         (0)      912 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_host.2
--rw-rw-r--   0 root         (0) root         (0)      610 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_nid_type.2
--rw-rw-r--   0 root         (0) root         (0)     1108 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_primary_admin_host_flag.2
--rw-rw-r--   0 root         (0) root         (0)      344 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_security.2
--rw-rw-r--   0 root         (0) root         (0)     2350 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_info_subsystem_ns.2
--rw-rw-r--   0 root         (0) root         (0)     3608 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_security.2
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_security_flags.2
--rw-rw-r--   0 root         (0) root         (0)      501 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_security_secret_type.2
--rw-rw-r--   0 root         (0) root         (0)     5482 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_ssns.2
--rw-rw-r--   0 root         (0) root         (0)     1813 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_ssns_ext_info.2
--rw-rw-r--   0 root         (0) root         (0)      778 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_ssns_ext_info_flags.2
--rw-rw-r--   0 root         (0) root         (0)     4077 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_ssns_flags.2
--rw-rw-r--   0 root         (0) root         (0)     1513 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_ssns_trflags.2
--rw-rw-r--   0 root         (0) root         (0)      298 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nbft_trtype.2
--rw-rw-r--   0 root         (0) root         (0)     3526 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_admin_opcode.2
--rw-rw-r--   0 root         (0) root         (0)     1892 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_admin_passthru.2
--rw-rw-r--   0 root         (0) root         (0)     1910 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_admin_passthru64.2
--rw-rw-r--   0 root         (0) root         (0)      658 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ae_info_css_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      957 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ae_info_error.2
--rw-rw-r--   0 root         (0) root         (0)     1144 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ae_info_notice.2
--rw-rw-r--   0 root         (0) root         (0)      588 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ae_info_smart.2
--rw-rw-r--   0 root         (0) root         (0)      568 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ae_type.2
--rw-rw-r--   0 root         (0) root         (0)      412 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_aggregate_endurance_group_event.2
--rw-rw-r--   0 root         (0) root         (0)      420 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_aggregate_predictable_lat_event.2
--rw-rw-r--   0 root         (0) root         (0)      580 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ana_group_desc.2
--rw-rw-r--   0 root         (0) root         (0)      476 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ana_log.2
--rw-rw-r--   0 root         (0) root         (0)      736 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ana_state.2
--rw-rw-r--   0 root         (0) root         (0)      658 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_apst_entry.2
--rw-rw-r--   0 root         (0) root         (0)      576 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_boot_partition.2
--rw-rw-r--   0 root         (0) root         (0)      704 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_capacity_config_desc.2
--rw-rw-r--   0 root         (0) root         (0)      457 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_capacity_mgmt.2
--rw-rw-r--   0 root         (0) root         (0)     1071 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_change_ns_event.2
--rw-rw-r--   0 root         (0) root         (0)      542 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_channel_config_desc.2
--rw-rw-r--   0 root         (0) root         (0)      348 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmb_size.2
--rw-rw-r--   0 root         (0) root         (0)      907 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_effects.2
--rw-rw-r--   0 root         (0) root         (0)      419 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_effects_log.2
--rw-rw-r--   0 root         (0) root         (0)      513 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_format_mset.2
--rw-rw-r--   0 root         (0) root         (0)      659 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_format_pi.2
--rw-rw-r--   0 root         (0) root         (0)      496 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_format_pil.2
--rw-rw-r--   0 root         (0) root         (0)      958 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_format_ses.2
--rw-rw-r--   0 root         (0) root         (0)     3507 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_get_log_lid.2
--rw-rw-r--   0 root         (0) root         (0)      497 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_cmd_get_log_telemetry_host_lsp.2
--rw-rw-r--   0 root         (0) root         (0)      419 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_compare.2
--rw-rw-r--   0 root         (0) root         (0)     2268 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_connect_err.2
--rw-rw-r--   0 root         (0) root         (0)     4040 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_constants.2
--rw-rw-r--   0 root         (0) root         (0)      388 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy.2
--rw-rw-r--   0 root         (0) root         (0)      749 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy_range.2
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy_range_f1.2
--rw-rw-r--   0 root         (0) root         (0)      888 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy_range_f2.2
--rw-rw-r--   0 root         (0) root         (0)      941 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy_range_f3.2
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_copy_range_sopt.2
--rw-rw-r--   0 root         (0) root         (0)      820 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_create_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      388 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_create_root.2
--rw-rw-r--   0 root         (0) root         (0)      406 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_csi.2
--rw-rw-r--   0 root         (0) root         (0)     1010 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_config_match.2
--rw-rw-r--   0 root         (0) root         (0)     1179 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_find.2
--rw-rw-r--   0 root         (0) root         (0)      332 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_first_ns.2
--rw-rw-r--   0 root         (0) root         (0)      339 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_first_path.2
--rw-rw-r--   0 root         (0) root         (0)      299 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_for_each_ns.2
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_for_each_ns_safe.2
--rw-rw-r--   0 root         (0) root         (0)      304 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_for_each_path.2
--rw-rw-r--   0 root         (0) root         (0)      404 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_for_each_path_safe.2
--rw-rw-r--   0 root         (0) root         (0)      387 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_address.2
--rw-rw-r--   0 root         (0) root         (0)      353 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_config.2
--rw-rw-r--   0 root         (0) root         (0)      364 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_dhchap_host_key.2
--rw-rw-r--   0 root         (0) root         (0)      374 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_dhchap_key.2
--rw-rw-r--   0 root         (0) root         (0)      667 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_fd.2
--rw-rw-r--   0 root         (0) root         (0)      333 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_firmware.2
--rw-rw-r--   0 root         (0) root         (0)      362 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_host_iface.2
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_host_traddr.2
--rw-rw-r--   0 root         (0) root         (0)      308 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_model.2
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_name.2
--rw-rw-r--   0 root         (0) root         (0)      336 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_numa_node.2
--rw-rw-r--   0 root         (0) root         (0)      398 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_phy_slot.2
--rw-rw-r--   0 root         (0) root         (0)      337 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_queue_count.2
--rw-rw-r--   0 root         (0) root         (0)      328 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_serial.2
--rw-rw-r--   0 root         (0) root         (0)      321 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_sqsize.2
--rw-rw-r--   0 root         (0) root         (0)      595 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_src_addr.2
--rw-rw-r--   0 root         (0) root         (0)      339 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_state.2
--rw-rw-r--   0 root         (0) root         (0)      333 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_subsysnqn.2
--rw-rw-r--   0 root         (0) root         (0)      346 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      342 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_sysfs_dir.2
--rw-rw-r--   0 root         (0) root         (0)      329 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_traddr.2
--rw-rw-r--   0 root         (0) root         (0)      335 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_transport.2
--rw-rw-r--   0 root         (0) root         (0)      368 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_get_trsvcid.2
--rw-rw-r--   0 root         (0) root         (0)      507 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_identify.2
--rw-rw-r--   0 root         (0) root         (0)      355 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_is_discovered.2
--rw-rw-r--   0 root         (0) root         (0)      489 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_is_discovery_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      355 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_is_persistent.2
--rw-rw-r--   0 root         (0) root         (0)      400 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_is_unique_discovery_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)     2396 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_metadata_type.2
--rw-rw-r--   0 root         (0) root         (0)      383 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_next_ns.2
--rw-rw-r--   0 root         (0) root         (0)      427 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_next_path.2
--rw-rw-r--   0 root         (0) root         (0)      290 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_release_fd.2
--rw-rw-r--   0 root         (0) root         (0)      414 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_reset.2
--rw-rw-r--   0 root         (0) root         (0)      406 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_dhchap_host_key.2
--rw-rw-r--   0 root         (0) root         (0)      398 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_dhchap_key.2
--rw-rw-r--   0 root         (0) root         (0)      440 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_discovered.2
--rw-rw-r--   0 root         (0) root         (0)      514 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_discovery_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      441 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_persistent.2
--rw-rw-r--   0 root         (0) root         (0)      549 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ctrls_filter.2
--rw-rw-r--   0 root         (0) root         (0)      592 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_data_tfr.2
--rw-rw-r--   0 root         (0) root         (0)      456 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_default_host.2
--rw-rw-r--   0 root         (0) root         (0)      515 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_describe_key_serial.2
--rw-rw-r--   0 root         (0) root         (0)     1038 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dev_self_test.2
--rw-rw-r--   0 root         (0) root         (0)      410 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_dtype.2
--rw-rw-r--   0 root         (0) root         (0)      705 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_receive_doper.2
--rw-rw-r--   0 root         (0) root         (0)      467 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_recv.2
--rw-rw-r--   0 root         (0) root         (0)      627 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_recv_identify_parameters.2
--rw-rw-r--   0 root         (0) root         (0)      665 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_recv_stream_allocate.2
--rw-rw-r--   0 root         (0) root         (0)      641 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_recv_stream_parameters.2
--rw-rw-r--   0 root         (0) root         (0)      685 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_recv_stream_status.2
--rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send.2
--rw-rw-r--   0 root         (0) root         (0)      599 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send_doper.2
--rw-rw-r--   0 root         (0) root         (0)      725 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send_id_endir.2
--rw-rw-r--   0 root         (0) root         (0)      458 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send_identify_endir.2
--rw-rw-r--   0 root         (0) root         (0)      625 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send_stream_release_identifier.2
--rw-rw-r--   0 root         (0) root         (0)      562 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_send_stream_release_resource.2
--rw-rw-r--   0 root         (0) root         (0)      508 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_directive_types.2
--rw-rw-r--   0 root         (0) root         (0)      377 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_disconnect_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      758 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dsm.2
--rw-rw-r--   0 root         (0) root         (0)      479 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dsm_attributes.2
--rw-rw-r--   0 root         (0) root         (0)      394 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dsm_range.2
--rw-rw-r--   0 root         (0) root         (0)      624 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dst_stc.2
--rw-rw-r--   0 root         (0) root         (0)      386 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dump_config.2
--rw-rw-r--   0 root         (0) root         (0)      363 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_dump_tree.2
--rw-rw-r--   0 root         (0) root         (0)      716 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_eg_critical_warning_flags.2
--rw-rw-r--   0 root         (0) root         (0)      390 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_eg_event_aggregate_log.2
--rw-rw-r--   0 root         (0) root         (0)      477 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_end_grp_chan_desc.2
--rw-rw-r--   0 root         (0) root         (0)      875 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_end_grp_config_desc.2
--rw-rw-r--   0 root         (0) root         (0)     1870 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_endurance_group_log.2
--rw-rw-r--   0 root         (0) root         (0)     1139 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_eom_lane_desc.2
--rw-rw-r--   0 root         (0) root         (0)      421 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_eom_optional_data.2
--rw-rw-r--   0 root         (0) root         (0)      389 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_errno_to_string.2
--rw-rw-r--   0 root         (0) root         (0)     3987 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_error_log_page.2
--rw-rw-r--   0 root         (0) root         (0)     1974 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fabrics_config.2
--rw-rw-r--   0 root         (0) root         (0)      784 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fctype.2
--rw-rw-r--   0 root         (0) root         (0)     1033 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_config_desc.2
--rw-rw-r--   0 root         (0) root         (0)      949 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_config_fdpa.2
--rw-rw-r--   0 root         (0) root         (0)      648 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_config_log.2
--rw-rw-r--   0 root         (0) root         (0)      881 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_event.2
--rw-rw-r--   0 root         (0) root         (0)      472 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_event_flags.2
--rw-rw-r--   0 root         (0) root         (0)      589 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_event_realloc.2
--rw-rw-r--   0 root         (0) root         (0)      337 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_event_realloc_flags.2
--rw-rw-r--   0 root         (0) root         (0)      820 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_event_type.2
--rw-rw-r--   0 root         (0) root         (0)      426 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_events_log.2
--rw-rw-r--   0 root         (0) root         (0)      653 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_reclaim_unit_handle_status.2
--rw-rw-r--   0 root         (0) root         (0)      682 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_reclaim_unit_handle_update.2
--rw-rw-r--   0 root         (0) root         (0)      333 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruh_desc.2
--rw-rw-r--   0 root         (0) root         (0)      475 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruh_status.2
--rw-rw-r--   0 root         (0) root         (0)      603 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruh_status_desc.2
--rw-rw-r--   0 root         (0) root         (0)      424 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruh_type.2
--rw-rw-r--   0 root         (0) root         (0)      669 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruha.2
--rw-rw-r--   0 root         (0) root         (0)      375 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruhu_desc.2
--rw-rw-r--   0 root         (0) root         (0)      447 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_ruhu_log.2
--rw-rw-r--   0 root         (0) root         (0)      481 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_stats_log.2
--rw-rw-r--   0 root         (0) root         (0)      484 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_supported_event_attributes.2
--rw-rw-r--   0 root         (0) root         (0)      418 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fdp_supported_event_desc.2
--rw-rw-r--   0 root         (0) root         (0)     8680 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat.2
--rw-rw-r--   0 root         (0) root         (0)      310 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_auto_pst.2
--rw-rw-r--   0 root         (0) root         (0)      425 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_fdp_events_cdw11.2
--rw-rw-r--   0 root         (0) root         (0)      640 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_host_behavior.2
--rw-rw-r--   0 root         (0) root         (0)      689 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_nswpcfg_state.2
--rw-rw-r--   0 root         (0) root         (0)      438 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_plm_window_select.2
--rw-rw-r--   0 root         (0) root         (0)      613 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_resv_notify_flags.2
--rw-rw-r--   0 root         (0) root         (0)      501 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_feat_tmpthresh_thsel.2
--rw-rw-r--   0 root         (0) root         (0)     1858 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_features_async_event_config_flags.2
--rw-rw-r--   0 root         (0) root         (0)     3960 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_features_id.2
--rw-rw-r--   0 root         (0) root         (0)     1947 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fid_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)      386 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fid_supported_effects_log.2
--rw-rw-r--   0 root         (0) root         (0)      454 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_firmware_slot.2
--rw-rw-r--   0 root         (0) root         (0)      316 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_first_host.2
--rw-rw-r--   0 root         (0) root         (0)      351 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_first_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      534 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_flush.2
--rw-rw-r--   0 root         (0) root         (0)      293 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_for_each_host.2
--rw-rw-r--   0 root         (0) root         (0)      375 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_for_each_host_safe.2
--rw-rw-r--   0 root         (0) root         (0)      319 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_for_each_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      406 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_for_each_subsystem_safe.2
--rw-rw-r--   0 root         (0) root         (0)      737 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_format_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      634 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_format_nvm_compln_event.2
--rw-rw-r--   0 root         (0) root         (0)      499 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_format_nvm_start_event.2
--rw-rw-r--   0 root         (0) root         (0)      243 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_free_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      244 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_free_host.2
--rw-rw-r--   0 root         (0) root         (0)      240 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_free_ns.2
--rw-rw-r--   0 root         (0) root         (0)      316 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_free_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      319 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_free_tree.2
--rw-rw-r--   0 root         (0) root         (0)      648 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fw_commit.2
--rw-rw-r--   0 root         (0) root         (0)     1625 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fw_commit_ca.2
--rw-rw-r--   0 root         (0) root         (0)      814 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fw_commit_event.2
--rw-rw-r--   0 root         (0) root         (0)     1103 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fw_download.2
--rw-rw-r--   0 root         (0) root         (0)      766 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_fw_download_seq.2
--rw-rw-r--   0 root         (0) root         (0)      660 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_gen_dhchap_key.2
--rw-rw-r--   0 root         (0) root         (0)      946 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_generate_tls_key_identity.2
--rw-rw-r--   0 root         (0) root         (0)      511 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_ana_log_len.2
--rw-rw-r--   0 root         (0) root         (0)      445 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_attr.2
--rw-rw-r--   0 root         (0) root         (0)      480 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_ctrl_attr.2
--rw-rw-r--   0 root         (0) root         (0)      937 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_ctrl_telemetry.2
--rw-rw-r--   0 root         (0) root         (0)      732 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_directive_receive_length.2
--rw-rw-r--   0 root         (0) root         (0)      745 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_discovery_args.2
--rw-rw-r--   0 root         (0) root         (0)      670 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_feature_length.2
--rw-rw-r--   0 root         (0) root         (0)      873 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_feature_length2.2
--rw-rw-r--   0 root         (0) root         (0)      452 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features.2
--rw-rw-r--   0 root         (0) root         (0)      663 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_arbitration.2
--rw-rw-r--   0 root         (0) root         (0)      670 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_async_event.2
--rw-rw-r--   0 root         (0) root         (0)      720 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_auto_pst.2
--rw-rw-r--   0 root         (0) root         (0)      826 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_data.2
--rw-rw-r--   0 root         (0) root         (0)      774 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_endurance_event_cfg.2
--rw-rw-r--   0 root         (0) root         (0)      787 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_err_recovery.2
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_err_recovery2.2
--rw-rw-r--   0 root         (0) root         (0)      642 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_hctm.2
--rw-rw-r--   0 root         (0) root         (0)      781 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_host_behavior.2
--rw-rw-r--   0 root         (0) root         (0)      752 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_host_id.2
--rw-rw-r--   0 root         (0) root         (0)      820 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_host_mem_buf.2
--rw-rw-r--   0 root         (0) root         (0)      793 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_host_mem_buf2.2
--rw-rw-r--   0 root         (0) root         (0)      668 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_iocs_profile.2
--rw-rw-r--   0 root         (0) root         (0)      668 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_irq_coalesce.2
--rw-rw-r--   0 root         (0) root         (0)      691 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_irq_config.2
--rw-rw-r--   0 root         (0) root         (0)      642 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_kato.2
--rw-rw-r--   0 root         (0) root         (0)      870 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_lba_range.2
--rw-rw-r--   0 root         (0) root         (0)      814 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_lba_range2.2
--rw-rw-r--   0 root         (0) root         (0)      694 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_lba_sts_interval.2
--rw-rw-r--   0 root         (0) root         (0)      655 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_nopsc.2
--rw-rw-r--   0 root         (0) root         (0)      664 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_num_queues.2
--rw-rw-r--   0 root         (0) root         (0)      778 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_plm_config.2
--rw-rw-r--   0 root         (0) root         (0)      717 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_plm_window.2
--rw-rw-r--   0 root         (0) root         (0)      664 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_power_mgmt.2
--rw-rw-r--   0 root         (0) root         (0)      774 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_resv_mask.2
--rw-rw-r--   0 root         (0) root         (0)      714 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_resv_mask2.2
--rw-rw-r--   0 root         (0) root         (0)      792 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_resv_persist.2
--rw-rw-r--   0 root         (0) root         (0)      729 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_resv_persist2.2
--rw-rw-r--   0 root         (0) root         (0)      639 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_rrl.2
--rw-rw-r--   0 root         (0) root         (0)      648 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_sanitize.2
--rw-rw-r--   0 root         (0) root         (0)      617 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_sel.2
--rw-rw-r--   0 root         (0) root         (0)      660 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_simple.2
--rw-rw-r--   0 root         (0) root         (0)      669 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_sw_progress.2
--rw-rw-r--   0 root         (0) root         (0)      673 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_temp_thresh.2
--rw-rw-r--   0 root         (0) root         (0)      633 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_timestamp.2
--rw-rw-r--   0 root         (0) root         (0)      672 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_volatile_wc.2
--rw-rw-r--   0 root         (0) root         (0)      668 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_write_atomic.2
--rw-rw-r--   0 root         (0) root         (0)      723 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_features_write_protect.2
--rw-rw-r--   0 root         (0) root         (0)      870 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_host_telemetry.2
--rw-rw-r--   0 root         (0) root         (0)      648 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_lba_status.2
--rw-rw-r--   0 root         (0) root         (0)      613 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_lba_status_log.2
--rw-rw-r--   0 root         (0) root         (0)      420 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log.2
--rw-rw-r--   0 root         (0) root         (0)     1108 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_ana.2
--rw-rw-r--   0 root         (0) root         (0)      781 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_ana_groups.2
--rw-rw-r--   0 root         (0) root         (0)      741 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_boot_partition.2
--rw-rw-r--   0 root         (0) root         (0)      769 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_changed_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)      761 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_cmd_effects.2
--rw-rw-r--   0 root         (0) root         (0)      555 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_create_telemetry_host.2
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_device_self_test.2
--rw-rw-r--   0 root         (0) root         (0)      802 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_discovery.2
--rw-rw-r--   0 root         (0) root         (0)     1010 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_endurance_group.2
--rw-rw-r--   0 root         (0) root         (0)      738 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_endurance_grp_evt.2
--rw-rw-r--   0 root         (0) root         (0)      833 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_error.2
--rw-rw-r--   0 root         (0) root         (0)      624 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_fdp_configurations.2
--rw-rw-r--   0 root         (0) root         (0)      670 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_fdp_events.2
--rw-rw-r--   0 root         (0) root         (0)      576 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_fdp_stats.2
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_fid_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)      787 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_fw_slot.2
--rw-rw-r--   0 root         (0) root         (0)      692 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_lba_status.2
--rw-rw-r--   0 root         (0) root         (0)      633 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_media_unit_stat.2
--rw-rw-r--   0 root         (0) root         (0)      680 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_mi_cmd_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)      592 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_page.2
--rw-rw-r--   0 root         (0) root         (0)      732 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_persistent_event.2
--rw-rw-r--   0 root         (0) root         (0)      796 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_phy_rx_eom.2
--rw-rw-r--   0 root         (0) root         (0)      796 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_predictable_lat_event.2
--rw-rw-r--   0 root         (0) root         (0)      647 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_predictable_lat_nvmset.2
--rw-rw-r--   0 root         (0) root         (0)      631 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_reclaim_unit_handle_usage.2
--rw-rw-r--   0 root         (0) root         (0)      596 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_reservation.2
--rw-rw-r--   0 root         (0) root         (0)      716 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_sanitize.2
--rw-rw-r--   0 root         (0) root         (0)     1049 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_smart.2
--rw-rw-r--   0 root         (0) root         (0)      700 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_support_cap_config_list.2
--rw-rw-r--   0 root         (0) root         (0)      636 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_supported_log_pages.2
--rw-rw-r--   0 root         (0) root         (0)      882 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_telemetry_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      809 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_telemetry_host.2
--rw-rw-r--   0 root         (0) root         (0)      767 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_log_zns_changed_zones.2
--rw-rw-r--   0 root         (0) root         (0)      575 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_logical_block_size.2
--rw-rw-r--   0 root         (0) root         (0)      890 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_new_host_telemetry.2
--rw-rw-r--   0 root         (0) root         (0)      466 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_ns_attr.2
--rw-rw-r--   0 root         (0) root         (0)      717 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_nsid.2
--rw-rw-r--   0 root         (0) root         (0)      473 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_path_attr.2
--rw-rw-r--   0 root         (0) root         (0)      598 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_property.2
--rw-rw-r--   0 root         (0) root         (0)      496 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_subsys_attr.2
--rw-rw-r--   0 root         (0) root         (0)     1199 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_telemetry_log.2
--rw-rw-r--   0 root         (0) root         (0)      620 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_get_telemetry_max.2
--rw-rw-r--   0 root         (0) root         (0)      504 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_hmac_alg.2
--rw-rw-r--   0 root         (0) root         (0)      312 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_behavior_support.2
--rw-rw-r--   0 root         (0) root         (0)      361 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_get_dhchap_key.2
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_get_hostid.2
--rw-rw-r--   0 root         (0) root         (0)      323 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_get_hostnqn.2
--rw-rw-r--   0 root         (0) root         (0)      416 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_get_hostsymname.2
--rw-rw-r--   0 root         (0) root         (0)      327 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_get_root.2
--rw-rw-r--   0 root         (0) root         (0)      536 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_is_pdc_enabled.2
--rw-rw-r--   0 root         (0) root         (0)      634 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_mem_buf_attrs.2
--rw-rw-r--   0 root         (0) root         (0)      617 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_metadata.2
--rw-rw-r--   0 root         (0) root         (0)      473 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_release_fds.2
--rw-rw-r--   0 root         (0) root         (0)      386 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_set_dhchap_key.2
--rw-rw-r--   0 root         (0) root         (0)      393 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_set_hostsymname.2
--rw-rw-r--   0 root         (0) root         (0)      617 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_host_set_pdc_enabled.2
--rw-rw-r--   0 root         (0) root         (0)    14997 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)     1485 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_anacap.2
--rw-rw-r--   0 root         (0) root         (0)      390 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_apsta.2
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_avscc.2
--rw-rw-r--   0 root         (0) root         (0)     1241 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_cmic.2
--rw-rw-r--   0 root         (0) root         (0)      497 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_cntrltype.2
--rw-rw-r--   0 root         (0) root         (0)      584 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_cqes.2
--rw-rw-r--   0 root         (0) root         (0)     2243 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_ctratt.2
--rw-rw-r--   0 root         (0) root         (0)      526 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_dctype.2
--rw-rw-r--   0 root         (0) root         (0)      460 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_dsto.2
--rw-rw-r--   0 root         (0) root         (0)      462 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_fcatt.2
--rw-rw-r--   0 root         (0) root         (0)     1350 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_fna.2
--rw-rw-r--   0 root         (0) root         (0)      883 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_frmw.2
--rw-rw-r--   0 root         (0) root         (0)      409 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_fuses.2
--rw-rw-r--   0 root         (0) root         (0)      492 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_hctm.2
--rw-rw-r--   0 root         (0) root         (0)     1650 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_lpa.2
--rw-rw-r--   0 root         (0) root         (0)      571 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_mec.2
--rw-rw-r--   0 root         (0) root         (0)      709 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      684 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_nvmsr.2
--rw-rw-r--   0 root         (0) root         (0)      404 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_nvscc.2
--rw-rw-r--   0 root         (0) root         (0)      959 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_nwpc.2
--rw-rw-r--   0 root         (0) root         (0)     2003 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_oacs.2
--rw-rw-r--   0 root         (0) root         (0)     1250 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_oaes.2
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_ofcs.2
--rw-rw-r--   0 root         (0) root         (0)     2076 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_oncs.2
--rw-rw-r--   0 root         (0) root         (0)      798 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_rpmbs.2
--rw-rw-r--   0 root         (0) root         (0)     1158 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_sanicap.2
--rw-rw-r--   0 root         (0) root         (0)      899 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_sgls.2
--rw-rw-r--   0 root         (0) root         (0)      584 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_sqes.2
--rw-rw-r--   0 root         (0) root         (0)      609 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_vwc.2
--rw-rw-r--   0 root         (0) root         (0)     1078 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ctrl_vwci.2
--rw-rw-r--   0 root         (0) root         (0)      464 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_directives.2
--rw-rw-r--   0 root         (0) root         (0)      655 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_domain_attr.2
--rw-rw-r--   0 root         (0) root         (0)      447 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_domain_list.2
--rw-rw-r--   0 root         (0) root         (0)      414 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_endurance_group_list.2
--rw-rw-r--   0 root         (0) root         (0)     1021 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_independent_id_ns.2
--rw-rw-r--   0 root         (0) root         (0)      315 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_iocs.2
--rw-rw-r--   0 root         (0) root         (0)     7088 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns.2
--rw-rw-r--   0 root         (0) root         (0)      391 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_attr.2
--rw-rw-r--   0 root         (0) root         (0)     1233 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_dlfeat.2
--rw-rw-r--   0 root         (0) root         (0)     1059 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_dpc.2
--rw-rw-r--   0 root         (0) root         (0)      979 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_dps.2
--rw-rw-r--   0 root         (0) root         (0)     1076 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_flbas.2
--rw-rw-r--   0 root         (0) root         (0)      404 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_granularity_desc.2
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_granularity_list.2
--rw-rw-r--   0 root         (0) root         (0)      594 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_mc.2
--rw-rw-r--   0 root         (0) root         (0)      417 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_nmic.2
--rw-rw-r--   0 root         (0) root         (0)     1564 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_ns_rescap.2
--rw-rw-r--   0 root         (0) root         (0)     1414 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_nsfeat.2
--rw-rw-r--   0 root         (0) root         (0)      402 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_nvmset_list.2
--rw-rw-r--   0 root         (0) root         (0)     2977 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_psd.2
--rw-rw-r--   0 root         (0) root         (0)      564 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_uuid.2
--rw-rw-r--   0 root         (0) root         (0)      355 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_uuid_list.2
--rw-rw-r--   0 root         (0) root         (0)      421 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_id_uuid_list_entry.2
--rw-rw-r--   0 root         (0) root         (0)      579 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify.2
--rw-rw-r--   0 root         (0) root         (0)      920 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_active_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)     1117 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_active_ns_list_csi.2
--rw-rw-r--   0 root         (0) root         (0)      621 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_allocated_ns.2
--rw-rw-r--   0 root         (0) root         (0)      934 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_allocated_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)     1118 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_allocated_ns_list_csi.2
--rw-rw-r--   0 root         (0) root         (0)     3621 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_cns.2
--rw-rw-r--   0 root         (0) root         (0)      650 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      831 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ctrl_csi.2
--rw-rw-r--   0 root         (0) root         (0)      870 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      846 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_domain_list.2
--rw-rw-r--   0 root         (0) root         (0)      641 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_endurance_group_list.2
--rw-rw-r--   0 root         (0) root         (0)      859 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_independent_identify_ns.2
--rw-rw-r--   0 root         (0) root         (0)      680 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_iocs.2
--rw-rw-r--   0 root         (0) root         (0)     1052 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2
--rw-rw-r--   0 root         (0) root         (0)     1061 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ns.2
--rw-rw-r--   0 root         (0) root         (0)      872 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ns_csi.2
--rw-rw-r--   0 root         (0) root         (0)      966 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ns_csi_user_data_format.2
--rw-rw-r--   0 root         (0) root         (0)      959 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ns_descs.2
--rw-rw-r--   0 root         (0) root         (0)      867 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_ns_granularity.2
--rw-rw-r--   0 root         (0) root         (0)      986 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_nsid_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      957 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_nvmset_list.2
--rw-rw-r--   0 root         (0) root         (0)      770 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_primary_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)     1070 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_secondary_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      767 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_identify_uuid.2
--rw-rw-r--   0 root         (0) root         (0)      736 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_copy_range.2
--rw-rw-r--   0 root         (0) root         (0)      754 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_copy_range_f1.2
--rw-rw-r--   0 root         (0) root         (0)      879 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_copy_range_f2.2
--rw-rw-r--   0 root         (0) root         (0)      879 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_copy_range_f3.2
--rw-rw-r--   0 root         (0) root         (0)      477 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      704 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      820 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_dsm_range.2
--rw-rw-r--   0 root         (0) root         (0)      546 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_init_logging.2
--rw-rw-r--   0 root         (0) root         (0)     1004 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_insert_tls_key.2
--rw-rw-r--   0 root         (0) root         (0)     1183 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_insert_tls_key_versioned.2
--rw-rw-r--   0 root         (0) root         (0)      453 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io.2
--rw-rw-r--   0 root         (0) root         (0)     1152 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_control_flags.2
--rw-rw-r--   0 root         (0) root         (0)     1788 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_dsm_flags.2
--rw-rw-r--   0 root         (0) root         (0)      454 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_mgmt_recv.2
--rw-rw-r--   0 root         (0) root         (0)      330 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_mgmt_recv_mo.2
--rw-rw-r--   0 root         (0) root         (0)      451 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_mgmt_send.2
--rw-rw-r--   0 root         (0) root         (0)      327 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_mgmt_send_mo.2
--rw-rw-r--   0 root         (0) root         (0)     1674 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_opcode.2
--rw-rw-r--   0 root         (0) root         (0)     1877 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_passthru.2
--rw-rw-r--   0 root         (0) root         (0)     1889 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_io_passthru64.2
--rw-rw-r--   0 root         (0) root         (0)      718 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_is_64bit_reg.2
--rw-rw-r--   0 root         (0) root         (0)      365 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_range_type.2
--rw-rw-r--   0 root         (0) root         (0)      700 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_range_type_entry.2
--rw-rw-r--   0 root         (0) root         (0)      377 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_rd.2
--rw-rw-r--   0 root         (0) root         (0)      487 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_status.2
--rw-rw-r--   0 root         (0) root         (0)      502 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_status_atype.2
--rw-rw-r--   0 root         (0) root         (0)      542 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_status_desc.2
--rw-rw-r--   0 root         (0) root         (0)      703 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lba_status_log.2
--rw-rw-r--   0 root         (0) root         (0)      534 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lbaf.2
--rw-rw-r--   0 root         (0) root         (0)      752 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lbaf_rp.2
--rw-rw-r--   0 root         (0) root         (0)      750 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lbart.2
--rw-rw-r--   0 root         (0) root         (0)      608 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lbas_ns_element.2
--rw-rw-r--   0 root         (0) root         (0)      422 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lockdown.2
--rw-rw-r--   0 root         (0) root         (0)      396 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_log_ana_lsp.2
--rw-rw-r--   0 root         (0) root         (0)      599 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_log_phy_rx_eom_action.2
--rw-rw-r--   0 root         (0) root         (0)      563 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_log_phy_rx_eom_quality.2
--rw-rw-r--   0 root         (0) root         (0)     1111 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lookup_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      532 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lookup_host.2
--rw-rw-r--   0 root         (0) root         (0)      507 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lookup_key.2
--rw-rw-r--   0 root         (0) root         (0)      431 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lookup_keyring.2
--rw-rw-r--   0 root         (0) root         (0)      634 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_lookup_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_media_unit_config_desc.2
--rw-rw-r--   0 root         (0) root         (0)      874 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_media_unit_stat_desc.2
--rw-rw-r--   0 root         (0) root         (0)      597 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_media_unit_stat_log.2
--rw-rw-r--   0 root         (0) root         (0)      492 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_metadata_element_desc.2
--rw-rw-r--   0 root         (0) root         (0)     2125 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_admin_passthru.2
--rw-rw-r--   0 root         (0) root         (0)      659 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_format_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      578 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_fw_commit.2
--rw-rw-r--   0 root         (0) root         (0)     1146 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_fw_download.2
--rw-rw-r--   0 root         (0) root         (0)     1029 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_features_data.2
--rw-rw-r--   0 root         (0) root         (0)      938 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log.2
--rw-rw-r--   0 root         (0) root         (0)     1148 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_ana.2
--rw-rw-r--   0 root         (0) root         (0)      821 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_ana_groups.2
--rw-rw-r--   0 root         (0) root         (0)      782 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_boot_partition.2
--rw-rw-r--   0 root         (0) root         (0)      809 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_changed_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)      801 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_cmd_effects.2
--rw-rw-r--   0 root         (0) root         (0)      595 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2
--rw-rw-r--   0 root         (0) root         (0)      764 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_device_self_test.2
--rw-rw-r--   0 root         (0) root         (0)      842 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_discovery.2
--rw-rw-r--   0 root         (0) root         (0)     1050 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_endurance_group.2
--rw-rw-r--   0 root         (0) root         (0)      778 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2
--rw-rw-r--   0 root         (0) root         (0)      873 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_error.2
--rw-rw-r--   0 root         (0) root         (0)      697 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)      827 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_fw_slot.2
--rw-rw-r--   0 root         (0) root         (0)      732 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_lba_status.2
--rw-rw-r--   0 root         (0) root         (0)      674 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_media_unit_stat.2
--rw-rw-r--   0 root         (0) root         (0)      721 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)     1030 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_page.2
--rw-rw-r--   0 root         (0) root         (0)      772 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_persistent_event.2
--rw-rw-r--   0 root         (0) root         (0)      836 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_phy_rx_eom.2
--rw-rw-r--   0 root         (0) root         (0)      836 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2
--rw-rw-r--   0 root         (0) root         (0)      687 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2
--rw-rw-r--   0 root         (0) root         (0)      637 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_reservation.2
--rw-rw-r--   0 root         (0) root         (0)      756 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_sanitize.2
--rw-rw-r--   0 root         (0) root         (0)      836 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_simple.2
--rw-rw-r--   0 root         (0) root         (0)     1089 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_smart.2
--rw-rw-r--   0 root         (0) root         (0)      741 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2
--rw-rw-r--   0 root         (0) root         (0)      676 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_supported_log_pages.2
--rw-rw-r--   0 root         (0) root         (0)      922 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      849 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_telemetry_host.2
--rw-rw-r--   0 root         (0) root         (0)      807 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2
--rw-rw-r--   0 root         (0) root         (0)     1052 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_get_nsid_log.2
--rw-rw-r--   0 root         (0) root         (0)      882 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify.2
--rw-rw-r--   0 root         (0) root         (0)     1069 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_active_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_allocated_ns.2
--rw-rw-r--   0 root         (0) root         (0)     1087 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_allocated_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)     1135 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_cns_nsid.2
--rw-rw-r--   0 root         (0) root         (0)      889 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      984 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      759 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_ns.2
--rw-rw-r--   0 root         (0) root         (0)      856 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_ns_descs.2
--rw-rw-r--   0 root         (0) root         (0)     1104 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)     1553 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_partial.2
--rw-rw-r--   0 root         (0) root         (0)      994 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_primary_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)     1046 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      544 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_ns_attach.2
--rw-rw-r--   0 root         (0) root         (0)      633 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_ns_attach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      635 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_ns_detach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)     1692 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_req_hdr.2
--rw-rw-r--   0 root         (0) root         (0)      776 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_resp_hdr.2
--rw-rw-r--   0 root         (0) root         (0)     1119 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_sanitize_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      996 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_security_recv.2
--rw-rw-r--   0 root         (0) root         (0)      981 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_security_send.2
--rw-rw-r--   0 root         (0) root         (0)     1706 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_admin_xfer.2
--rw-rw-r--   0 root         (0) root         (0)     1259 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_ccs.2
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_close.2
--rw-rw-r--   0 root         (0) root         (0)      263 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_close_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)     1908 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_cmd_supported_effects.2
--rw-rw-r--   0 root         (0) root         (0)      507 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_cmd_supported_effects_log.2
--rw-rw-r--   0 root         (0) root         (0)      799 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_config_id.2
--rw-rw-r--   0 root         (0) root         (0)      678 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_config_smbus_freq.2
--rw-rw-r--   0 root         (0) root         (0)      637 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_create_root.2
--rw-rw-r--   0 root         (0) root         (0)      822 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_csts.2
--rw-rw-r--   0 root         (0) root         (0)      664 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_ctrl_health_status.2
--rw-rw-r--   0 root         (0) root         (0)      567 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_ctrl_id.2
--rw-rw-r--   0 root         (0) root         (0)      657 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_cwarn.2
--rw-rw-r--   0 root         (0) root         (0)      967 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_dtyp.2
--rw-rw-r--   0 root         (0) root         (0)      867 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_elem.2
--rw-rw-r--   0 root         (0) root         (0)      250 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_free_root.2
--rw-rw-r--   0 root         (0) root         (0)      636 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_init_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      677 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_message_type.2
--rw-rw-r--   0 root         (0) root         (0)      720 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_opcode.2
--rw-rw-r--   0 root         (0) root         (0)      818 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      835 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      870 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_port.2
--rw-rw-r--   0 root         (0) root         (0)      744 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_subsys.2
--rw-rw-r--   0 root         (0) root         (0)      709 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_req_hdr.2
--rw-rw-r--   0 root         (0) root         (0)      605 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_resp_hdr.2
--rw-rw-r--   0 root         (0) root         (0)     1015 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_mi_subsystem_health_status_poll.2
--rw-rw-r--   0 root         (0) root         (0)      710 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_msg_hdr.2
--rw-rw-r--   0 root         (0) root         (0)      659 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_msg_resp.2
--rw-rw-r--   0 root         (0) root         (0)      611 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_nvm_ss_health_status.2
--rw-rw-r--   0 root         (0) root         (0)      701 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_open_mctp.2
--rw-rw-r--   0 root         (0) root         (0)      307 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_osc.2
--rw-rw-r--   0 root         (0) root         (0)      637 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_port_pcie.2
--rw-rw-r--   0 root         (0) root         (0)      681 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_port_smb.2
--rw-rw-r--   0 root         (0) root         (0)      766 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_read_ctrl_info.2
--rw-rw-r--   0 root         (0) root         (0)      488 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_read_nvm_ss_info.2
--rw-rw-r--   0 root         (0) root         (0)      731 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_read_port_info.2
--rw-rw-r--   0 root         (0) root         (0)      445 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_read_sc_list.2
--rw-rw-r--   0 root         (0) root         (0)     2414 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_resp_status.2
--rw-rw-r--   0 root         (0) root         (0)      602 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_set_probe_enabled.2
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_status_to_string.2
--rw-rw-r--   0 root         (0) root         (0)      843 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_hdr.2
--rw-rw-r--   0 root         (0) root         (0)      837 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_mr_common.2
--rw-rw-r--   0 root         (0) root         (0)     1385 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_mra.2
--rw-rw-r--   0 root         (0) root         (0)      751 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_ppmra.2
--rw-rw-r--   0 root         (0) root         (0)      551 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_telem.2
--rw-rw-r--   0 root         (0) root         (0)      451 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_mi_vpd_tra.2
--rw-rw-r--   0 root         (0) root         (0)      678 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_attach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      680 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_detach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      322 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_filter.2
--rw-rw-r--   0 root         (0) root         (0)      359 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_first_path.2
--rw-rw-r--   0 root         (0) root         (0)      323 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_for_each_path.2
--rw-rw-r--   0 root         (0) root         (0)      423 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_for_each_path_safe.2
--rw-rw-r--   0 root         (0) root         (0)      448 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_namespace_next_path.2
--rw-rw-r--   0 root         (0) root         (0)      280 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nbft_free.2
--rw-rw-r--   0 root         (0) root         (0)      532 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nbft_read.2
--rw-rw-r--   0 root         (0) root         (0)      566 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nd_ns_fpi.2
--rw-rw-r--   0 root         (0) root         (0)      383 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_next_host.2
--rw-rw-r--   0 root         (0) root         (0)      428 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_next_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      449 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_attach.2
--rw-rw-r--   0 root         (0) root         (0)      583 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_attach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      435 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_attach_sel.2
--rw-rw-r--   0 root         (0) root         (0)      490 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_compare.2
--rw-rw-r--   0 root         (0) root         (0)      585 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_detach_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      279 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_flush.2
--rw-rw-r--   0 root         (0) root         (0)      328 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_csi.2
--rw-rw-r--   0 root         (0) root         (0)      392 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      308 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_eui64.2
--rw-rw-r--   0 root         (0) root         (0)      646 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_fd.2
--rw-rw-r--   0 root         (0) root         (0)      321 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_firmware.2
--rw-rw-r--   0 root         (0) root         (0)      356 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_generic_name.2
--rw-rw-r--   0 root         (0) root         (0)      309 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_lba_count.2
--rw-rw-r--   0 root         (0) root         (0)      298 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_lba_size.2
--rw-rw-r--   0 root         (0) root         (0)      317 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_lba_util.2
--rw-rw-r--   0 root         (0) root         (0)      312 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_meta_size.2
--rw-rw-r--   0 root         (0) root         (0)      296 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_model.2
--rw-rw-r--   0 root         (0) root         (0)      295 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_name.2
--rw-rw-r--   0 root         (0) root         (0)      314 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_nguid.2
--rw-rw-r--   0 root         (0) root         (0)      274 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_nsid.2
--rw-rw-r--   0 root         (0) root         (0)      316 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_serial.2
--rw-rw-r--   0 root         (0) root         (0)      339 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_subsystem.2
--rw-rw-r--   0 root         (0) root         (0)      330 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_sysfs_dir.2
--rw-rw-r--   0 root         (0) root         (0)      385 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_get_uuid.2
--rw-rw-r--   0 root         (0) root         (0)      717 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_id_desc.2
--rw-rw-r--   0 root         (0) root         (0)      820 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_id_desc_nidt.2
--rw-rw-r--   0 root         (0) root         (0)      467 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_identify.2
--rw-rw-r--   0 root         (0) root         (0)      514 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_identify_descs.2
--rw-rw-r--   0 root         (0) root         (0)      264 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_list.2
--rw-rw-r--   0 root         (0) root         (0)      779 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_metadata_type.2
--rw-rw-r--   0 root         (0) root         (0)      430 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_mgmt.2
--rw-rw-r--   0 root         (0) root         (0)     1146 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_mgmt_create.2
--rw-rw-r--   0 root         (0) root         (0)      655 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_mgmt_delete.2
--rw-rw-r--   0 root         (0) root         (0)     2930 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_mgmt_host_sw_specified.2
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_mgmt_sel.2
--rw-rw-r--   0 root         (0) root         (0)      499 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_read.2
--rw-rw-r--   0 root         (0) root         (0)      271 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_release_fd.2
--rw-rw-r--   0 root         (0) root         (0)      412 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_rescan.2
--rw-rw-r--   0 root         (0) root         (0)      420 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_verify.2
--rw-rw-r--   0 root         (0) root         (0)      488 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_write.2
--rw-rw-r--   0 root         (0) root         (0)      655 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_write_protect_cfg.2
--rw-rw-r--   0 root         (0) root         (0)      481 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_write_uncorrectable.2
--rw-rw-r--   0 root         (0) root         (0)      438 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_ns_write_zeros.2
--rw-rw-r--   0 root         (0) root         (0)      500 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nss_hw_err_event.2
--rw-rw-r--   0 root         (0) root         (0)      595 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvm_id_ns.2
--rw-rw-r--   0 root         (0) root         (0)      548 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvm_id_ns_elbaf.2
--rw-rw-r--   0 root         (0) root         (0)      618 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvm_identify_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      594 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvmeset_pl_status.2
--rw-rw-r--   0 root         (0) root         (0)      947 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvmset_attr.2
--rw-rw-r--   0 root         (0) root         (0)      957 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvmset_pl_events.2
--rw-rw-r--   0 root         (0) root         (0)     1216 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_nvmset_predictable_lat_log.2
--rw-rw-r--   0 root         (0) root         (0)      482 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_open.2
--rw-rw-r--   0 root         (0) root         (0)     1798 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_passthru_cmd.2
--rw-rw-r--   0 root         (0) root         (0)     1913 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_passthru_cmd64.2
--rw-rw-r--   0 root         (0) root         (0)      371 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_path_get_ana_state.2
--rw-rw-r--   0 root         (0) root         (0)      334 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_path_get_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      322 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_path_get_name.2
--rw-rw-r--   0 root         (0) root         (0)      322 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_path_get_ns.2
--rw-rw-r--   0 root         (0) root         (0)      351 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_path_get_sysfs_dir.2
--rw-rw-r--   0 root         (0) root         (0)      301 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_paths_filter.2
--rw-rw-r--   0 root         (0) root         (0)      842 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_persistent_event_entry.2
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_persistent_event_log.2
--rw-rw-r--   0 root         (0) root         (0)     1676 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_persistent_event_types.2
--rw-rw-r--   0 root         (0) root         (0)      525 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_pevent_log_action.2
--rw-rw-r--   0 root         (0) root         (0)     1648 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_phy_rx_eom_log.2
--rw-rw-r--   0 root         (0) root         (0)      504 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_phy_rx_eom_progress.2
--rw-rw-r--   0 root         (0) root         (0)      627 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_plm_config.2
--rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_pmr_size.2
--rw-rw-r--   0 root         (0) root         (0)      404 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_pmr_throughput.2
--rw-rw-r--   0 root         (0) root         (0)      758 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_power_on_reset_info_list.2
--rw-rw-r--   0 root         (0) root         (0)     1553 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_primary_ctrl_cap.2
--rw-rw-r--   0 root         (0) root         (0)      814 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_psd_flags.2
--rw-rw-r--   0 root         (0) root         (0)      315 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_psd_power_scale.2
--rw-rw-r--   0 root         (0) root         (0)      569 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_psd_ps.2
--rw-rw-r--   0 root         (0) root         (0)     1182 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_psd_workload.2
--rw-rw-r--   0 root         (0) root         (0)      404 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_read.2
--rw-rw-r--   0 root         (0) root         (0)      504 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_read_config.2
--rw-rw-r--   0 root         (0) root         (0)      369 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_refresh_topology.2
--rw-rw-r--   0 root         (0) root         (0)     2856 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_register_offsets.2
--rw-rw-r--   0 root         (0) root         (0)      521 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_registered_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      600 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_registered_ctrl_ext.2
--rw-rw-r--   0 root         (0) root         (0)      259 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_rescan_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      628 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_acquire.2
--rw-rw-r--   0 root         (0) root         (0)      642 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_cptpl.2
--rw-rw-r--   0 root         (0) root         (0)      607 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_notification_log.2
--rw-rw-r--   0 root         (0) root         (0)      774 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_notify_rnlpt.2
--rw-rw-r--   0 root         (0) root         (0)      533 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_racqa.2
--rw-rw-r--   0 root         (0) root         (0)      569 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_register.2
--rw-rw-r--   0 root         (0) root         (0)      456 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_release.2
--rw-rw-r--   0 root         (0) root         (0)      689 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_report.2
--rw-rw-r--   0 root         (0) root         (0)      589 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_rrega.2
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_rrela.2
--rw-rw-r--   0 root         (0) root         (0)      933 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_rtype.2
--rw-rw-r--   0 root         (0) root         (0)     1045 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_resv_status.2
--rw-rw-r--   0 root         (0) root         (0)      512 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_compln_event.2
--rw-rw-r--   0 root         (0) root         (0)     4692 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_log_page.2
--rw-rw-r--   0 root         (0) root         (0)     1025 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_nvm.2
--rw-rw-r--   0 root         (0) root         (0)      744 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_sanact.2
--rw-rw-r--   0 root         (0) root         (0)     2817 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_sstat.2
--rw-rw-r--   0 root         (0) root         (0)      428 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_sanitize_start_event.2
--rw-rw-r--   0 root         (0) root         (0)      296 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan.2
--rw-rw-r--   0 root         (0) root         (0)      433 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      448 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_ctrl_namespace_paths.2
--rw-rw-r--   0 root         (0) root         (0)      414 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_ctrl_namespaces.2
--rw-rw-r--   0 root         (0) root         (0)      312 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_ctrls.2
--rw-rw-r--   0 root         (0) root         (0)      355 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_namespace.2
--rw-rw-r--   0 root         (0) root         (0)      437 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_subsystem_namespaces.2
--rw-rw-r--   0 root         (0) root         (0)      334 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_subsystems.2
--rw-rw-r--   0 root         (0) root         (0)      549 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_scan_topology.2
--rw-rw-r--   0 root         (0) root         (0)      758 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_secondary_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      467 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_secondary_ctrl_list.2
--rw-rw-r--   0 root         (0) root         (0)      467 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_security_receive.2
--rw-rw-r--   0 root         (0) root         (0)      896 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_security_send.2
--rw-rw-r--   0 root         (0) root         (0)     1535 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_self_test_log.2
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_feature_event.2
--rw-rw-r--   0 root         (0) root         (0)      447 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features.2
--rw-rw-r--   0 root         (0) root         (0)      812 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_arbitration.2
--rw-rw-r--   0 root         (0) root         (0)      660 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_async_event.2
--rw-rw-r--   0 root         (0) root         (0)      765 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_auto_pst.2
--rw-rw-r--   0 root         (0) root         (0)      943 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_data.2
--rw-rw-r--   0 root         (0) root         (0)      809 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_endurance_evt_cfg.2
--rw-rw-r--   0 root         (0) root         (0)      813 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_err_recovery.2
--rw-rw-r--   0 root         (0) root         (0)      714 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_hctm.2
--rw-rw-r--   0 root         (0) root         (0)      625 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_host_behavior.2
--rw-rw-r--   0 root         (0) root         (0)      638 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_host_id.2
--rw-rw-r--   0 root         (0) root         (0)      596 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_iocs_profile.2
--rw-rw-r--   0 root         (0) root         (0)      709 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_irq_coalesce.2
--rw-rw-r--   0 root         (0) root         (0)      691 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_irq_config.2
--rw-rw-r--   0 root         (0) root         (0)      800 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_lba_range.2
--rw-rw-r--   0 root         (0) root         (0)      780 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_lba_sts_interval.2
--rw-rw-r--   0 root         (0) root         (0)      678 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_nopsc.2
--rw-rw-r--   0 root         (0) root         (0)      822 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_plm_config.2
--rw-rw-r--   0 root         (0) root         (0)      733 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_plm_window.2
--rw-rw-r--   0 root         (0) root         (0)      686 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_power_mgmt.2
--rw-rw-r--   0 root         (0) root         (0)      792 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_resv_mask.2
--rw-rw-r--   0 root         (0) root         (0)      732 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_resv_mask2.2
--rw-rw-r--   0 root         (0) root         (0)      794 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_resv_persist.2
--rw-rw-r--   0 root         (0) root         (0)      731 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_resv_persist2.2
--rw-rw-r--   0 root         (0) root         (0)      689 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_rrl.2
--rw-rw-r--   0 root         (0) root         (0)      646 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_sanitize.2
--rw-rw-r--   0 root         (0) root         (0)      777 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_simple.2
--rw-rw-r--   0 root         (0) root         (0)      679 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_sw_progress.2
--rw-rw-r--   0 root         (0) root         (0)      821 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_temp_thresh.2
--rw-rw-r--   0 root         (0) root         (0)      598 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_timestamp.2
--rw-rw-r--   0 root         (0) root         (0)      657 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_volatile_wc.2
--rw-rw-r--   0 root         (0) root         (0)      647 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_write_atomic.2
--rw-rw-r--   0 root         (0) root         (0)      808 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_write_protect.2
--rw-rw-r--   0 root         (0) root         (0)      744 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_features_write_protect2.2
--rw-rw-r--   0 root         (0) root         (0)      448 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_keyring.2
--rw-rw-r--   0 root         (0) root         (0)      597 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_property.2
--rw-rw-r--   0 root         (0) root         (0)      678 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_set_root.2
--rw-rw-r--   0 root         (0) root         (0)     1475 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_smart_crit.2
--rw-rw-r--   0 root         (0) root         (0)      874 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_smart_egcw.2
--rw-rw-r--   0 root         (0) root         (0)     9367 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_smart_log.2
--rw-rw-r--   0 root         (0) root         (0)      796 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_st_code.2
--rw-rw-r--   0 root         (0) root         (0)     1112 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_st_curr_op.2
--rw-rw-r--   0 root         (0) root         (0)     2754 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_st_result.2
--rw-rw-r--   0 root         (0) root         (0)      860 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_st_valid_diag_info.2
--rw-rw-r--   0 root         (0) root         (0)      360 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_code.2
--rw-rw-r--   0 root         (0) root         (0)      390 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_code_type.2
--rw-rw-r--   0 root         (0) root         (0)      521 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_equals.2
--rw-rw-r--   0 root         (0) root         (0)    28152 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_field.2
--rw-rw-r--   0 root         (0) root         (0)      369 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_get_type.2
--rw-rw-r--   0 root         (0) root         (0)      432 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_get_value.2
--rw-rw-r--   0 root         (0) root         (0)     2076 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_result.2
--rw-rw-r--   0 root         (0) root         (0)      542 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_to_errno.2
--rw-rw-r--   0 root         (0) root         (0)      556 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_to_string.2
--rw-rw-r--   0 root         (0) root         (0)     1074 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_status_type.2
--rw-rw-r--   0 root         (0) root         (0)      896 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_streams_directive_params.2
--rw-rw-r--   0 root         (0) root         (0)      383 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_streams_directive_status.2
--rw-rw-r--   0 root         (0) root         (0)      693 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_submit_admin_passthru.2
--rw-rw-r--   0 root         (0) root         (0)      713 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_submit_admin_passthru64.2
--rw-rw-r--   0 root         (0) root         (0)      669 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_submit_io_passthru.2
--rw-rw-r--   0 root         (0) root         (0)      689 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_submit_io_passthru64.2
--rw-rw-r--   0 root         (0) root         (0)      310 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsys_filter.2
--rw-rw-r--   0 root         (0) root         (0)     1299 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsys_type.2
--rw-rw-r--   0 root         (0) root         (0)      360 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_first_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_first_ns.2
--rw-rw-r--   0 root         (0) root         (0)      335 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_for_each_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      435 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_for_each_ctrl_safe.2
--rw-rw-r--   0 root         (0) root         (0)      329 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_for_each_ns.2
--rw-rw-r--   0 root         (0) root         (0)      427 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_for_each_ns_safe.2
--rw-rw-r--   0 root         (0) root         (0)      393 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_application.2
--rw-rw-r--   0 root         (0) root         (0)      337 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_host.2
--rw-rw-r--   0 root         (0) root         (0)      372 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_iopolicy.2
--rw-rw-r--   0 root         (0) root         (0)      350 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_name.2
--rw-rw-r--   0 root         (0) root         (0)      328 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_nqn.2
--rw-rw-r--   0 root         (0) root         (0)      385 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_sysfs_dir.2
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_get_type.2
--rw-rw-r--   0 root         (0) root         (0)      464 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_lookup_namespace.2
--rw-rw-r--   0 root         (0) root         (0)      443 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_next_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      430 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_next_ns.2
--rw-rw-r--   0 root         (0) root         (0)      500 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_release_fds.2
--rw-rw-r--   0 root         (0) root         (0)      446 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_reset.2
--rw-rw-r--   0 root         (0) root         (0)      445 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_subsystem_set_application.2
--rw-rw-r--   0 root         (0) root         (0)      578 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_supported_cap_config_list_log.2
--rw-rw-r--   0 root         (0) root         (0)      410 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_supported_log_pages.2
--rw-rw-r--   0 root         (0) root         (0)      512 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_telemetry_da.2
--rw-rw-r--   0 root         (0) root         (0)     2630 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_telemetry_log.2
--rw-rw-r--   0 root         (0) root         (0)      366 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_thermal_exc_event.2
--rw-rw-r--   0 root         (0) root         (0)      425 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_time_stamp_change_event.2
--rw-rw-r--   0 root         (0) root         (0)      417 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_timestamp.2
--rw-rw-r--   0 root         (0) root         (0)      253 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_unlink_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      387 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_update_config.2
--rw-rw-r--   0 root         (0) root         (0)     1772 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_uring_cmd.2
--rw-rw-r--   0 root         (0) root         (0)      608 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_verify.2
--rw-rw-r--   0 root         (0) root         (0)      376 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_version.2
--rw-rw-r--   0 root         (0) root         (0)      734 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_virt_mgmt_act.2
--rw-rw-r--   0 root         (0) root         (0)      408 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_virt_mgmt_rt.2
--rw-rw-r--   0 root         (0) root         (0)      842 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_virtual_mgmt.2
--rw-rw-r--   0 root         (0) root         (0)      409 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_write.2
--rw-rw-r--   0 root         (0) root         (0)      791 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_write_uncorrectable.2
--rw-rw-r--   0 root         (0) root         (0)      708 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_write_zeros.2
--rw-rw-r--   0 root         (0) root         (0)      433 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_append.2
--rw-rw-r--   0 root         (0) root         (0)      441 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_changed_zone_log.2
--rw-rw-r--   0 root         (0) root         (0)      702 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_desc.2
--rw-rw-r--   0 root         (0) root         (0)      396 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_id_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)     1502 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_id_ns.2
--rw-rw-r--   0 root         (0) root         (0)      521 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_identify_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      573 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_identify_ns.2
--rw-rw-r--   0 root         (0) root         (0)      386 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_lbafe.2
--rw-rw-r--   0 root         (0) root         (0)      460 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_mgmt_recv.2
--rw-rw-r--   0 root         (0) root         (0)      457 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_mgmt_send.2
--rw-rw-r--   0 root         (0) root         (0)      450 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_recv_action.2
--rw-rw-r--   0 root         (0) root         (0)     1257 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_report_options.2
--rw-rw-r--   0 root         (0) root         (0)     1010 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_report_zones.2
--rw-rw-r--   0 root         (0) root         (0)      806 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_send_action.2
--rw-rw-r--   0 root         (0) root         (0)      596 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_za.2
--rw-rw-r--   0 root         (0) root         (0)      786 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_zs.2
--rw-rw-r--   0 root         (0) root         (0)      297 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zns_zt.2
--rw-rw-r--   0 root         (0) root         (0)      446 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvme_zone_report.2
--rw-rw-r--   0 root         (0) root         (0)      721 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_add_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      844 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_addr_family.2
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_adrfam_str.2
--rw-rw-r--   0 root         (0) root         (0)      397 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_cms_str.2
--rw-rw-r--   0 root         (0) root         (0)      669 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_connect_data.2
--rw-rw-r--   0 root         (0) root         (0)      703 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_connect_disc_entry.2
--rw-rw-r--   0 root         (0) root         (0)      364 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_default_config.2
--rw-rw-r--   0 root         (0) root         (0)     1157 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_dim_data.2
--rw-rw-r--   0 root         (0) root         (0)      425 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_dim_entfmt.2
--rw-rw-r--   0 root         (0) root         (0)      468 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_dim_etype.2
--rw-rw-r--   0 root         (0) root         (0)      432 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_dim_tas.2
--rw-rw-r--   0 root         (0) root         (0)     1333 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_disc_eflags.2
--rw-rw-r--   0 root         (0) root         (0)     3361 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_disc_log_entry.2
--rw-rw-r--   0 root         (0) root         (0)     1158 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_discovery_log.2
--rw-rw-r--   0 root         (0) root         (0)      360 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_eflags_str.2
--rw-rw-r--   0 root         (0) root         (0)      445 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_exat_len.2
--rw-rw-r--   0 root         (0) root         (0)      347 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_exattype.2
--rw-rw-r--   0 root         (0) root         (0)      536 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_ext_attr.2
--rw-rw-r--   0 root         (0) root         (0)     1512 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_ext_die.2
--rw-rw-r--   0 root         (0) root         (0)      739 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_get_discovery_log.2
--rw-rw-r--   0 root         (0) root         (0)      804 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_get_discovery_wargs.2
--rw-rw-r--   0 root         (0) root         (0)      495 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_hostid_from_file.2
--rw-rw-r--   0 root         (0) root         (0)      497 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_hostnqn_from_file.2
--rw-rw-r--   0 root         (0) root         (0)      341 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_hostnqn_generate.2
--rw-rw-r--   0 root         (0) root         (0)      673 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_log_discovery_lid_support.2
--rw-rw-r--   0 root         (0) root         (0)      611 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_log_discovery_lsp.2
--rw-rw-r--   0 root         (0) root         (0)      383 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_prtype_str.2
--rw-rw-r--   0 root         (0) root         (0)      387 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_qptype_str.2
--rw-rw-r--   0 root         (0) root         (0)      351 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_rdma_cms.2
--rw-rw-r--   0 root         (0) root         (0)      697 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_rdma_prtype.2
--rw-rw-r--   0 root         (0) root         (0)      439 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_rdma_qptype.2
--rw-rw-r--   0 root         (0) root         (0)      784 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_register_ctrl.2
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_sectype_str.2
--rw-rw-r--   0 root         (0) root         (0)      374 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_subtype_str.2
--rw-rw-r--   0 root         (0) root         (0)      641 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_tcp_sectype.2
--rw-rw-r--   0 root         (0) root         (0)      577 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_treq.2
--rw-rw-r--   0 root         (0) root         (0)      361 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_treq_str.2
--rw-rw-r--   0 root         (0) root         (0)      737 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_trtype.2
--rw-rw-r--   0 root         (0) root         (0)      367 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_trtype_str.2
--rw-rw-r--   0 root         (0) root         (0)      543 2024-02-14 09:40:43.000000 libnvme-1.8/doc/man/nvmf_update_config.2
--rw-rw-r--   0 root         (0) root         (0)     3076 2024-02-14 09:40:43.000000 libnvme-1.8/doc/meson.build
--rw-rw-r--   0 root         (0) root         (0)     2763 2024-02-14 09:40:43.000000 libnvme-1.8/doc/mi.rst.in
--rw-rw-r--   0 root         (0) root         (0)       37 2024-02-14 09:40:43.000000 libnvme-1.8/doc/quickstart.rst.in
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/
--rw-rw-r--   0 root         (0) root         (0)    10052 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/fabrics.rst
--rw-rw-r--   0 root         (0) root         (0)     2133 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/filters.rst
--rw-rw-r--   0 root         (0) root         (0)   126680 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/ioctl.rst
--rw-rw-r--   0 root         (0) root         (0)    12572 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/linux.rst
--rw-rw-r--   0 root         (0) root         (0)     1020 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/log.rst
--rw-rw-r--   0 root         (0) root         (0)     1018 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/meson.build
--rw-rw-r--   0 root         (0) root         (0)    80384 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/mi.rst
--rw-rw-r--   0 root         (0) root         (0)    50791 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/nbft.rst
--rw-rw-r--   0 root         (0) root         (0)    41582 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/tree.rst
--rw-rw-r--   0 root         (0) root         (0)   233283 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/types.rst
--rw-rw-r--   0 root         (0) root         (0)    15666 2024-02-14 09:40:43.000000 libnvme-1.8/doc/rst/util.rst
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/examples/
--rw-rw-r--   0 root         (0) root         (0)     2631 2024-02-14 09:40:43.000000 libnvme-1.8/examples/discover-loop.c
--rw-rw-r--   0 root         (0) root         (0)     1952 2024-02-14 09:40:43.000000 libnvme-1.8/examples/discover-loop.py
--rw-rw-r--   0 root         (0) root         (0)     3090 2024-02-14 09:40:43.000000 libnvme-1.8/examples/display-columnar.c
--rw-rw-r--   0 root         (0) root         (0)     1869 2024-02-14 09:40:43.000000 libnvme-1.8/examples/display-tree.c
--rw-rw-r--   0 root         (0) root         (0)     1085 2024-02-14 09:40:43.000000 libnvme-1.8/examples/meson.build
--rw-rw-r--   0 root         (0) root         (0)     4906 2024-02-14 09:40:43.000000 libnvme-1.8/examples/mi-conf.c
--rw-rw-r--   0 root         (0) root         (0)    18343 2024-02-14 09:40:43.000000 libnvme-1.8/examples/mi-mctp.c
--rw-rw-r--   0 root         (0) root         (0)     3306 2024-02-14 09:40:43.000000 libnvme-1.8/examples/telemetry-listen.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/internal/
--rw-rw-r--   0 root         (0) root         (0)      671 2024-02-14 09:40:43.000000 libnvme-1.8/internal/meson.build
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/
--rw-rw-r--   0 root         (0) root         (0)       40 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     2146 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/README.md
--rw-rw-r--   0 root         (0) root         (0)      231 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3243 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/meson.build
--rw-rw-r--   0 root         (0) root         (0)    30479 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/nvme.i
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/tests/
--rw-rw-r--   0 root         (0) root         (0)     1017 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/tests/NBFT
--rwxrwxr-x   0 root         (0) root         (0)      393 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/tests/create-ctrl-obj.py
--rwxrwxr-x   0 root         (0) root         (0)      958 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/tests/gc.py
--rwxrwxr-x   0 root         (0) root         (0)     3468 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme/tests/test-nbft.py
--rw-rw-r--   0 root         (0) root         (0)     1313 2024-02-14 09:40:43.000000 libnvme-1.8/libnvme.spec.in
--rw-rw-r--   0 root         (0) root         (0)     9011 2024-02-14 09:40:43.000000 libnvme-1.8/meson.build
--rw-rw-r--   0 root         (0) root         (0)     1075 2024-02-14 09:40:43.000000 libnvme-1.8/meson_options.txt
--rw-rw-r--   0 root         (0) root         (0)      930 2024-02-14 09:40:43.000000 libnvme-1.8/pyproject.toml
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/
--rwxrwxr-x   0 root         (0) root         (0)     5987 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/build.sh
--rwxrwxr-x   0 root         (0) root         (0)      461 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/collect-sysfs.sh
--rwxrwxr-x   0 root         (0) root         (0)    70557 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/kernel-doc
--rwxrwxr-x   0 root         (0) root         (0)      264 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/kernel-doc-check
--rwxrwxr-x   0 root         (0) root         (0)      354 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/list-man-pages.sh
--rwxrwxr-x   0 root         (0) root         (0)       47 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/list-pre-compiled.sh
--rwxrwxr-x   0 root         (0) root         (0)      613 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/meson-vcs-tag.sh
--rwxrwxr-x   0 root         (0) root         (0)     3195 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/release.sh
--rwxrwxr-x   0 root         (0) root         (0)     1002 2024-02-14 09:40:43.000000 libnvme-1.8/scripts/update-docs.sh
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/src/
--rw-rw-r--   0 root         (0) root         (0)      394 2024-02-14 09:40:43.000000 libnvme-1.8/src/libnvme-mi.h
--rw-rw-r--   0 root         (0) root         (0)     1254 2024-02-14 09:40:43.000000 libnvme-1.8/src/libnvme-mi.map
--rw-rw-r--   0 root         (0) root         (0)      609 2024-02-14 09:40:43.000000 libnvme-1.8/src/libnvme.h
--rw-rw-r--   0 root         (0) root         (0)     8355 2024-02-14 09:40:43.000000 libnvme-1.8/src/libnvme.map
--rw-rw-r--   0 root         (0) root         (0)     3273 2024-02-14 09:40:43.000000 libnvme-1.8/src/meson.build
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/
--rw-rw-r--   0 root         (0) root         (0)    28102 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/api-types.h
--rw-rw-r--   0 root         (0) root         (0)     2028 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/base64.c
--rw-rw-r--   0 root         (0) root         (0)      239 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/base64.h
--rw-rw-r--   0 root         (0) root         (0)      874 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/cleanup.h
--rw-rw-r--   0 root         (0) root         (0)    45153 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/fabrics.c
--rw-rw-r--   0 root         (0) root         (0)     9778 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/fabrics.h
--rw-rw-r--   0 root         (0) root         (0)     3247 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/filters.c
--rw-rw-r--   0 root         (0) root         (0)     2216 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/filters.h
--rw-rw-r--   0 root         (0) root         (0)    60882 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/ioctl.c
--rw-rw-r--   0 root         (0) root         (0)   137285 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/ioctl.h
--rw-rw-r--   0 root         (0) root         (0)    18580 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/json.c
--rw-rw-r--   0 root         (0) root         (0)    27637 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/linux.c
--rw-rw-r--   0 root         (0) root         (0)    11892 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/linux.h
--rw-rw-r--   0 root         (0) root         (0)     1999 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/log.c
--rw-rw-r--   0 root         (0) root         (0)     1315 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/log.h
--rw-rw-r--   0 root         (0) root         (0)    18546 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/mi-mctp.c
--rw-rw-r--   0 root         (0) root         (0)    40182 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/mi.c
--rw-rw-r--   0 root         (0) root         (0)    90262 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/mi.h
--rw-rw-r--   0 root         (0) root         (0)    21502 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/nbft.c
--rw-rw-r--   0 root         (0) root         (0)    55759 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/nbft.h
--rw-rw-r--   0 root         (0) root         (0)      445 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/no-json.c
--rw-rw-r--   0 root         (0) root         (0)     6364 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/private.h
--rw-rw-r--   0 root         (0) root         (0)    62561 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/tree.c
--rw-rw-r--   0 root         (0) root         (0)    39572 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/tree.h
--rw-rw-r--   0 root         (0) root         (0)   288712 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/types.h
--rw-rw-r--   0 root         (0) root         (0)    42682 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/util.c
--rw-rw-r--   0 root         (0) root         (0)    23271 2024-02-14 09:40:43.000000 libnvme-1.8/src/nvme/util.h
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/subprojects/
--rw-rw-r--   0 root         (0) root         (0)      124 2024-02-14 09:40:43.000000 libnvme-1.8/subprojects/dbus.wrap
--rw-rw-r--   0 root         (0) root         (0)      587 2024-02-14 09:40:43.000000 libnvme-1.8/subprojects/json-c.wrap
--rw-rw-r--   0 root         (0) root         (0)      631 2024-02-14 09:40:43.000000 libnvme-1.8/subprojects/openssl.wrap
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/
--rw-rw-r--   0 root         (0) root         (0)     1490 2024-02-14 09:40:43.000000 libnvme-1.8/test/cpp.cc
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/
--rw-rw-r--   0 root         (0) root         (0)    12790 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/discovery.c
--rw-rw-r--   0 root         (0) root         (0)    45840 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/features.c
--rw-rw-r--   0 root         (0) root         (0)    16354 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/identify.c
--rw-rw-r--   0 root         (0) root         (0)     1245 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/meson.build
--rw-rw-r--   0 root         (0) root         (0)     5061 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/mock.c
--rw-rw-r--   0 root         (0) root         (0)     3817 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/mock.h
--rw-rw-r--   0 root         (0) root         (0)     1047 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/util.c
--rw-rw-r--   0 root         (0) root         (0)      521 2024-02-14 09:40:43.000000 libnvme-1.8/test/ioctl/util.h
--rw-rw-r--   0 root         (0) root         (0)     2374 2024-02-14 09:40:43.000000 libnvme-1.8/test/meson.build
--rw-rw-r--   0 root         (0) root         (0)    18560 2024-02-14 09:40:43.000000 libnvme-1.8/test/mi-mctp.c
--rw-rw-r--   0 root         (0) root         (0)    43409 2024-02-14 09:40:43.000000 libnvme-1.8/test/mi.c
--rw-rw-r--   0 root         (0) root         (0)     3291 2024-02-14 09:40:43.000000 libnvme-1.8/test/mock-ifaddrs.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/
--rw-rw-r--   0 root         (0) root         (0)      847 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/README
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/
--rw-rw-r--   0 root         (0) root         (0)     2199 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-Dell.PowerEdge.R660-fw1.5.5-single
--rw-rw-r--   0 root         (0) root         (0)     2454 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-Dell.PowerEdge.R760
--rw-rw-r--   0 root         (0) root         (0)     1551 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-auto-ipv6
--rw-rw-r--   0 root         (0) root         (0)     1756 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-dhcp-ipv4
--rw-rw-r--   0 root         (0) root         (0)     1516 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-dhcp-ipv6
--rw-rw-r--   0 root         (0) root         (0)     1526 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-rhpoc
--rw-rw-r--   0 root         (0) root         (0)     1525 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-static-ipv4
--rw-rw-r--   0 root         (0) root         (0)     1739 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-static-ipv4-discovery
--rw-rw-r--   0 root         (0) root         (0)     1525 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/diffs/NBFT-static-ipv6
--rwxrwxr-x   0 root         (0) root         (0)      101 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/gen-nbft-diffs.sh.in
--rw-rw-r--   0 root         (0) root         (0)     1761 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/meson.build
--rwxrwxr-x   0 root         (0) root         (0)      130 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/nbft-dump-diff.sh.in
--rw-rw-r--   0 root         (0) root         (0)     5100 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/nbft-dump.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/
--rw-rw-r--   0 root         (0) root         (0)      930 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-Dell.PowerEdge.R660-fw1.5.5-single
-lrwxrwxrwx   0 root         (0) root         (0)        0 2024-02-14 09:41:39.305446 libnvme-1.8/test/nbft/tables/NBFT-Dell.PowerEdge.R760 -> ../../../libnvme/tests/NBFT
--rw-rw-r--   0 root         (0) root         (0)      721 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-auto-ipv6
--rw-rw-r--   0 root         (0) root         (0)      825 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-dhcp-ipv4
--rw-rw-r--   0 root         (0) root         (0)      725 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-dhcp-ipv6
--rw-rw-r--   0 root         (0) root         (0)      724 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-rhpoc
--rw-rw-r--   0 root         (0) root         (0)      725 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-static-ipv4
--rw-rw-r--   0 root         (0) root         (0)      825 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-static-ipv4-discovery
--rw-rw-r--   0 root         (0) root         (0)      721 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables/NBFT-static-ipv6
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables_bad/
--rw-rw-r--   0 root         (0) root         (0)     1103 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables_bad/NBFT-bad-oldspec
--rw-rw-r--   0 root         (0) root         (0)      512 2024-02-14 09:40:43.000000 libnvme-1.8/test/nbft/tables_bad/NBFT-random-noise
--rw-rw-r--   0 root         (0) root         (0)     8522 2024-02-14 09:40:43.000000 libnvme-1.8/test/register.c
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/data/
--rw-rw-r--   0 root         (0) root         (0)      742 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.out
--rw-rw-r--   0 root         (0) root         (0)    19712 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.tar.xz
--rw-rw-r--   0 root         (0) root         (0)      858 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/meson.build
--rwxrwxr-x   0 root         (0) root         (0)      232 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/setup.sh
--rw-rw-r--   0 root         (0) root         (0)     1468 2024-02-14 09:40:43.000000 libnvme-1.8/test/sysfs/sysfs.c
--rw-rw-r--   0 root         (0) root         (0)     3659 2024-02-14 09:40:43.000000 libnvme-1.8/test/test-util.c
--rw-rw-r--   0 root         (0) root         (0)    12831 2024-02-14 09:40:43.000000 libnvme-1.8/test/test.c
--rw-rw-r--   0 root         (0) root         (0)    50475 2024-02-14 09:40:43.000000 libnvme-1.8/test/tree.c
--rw-rw-r--   0 root         (0) root         (0)      453 2024-02-14 09:40:43.000000 libnvme-1.8/test/tree.py
--rw-rw-r--   0 root         (0) root         (0)     1083 2024-02-14 09:40:43.000000 libnvme-1.8/test/utils.c
--rw-rw-r--   0 root         (0) root         (0)      455 2024-02-14 09:40:43.000000 libnvme-1.8/test/utils.h
--rw-rw-r--   0 root         (0) root         (0)     2648 2024-02-14 09:40:43.000000 libnvme-1.8/test/uuid.c
--rw-rw-r--   0 root         (0) root         (0)     1997 2024-02-14 09:40:43.000000 libnvme-1.8/test/zns.c
--rw-r--r--   0 root         (0) root         (0)     7683 2024-02-14 09:41:39.597449 libnvme-1.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 12:09:18.435984 libnvme-1.9/
+-rw-rw-r--   0 root         (0) root         (0)      619 2024-05-03 12:08:20.000000 libnvme-1.9/.checkpatch.conf
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/.github/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/.github/cross/
+-rw-rw-r--   0 root         (0) root         (0)      452 2024-05-03 12:08:20.000000 libnvme-1.9/.github/cross/ubuntu-cross-armhf.txt
+-rw-rw-r--   0 root         (0) root         (0)      465 2024-05-03 12:08:20.000000 libnvme-1.9/.github/cross/ubuntu-cross-ppc64le.txt
+-rw-rw-r--   0 root         (0) root         (0)      424 2024-05-03 12:08:20.000000 libnvme-1.9/.github/cross/ubuntu-cross-s390x.txt
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-05-03 12:08:20.000000 libnvme-1.9/.github/dependabot.yml
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/
+-rw-rw-r--   0 root         (0) root         (0)     2756 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/build.yml
+-rw-rw-r--   0 root         (0) root         (0)      465 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/checkpatch.yml
+-rw-rw-r--   0 root         (0) root         (0)      457 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/coverage.yml
+-rw-rw-r--   0 root         (0) root         (0)     1955 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/release-python.yml
+-rw-rw-r--   0 root         (0) root         (0)      395 2024-05-03 12:08:20.000000 libnvme-1.9/.github/workflows/release.yml
+-rw-rw-r--   0 root         (0) root         (0)      139 2024-05-03 12:08:20.000000 libnvme-1.9/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)      420 2024-05-03 12:08:20.000000 libnvme-1.9/.readthedocs.yaml
+-rw-rw-r--   0 root         (0) root         (0)    26530 2024-05-03 12:08:20.000000 libnvme-1.9/COPYING
+-rw-rw-r--   0 root         (0) root         (0)     1006 2024-05-03 12:08:20.000000 libnvme-1.9/Makefile
+-rw-rw-r--   0 root         (0) root         (0)     6900 2024-05-03 12:08:20.000000 libnvme-1.9/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/array_size/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.416360 libnvme-1.9/ccan/ccan/array_size/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1032 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/array_size/_info
+-rw-rw-r--   0 root         (0) root         (0)      889 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/array_size/array_size.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/build_assert/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.416360 libnvme-1.9/ccan/ccan/build_assert/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1350 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/build_assert/_info
+-rw-rw-r--   0 root         (0) root         (0)     1228 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/build_assert/build_assert.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/check_type/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.416360 libnvme-1.9/ccan/ccan/check_type/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)      841 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/check_type/_info
+-rw-rw-r--   0 root         (0) root         (0)     2368 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/check_type/check_type.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/container_of/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.416360 libnvme-1.9/ccan/ccan/container_of/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1386 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/container_of/_info
+-rw-rw-r--   0 root         (0) root         (0)     4278 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/container_of/container_of.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/endian/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.420360 libnvme-1.9/ccan/ccan/endian/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1419 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/endian/_info
+-rw-rw-r--   0 root         (0) root         (0)     9656 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/endian/endian.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/list/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.420360 libnvme-1.9/ccan/ccan/list/LICENSE -> ../../licenses/BSD-MIT
+-rw-rw-r--   0 root         (0) root         (0)     1519 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/list/_info
+-rw-rw-r--   0 root         (0) root         (0)     1000 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/list/list.c
+-rw-rw-r--   0 root         (0) root         (0)    24307 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/list/list.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/minmax/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.420360 libnvme-1.9/ccan/ccan/minmax/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1141 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/minmax/_info
+-rw-rw-r--   0 root         (0) root         (0)     1266 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/minmax/minmax.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/short_types/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.420360 libnvme-1.9/ccan/ccan/short_types/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)      793 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/short_types/short_types.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.420360 libnvme-1.9/ccan/ccan/str/LICENSE -> ../../licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/_info
+-rw-rw-r--   0 root         (0) root         (0)     1602 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/debug.c
+-rw-rw-r--   0 root         (0) root         (0)      283 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/str.c
+-rw-rw-r--   0 root         (0) root         (0)     5958 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/str.h
+-rw-rw-r--   0 root         (0) root         (0)      774 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/ccan/str/str_debug.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/licenses/
+-rw-rw-r--   0 root         (0) root         (0)     1023 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/licenses/BSD-MIT
+-rw-rw-r--   0 root         (0) root         (0)     6383 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/licenses/CC0
+-rw-rw-r--   0 root         (0) root         (0)      603 2024-05-03 12:08:20.000000 libnvme-1.9/ccan/meson.build
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-05-03 12:08:20.000000 libnvme-1.9/codecov.yml
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/doc/
+-rw-rw-r--   0 root         (0) root         (0)      418 2024-05-03 12:08:20.000000 libnvme-1.9/doc/api.rst.in
+-rw-rw-r--   0 root         (0) root         (0)     1054 2024-05-03 12:08:20.000000 libnvme-1.9/doc/conf.py
+-rw-rw-r--   0 root         (0) root         (0)     1060 2024-05-03 12:08:20.000000 libnvme-1.9/doc/conf.py.in
+-rw-rw-r--   0 root         (0) root         (0)     4533 2024-05-03 12:08:20.000000 libnvme-1.9/doc/config-schema.json
+-rw-rw-r--   0 root         (0) root         (0)     4533 2024-05-03 12:08:20.000000 libnvme-1.9/doc/config-schema.json.in
+-rw-rw-r--   0 root         (0) root         (0)      570 2024-05-03 12:08:20.000000 libnvme-1.9/doc/index.rst
+-rw-rw-r--   0 root         (0) root         (0)      570 2024-05-03 12:08:20.000000 libnvme-1.9/doc/index.rst.in
+-rw-rw-r--   0 root         (0) root         (0)      965 2024-05-03 12:08:20.000000 libnvme-1.9/doc/installation.rst.in
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/
+-rw-rw-r--   0 root         (0) root         (0)     5410 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_control.2
+-rw-rw-r--   0 root         (0) root         (0)      303 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_control_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     1567 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_desc_type.2
+-rw-rw-r--   0 root         (0) root         (0)     2319 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_discovery.2
+-rw-rw-r--   0 root         (0) root         (0)      378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_discovery_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     2980 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_header.2
+-rw-rw-r--   0 root         (0) root         (0)      421 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_heap_obj.2
+-rw-rw-r--   0 root         (0) root         (0)     1096 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_hfi.2
+-rw-rw-r--   0 root         (0) root         (0)      342 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_hfi_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     4746 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_hfi_info_tcp.2
+-rw-rw-r--   0 root         (0) root         (0)     1030 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_hfi_info_tcp_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      911 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_host.2
+-rw-rw-r--   0 root         (0) root         (0)     2237 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_host_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     1062 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info.2
+-rw-rw-r--   0 root         (0) root         (0)      812 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_discovery.2
+-rw-rw-r--   0 root         (0) root         (0)      595 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_hfi.2
+-rw-rw-r--   0 root         (0) root         (0)     2264 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_hfi_info_tcp.2
+-rw-rw-r--   0 root         (0) root         (0)      907 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_host.2
+-rw-rw-r--   0 root         (0) root         (0)      605 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_nid_type.2
+-rw-rw-r--   0 root         (0) root         (0)     1103 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_primary_admin_host_flag.2
+-rw-rw-r--   0 root         (0) root         (0)      339 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_security.2
+-rw-rw-r--   0 root         (0) root         (0)     2571 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_info_subsystem_ns.2
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_security.2
+-rw-rw-r--   0 root         (0) root         (0)     5118 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_security_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      496 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_security_secret_type.2
+-rw-rw-r--   0 root         (0) root         (0)     5477 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_ssns.2
+-rw-rw-r--   0 root         (0) root         (0)     1808 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_ssns_ext_info.2
+-rw-rw-r--   0 root         (0) root         (0)      773 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_ssns_ext_info_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     4072 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_ssns_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     1508 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_ssns_trflags.2
+-rw-rw-r--   0 root         (0) root         (0)      293 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nbft_trtype.2
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_acq.2
+-rw-rw-r--   0 root         (0) root         (0)     3521 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_admin_opcode.2
+-rw-rw-r--   0 root         (0) root         (0)     1887 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_admin_passthru.2
+-rw-rw-r--   0 root         (0) root         (0)     1905 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_admin_passthru64.2
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ae_info_css_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      952 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ae_info_error.2
+-rw-rw-r--   0 root         (0) root         (0)     1139 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ae_info_notice.2
+-rw-rw-r--   0 root         (0) root         (0)      583 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ae_info_smart.2
+-rw-rw-r--   0 root         (0) root         (0)      563 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ae_type.2
+-rw-rw-r--   0 root         (0) root         (0)      407 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_aggregate_endurance_group_event.2
+-rw-rw-r--   0 root         (0) root         (0)      415 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_aggregate_predictable_lat_event.2
+-rw-rw-r--   0 root         (0) root         (0)      575 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ana_group_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      471 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ana_log.2
+-rw-rw-r--   0 root         (0) root         (0)      731 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ana_state.2
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_apst_entry.2
+-rw-rw-r--   0 root         (0) root         (0)      644 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_aqa.2
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_asq.2
+-rw-rw-r--   0 root         (0) root         (0)      571 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_boot_partition.2
+-rw-rw-r--   0 root         (0) root         (0)     1030 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_boot_partition_info.2
+-rw-rw-r--   0 root         (0) root         (0)     1378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_bpinfo.2
+-rw-rw-r--   0 root         (0) root         (0)      339 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_bpmbl.2
+-rw-rw-r--   0 root         (0) root         (0)      923 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_bprsel.2
+-rw-rw-r--   0 root         (0) root         (0)     4694 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cap.2
+-rw-rw-r--   0 root         (0) root         (0)      699 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_capacity_config_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      452 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_capacity_mgmt.2
+-rw-rw-r--   0 root         (0) root         (0)     2986 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cc.2
+-rw-rw-r--   0 root         (0) root         (0)     1066 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_change_ns_event.2
+-rw-rw-r--   0 root         (0) root         (0)      537 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_channel_config_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      343 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmb_size.2
+-rw-rw-r--   0 root         (0) root         (0)     1332 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbebs.2
+-rw-rw-r--   0 root         (0) root         (0)     2288 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbloc.2
+-rw-rw-r--   0 root         (0) root         (0)      830 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbmsc.2
+-rw-rw-r--   0 root         (0) root         (0)      448 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbsts.2
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbswtp.2
+-rw-rw-r--   0 root         (0) root         (0)     2234 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmbsz.2
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      414 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_effects_log.2
+-rw-rw-r--   0 root         (0) root         (0)      508 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_format_mset.2
+-rw-rw-r--   0 root         (0) root         (0)      654 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_format_pi.2
+-rw-rw-r--   0 root         (0) root         (0)      491 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_format_pil.2
+-rw-rw-r--   0 root         (0) root         (0)      953 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_format_ses.2
+-rw-rw-r--   0 root         (0) root         (0)     3631 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_get_log_lid.2
+-rw-rw-r--   0 root         (0) root         (0)      492 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmd_get_log_telemetry_host_lsp.2
+-rw-rw-r--   0 root         (0) root         (0)     1444 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_cmic.2
+-rw-rw-r--   0 root         (0) root         (0)      414 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_compare.2
+-rw-rw-r--   0 root         (0) root         (0)     2263 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_connect_err.2
+-rw-rw-r--   0 root         (0) root         (0)     4035 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_constants.2
+-rw-rw-r--   0 root         (0) root         (0)      383 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy.2
+-rw-rw-r--   0 root         (0) root         (0)      744 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy_range.2
+-rw-rw-r--   0 root         (0) root         (0)      754 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy_range_f1.2
+-rw-rw-r--   0 root         (0) root         (0)      883 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy_range_f2.2
+-rw-rw-r--   0 root         (0) root         (0)      936 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy_range_f3.2
+-rw-rw-r--   0 root         (0) root         (0)      302 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_copy_range_sopt.2
+-rw-rw-r--   0 root         (0) root         (0)      815 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_create_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      383 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_create_root.2
+-rw-rw-r--   0 root         (0) root         (0)      719 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_crto.2
+-rw-rw-r--   0 root         (0) root         (0)      401 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_csi.2
+-rw-rw-r--   0 root         (0) root         (0)     1874 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_csts.2
+-rw-rw-r--   0 root         (0) root         (0)     1005 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_config_match.2
+-rw-rw-r--   0 root         (0) root         (0)     1174 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_find.2
+-rw-rw-r--   0 root         (0) root         (0)      327 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_first_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      334 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_first_path.2
+-rw-rw-r--   0 root         (0) root         (0)      294 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_for_each_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_for_each_ns_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      299 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_for_each_path.2
+-rw-rw-r--   0 root         (0) root         (0)      399 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_for_each_path_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      382 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_address.2
+-rw-rw-r--   0 root         (0) root         (0)      348 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_config.2
+-rw-rw-r--   0 root         (0) root         (0)      359 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_dhchap_host_key.2
+-rw-rw-r--   0 root         (0) root         (0)      369 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_dhchap_key.2
+-rw-rw-r--   0 root         (0) root         (0)      662 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_fd.2
+-rw-rw-r--   0 root         (0) root         (0)      328 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_firmware.2
+-rw-rw-r--   0 root         (0) root         (0)      357 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_host_iface.2
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_host_traddr.2
+-rw-rw-r--   0 root         (0) root         (0)      303 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_model.2
+-rw-rw-r--   0 root         (0) root         (0)      302 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_name.2
+-rw-rw-r--   0 root         (0) root         (0)      331 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_numa_node.2
+-rw-rw-r--   0 root         (0) root         (0)      393 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_phy_slot.2
+-rw-rw-r--   0 root         (0) root         (0)      332 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_queue_count.2
+-rw-rw-r--   0 root         (0) root         (0)      323 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_serial.2
+-rw-rw-r--   0 root         (0) root         (0)      316 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_sqsize.2
+-rw-rw-r--   0 root         (0) root         (0)      590 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_src_addr.2
+-rw-rw-r--   0 root         (0) root         (0)      334 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_state.2
+-rw-rw-r--   0 root         (0) root         (0)      328 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_subsysnqn.2
+-rw-rw-r--   0 root         (0) root         (0)      341 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      337 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_sysfs_dir.2
+-rw-rw-r--   0 root         (0) root         (0)      324 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_traddr.2
+-rw-rw-r--   0 root         (0) root         (0)      330 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_transport.2
+-rw-rw-r--   0 root         (0) root         (0)      363 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_get_trsvcid.2
+-rw-rw-r--   0 root         (0) root         (0)      502 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_identify.2
+-rw-rw-r--   0 root         (0) root         (0)      350 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_is_discovered.2
+-rw-rw-r--   0 root         (0) root         (0)      484 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_is_discovery_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      350 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_is_persistent.2
+-rw-rw-r--   0 root         (0) root         (0)      395 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_is_unique_discovery_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)     2391 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_metadata_type.2
+-rw-rw-r--   0 root         (0) root         (0)      378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_next_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      422 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_next_path.2
+-rw-rw-r--   0 root         (0) root         (0)      285 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_release_fd.2
+-rw-rw-r--   0 root         (0) root         (0)      409 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_reset.2
+-rw-rw-r--   0 root         (0) root         (0)      401 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_dhchap_host_key.2
+-rw-rw-r--   0 root         (0) root         (0)      393 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_dhchap_key.2
+-rw-rw-r--   0 root         (0) root         (0)      435 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_discovered.2
+-rw-rw-r--   0 root         (0) root         (0)      509 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_discovery_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      436 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_persistent.2
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      302 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ctrls_filter.2
+-rw-rw-r--   0 root         (0) root         (0)      587 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_data_tfr.2
+-rw-rw-r--   0 root         (0) root         (0)      451 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_default_host.2
+-rw-rw-r--   0 root         (0) root         (0)      510 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_describe_key_serial.2
+-rw-rw-r--   0 root         (0) root         (0)     1033 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dev_self_test.2
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_dtype.2
+-rw-rw-r--   0 root         (0) root         (0)      700 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_receive_doper.2
+-rw-rw-r--   0 root         (0) root         (0)      462 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_recv.2
+-rw-rw-r--   0 root         (0) root         (0)      622 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_recv_identify_parameters.2
+-rw-rw-r--   0 root         (0) root         (0)      660 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_recv_stream_allocate.2
+-rw-rw-r--   0 root         (0) root         (0)      636 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_recv_stream_parameters.2
+-rw-rw-r--   0 root         (0) root         (0)      680 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_recv_stream_status.2
+-rw-rw-r--   0 root         (0) root         (0)      728 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send.2
+-rw-rw-r--   0 root         (0) root         (0)      594 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send_doper.2
+-rw-rw-r--   0 root         (0) root         (0)      720 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send_id_endir.2
+-rw-rw-r--   0 root         (0) root         (0)      453 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send_identify_endir.2
+-rw-rw-r--   0 root         (0) root         (0)      620 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send_stream_release_identifier.2
+-rw-rw-r--   0 root         (0) root         (0)      557 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_send_stream_release_resource.2
+-rw-rw-r--   0 root         (0) root         (0)      503 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_directive_types.2
+-rw-rw-r--   0 root         (0) root         (0)      372 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_disconnect_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dsm.2
+-rw-rw-r--   0 root         (0) root         (0)      474 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dsm_attributes.2
+-rw-rw-r--   0 root         (0) root         (0)      389 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dsm_range.2
+-rw-rw-r--   0 root         (0) root         (0)      619 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dst_stc.2
+-rw-rw-r--   0 root         (0) root         (0)      381 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dump_config.2
+-rw-rw-r--   0 root         (0) root         (0)      358 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_dump_tree.2
+-rw-rw-r--   0 root         (0) root         (0)      711 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_eg_critical_warning_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      385 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_eg_event_aggregate_log.2
+-rw-rw-r--   0 root         (0) root         (0)      472 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_end_grp_chan_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      870 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_end_grp_config_desc.2
+-rw-rw-r--   0 root         (0) root         (0)     1865 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_endurance_group_log.2
+-rw-rw-r--   0 root         (0) root         (0)     1134 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_eom_lane_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      429 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_eom_optional_data.2
+-rw-rw-r--   0 root         (0) root         (0)     1282 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_eom_optional_data_present.2
+-rw-rw-r--   0 root         (0) root         (0)      384 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_errno_to_string.2
+-rw-rw-r--   0 root         (0) root         (0)     3982 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_error_log_page.2
+-rw-rw-r--   0 root         (0) root         (0)      639 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_export_tls_key.2
+-rw-rw-r--   0 root         (0) root         (0)     1971 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fabrics_config.2
+-rw-rw-r--   0 root         (0) root         (0)      779 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fctype.2
+-rw-rw-r--   0 root         (0) root         (0)     1028 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_config_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      944 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_config_fdpa.2
+-rw-rw-r--   0 root         (0) root         (0)      643 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_config_log.2
+-rw-rw-r--   0 root         (0) root         (0)      876 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_event.2
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_event_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_event_realloc.2
+-rw-rw-r--   0 root         (0) root         (0)      332 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_event_realloc_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      815 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_event_type.2
+-rw-rw-r--   0 root         (0) root         (0)      421 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_events_log.2
+-rw-rw-r--   0 root         (0) root         (0)      648 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_reclaim_unit_handle_status.2
+-rw-rw-r--   0 root         (0) root         (0)      677 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_reclaim_unit_handle_update.2
+-rw-rw-r--   0 root         (0) root         (0)      328 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruh_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      470 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruh_status.2
+-rw-rw-r--   0 root         (0) root         (0)      598 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruh_status_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      419 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruh_type.2
+-rw-rw-r--   0 root         (0) root         (0)      664 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruha.2
+-rw-rw-r--   0 root         (0) root         (0)      370 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruhu_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_ruhu_log.2
+-rw-rw-r--   0 root         (0) root         (0)      476 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_stats_log.2
+-rw-rw-r--   0 root         (0) root         (0)      479 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_supported_event_attributes.2
+-rw-rw-r--   0 root         (0) root         (0)      413 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fdp_supported_event_desc.2
+-rw-rw-r--   0 root         (0) root         (0)     8675 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat.2
+-rw-rw-r--   0 root         (0) root         (0)      305 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_auto_pst.2
+-rw-rw-r--   0 root         (0) root         (0)      420 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_fdp_events_cdw11.2
+-rw-rw-r--   0 root         (0) root         (0)      635 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_host_behavior.2
+-rw-rw-r--   0 root         (0) root         (0)      684 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_nswpcfg_state.2
+-rw-rw-r--   0 root         (0) root         (0)      433 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_plm_window_select.2
+-rw-rw-r--   0 root         (0) root         (0)      608 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_resv_notify_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      496 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_feat_tmpthresh_thsel.2
+-rw-rw-r--   0 root         (0) root         (0)     1853 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_features_async_event_config_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     3955 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_features_id.2
+-rw-rw-r--   0 root         (0) root         (0)     1942 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fid_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      381 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fid_supported_effects_log.2
+-rw-rw-r--   0 root         (0) root         (0)      449 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_firmware_slot.2
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_first_host.2
+-rw-rw-r--   0 root         (0) root         (0)      346 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_first_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      956 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_flbas.2
+-rw-rw-r--   0 root         (0) root         (0)      529 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_flush.2
+-rw-rw-r--   0 root         (0) root         (0)      288 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_for_each_host.2
+-rw-rw-r--   0 root         (0) root         (0)      370 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_for_each_host_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      314 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_for_each_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      401 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_for_each_subsystem_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      732 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_format_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_format_nvm_compln_event.2
+-rw-rw-r--   0 root         (0) root         (0)      494 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_format_nvm_start_event.2
+-rw-rw-r--   0 root         (0) root         (0)      238 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_free_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      239 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_free_host.2
+-rw-rw-r--   0 root         (0) root         (0)      235 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_free_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_free_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      314 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_free_tree.2
+-rw-rw-r--   0 root         (0) root         (0)      643 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fw_commit.2
+-rw-rw-r--   0 root         (0) root         (0)     1620 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fw_commit_ca.2
+-rw-rw-r--   0 root         (0) root         (0)      809 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fw_commit_event.2
+-rw-rw-r--   0 root         (0) root         (0)     1098 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fw_download.2
+-rw-rw-r--   0 root         (0) root         (0)      761 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_fw_download_seq.2
+-rw-rw-r--   0 root         (0) root         (0)      655 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_gen_dhchap_key.2
+-rw-rw-r--   0 root         (0) root         (0)      941 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_generate_tls_key_identity.2
+-rw-rw-r--   0 root         (0) root         (0)      506 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_ana_log_len.2
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      475 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_ctrl_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      932 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_ctrl_telemetry.2
+-rw-rw-r--   0 root         (0) root         (0)      727 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_directive_receive_length.2
+-rw-rw-r--   0 root         (0) root         (0)      740 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_discovery_args.2
+-rw-rw-r--   0 root         (0) root         (0)      665 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_feature_length.2
+-rw-rw-r--   0 root         (0) root         (0)      868 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_feature_length2.2
+-rw-rw-r--   0 root         (0) root         (0)      447 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features.2
+-rw-rw-r--   0 root         (0) root         (0)      658 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_arbitration.2
+-rw-rw-r--   0 root         (0) root         (0)      665 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_async_event.2
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_auto_pst.2
+-rw-rw-r--   0 root         (0) root         (0)      821 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_data.2
+-rw-rw-r--   0 root         (0) root         (0)      769 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_endurance_event_cfg.2
+-rw-rw-r--   0 root         (0) root         (0)      782 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_err_recovery.2
+-rw-rw-r--   0 root         (0) root         (0)      719 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_err_recovery2.2
+-rw-rw-r--   0 root         (0) root         (0)      637 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_hctm.2
+-rw-rw-r--   0 root         (0) root         (0)      776 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_host_behavior.2
+-rw-rw-r--   0 root         (0) root         (0)      747 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_host_id.2
+-rw-rw-r--   0 root         (0) root         (0)      815 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_host_mem_buf.2
+-rw-rw-r--   0 root         (0) root         (0)      788 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_host_mem_buf2.2
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_iocs_profile.2
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_irq_coalesce.2
+-rw-rw-r--   0 root         (0) root         (0)      686 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_irq_config.2
+-rw-rw-r--   0 root         (0) root         (0)      637 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_kato.2
+-rw-rw-r--   0 root         (0) root         (0)      865 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_lba_range.2
+-rw-rw-r--   0 root         (0) root         (0)      809 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_lba_range2.2
+-rw-rw-r--   0 root         (0) root         (0)      689 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_lba_sts_interval.2
+-rw-rw-r--   0 root         (0) root         (0)      650 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_nopsc.2
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_num_queues.2
+-rw-rw-r--   0 root         (0) root         (0)      773 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_plm_config.2
+-rw-rw-r--   0 root         (0) root         (0)      712 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_plm_window.2
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_power_mgmt.2
+-rw-rw-r--   0 root         (0) root         (0)      769 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_resv_mask.2
+-rw-rw-r--   0 root         (0) root         (0)      709 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_resv_mask2.2
+-rw-rw-r--   0 root         (0) root         (0)      787 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_resv_persist.2
+-rw-rw-r--   0 root         (0) root         (0)      724 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_resv_persist2.2
+-rw-rw-r--   0 root         (0) root         (0)      634 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_rrl.2
+-rw-rw-r--   0 root         (0) root         (0)      643 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_sanitize.2
+-rw-rw-r--   0 root         (0) root         (0)      612 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_sel.2
+-rw-rw-r--   0 root         (0) root         (0)      655 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_simple.2
+-rw-rw-r--   0 root         (0) root         (0)      664 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_sw_progress.2
+-rw-rw-r--   0 root         (0) root         (0)      668 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_temp_thresh.2
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_timestamp.2
+-rw-rw-r--   0 root         (0) root         (0)      667 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_volatile_wc.2
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_write_atomic.2
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_features_write_protect.2
+-rw-rw-r--   0 root         (0) root         (0)      865 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_host_telemetry.2
+-rw-rw-r--   0 root         (0) root         (0)      643 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_lba_status.2
+-rw-rw-r--   0 root         (0) root         (0)      608 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_lba_status_log.2
+-rw-rw-r--   0 root         (0) root         (0)      415 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log.2
+-rw-rw-r--   0 root         (0) root         (0)     1103 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_ana.2
+-rw-rw-r--   0 root         (0) root         (0)      776 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_ana_groups.2
+-rw-rw-r--   0 root         (0) root         (0)      736 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_boot_partition.2
+-rw-rw-r--   0 root         (0) root         (0)      764 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_changed_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)      756 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_cmd_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      550 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_create_telemetry_host.2
+-rw-rw-r--   0 root         (0) root         (0)      719 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_device_self_test.2
+-rw-rw-r--   0 root         (0) root         (0)      797 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_discovery.2
+-rw-rw-r--   0 root         (0) root         (0)     1005 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_endurance_group.2
+-rw-rw-r--   0 root         (0) root         (0)      733 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_endurance_grp_evt.2
+-rw-rw-r--   0 root         (0) root         (0)      828 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_error.2
+-rw-rw-r--   0 root         (0) root         (0)      619 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_fdp_configurations.2
+-rw-rw-r--   0 root         (0) root         (0)      665 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_fdp_events.2
+-rw-rw-r--   0 root         (0) root         (0)      571 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_fdp_stats.2
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_fid_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      782 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_fw_slot.2
+-rw-rw-r--   0 root         (0) root         (0)      687 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_lba_status.2
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_media_unit_stat.2
+-rw-rw-r--   0 root         (0) root         (0)      675 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_mi_cmd_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      587 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_page.2
+-rw-rw-r--   0 root         (0) root         (0)      727 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_persistent_event.2
+-rw-rw-r--   0 root         (0) root         (0)      791 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_phy_rx_eom.2
+-rw-rw-r--   0 root         (0) root         (0)      791 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_predictable_lat_event.2
+-rw-rw-r--   0 root         (0) root         (0)      642 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_predictable_lat_nvmset.2
+-rw-rw-r--   0 root         (0) root         (0)      626 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_reclaim_unit_handle_usage.2
+-rw-rw-r--   0 root         (0) root         (0)      591 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_reservation.2
+-rw-rw-r--   0 root         (0) root         (0)      711 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_sanitize.2
+-rw-rw-r--   0 root         (0) root         (0)     1044 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_smart.2
+-rw-rw-r--   0 root         (0) root         (0)      695 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_support_cap_config_list.2
+-rw-rw-r--   0 root         (0) root         (0)      631 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_supported_log_pages.2
+-rw-rw-r--   0 root         (0) root         (0)      877 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_telemetry_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      804 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_telemetry_host.2
+-rw-rw-r--   0 root         (0) root         (0)      762 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_log_zns_changed_zones.2
+-rw-rw-r--   0 root         (0) root         (0)      663 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_logging_level.2
+-rw-rw-r--   0 root         (0) root         (0)      570 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_logical_block_size.2
+-rw-rw-r--   0 root         (0) root         (0)      885 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_new_host_telemetry.2
+-rw-rw-r--   0 root         (0) root         (0)      461 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_ns_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      712 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_nsid.2
+-rw-rw-r--   0 root         (0) root         (0)      468 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_path_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_property.2
+-rw-rw-r--   0 root         (0) root         (0)      491 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_subsys_attr.2
+-rw-rw-r--   0 root         (0) root         (0)     1194 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_telemetry_log.2
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_get_telemetry_max.2
+-rw-rw-r--   0 root         (0) root         (0)      499 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_hmac_alg.2
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_behavior_support.2
+-rw-rw-r--   0 root         (0) root         (0)      356 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_get_dhchap_key.2
+-rw-rw-r--   0 root         (0) root         (0)      312 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_get_hostid.2
+-rw-rw-r--   0 root         (0) root         (0)      318 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_get_hostnqn.2
+-rw-rw-r--   0 root         (0) root         (0)      411 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_get_hostsymname.2
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_get_root.2
+-rw-rw-r--   0 root         (0) root         (0)      531 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_is_pdc_enabled.2
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_mem_buf_attrs.2
+-rw-rw-r--   0 root         (0) root         (0)      612 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_metadata.2
+-rw-rw-r--   0 root         (0) root         (0)      468 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_release_fds.2
+-rw-rw-r--   0 root         (0) root         (0)      381 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_set_dhchap_key.2
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_set_hostsymname.2
+-rw-rw-r--   0 root         (0) root         (0)      612 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_host_set_pdc_enabled.2
+-rw-rw-r--   0 root         (0) root         (0)    14992 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)     1480 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_anacap.2
+-rw-rw-r--   0 root         (0) root         (0)      385 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_apsta.2
+-rw-rw-r--   0 root         (0) root         (0)      432 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_avscc.2
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_cmic.2
+-rw-rw-r--   0 root         (0) root         (0)      492 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_cntrltype.2
+-rw-rw-r--   0 root         (0) root         (0)      579 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_cqes.2
+-rw-rw-r--   0 root         (0) root         (0)     2238 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_ctratt.2
+-rw-rw-r--   0 root         (0) root         (0)      521 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_dctype.2
+-rw-rw-r--   0 root         (0) root         (0)      455 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_dsto.2
+-rw-rw-r--   0 root         (0) root         (0)      457 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_fcatt.2
+-rw-rw-r--   0 root         (0) root         (0)     1345 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_fna.2
+-rw-rw-r--   0 root         (0) root         (0)      878 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_frmw.2
+-rw-rw-r--   0 root         (0) root         (0)      404 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_fuses.2
+-rw-rw-r--   0 root         (0) root         (0)      487 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_hctm.2
+-rw-rw-r--   0 root         (0) root         (0)     1645 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_lpa.2
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_mec.2
+-rw-rw-r--   0 root         (0) root         (0)      704 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      679 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_nvmsr.2
+-rw-rw-r--   0 root         (0) root         (0)      399 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_nvscc.2
+-rw-rw-r--   0 root         (0) root         (0)      954 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_nwpc.2
+-rw-rw-r--   0 root         (0) root         (0)     1998 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_oacs.2
+-rw-rw-r--   0 root         (0) root         (0)     1245 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_oaes.2
+-rw-rw-r--   0 root         (0) root         (0)      403 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_ofcs.2
+-rw-rw-r--   0 root         (0) root         (0)     2071 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_oncs.2
+-rw-rw-r--   0 root         (0) root         (0)      793 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_rpmbs.2
+-rw-rw-r--   0 root         (0) root         (0)     1153 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_sanicap.2
+-rw-rw-r--   0 root         (0) root         (0)      894 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_sgls.2
+-rw-rw-r--   0 root         (0) root         (0)      579 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_sqes.2
+-rw-rw-r--   0 root         (0) root         (0)      604 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_vwc.2
+-rw-rw-r--   0 root         (0) root         (0)     1073 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ctrl_vwci.2
+-rw-rw-r--   0 root         (0) root         (0)      459 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_directives.2
+-rw-rw-r--   0 root         (0) root         (0)      650 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_domain_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_domain_list.2
+-rw-rw-r--   0 root         (0) root         (0)      409 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_endurance_group_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1016 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_independent_id_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      310 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_iocs.2
+-rw-rw-r--   0 root         (0) root         (0)     7083 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      386 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_attr.2
+-rw-rw-r--   0 root         (0) root         (0)     1228 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_dlfeat.2
+-rw-rw-r--   0 root         (0) root         (0)     1054 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_dpc.2
+-rw-rw-r--   0 root         (0) root         (0)      974 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_dps.2
+-rw-rw-r--   0 root         (0) root         (0)     1071 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_flbas.2
+-rw-rw-r--   0 root         (0) root         (0)      399 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_granularity_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_granularity_list.2
+-rw-rw-r--   0 root         (0) root         (0)      589 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_mc.2
+-rw-rw-r--   0 root         (0) root         (0)      412 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_nmic.2
+-rw-rw-r--   0 root         (0) root         (0)     1559 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_ns_rescap.2
+-rw-rw-r--   0 root         (0) root         (0)     1409 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_nsfeat.2
+-rw-rw-r--   0 root         (0) root         (0)      397 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_nvmset_list.2
+-rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_psd.2
+-rw-rw-r--   0 root         (0) root         (0)      559 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_uuid.2
+-rw-rw-r--   0 root         (0) root         (0)      350 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_uuid_list.2
+-rw-rw-r--   0 root         (0) root         (0)      416 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_id_uuid_list_entry.2
+-rw-rw-r--   0 root         (0) root         (0)      574 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify.2
+-rw-rw-r--   0 root         (0) root         (0)      915 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_active_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1112 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_active_ns_list_csi.2
+-rw-rw-r--   0 root         (0) root         (0)      616 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_allocated_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      929 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_allocated_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1113 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_allocated_ns_list_csi.2
+-rw-rw-r--   0 root         (0) root         (0)     3616 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_cns.2
+-rw-rw-r--   0 root         (0) root         (0)      645 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      826 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ctrl_csi.2
+-rw-rw-r--   0 root         (0) root         (0)      865 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      841 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_domain_list.2
+-rw-rw-r--   0 root         (0) root         (0)      636 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_endurance_group_list.2
+-rw-rw-r--   0 root         (0) root         (0)      854 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_independent_identify_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      675 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_iocs.2
+-rw-rw-r--   0 root         (0) root         (0)     1047 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2
+-rw-rw-r--   0 root         (0) root         (0)     1056 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      867 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ns_csi.2
+-rw-rw-r--   0 root         (0) root         (0)      961 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ns_csi_user_data_format.2
+-rw-rw-r--   0 root         (0) root         (0)      954 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ns_descs.2
+-rw-rw-r--   0 root         (0) root         (0)      862 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_ns_granularity.2
+-rw-rw-r--   0 root         (0) root         (0)      981 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_nsid_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      952 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_nvmset_list.2
+-rw-rw-r--   0 root         (0) root         (0)      765 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_primary_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)     1065 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_secondary_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      762 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_identify_uuid.2
+-rw-rw-r--   0 root         (0) root         (0)      713 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_import_tls_key.2
+-rw-rw-r--   0 root         (0) root         (0)      731 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_copy_range.2
+-rw-rw-r--   0 root         (0) root         (0)      749 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_copy_range_f1.2
+-rw-rw-r--   0 root         (0) root         (0)      874 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_copy_range_f2.2
+-rw-rw-r--   0 root         (0) root         (0)      874 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_copy_range_f3.2
+-rw-rw-r--   0 root         (0) root         (0)      472 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      699 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      815 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_dsm_range.2
+-rw-rw-r--   0 root         (0) root         (0)      541 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_init_logging.2
+-rw-rw-r--   0 root         (0) root         (0)      999 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_insert_tls_key.2
+-rw-rw-r--   0 root         (0) root         (0)     1178 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_insert_tls_key_versioned.2
+-rw-rw-r--   0 root         (0) root         (0)      448 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io.2
+-rw-rw-r--   0 root         (0) root         (0)     1147 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_control_flags.2
+-rw-rw-r--   0 root         (0) root         (0)     1783 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_dsm_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      449 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_mgmt_recv.2
+-rw-rw-r--   0 root         (0) root         (0)      325 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_mgmt_recv_mo.2
+-rw-rw-r--   0 root         (0) root         (0)      446 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_mgmt_send.2
+-rw-rw-r--   0 root         (0) root         (0)      322 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_mgmt_send_mo.2
+-rw-rw-r--   0 root         (0) root         (0)     1669 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_opcode.2
+-rw-rw-r--   0 root         (0) root         (0)     1872 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_passthru.2
+-rw-rw-r--   0 root         (0) root         (0)     1884 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_io_passthru64.2
+-rw-rw-r--   0 root         (0) root         (0)      713 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_is_64bit_reg.2
+-rw-rw-r--   0 root         (0) root         (0)      360 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_range_type.2
+-rw-rw-r--   0 root         (0) root         (0)      695 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_range_type_entry.2
+-rw-rw-r--   0 root         (0) root         (0)      372 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_rd.2
+-rw-rw-r--   0 root         (0) root         (0)      482 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_status.2
+-rw-rw-r--   0 root         (0) root         (0)      497 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_status_atype.2
+-rw-rw-r--   0 root         (0) root         (0)      537 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_status_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      698 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lba_status_log.2
+-rw-rw-r--   0 root         (0) root         (0)      529 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lbaf.2
+-rw-rw-r--   0 root         (0) root         (0)      747 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lbaf_rp.2
+-rw-rw-r--   0 root         (0) root         (0)      745 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lbart.2
+-rw-rw-r--   0 root         (0) root         (0)      603 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lbas_ns_element.2
+-rw-rw-r--   0 root         (0) root         (0)      417 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lockdown.2
+-rw-rw-r--   0 root         (0) root         (0)      391 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_log_ana_lsp.2
+-rw-rw-r--   0 root         (0) root         (0)      594 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_log_phy_rx_eom_action.2
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_log_phy_rx_eom_quality.2
+-rw-rw-r--   0 root         (0) root         (0)     1106 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lookup_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lookup_host.2
+-rw-rw-r--   0 root         (0) root         (0)      502 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lookup_key.2
+-rw-rw-r--   0 root         (0) root         (0)      426 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lookup_keyring.2
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_lookup_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      432 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_media_unit_config_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_media_unit_stat_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      592 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_media_unit_stat_log.2
+-rw-rw-r--   0 root         (0) root         (0)      487 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_metadata_element_desc.2
+-rw-rw-r--   0 root         (0) root         (0)     2120 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_admin_passthru.2
+-rw-rw-r--   0 root         (0) root         (0)      654 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_format_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      573 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_fw_commit.2
+-rw-rw-r--   0 root         (0) root         (0)     1141 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_fw_download.2
+-rw-rw-r--   0 root         (0) root         (0)     1024 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_features_data.2
+-rw-rw-r--   0 root         (0) root         (0)      933 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log.2
+-rw-rw-r--   0 root         (0) root         (0)     1143 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_ana.2
+-rw-rw-r--   0 root         (0) root         (0)      816 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_ana_groups.2
+-rw-rw-r--   0 root         (0) root         (0)      777 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_boot_partition.2
+-rw-rw-r--   0 root         (0) root         (0)      804 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_changed_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)      796 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_cmd_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      590 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2
+-rw-rw-r--   0 root         (0) root         (0)      759 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_device_self_test.2
+-rw-rw-r--   0 root         (0) root         (0)      837 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_discovery.2
+-rw-rw-r--   0 root         (0) root         (0)     1045 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_endurance_group.2
+-rw-rw-r--   0 root         (0) root         (0)      773 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2
+-rw-rw-r--   0 root         (0) root         (0)      868 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_error.2
+-rw-rw-r--   0 root         (0) root         (0)      692 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      822 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_fw_slot.2
+-rw-rw-r--   0 root         (0) root         (0)      727 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_lba_status.2
+-rw-rw-r--   0 root         (0) root         (0)      669 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_media_unit_stat.2
+-rw-rw-r--   0 root         (0) root         (0)      716 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)     1025 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_page.2
+-rw-rw-r--   0 root         (0) root         (0)      767 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_persistent_event.2
+-rw-rw-r--   0 root         (0) root         (0)      831 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_phy_rx_eom.2
+-rw-rw-r--   0 root         (0) root         (0)      831 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2
+-rw-rw-r--   0 root         (0) root         (0)      682 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2
+-rw-rw-r--   0 root         (0) root         (0)      632 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_reservation.2
+-rw-rw-r--   0 root         (0) root         (0)      751 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_sanitize.2
+-rw-rw-r--   0 root         (0) root         (0)      831 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_simple.2
+-rw-rw-r--   0 root         (0) root         (0)     1084 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_smart.2
+-rw-rw-r--   0 root         (0) root         (0)      736 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2
+-rw-rw-r--   0 root         (0) root         (0)      671 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_supported_log_pages.2
+-rw-rw-r--   0 root         (0) root         (0)      917 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      844 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_telemetry_host.2
+-rw-rw-r--   0 root         (0) root         (0)      802 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2
+-rw-rw-r--   0 root         (0) root         (0)     1047 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_get_nsid_log.2
+-rw-rw-r--   0 root         (0) root         (0)      877 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify.2
+-rw-rw-r--   0 root         (0) root         (0)     1064 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_active_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)      754 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_allocated_ns.2
+-rw-rw-r--   0 root         (0) root         (0)     1082 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_allocated_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1130 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_cns_nsid.2
+-rw-rw-r--   0 root         (0) root         (0)      884 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      979 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      754 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      851 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_ns_descs.2
+-rw-rw-r--   0 root         (0) root         (0)     1099 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1548 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_partial.2
+-rw-rw-r--   0 root         (0) root         (0)      989 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_primary_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)     1041 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      539 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_ns_attach.2
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_ns_attach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      630 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_ns_detach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)     1687 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_req_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)      771 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_resp_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)     1114 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_sanitize_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      991 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_security_recv.2
+-rw-rw-r--   0 root         (0) root         (0)      976 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_security_send.2
+-rw-rw-r--   0 root         (0) root         (0)     1701 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_admin_xfer.2
+-rw-rw-r--   0 root         (0) root         (0)     1254 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_ccs.2
+-rw-rw-r--   0 root         (0) root         (0)      302 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_close.2
+-rw-rw-r--   0 root         (0) root         (0)      258 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_close_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)     1903 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_cmd_supported_effects.2
+-rw-rw-r--   0 root         (0) root         (0)      502 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_cmd_supported_effects_log.2
+-rw-rw-r--   0 root         (0) root         (0)      794 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_config_id.2
+-rw-rw-r--   0 root         (0) root         (0)      673 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_config_smbus_freq.2
+-rw-rw-r--   0 root         (0) root         (0)      632 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_create_root.2
+-rw-rw-r--   0 root         (0) root         (0)      817 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_csts.2
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_ctrl_health_status.2
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_ctrl_id.2
+-rw-rw-r--   0 root         (0) root         (0)      652 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_cwarn.2
+-rw-rw-r--   0 root         (0) root         (0)      962 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_dtyp.2
+-rw-rw-r--   0 root         (0) root         (0)      862 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_elem.2
+-rw-rw-r--   0 root         (0) root         (0)      245 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_free_root.2
+-rw-rw-r--   0 root         (0) root         (0)      631 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_init_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      672 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_message_type.2
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_opcode.2
+-rw-rw-r--   0 root         (0) root         (0)      813 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      830 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      865 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_port.2
+-rw-rw-r--   0 root         (0) root         (0)      739 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_subsys.2
+-rw-rw-r--   0 root         (0) root         (0)      704 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_req_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)      600 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_resp_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)     1010 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_mi_subsystem_health_status_poll.2
+-rw-rw-r--   0 root         (0) root         (0)      705 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_msg_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)      654 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_msg_resp.2
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_nvm_ss_health_status.2
+-rw-rw-r--   0 root         (0) root         (0)      696 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_open_mctp.2
+-rw-rw-r--   0 root         (0) root         (0)      302 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_osc.2
+-rw-rw-r--   0 root         (0) root         (0)      632 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_port_pcie.2
+-rw-rw-r--   0 root         (0) root         (0)      676 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_port_smb.2
+-rw-rw-r--   0 root         (0) root         (0)      761 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_read_ctrl_info.2
+-rw-rw-r--   0 root         (0) root         (0)      483 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_read_nvm_ss_info.2
+-rw-rw-r--   0 root         (0) root         (0)      726 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_read_port_info.2
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_read_sc_list.2
+-rw-rw-r--   0 root         (0) root         (0)     2409 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_resp_status.2
+-rw-rw-r--   0 root         (0) root         (0)      597 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_set_probe_enabled.2
+-rw-rw-r--   0 root         (0) root         (0)      651 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_status_to_string.2
+-rw-rw-r--   0 root         (0) root         (0)      838 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_hdr.2
+-rw-rw-r--   0 root         (0) root         (0)      832 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_mr_common.2
+-rw-rw-r--   0 root         (0) root         (0)     1380 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_mra.2
+-rw-rw-r--   0 root         (0) root         (0)      746 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_ppmra.2
+-rw-rw-r--   0 root         (0) root         (0)      546 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_telem.2
+-rw-rw-r--   0 root         (0) root         (0)      446 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_mi_vpd_tra.2
+-rw-rw-r--   0 root         (0) root         (0)      673 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_attach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      675 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_detach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_filter.2
+-rw-rw-r--   0 root         (0) root         (0)      354 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_first_path.2
+-rw-rw-r--   0 root         (0) root         (0)      318 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_for_each_path.2
+-rw-rw-r--   0 root         (0) root         (0)      418 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_for_each_path_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      443 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_namespace_next_path.2
+-rw-rw-r--   0 root         (0) root         (0)      275 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nbft_free.2
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nbft_read.2
+-rw-rw-r--   0 root         (0) root         (0)      561 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nd_ns_fpi.2
+-rw-rw-r--   0 root         (0) root         (0)      378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_next_host.2
+-rw-rw-r--   0 root         (0) root         (0)      423 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_next_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      444 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_attach.2
+-rw-rw-r--   0 root         (0) root         (0)      578 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_attach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      430 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_attach_sel.2
+-rw-rw-r--   0 root         (0) root         (0)      485 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_compare.2
+-rw-rw-r--   0 root         (0) root         (0)      580 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_detach_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      274 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_flush.2
+-rw-rw-r--   0 root         (0) root         (0)      323 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_csi.2
+-rw-rw-r--   0 root         (0) root         (0)      387 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      303 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_eui64.2
+-rw-rw-r--   0 root         (0) root         (0)      641 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_fd.2
+-rw-rw-r--   0 root         (0) root         (0)      316 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_firmware.2
+-rw-rw-r--   0 root         (0) root         (0)      351 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_generic_name.2
+-rw-rw-r--   0 root         (0) root         (0)      304 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_lba_count.2
+-rw-rw-r--   0 root         (0) root         (0)      293 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_lba_size.2
+-rw-rw-r--   0 root         (0) root         (0)      312 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_lba_util.2
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_meta_size.2
+-rw-rw-r--   0 root         (0) root         (0)      291 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_model.2
+-rw-rw-r--   0 root         (0) root         (0)      290 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_name.2
+-rw-rw-r--   0 root         (0) root         (0)      309 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_nguid.2
+-rw-rw-r--   0 root         (0) root         (0)      269 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_nsid.2
+-rw-rw-r--   0 root         (0) root         (0)      311 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_serial.2
+-rw-rw-r--   0 root         (0) root         (0)      334 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_subsystem.2
+-rw-rw-r--   0 root         (0) root         (0)      325 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_sysfs_dir.2
+-rw-rw-r--   0 root         (0) root         (0)      380 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_get_uuid.2
+-rw-rw-r--   0 root         (0) root         (0)      712 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_id_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      815 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_id_desc_nidt.2
+-rw-rw-r--   0 root         (0) root         (0)      462 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_identify.2
+-rw-rw-r--   0 root         (0) root         (0)      509 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_identify_descs.2
+-rw-rw-r--   0 root         (0) root         (0)      259 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_list.2
+-rw-rw-r--   0 root         (0) root         (0)      774 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_metadata_type.2
+-rw-rw-r--   0 root         (0) root         (0)      425 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt.2
+-rw-rw-r--   0 root         (0) root         (0)     1141 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt_create.2
+-rw-rw-r--   0 root         (0) root         (0)      650 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt_delete.2
+-rw-rw-r--   0 root         (0) root         (0)      834 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt_delete_timeout.2
+-rw-rw-r--   0 root         (0) root         (0)     2925 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt_host_sw_specified.2
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_mgmt_sel.2
+-rw-rw-r--   0 root         (0) root         (0)      494 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_read.2
+-rw-rw-r--   0 root         (0) root         (0)      266 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_release_fd.2
+-rw-rw-r--   0 root         (0) root         (0)      407 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_rescan.2
+-rw-rw-r--   0 root         (0) root         (0)      415 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_verify.2
+-rw-rw-r--   0 root         (0) root         (0)      483 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_write.2
+-rw-rw-r--   0 root         (0) root         (0)      650 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_write_protect_cfg.2
+-rw-rw-r--   0 root         (0) root         (0)      476 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_write_uncorrectable.2
+-rw-rw-r--   0 root         (0) root         (0)      433 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_ns_write_zeros.2
+-rw-rw-r--   0 root         (0) root         (0)      495 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nss_hw_err_event.2
+-rw-rw-r--   0 root         (0) root         (0)      590 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvm_id_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvm_id_ns_elbaf.2
+-rw-rw-r--   0 root         (0) root         (0)      613 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvm_identify_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      589 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvmeset_pl_status.2
+-rw-rw-r--   0 root         (0) root         (0)      942 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvmset_attr.2
+-rw-rw-r--   0 root         (0) root         (0)      952 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvmset_pl_events.2
+-rw-rw-r--   0 root         (0) root         (0)     1211 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_nvmset_predictable_lat_log.2
+-rw-rw-r--   0 root         (0) root         (0)      477 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_open.2
+-rw-rw-r--   0 root         (0) root         (0)     1793 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_passthru_cmd.2
+-rw-rw-r--   0 root         (0) root         (0)     1908 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_passthru_cmd64.2
+-rw-rw-r--   0 root         (0) root         (0)      366 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_path_get_ana_state.2
+-rw-rw-r--   0 root         (0) root         (0)      329 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_path_get_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_path_get_name.2
+-rw-rw-r--   0 root         (0) root         (0)      317 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_path_get_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      346 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_path_get_sysfs_dir.2
+-rw-rw-r--   0 root         (0) root         (0)      296 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_paths_filter.2
+-rw-rw-r--   0 root         (0) root         (0)      945 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pel_ehai.2
+-rw-rw-r--   0 root         (0) root         (0)      717 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pel_ehai_pit.2
+-rw-rw-r--   0 root         (0) root         (0)     1706 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pel_rci.2
+-rw-rw-r--   0 root         (0) root         (0)      573 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pel_rci_rcpit.2
+-rw-rw-r--   0 root         (0) root         (0)      837 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_persistent_event_entry.2
+-rw-rw-r--   0 root         (0) root         (0)     1350 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_persistent_event_log.2
+-rw-rw-r--   0 root         (0) root         (0)     1671 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_persistent_event_types.2
+-rw-rw-r--   0 root         (0) root         (0)      520 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pevent_log_action.2
+-rw-rw-r--   0 root         (0) root         (0)     1643 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_phy_rx_eom_log.2
+-rw-rw-r--   0 root         (0) root         (0)      499 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_phy_rx_eom_progress.2
+-rw-rw-r--   0 root         (0) root         (0)      622 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_plm_config.2
+-rw-rw-r--   0 root         (0) root         (0)      371 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmr_size.2
+-rw-rw-r--   0 root         (0) root         (0)      399 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmr_throughput.2
+-rw-rw-r--   0 root         (0) root         (0)     2459 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrcap.2
+-rw-rw-r--   0 root         (0) root         (0)      391 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrctl.2
+-rw-rw-r--   0 root         (0) root         (0)     1282 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrebs.2
+-rw-rw-r--   0 root         (0) root         (0)      582 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrmsc.2
+-rw-rw-r--   0 root         (0) root         (0)     1074 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrsts.2
+-rw-rw-r--   0 root         (0) root         (0)     1138 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_pmrswtp.2
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_power_on_reset_info_list.2
+-rw-rw-r--   0 root         (0) root         (0)     1548 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_primary_ctrl_cap.2
+-rw-rw-r--   0 root         (0) root         (0)      809 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_psd_flags.2
+-rw-rw-r--   0 root         (0) root         (0)      310 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_psd_power_scale.2
+-rw-rw-r--   0 root         (0) root         (0)      564 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_psd_ps.2
+-rw-rw-r--   0 root         (0) root         (0)     1177 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_psd_workload.2
+-rw-rw-r--   0 root         (0) root         (0)      399 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_read.2
+-rw-rw-r--   0 root         (0) root         (0)      499 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_read_config.2
+-rw-rw-r--   0 root         (0) root         (0)      715 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_read_key.2
+-rw-rw-r--   0 root         (0) root         (0)      364 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_refresh_topology.2
+-rw-rw-r--   0 root         (0) root         (0)     2851 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_register_offsets.2
+-rw-rw-r--   0 root         (0) root         (0)      516 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_registered_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      595 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_registered_ctrl_ext.2
+-rw-rw-r--   0 root         (0) root         (0)      254 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_rescan_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      623 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_acquire.2
+-rw-rw-r--   0 root         (0) root         (0)      637 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_cptpl.2
+-rw-rw-r--   0 root         (0) root         (0)      602 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_notification_log.2
+-rw-rw-r--   0 root         (0) root         (0)      769 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_notify_rnlpt.2
+-rw-rw-r--   0 root         (0) root         (0)      528 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_racqa.2
+-rw-rw-r--   0 root         (0) root         (0)      564 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_register.2
+-rw-rw-r--   0 root         (0) root         (0)      451 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_release.2
+-rw-rw-r--   0 root         (0) root         (0)      684 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_report.2
+-rw-rw-r--   0 root         (0) root         (0)      584 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_rrega.2
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_rrela.2
+-rw-rw-r--   0 root         (0) root         (0)      928 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_rtype.2
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_resv_status.2
+-rw-rw-r--   0 root         (0) root         (0)      507 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_compln_event.2
+-rw-rw-r--   0 root         (0) root         (0)     4687 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_log_page.2
+-rw-rw-r--   0 root         (0) root         (0)     1020 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_nvm.2
+-rw-rw-r--   0 root         (0) root         (0)      739 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_sanact.2
+-rw-rw-r--   0 root         (0) root         (0)     2812 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_sstat.2
+-rw-rw-r--   0 root         (0) root         (0)      423 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_sanitize_start_event.2
+-rw-rw-r--   0 root         (0) root         (0)      291 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan.2
+-rw-rw-r--   0 root         (0) root         (0)      428 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      443 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_ctrl_namespace_paths.2
+-rw-rw-r--   0 root         (0) root         (0)      409 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_ctrl_namespaces.2
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_ctrls.2
+-rw-rw-r--   0 root         (0) root         (0)      350 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_namespace.2
+-rw-rw-r--   0 root         (0) root         (0)      432 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_subsystem_namespaces.2
+-rw-rw-r--   0 root         (0) root         (0)      329 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_subsystems.2
+-rw-rw-r--   0 root         (0) root         (0)      816 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_tls_keys.2
+-rw-rw-r--   0 root         (0) root         (0)      544 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_scan_topology.2
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_secondary_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      462 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_secondary_ctrl_list.2
+-rw-rw-r--   0 root         (0) root         (0)      462 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_security_receive.2
+-rw-rw-r--   0 root         (0) root         (0)      891 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_security_send.2
+-rw-rw-r--   0 root         (0) root         (0)     1530 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_self_test_log.2
+-rw-rw-r--   0 root         (0) root         (0)     1424 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_feat_event_layout.2
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_feature_event.2
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features.2
+-rw-rw-r--   0 root         (0) root         (0)      807 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_arbitration.2
+-rw-rw-r--   0 root         (0) root         (0)      655 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_async_event.2
+-rw-rw-r--   0 root         (0) root         (0)      760 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_auto_pst.2
+-rw-rw-r--   0 root         (0) root         (0)      938 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_data.2
+-rw-rw-r--   0 root         (0) root         (0)      804 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_endurance_evt_cfg.2
+-rw-rw-r--   0 root         (0) root         (0)      808 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_err_recovery.2
+-rw-rw-r--   0 root         (0) root         (0)      709 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_hctm.2
+-rw-rw-r--   0 root         (0) root         (0)      620 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_host_behavior.2
+-rw-rw-r--   0 root         (0) root         (0)      633 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_host_id.2
+-rw-rw-r--   0 root         (0) root         (0)      591 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_iocs_profile.2
+-rw-rw-r--   0 root         (0) root         (0)      704 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_irq_coalesce.2
+-rw-rw-r--   0 root         (0) root         (0)      686 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_irq_config.2
+-rw-rw-r--   0 root         (0) root         (0)      795 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_lba_range.2
+-rw-rw-r--   0 root         (0) root         (0)      775 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_lba_sts_interval.2
+-rw-rw-r--   0 root         (0) root         (0)      673 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_nopsc.2
+-rw-rw-r--   0 root         (0) root         (0)      817 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_plm_config.2
+-rw-rw-r--   0 root         (0) root         (0)      728 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_plm_window.2
+-rw-rw-r--   0 root         (0) root         (0)      681 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_power_mgmt.2
+-rw-rw-r--   0 root         (0) root         (0)      787 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_resv_mask.2
+-rw-rw-r--   0 root         (0) root         (0)      727 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_resv_mask2.2
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_resv_persist.2
+-rw-rw-r--   0 root         (0) root         (0)      726 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_resv_persist2.2
+-rw-rw-r--   0 root         (0) root         (0)      684 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_rrl.2
+-rw-rw-r--   0 root         (0) root         (0)      641 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_sanitize.2
+-rw-rw-r--   0 root         (0) root         (0)      772 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_simple.2
+-rw-rw-r--   0 root         (0) root         (0)      674 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_sw_progress.2
+-rw-rw-r--   0 root         (0) root         (0)      816 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_temp_thresh.2
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_timestamp.2
+-rw-rw-r--   0 root         (0) root         (0)      652 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_volatile_wc.2
+-rw-rw-r--   0 root         (0) root         (0)      642 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_write_atomic.2
+-rw-rw-r--   0 root         (0) root         (0)      803 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_write_protect.2
+-rw-rw-r--   0 root         (0) root         (0)      739 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_features_write_protect2.2
+-rw-rw-r--   0 root         (0) root         (0)      443 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_keyring.2
+-rw-rw-r--   0 root         (0) root         (0)      592 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_property.2
+-rw-rw-r--   0 root         (0) root         (0)      673 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_set_root.2
+-rw-rw-r--   0 root         (0) root         (0)     1470 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_smart_crit.2
+-rw-rw-r--   0 root         (0) root         (0)      869 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_smart_egcw.2
+-rw-rw-r--   0 root         (0) root         (0)     9362 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_smart_log.2
+-rw-rw-r--   0 root         (0) root         (0)      791 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_st_code.2
+-rw-rw-r--   0 root         (0) root         (0)     1107 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_st_curr_op.2
+-rw-rw-r--   0 root         (0) root         (0)     2749 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_st_result.2
+-rw-rw-r--   0 root         (0) root         (0)      855 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_st_valid_diag_info.2
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_code.2
+-rw-rw-r--   0 root         (0) root         (0)      385 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_code_type.2
+-rw-rw-r--   0 root         (0) root         (0)      516 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_equals.2
+-rw-rw-r--   0 root         (0) root         (0)    28147 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_field.2
+-rw-rw-r--   0 root         (0) root         (0)      364 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_get_type.2
+-rw-rw-r--   0 root         (0) root         (0)      427 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_get_value.2
+-rw-rw-r--   0 root         (0) root         (0)     2071 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_result.2
+-rw-rw-r--   0 root         (0) root         (0)      537 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_to_errno.2
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_to_string.2
+-rw-rw-r--   0 root         (0) root         (0)     1069 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_status_type.2
+-rw-rw-r--   0 root         (0) root         (0)      891 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_streams_directive_params.2
+-rw-rw-r--   0 root         (0) root         (0)      378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_streams_directive_status.2
+-rw-rw-r--   0 root         (0) root         (0)      688 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_submit_admin_passthru.2
+-rw-rw-r--   0 root         (0) root         (0)      708 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_submit_admin_passthru64.2
+-rw-rw-r--   0 root         (0) root         (0)      664 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_submit_io_passthru.2
+-rw-rw-r--   0 root         (0) root         (0)      684 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_submit_io_passthru64.2
+-rw-rw-r--   0 root         (0) root         (0)      305 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsys_filter.2
+-rw-rw-r--   0 root         (0) root         (0)     1294 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsys_type.2
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_first_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      362 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_first_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      330 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_for_each_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      430 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_for_each_ctrl_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      324 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_for_each_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      422 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_for_each_ns_safe.2
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_application.2
+-rw-rw-r--   0 root         (0) root         (0)      332 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_host.2
+-rw-rw-r--   0 root         (0) root         (0)      367 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_iopolicy.2
+-rw-rw-r--   0 root         (0) root         (0)      345 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_name.2
+-rw-rw-r--   0 root         (0) root         (0)      323 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_nqn.2
+-rw-rw-r--   0 root         (0) root         (0)      380 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_sysfs_dir.2
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_get_type.2
+-rw-rw-r--   0 root         (0) root         (0)      459 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_lookup_namespace.2
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_next_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      425 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_next_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      495 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_release_fds.2
+-rw-rw-r--   0 root         (0) root         (0)      441 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_reset.2
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_subsystem_set_application.2
+-rw-rw-r--   0 root         (0) root         (0)      573 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_supported_cap_config_list_log.2
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_supported_log_pages.2
+-rw-rw-r--   0 root         (0) root         (0)      507 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_telemetry_da.2
+-rw-rw-r--   0 root         (0) root         (0)     2625 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_telemetry_log.2
+-rw-rw-r--   0 root         (0) root         (0)      361 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_thermal_exc_event.2
+-rw-rw-r--   0 root         (0) root         (0)      420 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_time_stamp_change_event.2
+-rw-rw-r--   0 root         (0) root         (0)      412 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_timestamp.2
+-rw-rw-r--   0 root         (0) root         (0)      500 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_unit.2
+-rw-rw-r--   0 root         (0) root         (0)      248 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_unlink_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      382 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_update_config.2
+-rw-rw-r--   0 root         (0) root         (0)      860 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_update_key.2
+-rw-rw-r--   0 root         (0) root         (0)     1767 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_uring_cmd.2
+-rw-rw-r--   0 root         (0) root         (0)      603 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_verify.2
+-rw-rw-r--   0 root         (0) root         (0)      371 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_version.2
+-rw-rw-r--   0 root         (0) root         (0)      729 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_virt_mgmt_act.2
+-rw-rw-r--   0 root         (0) root         (0)      403 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_virt_mgmt_rt.2
+-rw-rw-r--   0 root         (0) root         (0)      837 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_virtual_mgmt.2
+-rw-rw-r--   0 root         (0) root         (0)      758 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_vs.2
+-rw-rw-r--   0 root         (0) root         (0)      404 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_write.2
+-rw-rw-r--   0 root         (0) root         (0)      786 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_write_uncorrectable.2
+-rw-rw-r--   0 root         (0) root         (0)      703 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_write_zeros.2
+-rw-rw-r--   0 root         (0) root         (0)      428 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_append.2
+-rw-rw-r--   0 root         (0) root         (0)      436 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_changed_zone_log.2
+-rw-rw-r--   0 root         (0) root         (0)      697 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_desc.2
+-rw-rw-r--   0 root         (0) root         (0)      391 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_id_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)     1497 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_id_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      516 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_identify_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      568 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_identify_ns.2
+-rw-rw-r--   0 root         (0) root         (0)      381 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_lbafe.2
+-rw-rw-r--   0 root         (0) root         (0)      455 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_mgmt_recv.2
+-rw-rw-r--   0 root         (0) root         (0)      452 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_mgmt_send.2
+-rw-rw-r--   0 root         (0) root         (0)      445 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_recv_action.2
+-rw-rw-r--   0 root         (0) root         (0)     1252 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_report_options.2
+-rw-rw-r--   0 root         (0) root         (0)     1005 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_report_zones.2
+-rw-rw-r--   0 root         (0) root         (0)      801 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_send_action.2
+-rw-rw-r--   0 root         (0) root         (0)      591 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_za.2
+-rw-rw-r--   0 root         (0) root         (0)      781 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_zs.2
+-rw-rw-r--   0 root         (0) root         (0)      292 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zns_zt.2
+-rw-rw-r--   0 root         (0) root         (0)      441 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvme_zone_report.2
+-rw-rw-r--   0 root         (0) root         (0)      716 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_add_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      839 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_addr_family.2
+-rw-rw-r--   0 root         (0) root         (0)      362 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_adrfam_str.2
+-rw-rw-r--   0 root         (0) root         (0)      392 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_cms_str.2
+-rw-rw-r--   0 root         (0) root         (0)      664 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_connect_data.2
+-rw-rw-r--   0 root         (0) root         (0)      698 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_connect_disc_entry.2
+-rw-rw-r--   0 root         (0) root         (0)      359 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_default_config.2
+-rw-rw-r--   0 root         (0) root         (0)     1152 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_dim_data.2
+-rw-rw-r--   0 root         (0) root         (0)      420 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_dim_entfmt.2
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_dim_etype.2
+-rw-rw-r--   0 root         (0) root         (0)      427 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_dim_tas.2
+-rw-rw-r--   0 root         (0) root         (0)     1328 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_disc_eflags.2
+-rw-rw-r--   0 root         (0) root         (0)     3356 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_disc_log_entry.2
+-rw-rw-r--   0 root         (0) root         (0)     1153 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_discovery_log.2
+-rw-rw-r--   0 root         (0) root         (0)      355 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_eflags_str.2
+-rw-rw-r--   0 root         (0) root         (0)      440 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_exat_len.2
+-rw-rw-r--   0 root         (0) root         (0)      342 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_exattype.2
+-rw-rw-r--   0 root         (0) root         (0)      531 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_ext_attr.2
+-rw-rw-r--   0 root         (0) root         (0)     1507 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_ext_die.2
+-rw-rw-r--   0 root         (0) root         (0)      734 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_get_discovery_log.2
+-rw-rw-r--   0 root         (0) root         (0)      799 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_get_discovery_wargs.2
+-rw-rw-r--   0 root         (0) root         (0)      490 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_hostid_from_file.2
+-rw-rw-r--   0 root         (0) root         (0)      492 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_hostnqn_from_file.2
+-rw-rw-r--   0 root         (0) root         (0)      336 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_hostnqn_generate.2
+-rw-rw-r--   0 root         (0) root         (0)      668 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_log_discovery_lid_support.2
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_log_discovery_lsp.2
+-rw-rw-r--   0 root         (0) root         (0)      378 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_prtype_str.2
+-rw-rw-r--   0 root         (0) root         (0)      382 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_qptype_str.2
+-rw-rw-r--   0 root         (0) root         (0)      346 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_rdma_cms.2
+-rw-rw-r--   0 root         (0) root         (0)      692 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_rdma_prtype.2
+-rw-rw-r--   0 root         (0) root         (0)      434 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_rdma_qptype.2
+-rw-rw-r--   0 root         (0) root         (0)      779 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_register_ctrl.2
+-rw-rw-r--   0 root         (0) root         (0)      362 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_sectype_str.2
+-rw-rw-r--   0 root         (0) root         (0)      369 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_subtype_str.2
+-rw-rw-r--   0 root         (0) root         (0)      636 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_tcp_sectype.2
+-rw-rw-r--   0 root         (0) root         (0)      572 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_treq.2
+-rw-rw-r--   0 root         (0) root         (0)      356 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_treq_str.2
+-rw-rw-r--   0 root         (0) root         (0)      732 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_trtype.2
+-rw-rw-r--   0 root         (0) root         (0)      362 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_trtype_str.2
+-rw-rw-r--   0 root         (0) root         (0)      538 2024-05-03 12:08:20.000000 libnvme-1.9/doc/man/nvmf_update_config.2
+-rw-rw-r--   0 root         (0) root         (0)     3076 2024-05-03 12:08:20.000000 libnvme-1.9/doc/meson.build
+-rw-rw-r--   0 root         (0) root         (0)     2763 2024-05-03 12:08:20.000000 libnvme-1.9/doc/mi.rst.in
+-rw-rw-r--   0 root         (0) root         (0)       37 2024-05-03 12:08:20.000000 libnvme-1.9/doc/quickstart.rst.in
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/
+-rw-rw-r--   0 root         (0) root         (0)    10054 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/fabrics.rst
+-rw-rw-r--   0 root         (0) root         (0)     2133 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/filters.rst
+-rw-rw-r--   0 root         (0) root         (0)   127041 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/ioctl.rst
+-rw-rw-r--   0 root         (0) root         (0)    17664 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/linux.rst
+-rw-rw-r--   0 root         (0) root         (0)     1980 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/log.rst
+-rw-rw-r--   0 root         (0) root         (0)     1018 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/meson.build
+-rw-rw-r--   0 root         (0) root         (0)    80384 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/mi.rst
+-rw-rw-r--   0 root         (0) root         (0)    51138 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/nbft.rst
+-rw-rw-r--   0 root         (0) root         (0)    41766 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/tree.rst
+-rw-rw-r--   0 root         (0) root         (0)   259188 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/types.rst
+-rw-rw-r--   0 root         (0) root         (0)    15666 2024-05-03 12:08:20.000000 libnvme-1.9/doc/rst/util.rst
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/examples/
+-rw-rw-r--   0 root         (0) root         (0)     2631 2024-05-03 12:08:20.000000 libnvme-1.9/examples/discover-loop.c
+-rw-rw-r--   0 root         (0) root         (0)     1952 2024-05-03 12:08:20.000000 libnvme-1.9/examples/discover-loop.py
+-rw-rw-r--   0 root         (0) root         (0)     3090 2024-05-03 12:08:20.000000 libnvme-1.9/examples/display-columnar.c
+-rw-rw-r--   0 root         (0) root         (0)     1869 2024-05-03 12:08:20.000000 libnvme-1.9/examples/display-tree.c
+-rw-rw-r--   0 root         (0) root         (0)     1085 2024-05-03 12:08:20.000000 libnvme-1.9/examples/meson.build
+-rw-rw-r--   0 root         (0) root         (0)     4906 2024-05-03 12:08:20.000000 libnvme-1.9/examples/mi-conf.c
+-rw-rw-r--   0 root         (0) root         (0)    18351 2024-05-03 12:08:20.000000 libnvme-1.9/examples/mi-mctp.c
+-rw-rw-r--   0 root         (0) root         (0)     3306 2024-05-03 12:08:20.000000 libnvme-1.9/examples/telemetry-listen.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/internal/
+-rw-rw-r--   0 root         (0) root         (0)      671 2024-05-03 12:08:20.000000 libnvme-1.9/internal/meson.build
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/
+-rw-rw-r--   0 root         (0) root         (0)       40 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     2146 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/README.md
+-rw-rw-r--   0 root         (0) root         (0)      231 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3243 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/meson.build
+-rw-rw-r--   0 root         (0) root         (0)    30479 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/nvme.i
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/tests/
+-rw-rw-r--   0 root         (0) root         (0)     1017 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/tests/NBFT
+-rwxrwxr-x   0 root         (0) root         (0)      393 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/tests/create-ctrl-obj.py
+-rwxrwxr-x   0 root         (0) root         (0)      958 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/tests/gc.py
+-rwxrwxr-x   0 root         (0) root         (0)     3468 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme/tests/test-nbft.py
+-rw-rw-r--   0 root         (0) root         (0)     1313 2024-05-03 12:08:20.000000 libnvme-1.9/libnvme.spec.in
+-rw-rw-r--   0 root         (0) root         (0)     9020 2024-05-03 12:08:20.000000 libnvme-1.9/meson.build
+-rw-rw-r--   0 root         (0) root         (0)     1075 2024-05-03 12:08:20.000000 libnvme-1.9/meson_options.txt
+-rw-rw-r--   0 root         (0) root         (0)      930 2024-05-03 12:08:20.000000 libnvme-1.9/pyproject.toml
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/
+-rwxrwxr-x   0 root         (0) root         (0)     5987 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/build.sh
+-rwxrwxr-x   0 root         (0) root         (0)      461 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/collect-sysfs.sh
+-rwxrwxr-x   0 root         (0) root         (0)    70557 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/kernel-doc
+-rwxrwxr-x   0 root         (0) root         (0)      264 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/kernel-doc-check
+-rwxrwxr-x   0 root         (0) root         (0)      354 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/list-man-pages.sh
+-rwxrwxr-x   0 root         (0) root         (0)       47 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/list-pre-compiled.sh
+-rwxrwxr-x   0 root         (0) root         (0)      613 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/meson-vcs-tag.sh
+-rwxrwxr-x   0 root         (0) root         (0)     3195 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/release.sh
+-rwxrwxr-x   0 root         (0) root         (0)     1002 2024-05-03 12:08:20.000000 libnvme-1.9/scripts/update-docs.sh
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/src/
+-rw-rw-r--   0 root         (0) root         (0)      394 2024-05-03 12:08:20.000000 libnvme-1.9/src/libnvme-mi.h
+-rw-rw-r--   0 root         (0) root         (0)     1254 2024-05-03 12:08:20.000000 libnvme-1.9/src/libnvme-mi.map
+-rw-rw-r--   0 root         (0) root         (0)      609 2024-05-03 12:08:20.000000 libnvme-1.9/src/libnvme.h
+-rw-rw-r--   0 root         (0) root         (0)     8586 2024-05-03 12:08:20.000000 libnvme-1.9/src/libnvme.map
+-rw-rw-r--   0 root         (0) root         (0)     3313 2024-05-03 12:08:20.000000 libnvme-1.9/src/meson.build
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/
+-rw-rw-r--   0 root         (0) root         (0)    28102 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/api-types.h
+-rw-rw-r--   0 root         (0) root         (0)     2028 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/base64.c
+-rw-rw-r--   0 root         (0) root         (0)      239 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/base64.h
+-rw-rw-r--   0 root         (0) root         (0)      874 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/cleanup.h
+-rw-rw-r--   0 root         (0) root         (0)     5677 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/crc32.c
+-rw-rw-r--   0 root         (0) root         (0)      141 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/crc32.h
+-rw-rw-r--   0 root         (0) root         (0)    44548 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/fabrics.c
+-rw-rw-r--   0 root         (0) root         (0)     9780 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/fabrics.h
+-rw-rw-r--   0 root         (0) root         (0)     2180 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/filters.c
+-rw-rw-r--   0 root         (0) root         (0)     2216 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/filters.h
+-rw-rw-r--   0 root         (0) root         (0)    54666 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/ioctl.c
+-rw-rw-r--   0 root         (0) root         (0)   142474 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/ioctl.h
+-rw-rw-r--   0 root         (0) root         (0)    20274 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/json.c
+-rw-rw-r--   0 root         (0) root         (0)    32662 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/linux.c
+-rw-rw-r--   0 root         (0) root         (0)    16617 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/linux.h
+-rw-rw-r--   0 root         (0) root         (0)     2456 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/log.c
+-rw-rw-r--   0 root         (0) root         (0)     2166 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/log.h
+-rw-rw-r--   0 root         (0) root         (0)    18546 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/mi-mctp.c
+-rw-rw-r--   0 root         (0) root         (0)    40182 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/mi.c
+-rw-rw-r--   0 root         (0) root         (0)    90262 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/mi.h
+-rw-rw-r--   0 root         (0) root         (0)    21715 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/nbft.c
+-rw-rw-r--   0 root         (0) root         (0)    56067 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/nbft.h
+-rw-rw-r--   0 root         (0) root         (0)      445 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/no-json.c
+-rw-rw-r--   0 root         (0) root         (0)     6611 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/private.h
+-rw-rw-r--   0 root         (0) root         (0)     1507 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/sysfs.c
+-rw-rw-r--   0 root         (0) root         (0)    62608 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/tree.c
+-rw-rw-r--   0 root         (0) root         (0)    39742 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/tree.h
+-rw-rw-r--   0 root         (0) root         (0)   318442 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/types.h
+-rw-rw-r--   0 root         (0) root         (0)    42957 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/util.c
+-rw-rw-r--   0 root         (0) root         (0)    23314 2024-05-03 12:08:20.000000 libnvme-1.9/src/nvme/util.h
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/subprojects/
+-rw-rw-r--   0 root         (0) root         (0)      124 2024-05-03 12:08:20.000000 libnvme-1.9/subprojects/dbus.wrap
+-rw-rw-r--   0 root         (0) root         (0)      587 2024-05-03 12:08:20.000000 libnvme-1.9/subprojects/json-c.wrap
+-rw-rw-r--   0 root         (0) root         (0)      631 2024-05-03 12:08:20.000000 libnvme-1.9/subprojects/openssl.wrap
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/
+-rw-rw-r--   0 root         (0) root         (0)     1490 2024-05-03 12:08:20.000000 libnvme-1.9/test/cpp.cc
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/
+-rw-rw-r--   0 root         (0) root         (0)    12790 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/discovery.c
+-rw-rw-r--   0 root         (0) root         (0)    45840 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/features.c
+-rw-rw-r--   0 root         (0) root         (0)    16354 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/identify.c
+-rw-rw-r--   0 root         (0) root         (0)     1245 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/meson.build
+-rw-rw-r--   0 root         (0) root         (0)     5061 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/mock.c
+-rw-rw-r--   0 root         (0) root         (0)     3817 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/mock.h
+-rw-rw-r--   0 root         (0) root         (0)     1047 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/util.c
+-rw-rw-r--   0 root         (0) root         (0)      521 2024-05-03 12:08:20.000000 libnvme-1.9/test/ioctl/util.h
+-rw-rw-r--   0 root         (0) root         (0)     2374 2024-05-03 12:08:20.000000 libnvme-1.9/test/meson.build
+-rw-rw-r--   0 root         (0) root         (0)    18560 2024-05-03 12:08:20.000000 libnvme-1.9/test/mi-mctp.c
+-rw-rw-r--   0 root         (0) root         (0)    43409 2024-05-03 12:08:20.000000 libnvme-1.9/test/mi.c
+-rw-rw-r--   0 root         (0) root         (0)     3291 2024-05-03 12:08:20.000000 libnvme-1.9/test/mock-ifaddrs.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/
+-rw-rw-r--   0 root         (0) root         (0)      847 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/README
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/
+-rw-rw-r--   0 root         (0) root         (0)    13106 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-Dell.PowerEdge.R660-fw1.5.5-mpath+discovery
+-rw-rw-r--   0 root         (0) root         (0)     2341 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-Dell.PowerEdge.R660-fw1.5.5-single
+-rw-rw-r--   0 root         (0) root         (0)     2596 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-Dell.PowerEdge.R760
+-rw-rw-r--   0 root         (0) root         (0)     1622 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-auto-ipv6
+-rw-rw-r--   0 root         (0) root         (0)     1827 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-dhcp-ipv4
+-rw-rw-r--   0 root         (0) root         (0)     1587 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-dhcp-ipv6
+-rw-rw-r--   0 root         (0) root         (0)     5687 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-mpath+disc-ipv4+6_half
+-rw-rw-r--   0 root         (0) root         (0)     1597 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-rhpoc
+-rw-rw-r--   0 root         (0) root         (0)     1596 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-static-ipv4
+-rw-rw-r--   0 root         (0) root         (0)     1810 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-static-ipv4-discovery
+-rw-rw-r--   0 root         (0) root         (0)     1596 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/diffs/NBFT-static-ipv6
+-rwxrwxr-x   0 root         (0) root         (0)      101 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/gen-nbft-diffs.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     1852 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/meson.build
+-rwxrwxr-x   0 root         (0) root         (0)      130 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/nbft-dump-diff.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     5254 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/nbft-dump.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/
+-rw-rw-r--   0 root         (0) root         (0)     4147 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-Dell.PowerEdge.R660-fw1.5.5-mpath+discovery
+-rw-rw-r--   0 root         (0) root         (0)      930 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-Dell.PowerEdge.R660-fw1.5.5-single
+lrwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 12:09:45.652363 libnvme-1.9/test/nbft/tables/NBFT-Dell.PowerEdge.R760 -> ../../../libnvme/tests/NBFT
+-rw-rw-r--   0 root         (0) root         (0)      721 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-auto-ipv6
+-rw-rw-r--   0 root         (0) root         (0)      825 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-dhcp-ipv4
+-rw-rw-r--   0 root         (0) root         (0)      725 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-dhcp-ipv6
+-rw-rw-r--   0 root         (0) root         (0)     1922 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-mpath+disc-ipv4+6_half
+-rw-rw-r--   0 root         (0) root         (0)      724 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-rhpoc
+-rw-rw-r--   0 root         (0) root         (0)      725 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-static-ipv4
+-rw-rw-r--   0 root         (0) root         (0)      825 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-static-ipv4-discovery
+-rw-rw-r--   0 root         (0) root         (0)      721 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables/NBFT-static-ipv6
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables_bad/
+-rw-rw-r--   0 root         (0) root         (0)     1103 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables_bad/NBFT-bad-oldspec
+-rw-rw-r--   0 root         (0) root         (0)      512 2024-05-03 12:08:20.000000 libnvme-1.9/test/nbft/tables_bad/NBFT-random-noise
+-rw-rw-r--   0 root         (0) root         (0)     8740 2024-05-03 12:08:20.000000 libnvme-1.9/test/register.c
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/data/
+-rw-rw-r--   0 root         (0) root         (0)      742 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.out
+-rw-rw-r--   0 root         (0) root         (0)    19712 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.tar.xz
+-rw-rw-r--   0 root         (0) root         (0)      899 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/meson.build
+-rw-rw-r--   0 root         (0) root         (0)      559 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/sysfs-tree-diff.sh
+-rw-rw-r--   0 root         (0) root         (0)      403 2024-05-03 12:08:20.000000 libnvme-1.9/test/sysfs/sysfs.c
+-rw-rw-r--   0 root         (0) root         (0)     6079 2024-05-03 12:08:20.000000 libnvme-1.9/test/test-util.c
+-rw-rw-r--   0 root         (0) root         (0)    12831 2024-05-03 12:08:20.000000 libnvme-1.9/test/test.c
+-rw-rw-r--   0 root         (0) root         (0)    50475 2024-05-03 12:08:20.000000 libnvme-1.9/test/tree.c
+-rw-rw-r--   0 root         (0) root         (0)      453 2024-05-03 12:08:20.000000 libnvme-1.9/test/tree.py
+-rw-rw-r--   0 root         (0) root         (0)     1083 2024-05-03 12:08:20.000000 libnvme-1.9/test/utils.c
+-rw-rw-r--   0 root         (0) root         (0)      455 2024-05-03 12:08:20.000000 libnvme-1.9/test/utils.h
+-rw-rw-r--   0 root         (0) root         (0)     2648 2024-05-03 12:08:20.000000 libnvme-1.9/test/uuid.c
+-rw-rw-r--   0 root         (0) root         (0)     1997 2024-05-03 12:08:20.000000 libnvme-1.9/test/zns.c
+-rw-r--r--   0 root         (0) root         (0)     7683 2024-05-03 12:09:45.972368 libnvme-1.9/PKG-INFO
```

### Comparing `libnvme-1.8/.checkpatch.conf` & `libnvme-1.9/.checkpatch.conf`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/.github/workflows/build.yml` & `libnvme-1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/.github/workflows/release-python.yml` & `libnvme-1.9/.github/workflows/release-python.yml`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/COPYING` & `libnvme-1.9/COPYING`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/Makefile` & `libnvme-1.9/Makefile`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/README.md` & `libnvme-1.9/README.md`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/array_size/_info` & `libnvme-1.9/ccan/ccan/array_size/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/array_size/array_size.h` & `libnvme-1.9/ccan/ccan/array_size/array_size.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/build_assert/_info` & `libnvme-1.9/ccan/ccan/build_assert/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/build_assert/build_assert.h` & `libnvme-1.9/ccan/ccan/build_assert/build_assert.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/check_type/_info` & `libnvme-1.9/ccan/ccan/check_type/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/check_type/check_type.h` & `libnvme-1.9/ccan/ccan/check_type/check_type.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/container_of/_info` & `libnvme-1.9/ccan/ccan/container_of/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/container_of/container_of.h` & `libnvme-1.9/ccan/ccan/container_of/container_of.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/endian/_info` & `libnvme-1.9/ccan/ccan/endian/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/endian/endian.h` & `libnvme-1.9/ccan/ccan/endian/endian.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/list/_info` & `libnvme-1.9/ccan/ccan/list/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/list/list.c` & `libnvme-1.9/ccan/ccan/list/list.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/list/list.h` & `libnvme-1.9/ccan/ccan/list/list.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/minmax/_info` & `libnvme-1.9/ccan/ccan/minmax/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/minmax/minmax.h` & `libnvme-1.9/ccan/ccan/minmax/minmax.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/short_types/short_types.h` & `libnvme-1.9/ccan/ccan/short_types/short_types.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/str/_info` & `libnvme-1.9/ccan/ccan/str/_info`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/str/debug.c` & `libnvme-1.9/ccan/ccan/str/debug.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/str/str.h` & `libnvme-1.9/ccan/ccan/str/str.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/ccan/str/str_debug.h` & `libnvme-1.9/ccan/ccan/str/str_debug.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/licenses/BSD-MIT` & `libnvme-1.9/ccan/licenses/BSD-MIT`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/licenses/CC0` & `libnvme-1.9/ccan/licenses/CC0`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/ccan/meson.build` & `libnvme-1.9/ccan/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/conf.py` & `libnvme-1.9/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'libnvme'
 copyright = '2020, Keith Busch'
 author = 'Keith Busch <kbusch@kernel.org>'
 master_doc = 'index'
 
-release = '1.8'
+release = '1.9'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `libnvme-1.8/doc/conf.py.in` & `libnvme-1.9/doc/conf.py.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/config-schema.json` & `libnvme-1.9/doc/config-schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999856913919414%*

 * *Differences: {"'$defs'": "{'port': {'properties': {'keyring': {'type': 'string'}, 'tls_key': {'type': "*

 * *            "'string'}}}}"}*

```diff
@@ -96,15 +96,15 @@
                 },
                 "keep_alive_tmo": {
                     "description": "Keep-Alive timeout (in seconds)",
                     "type": "integer"
                 },
                 "keyring": {
                     "description": "Keyring for TLS key lookup",
-                    "type": "integer"
+                    "type": "string"
                 },
                 "nr_io_queues": {
                     "description": "Number of I/O queues",
                     "type": "integer"
                 },
                 "nr_poll_queues": {
                     "description": "Number of poll queues",
@@ -129,15 +129,15 @@
                 "tls": {
                     "default": false,
                     "description": "Enable TLS encryption",
                     "type": "boolean"
                 },
                 "tls_key": {
                     "description": "TLS key for the connection",
-                    "type": "integer"
+                    "type": "string"
                 },
                 "tos": {
                     "default": -1,
                     "description": "Type of service",
                     "type": "integer"
                 },
                 "traddr": {
```

### Comparing `libnvme-1.8/doc/config-schema.json.in` & `libnvme-1.9/doc/config-schema.json.in`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999856913919414%*

 * *Differences: {"'$defs'": "{'port': {'properties': {'keyring': {'type': 'string'}, 'tls_key': {'type': "*

 * *            "'string'}}}}"}*

```diff
@@ -96,15 +96,15 @@
                 },
                 "keep_alive_tmo": {
                     "description": "Keep-Alive timeout (in seconds)",
                     "type": "integer"
                 },
                 "keyring": {
                     "description": "Keyring for TLS key lookup",
-                    "type": "integer"
+                    "type": "string"
                 },
                 "nr_io_queues": {
                     "description": "Number of I/O queues",
                     "type": "integer"
                 },
                 "nr_poll_queues": {
                     "description": "Number of poll queues",
@@ -129,15 +129,15 @@
                 "tls": {
                     "default": false,
                     "description": "Enable TLS encryption",
                     "type": "boolean"
                 },
                 "tls_key": {
                     "description": "TLS key for the connection",
-                    "type": "integer"
+                    "type": "string"
                 },
                 "tos": {
                     "default": -1,
                     "description": "Type of service",
                     "type": "integer"
                 },
                 "traddr": {
```

### Comparing `libnvme-1.8/doc/index.rst` & `libnvme-1.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/index.rst.in` & `libnvme-1.9/doc/index.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/installation.rst.in` & `libnvme-1.9/doc/installation.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/man/nbft_control.2` & `libnvme-1.9/doc/man/nbft_control.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_control" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_control" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_control \- NBFT Table - Control Descriptor (Figure 8)
 .SH SYNOPSIS
 struct nbft_control {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_desc_type.2` & `libnvme-1.9/doc/man/nbft_desc_type.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_desc_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_desc_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_desc_type \- NBFT Elements - Descriptor Types (Figure 5)
 .SH SYNOPSIS
 enum nbft_desc_type {
 .br
 .BI "    NBFT_DESC_HEADER"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_discovery.2` & `libnvme-1.9/doc/man/nbft_discovery.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_discovery" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_discovery" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_discovery \- Discovery Descriptor (Figure 24)
 .SH SYNOPSIS
 struct nbft_discovery {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_header.2` & `libnvme-1.9/doc/man/nbft_header.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_header" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_header" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_header \- NBFT Table - Header (Figure 8)
 .SH SYNOPSIS
 struct nbft_header {
 .br
 .BI "    char signature[4];"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_hfi.2` & `libnvme-1.9/doc/man/nbft_hfi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_hfi" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_hfi" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_hfi \- Host Fabric Interface (HFI) Descriptor (Figure 11)
 .SH SYNOPSIS
 struct nbft_hfi {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_hfi_info_tcp.2` & `libnvme-1.9/doc/man/nbft_hfi_info_tcp.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_hfi_info_tcp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_hfi_info_tcp" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_hfi_info_tcp \- HFI Transport Info Descriptor - NVMe/TCP (Figure 13)
 .SH SYNOPSIS
 struct nbft_hfi_info_tcp {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_hfi_info_tcp_flags.2` & `libnvme-1.9/doc/man/nbft_hfi_info_tcp_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_hfi_info_tcp_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_hfi_info_tcp_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_hfi_info_tcp_flags \- HFI Transport Flags
 .SH SYNOPSIS
 enum nbft_hfi_info_tcp_flags {
 .br
 .BI "    NBFT_HFI_INFO_TCP_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_host.2` & `libnvme-1.9/doc/man/nbft_host.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_host" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_host" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_host \- Host Descriptor (Figure 9)
 .SH SYNOPSIS
 struct nbft_host {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_host_flags.2` & `libnvme-1.9/doc/man/nbft_host_flags.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_host_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_host_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_host_flags \- Host Flags
 .SH SYNOPSIS
 enum nbft_host_flags {
 .br
 .BI "    NBFT_HOST_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_info.2` & `libnvme-1.9/doc/man/nbft_info.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info \- The parsed NBFT table data.
 .SH SYNOPSIS
 struct nbft_info {
 .br
 .BI "    char *filename;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_info_discovery.2` & `libnvme-1.9/doc/man/nbft_info_discovery.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info_discovery" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info_discovery" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info_discovery \- Discovery Descriptor
 .SH SYNOPSIS
 struct nbft_info_discovery {
 .br
 .BI "    int index;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_info_hfi.2` & `libnvme-1.9/doc/man/nbft_info_hfi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info_hfi" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info_hfi" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info_hfi \- Host Fabric Interface (HFI) Descriptor
 .SH SYNOPSIS
 struct nbft_info_hfi {
 .br
 .BI "    int index;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_info_hfi_info_tcp.2` & `libnvme-1.9/doc/man/nbft_info_hfi_info_tcp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info_hfi_info_tcp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info_hfi_info_tcp" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info_hfi_info_tcp \- HFI Transport Info Descriptor - NVMe/TCP
 .SH SYNOPSIS
 struct nbft_info_hfi_info_tcp {
 .br
 .BI "    __u32 pci_sbdf;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_info_host.2` & `libnvme-1.9/doc/man/nbft_info_host.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info_host" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info_host" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info_host \- Host Descriptor
 .SH SYNOPSIS
 struct nbft_info_host {
 .br
 .BI "    unsigned char *id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_info_nid_type.2` & `libnvme-1.9/doc/man/nbft_info_nid_type.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_info_nid_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_info_nid_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_info_nid_type \- Namespace Identifier Type (NIDT)
 .SH SYNOPSIS
 enum nbft_info_nid_type {
 .br
 .BI "    NBFT_INFO_NID_TYPE_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_info_primary_admin_host_flag.2` & `libnvme-1.9/doc/man/nbft_info_primary_admin_host_flag.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_info_primary_admin_host_flag" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_info_primary_admin_host_flag" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_info_primary_admin_host_flag \- Primary Administrative Host Descriptor Flags
 .SH SYNOPSIS
 enum nbft_info_primary_admin_host_flag {
 .br
 .BI "    NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_NOT_INDICATED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_info_subsystem_ns.2` & `libnvme-1.9/doc/man/nbft_info_subsystem_ns.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_info_subsystem_ns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_info_subsystem_ns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_info_subsystem_ns \- Subsystem Namespace (SSNS) info
 .SH SYNOPSIS
 struct nbft_info_subsystem_ns {
 .br
 .BI "    int index;"
 .br
@@ -36,14 +36,18 @@
 .br
 .BI "    int controller_id;"
 .br
 .BI "    int asqsz;"
 .br
 .BI "    char *dhcp_root_path_string;"
 .br
+.BI "    bool discovered;"
+.br
+.BI "    bool unavailable;"
+.br
 .BI "
 };
 .br
 
 .SH Members
 .IP "index" 12
 SSNS Descriptor Index in the descriptor list.
@@ -88,7 +92,13 @@
 or 0 if not supported.
 .IP "asqsz" 12
 Admin Submission Queue Size (SSNS Extended Information
 Descriptor) or 0 if not supported.
 .IP "dhcp_root_path_string" 12
 DHCP Root Path Override string (SSNS Extended
 Information Descriptor).
+.IP "discovered" 12
+Indicates that this namespace was acquired
+through discovery.
+.IP "unavailable" 12
+Namespace is unavailable as indicated by
+the pre-OS driver.
```

### Comparing `libnvme-1.8/doc/man/nbft_security.2` & `libnvme-1.9/doc/man/nbft_security.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_security" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_security" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_security \- Security Profile Descriptor (Figure 21)
 .SH SYNOPSIS
 struct nbft_security {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_security_flags.2` & `libnvme-1.9/doc/man/nbft_security_flags.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_security_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_security_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_security_flags \- Security Profile Descriptor Flags (Figure 22)
 .SH SYNOPSIS
 enum nbft_security_flags {
 .br
 .BI "    NBFT_SECURITY_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_ssns.2` & `libnvme-1.9/doc/man/nbft_ssns.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_ssns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_ssns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_ssns \- Subsystem Namespace (SSNS) Descriptor (Figure 15)
 .SH SYNOPSIS
 struct nbft_ssns {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_ssns_ext_info.2` & `libnvme-1.9/doc/man/nbft_ssns_ext_info.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nbft_ssns_ext_info" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nbft_ssns_ext_info" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nbft_ssns_ext_info \- Subsystem and Namespace Extended Information Descriptor (Figure 19)
 .SH SYNOPSIS
 struct nbft_ssns_ext_info {
 .br
 .BI "    __u8 structure_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nbft_ssns_ext_info_flags.2` & `libnvme-1.9/doc/man/nbft_ssns_ext_info_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_ssns_ext_info_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_ssns_ext_info_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_ssns_ext_info_flags \- Subsystem and Namespace Extended Information Descriptor Flags
 .SH SYNOPSIS
 enum nbft_ssns_ext_info_flags {
 .br
 .BI "    NBFT_SSNS_EXT_INFO_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_ssns_flags.2` & `libnvme-1.9/doc/man/nbft_ssns_flags.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_ssns_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_ssns_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_ssns_flags \- Subsystem and Namespace Specific Flags Field (Figure 16)
 .SH SYNOPSIS
 enum nbft_ssns_flags {
 .br
 .BI "    NBFT_SSNS_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nbft_ssns_trflags.2` & `libnvme-1.9/doc/man/nbft_ssns_trflags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nbft_ssns_trflags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nbft_ssns_trflags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nbft_ssns_trflags \- SSNS Transport Specific Flags Field (Figure 17)
 .SH SYNOPSIS
 enum nbft_ssns_trflags {
 .br
 .BI "    NBFT_SSNS_TRFLAG_VALID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_admin_opcode.2` & `libnvme-1.9/doc/man/nvme_admin_opcode.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_admin_opcode" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_admin_opcode" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_admin_opcode \- Known NVMe admin opcodes
 .SH SYNOPSIS
 enum nvme_admin_opcode {
 .br
 .BI "    nvme_admin_delete_sq"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_admin_passthru.2` & `libnvme-1.9/doc/man/nvme_admin_passthru64.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_admin_passthru" 9 "nvme_admin_passthru" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_admin_passthru64" 9 "nvme_admin_passthru64" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_admin_passthru \- Submit an nvme passthrough command
+nvme_admin_passthru64 \- Submit a 64-bit nvme passthrough command
 .SH SYNOPSIS
-.B "int" nvme_admin_passthru
+.B "int" nvme_admin_passthru64
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -17,15 +17,15 @@
 .BI "__u32 cdw14 "  ","
 .BI "__u32 cdw15 "  ","
 .BI "__u32 data_len "  ","
 .BI "void *data "  ","
 .BI "__u32 metadata_len "  ","
 .BI "void *metadata "  ","
 .BI "__u32 timeout_ms "  ","
-.BI "__u32 *result "  ");"
+.BI "__u64 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "opcode" 12
 The nvme io command to send
 .IP "flags" 12
 NVMe command flags (not used)
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_admin_passthru\fP. This sets up and
-submits a \fIstruct nvme_passthru_cmd\fP.
+Parameterized form of \fBnvme_submit_admin_passthru64\fP. This sets up and
+submits a \fIstruct nvme_passthru_cmd64\fP.
 
 Known values for \fIopcode\fP are defined in \fIenum nvme_admin_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_admin_passthru64.2` & `libnvme-1.9/doc/man/nvme_io_passthru64.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_admin_passthru64" 9 "nvme_admin_passthru64" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_io_passthru64" 9 "nvme_io_passthru64" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_admin_passthru64 \- Submit a 64-bit nvme passthrough command
+nvme_io_passthru64 \- Submit an nvme io passthrough command
 .SH SYNOPSIS
-.B "int" nvme_admin_passthru64
+.B "int" nvme_io_passthru64
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_admin_passthru64\fP. This sets up and
-submits a \fIstruct nvme_passthru_cmd64\fP.
+Parameterized form of \fBnvme_submit_io_passthru64\fP. This sets up and submits
+a \fIstruct nvme_passthru_cmd64\fP.
 
-Known values for \fIopcode\fP are defined in \fIenum nvme_admin_opcode\fP.
+Known values for \fIopcode\fP are defined in \fIenum nvme_io_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_ae_info_css_nvm.2` & `libnvme-1.9/doc/man/nvme_ae_info_css_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_css_nvm" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_css_nvm" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_css_nvm \- Asynchronous Event Information - I/O Command Specific Status
 .SH SYNOPSIS
 enum nvme_ae_info_css_nvm {
 .br
 .BI "    NVME_AER_CSS_NVM_RESERVATION"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ae_info_error.2` & `libnvme-1.9/doc/man/nvme_ae_info_error.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_error" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_error" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_error \- Asynchronous Event Information - Error Status
 .SH SYNOPSIS
 enum nvme_ae_info_error {
 .br
 .BI "    NVME_AER_ERROR_INVALID_DB_REG"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ae_info_notice.2` & `libnvme-1.9/doc/man/nvme_ae_info_notice.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_notice" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_notice" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_notice \- Asynchronous Event Information - Notice
 .SH SYNOPSIS
 enum nvme_ae_info_notice {
 .br
 .BI "    NVME_AER_NOTICE_NS_CHANGED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ae_info_smart.2` & `libnvme-1.9/doc/man/nvme_ae_info_smart.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_info_smart" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_info_smart" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_info_smart \- Asynchronous Event Information - SMART / Health Status
 .SH SYNOPSIS
 enum nvme_ae_info_smart {
 .br
 .BI "    NVME_AER_SMART_SUBSYSTEM_RELIABILITY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ae_type.2` & `libnvme-1.9/doc/man/nvme_ae_type.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ae_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ae_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ae_type \- Asynchronous Event Type
 .SH SYNOPSIS
 enum nvme_ae_type {
 .br
 .BI "    NVME_AER_ERROR"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ana_group_desc.2` & `libnvme-1.9/doc/man/nvme_ana_group_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_ana_group_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_ana_group_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_ana_group_desc \- ANA Group Descriptor
 .SH SYNOPSIS
 struct nvme_ana_group_desc {
 .br
 .BI "    __le32 grpid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_ana_state.2` & `libnvme-1.9/doc/man/nvme_ana_state.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ana_state" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ana_state" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ana_state \- ANA Group Descriptor - Asymmetric Namespace Access State
 .SH SYNOPSIS
 enum nvme_ana_state {
 .br
 .BI "    NVME_ANA_STATE_OPTIMIZED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_apst_entry.2` & `libnvme-1.9/doc/man/nvme_apst_entry.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_apst_entry" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_apst_entry" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_apst_entry \- Autonomous Power State Transition
 .SH SYNOPSIS
 enum nvme_apst_entry {
 .br
 .BI "    NVME_APST_ENTRY_ITPS_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_boot_partition.2` & `libnvme-1.9/doc/man/nvme_boot_partition.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_boot_partition" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_boot_partition" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_boot_partition \- Boot Partition Log
 .SH SYNOPSIS
 struct nvme_boot_partition {
 .br
 .BI "    __u8 lid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_capacity_config_desc.2` & `libnvme-1.9/doc/man/nvme_capacity_config_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_capacity_config_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_capacity_config_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_capacity_config_desc \- Capacity Configuration structure definitions
 .SH SYNOPSIS
 struct nvme_capacity_config_desc {
 .br
 .BI "    __le16 cap_config_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_change_ns_event.2` & `libnvme-1.9/doc/man/nvme_change_ns_event.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_change_ns_event" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_change_ns_event" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_change_ns_event \- Change Namespace Event Data
 .SH SYNOPSIS
 struct nvme_change_ns_event {
 .br
 .BI "    __le32 nsmgt_cdw10;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_channel_config_desc.2` & `libnvme-1.9/doc/man/nvme_channel_config_desc.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_channel_config_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_channel_config_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_channel_config_desc \- Channel Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_channel_config_desc {
 .br
 .BI "    __le16 chanid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_cmd_effects.2` & `libnvme-1.9/doc/man/nvme_cmd_effects.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_effects" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_effects" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_effects \- Commands Supported and Effects
 .SH SYNOPSIS
 enum nvme_cmd_effects {
 .br
 .BI "    NVME_CMD_EFFECTS_CSUPP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_cmd_format_pi.2` & `libnvme-1.9/doc/man/nvme_cmd_format_pi.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_format_pi" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_format_pi" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_format_pi \- Format NVM - Protection Information
 .SH SYNOPSIS
 enum nvme_cmd_format_pi {
 .br
 .BI "    NVME_FORMAT_PI_DISABLE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_cmd_format_ses.2` & `libnvme-1.9/doc/man/nvme_cmd_format_ses.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_format_ses" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_format_ses" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_format_ses \- Format NVM - Secure Erase Settings
 .SH SYNOPSIS
 enum nvme_cmd_format_ses {
 .br
 .BI "    NVME_FORMAT_SES_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_cmd_get_log_lid.2` & `libnvme-1.9/doc/man/nvme_cmd_get_log_lid.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_cmd_get_log_lid" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_cmd_get_log_lid" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_cmd_get_log_lid \- Get Log Page -Log Page Identifiers
 .SH SYNOPSIS
 enum nvme_cmd_get_log_lid {
 .br
 .BI "    NVME_LOG_LID_SUPPORTED_LOG_PAGES"
 , 
@@ -80,14 +80,18 @@
 , 
 .br
 .br
 .BI "    NVME_LOG_LID_MI_CMD_SUPPORTED_EFFECTS"
 , 
 .br
 .br
+.BI "    NVME_LOG_LID_CMD_AND_FEAT_LOCKDOWN"
+, 
+.br
+.br
 .BI "    NVME_LOG_LID_BOOT_PARTITION"
 , 
 .br
 .br
 .BI "    NVME_LOG_LID_PHY_RX_EOM"
 , 
 .br
@@ -160,14 +164,16 @@
 Media Unit Status
 .IP "NVME_LOG_LID_SUPPORTED_CAP_CONFIG_LIST" 12
 Supported Capacity Configuration Lis
 .IP "NVME_LOG_LID_FID_SUPPORTED_EFFECTS" 12
 Feature Identifiers Supported and Effects
 .IP "NVME_LOG_LID_MI_CMD_SUPPORTED_EFFECTS" 12
 NVMe-MI Commands Supported and Effects
+.IP "NVME_LOG_LID_CMD_AND_FEAT_LOCKDOWN" 12
+Command and Feature Lockdown
 .IP "NVME_LOG_LID_BOOT_PARTITION" 12
 Boot Partition
 .IP "NVME_LOG_LID_PHY_RX_EOM" 12
 Physical Interface Receiver Eye Opening Measurement
 .IP "NVME_LOG_LID_FDP_CONFIGS" 12
 FDP Configurations
 .IP "NVME_LOG_LID_FDP_RUH_USAGE" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_connect_err.2` & `libnvme-1.9/doc/man/nvme_connect_err.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_connect_err" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_connect_err" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_connect_err \- nvme connect error codes
 .SH SYNOPSIS
 enum nvme_connect_err {
 .br
 .BI "    ENVME_CONNECT_RESOLVE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_constants.2` & `libnvme-1.9/doc/man/nvme_constants.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_constants" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_constants" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_constants \- A place to stash various constant nvme values
 .SH SYNOPSIS
 enum nvme_constants {
 .br
 .BI "    NVME_NSID_ALL"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_copy_range.2` & `libnvme-1.9/doc/man/nvme_copy_range.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range \- Copy - Source Range Entries Descriptor Format
 .SH SYNOPSIS
 struct nvme_copy_range {
 .br
 .BI "    __u8 rsvd0[8];"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_copy_range_f1.2` & `libnvme-1.9/doc/man/nvme_copy_range_f1.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range_f1" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range_f1" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range_f1 \- Copy - Source Range Entries Descriptor Format 1h
 .SH SYNOPSIS
 struct nvme_copy_range_f1 {
 .br
 .BI "    __u8 rsvd0[8];"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_copy_range_f2.2` & `libnvme-1.9/doc/man/nvme_copy_range_f2.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range_f2" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range_f2" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range_f2 \- Copy - Source Range Entries Descriptor Format 2h
 .SH SYNOPSIS
 struct nvme_copy_range_f2 {
 .br
 .BI "    __le32 snsid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_copy_range_f3.2` & `libnvme-1.9/doc/man/nvme_copy_range_f3.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_copy_range_f3" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_copy_range_f3" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_copy_range_f3 \- Copy - Source Range Entries Descriptor Format 3h
 .SH SYNOPSIS
 struct nvme_copy_range_f3 {
 .br
 .BI "    __le32 snsid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_create_ctrl.2` & `libnvme-1.9/doc/man/nvme_create_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_create_ctrl" 9 "nvme_create_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_create_ctrl" 9 "nvme_create_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_create_ctrl \- Allocate an unconnected NVMe controller
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvme_create_ctrl
 .BI "(nvme_root_t r "  ","
 .BI "const char *subsysnqn "  ","
 .BI "const char *transport "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_config_match.2` & `libnvme-1.9/doc/man/nvme_ctrl_config_match.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_config_match" 9 "nvme_ctrl_config_match" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ctrl_config_match" 9 "nvme_ctrl_config_match" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_config_match \- Check if ctrl @c matches config params
 .SH SYNOPSIS
 .B "bool" nvme_ctrl_config_match
 .BI "(struct nvme_ctrl *c "  ","
 .BI "const char *transport "  ","
 .BI "const char *traddr "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_find.2` & `libnvme-1.9/doc/man/nvme_ctrl_find.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_find" 9 "nvme_ctrl_find" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ctrl_find" 9 "nvme_ctrl_find" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_find \- Locate an existing controller
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvme_ctrl_find
 .BI "(nvme_subsystem_t s "  ","
 .BI "const char *transport "  ","
 .BI "const char *traddr "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_get_fd.2` & `libnvme-1.9/doc/man/nvme_ctrl_get_fd.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_get_fd" 9 "nvme_ctrl_get_fd" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ctrl_get_fd" 9 "nvme_ctrl_get_fd" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_get_fd \- Get associated file descriptor
 .SH SYNOPSIS
 .B "int" nvme_ctrl_get_fd
 .BI "(nvme_ctrl_t c "  ");"
 .SH ARGUMENTS
 .IP "c" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_get_src_addr.2` & `libnvme-1.9/doc/man/nvme_ctrl_get_src_addr.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_get_src_addr" 9 "nvme_ctrl_get_src_addr" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ctrl_get_src_addr" 9 "nvme_ctrl_get_src_addr" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_get_src_addr \- Extract src_addr from the c->address string
 .SH SYNOPSIS
 .B "char *" nvme_ctrl_get_src_addr
 .BI "(nvme_ctrl_t c "  ","
 .BI "char *src_addr "  ","
 .BI "size_t src_addr_len "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_metadata_type.2` & `libnvme-1.9/doc/man/nvme_ctrl_metadata_type.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ctrl_metadata_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ctrl_metadata_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ctrl_metadata_type \- Controller Metadata Element Types
 .SH SYNOPSIS
 enum nvme_ctrl_metadata_type {
 .br
 .BI "    NVME_CTRL_METADATA_OS_CTRL_NAME"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2` & `libnvme-1.9/doc/man/nvme_ctrl_set_unique_discovery_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ctrl_set_unique_discovery_ctrl" 9 "nvme_ctrl_set_unique_discovery_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ctrl_set_unique_discovery_ctrl" 9 "nvme_ctrl_set_unique_discovery_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ctrl_set_unique_discovery_ctrl \- Set the 'unique_discovery_ctrl' flag
 .SH SYNOPSIS
 .B "void" nvme_ctrl_set_unique_discovery_ctrl
 .BI "(nvme_ctrl_t c "  ","
 .BI "bool unique "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_data_tfr.2` & `libnvme-1.9/doc/man/nvme_data_tfr.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_data_tfr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_data_tfr" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_data_tfr \- Data transfer direction of the command
 .SH SYNOPSIS
 enum nvme_data_tfr {
 .br
 .BI "    NVME_DATA_TFR_NO_DATA_TFR"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_dev_self_test.2` & `libnvme-1.9/doc/man/nvme_dev_self_test.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_dev_self_test" 9 "nvme_dev_self_test" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_dev_self_test" 9 "nvme_dev_self_test" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_dev_self_test \- Start or abort a self test
 .SH SYNOPSIS
 .B "int" nvme_dev_self_test
 .BI "(struct nvme_dev_self_test_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_receive_doper.2` & `libnvme-1.9/doc/man/nvme_directive_receive_doper.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_directive_receive_doper" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_directive_receive_doper" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_directive_receive_doper \- Directive Receive Directive Operation
 .SH SYNOPSIS
 enum nvme_directive_receive_doper {
 .br
 .BI "    NVME_DIRECTIVE_RECEIVE_IDENTIFY_DOPER_PARAM"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_recv_identify_parameters.2` & `libnvme-1.9/doc/man/nvme_directive_recv_identify_parameters.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_identify_parameters" 9 "nvme_directive_recv_identify_parameters" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_identify_parameters" 9 "nvme_directive_recv_identify_parameters" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_identify_parameters \- Directive receive identifier parameters
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_identify_parameters
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_directives *id "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_recv_stream_allocate.2` & `libnvme-1.9/doc/man/nvme_directive_recv_stream_allocate.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_allocate" 9 "nvme_directive_recv_stream_allocate" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_allocate" 9 "nvme_directive_recv_stream_allocate" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_allocate \- Directive receive stream allocate
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_allocate
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 nsr "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_recv_stream_parameters.2` & `libnvme-1.9/doc/man/nvme_directive_recv_stream_parameters.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_parameters" 9 "nvme_directive_recv_stream_parameters" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_parameters" 9 "nvme_directive_recv_stream_parameters" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_parameters \- Directive receive stream parameters
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_parameters
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_streams_directive_params *parms "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_recv_stream_status.2` & `libnvme-1.9/doc/man/nvme_directive_recv_stream_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_recv_stream_status" 9 "nvme_directive_recv_stream_status" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_recv_stream_status" 9 "nvme_directive_recv_stream_status" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_recv_stream_status \- Directive receive stream status
 .SH SYNOPSIS
 .B "int" nvme_directive_recv_stream_status
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "unsigned int nr_entries "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_send.2` & `libnvme-1.9/doc/man/nvme_directive_send.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_send" 9 "nvme_directive_send" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_send" 9 "nvme_directive_send" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_send \- Send directive command
 .SH SYNOPSIS
 .B "int" nvme_directive_send
 .BI "(struct nvme_directive_send_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_send_doper.2` & `libnvme-1.9/doc/man/nvme_directive_send_doper.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_directive_send_doper" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_directive_send_doper" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_directive_send_doper \- Directive Send Directive Operation
 .SH SYNOPSIS
 enum nvme_directive_send_doper {
 .br
 .BI "    NVME_DIRECTIVE_SEND_IDENTIFY_DOPER_ENDIR"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_send_id_endir.2` & `libnvme-1.9/doc/man/nvme_directive_send_id_endir.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_send_id_endir" 9 "nvme_directive_send_id_endir" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_send_id_endir" 9 "nvme_directive_send_id_endir" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_send_id_endir \- Directive Send Enable Directive
 .SH SYNOPSIS
 .B "int" nvme_directive_send_id_endir
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool endir "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_send_stream_release_identifier.2` & `libnvme-1.9/doc/man/nvme_directive_send_stream_release_identifier.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_send_stream_release_identifier" 9 "nvme_directive_send_stream_release_identifier" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_send_stream_release_identifier" 9 "nvme_directive_send_stream_release_identifier" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_send_stream_release_identifier \- Directive Send Stream release
 .SH SYNOPSIS
 .B "int" nvme_directive_send_stream_release_identifier
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 stream_id "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_directive_send_stream_release_resource.2` & `libnvme-1.9/doc/man/nvme_directive_send_stream_release_resource.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_directive_send_stream_release_resource" 9 "nvme_directive_send_stream_release_resource" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_directive_send_stream_release_resource" 9 "nvme_directive_send_stream_release_resource" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_directive_send_stream_release_resource \- Directive Send Stream release resources
 .SH SYNOPSIS
 .B "int" nvme_directive_send_stream_release_resource
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_dsm.2` & `libnvme-1.9/doc/man/nvme_dsm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_dsm" 9 "nvme_dsm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_dsm" 9 "nvme_dsm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_dsm \- Send an nvme data set management command
 .SH SYNOPSIS
 .B "int" nvme_dsm
 .BI "(struct nvme_dsm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_dst_stc.2` & `libnvme-1.9/doc/man/nvme_dst_stc.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_dst_stc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_dst_stc" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_dst_stc \- Action taken by the Device Self-test command
 .SH SYNOPSIS
 enum nvme_dst_stc {
 .br
 .BI "    NVME_DST_STC_SHORT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_eg_critical_warning_flags.2` & `libnvme-1.9/doc/man/nvme_eg_critical_warning_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_eg_critical_warning_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_eg_critical_warning_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_eg_critical_warning_flags \- Endurance Group Information Log - Critical Warning
 .SH SYNOPSIS
 enum nvme_eg_critical_warning_flags {
 .br
 .BI "    NVME_EG_CRITICAL_WARNING_SPARE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_end_grp_config_desc.2` & `libnvme-1.9/doc/man/nvme_end_grp_config_desc.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_end_grp_config_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_end_grp_config_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_end_grp_config_desc \- Endurance Group Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_end_grp_config_desc {
 .br
 .BI "    __le16 endgid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_endurance_group_log.2` & `libnvme-1.9/doc/man/nvme_endurance_group_log.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_endurance_group_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_endurance_group_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_endurance_group_log \- Endurance Group Information Log
 .SH SYNOPSIS
 struct nvme_endurance_group_log {
 .br
 .BI "    __u8 critical_warning;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_eom_lane_desc.2` & `libnvme-1.9/doc/man/nvme_eom_lane_desc.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_eom_lane_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_eom_lane_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_eom_lane_desc \- EOM Lane Descriptor
 .SH SYNOPSIS
 struct nvme_eom_lane_desc {
 .br
 .BI "    __u8 rsvd0;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_error_log_page.2` & `libnvme-1.9/doc/man/nvme_error_log_page.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_error_log_page" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_error_log_page" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_error_log_page \- Error Information Log Entry (Log Identifier 01h)
 .SH SYNOPSIS
 struct nvme_error_log_page {
 .br
 .BI "    __le64 error_count;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fabrics_config.2` & `libnvme-1.9/doc/man/nvme_fabrics_config.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fabrics_config" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fabrics_config" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fabrics_config \- Defines all linux nvme fabrics initiator options
 .SH SYNOPSIS
 struct nvme_fabrics_config {
 .br
 .BI "    char *host_traddr;"
 .br
@@ -22,17 +22,17 @@
 .br
 .BI "    int nr_write_queues;"
 .br
 .BI "    int nr_poll_queues;"
 .br
 .BI "    int tos;"
 .br
-.BI "    int keyring;"
+.BI "    long keyring;"
 .br
-.BI "    int tls_key;"
+.BI "    long tls_key;"
 .br
 .BI "    bool duplicate_connect;"
 .br
 .BI "    bool disable_sqflow;"
 .br
 .BI "    bool hdr_digest;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fctype.2` & `libnvme-1.9/doc/man/nvme_fctype.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fctype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fctype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fctype \- Fabrics Command Types
 .SH SYNOPSIS
 enum nvme_fctype {
 .br
 .BI "    nvme_fabrics_type_property_set"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_config_desc.2` & `libnvme-1.9/doc/man/nvme_fdp_config_desc.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_config_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_config_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_config_desc \- FDP Configuration Descriptor
 .SH SYNOPSIS
 struct nvme_fdp_config_desc {
 .br
 .BI "    __le16 size;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_config_fdpa.2` & `libnvme-1.9/doc/man/nvme_fdp_config_fdpa.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_config_fdpa" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_config_fdpa" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_config_fdpa \- FDP Attributes
 .SH SYNOPSIS
 enum nvme_fdp_config_fdpa {
 .br
 .BI "    NVME_FDP_CONFIG_FDPA_RGIF_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_config_log.2` & `libnvme-1.9/doc/man/nvme_fdp_config_log.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_config_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_config_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_config_log \- FDP Configurations Log Page
 .SH SYNOPSIS
 struct nvme_fdp_config_log {
 .br
 .BI "    __le16 n;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_event.2` & `libnvme-1.9/doc/man/nvme_fdp_event.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_event" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_event" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_event \- FDP Event
 .SH SYNOPSIS
 struct nvme_fdp_event {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_event_realloc.2` & `libnvme-1.9/doc/man/nvme_fdp_event_realloc.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_event_realloc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_event_realloc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_event_realloc \- Media Reallocated Event Type Specific Information
 .SH SYNOPSIS
 struct nvme_fdp_event_realloc {
 .br
 .BI "    __u8 flags;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_event_type.2` & `libnvme-1.9/doc/man/nvme_fdp_event_type.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_event_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_event_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_event_type \- FDP Event Types
 .SH SYNOPSIS
 enum nvme_fdp_event_type {
 .br
 .BI "    NVME_FDP_EVENT_RUNFW"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_reclaim_unit_handle_status.2` & `libnvme-1.9/doc/man/nvme_fdp_reclaim_unit_handle_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fdp_reclaim_unit_handle_status" 9 "nvme_fdp_reclaim_unit_handle_status" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_fdp_reclaim_unit_handle_status" 9 "nvme_fdp_reclaim_unit_handle_status" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_fdp_reclaim_unit_handle_status \- Get reclaim unit handle status
 .SH SYNOPSIS
 .B "int" nvme_fdp_reclaim_unit_handle_status
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 data_len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_reclaim_unit_handle_update.2` & `libnvme-1.9/doc/man/nvme_fdp_reclaim_unit_handle_update.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fdp_reclaim_unit_handle_update" 9 "nvme_fdp_reclaim_unit_handle_update" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_fdp_reclaim_unit_handle_update" 9 "nvme_fdp_reclaim_unit_handle_update" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_fdp_reclaim_unit_handle_update \- Update a list of reclaim unit handles
 .SH SYNOPSIS
 .B "int" nvme_fdp_reclaim_unit_handle_update
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "unsigned int npids "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_ruh_status_desc.2` & `libnvme-1.9/doc/man/nvme_fdp_ruh_status_desc.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fdp_ruh_status_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fdp_ruh_status_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fdp_ruh_status_desc \- Reclaim Unit Handle Status Descriptor
 .SH SYNOPSIS
 struct nvme_fdp_ruh_status_desc {
 .br
 .BI "    __le16 pid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fdp_ruha.2` & `libnvme-1.9/doc/man/nvme_fdp_ruha.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fdp_ruha" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fdp_ruha" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fdp_ruha \- Reclaim Unit Handle Attributes
 .SH SYNOPSIS
 enum nvme_fdp_ruha {
 .br
 .BI "    NVME_FDP_RUHA_HOST_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_feat.2` & `libnvme-1.9/doc/man/nvme_feat.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_feat \- Features Access Shifts/Masks values
 .SH SYNOPSIS
 enum nvme_feat {
 .br
 .BI "    NVME_FEAT_ARBITRATION_BURST_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_feat_host_behavior.2` & `libnvme-1.9/doc/man/nvme_feat_host_behavior.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_feat_host_behavior" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_feat_host_behavior" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_feat_host_behavior \- Host Behavior Support - Data Structure
 .SH SYNOPSIS
 struct nvme_feat_host_behavior {
 .br
 .BI "    __u8 acre;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_feat_nswpcfg_state.2` & `libnvme-1.9/doc/man/nvme_feat_nswpcfg_state.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat_nswpcfg_state" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat_nswpcfg_state" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_feat_nswpcfg_state \- Write Protection - Write Protection State
 .SH SYNOPSIS
 enum nvme_feat_nswpcfg_state {
 .br
 .BI "    NVME_FEAT_NS_NO_WRITE_PROTECT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_feat_resv_notify_flags.2` & `libnvme-1.9/doc/man/nvme_feat_resv_notify_flags.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_feat_resv_notify_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_feat_resv_notify_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_feat_resv_notify_flags \- Reservation Notification Configuration
 .SH SYNOPSIS
 enum nvme_feat_resv_notify_flags {
 .br
 .BI "    NVME_FEAT_RESV_NOTIFY_REGPRE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_features_async_event_config_flags.2` & `libnvme-1.9/doc/man/nvme_features_async_event_config_flags.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_features_async_event_config_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_features_async_event_config_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_features_async_event_config_flags \- Asynchronous Event Configuration configuration flags
 .SH SYNOPSIS
 enum nvme_features_async_event_config_flags {
 .br
 .BI "    NVME_FEATURE_AENCFG_SMART_CRIT_SPARE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_features_id.2` & `libnvme-1.9/doc/man/nvme_features_id.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_features_id" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_features_id" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_features_id \- Features - Feature Identifiers
 .SH SYNOPSIS
 enum nvme_features_id {
 .br
 .BI "    NVME_FEAT_FID_ARBITRATION"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_fid_supported_effects.2` & `libnvme-1.9/doc/man/nvme_fid_supported_effects.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fid_supported_effects" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fid_supported_effects" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fid_supported_effects \- FID Supported and Effects Data Structure definitions
 .SH SYNOPSIS
 enum nvme_fid_supported_effects {
 .br
 .BI "    NVME_FID_SUPPORTED_EFFECTS_FSUPP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_flush.2` & `libnvme-1.9/doc/man/nvme_flush.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_flush" 9 "nvme_flush" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_flush" 9 "nvme_flush" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_flush \- Send an nvme flush command
 .SH SYNOPSIS
 .B "int" nvme_flush
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_format_nvm.2` & `libnvme-1.9/doc/man/nvme_format_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_format_nvm" 9 "nvme_format_nvm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_format_nvm" 9 "nvme_format_nvm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_format_nvm \- Format nvme namespace(s)
 .SH SYNOPSIS
 .B "int" nvme_format_nvm
 .BI "(struct nvme_format_nvm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_format_nvm_compln_event.2` & `libnvme-1.9/doc/man/nvme_format_nvm_compln_event.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_format_nvm_compln_event" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_format_nvm_compln_event" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_format_nvm_compln_event \- Format NVM Completion Event Data
 .SH SYNOPSIS
 struct nvme_format_nvm_compln_event {
 .br
 .BI "    __le32 nsid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fw_commit.2` & `libnvme-1.9/doc/man/nvme_fw_commit.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_commit" 9 "nvme_fw_commit" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_fw_commit" 9 "nvme_fw_commit" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_commit \- Commit firmware using the specified action
 .SH SYNOPSIS
 .B "int" nvme_fw_commit
 .BI "(struct nvme_fw_commit_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_fw_commit_ca.2` & `libnvme-1.9/doc/man/nvme_fw_commit_ca.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_fw_commit_ca" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_fw_commit_ca" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_fw_commit_ca \- Firmware Commit - Commit Action
 .SH SYNOPSIS
 enum nvme_fw_commit_ca {
 .br
 .BI "    NVME_FW_COMMIT_CA_REPLACE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_fw_commit_event.2` & `libnvme-1.9/doc/man/nvme_fw_commit_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_fw_commit_event" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_fw_commit_event" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_fw_commit_event \- Firmware Commit Event Data
 .SH SYNOPSIS
 struct nvme_fw_commit_event {
 .br
 .BI "    __le64 old_fw_rev;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_fw_download.2` & `libnvme-1.9/doc/man/nvme_fw_download.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_download" 9 "nvme_fw_download" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_fw_download" 9 "nvme_fw_download" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_download \- Download part or all of a firmware image to the controller
 .SH SYNOPSIS
 .B "int" nvme_fw_download
 .BI "(struct nvme_fw_download_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_fw_download_seq.2` & `libnvme-1.9/doc/man/nvme_fw_download_seq.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_fw_download_seq" 9 "nvme_fw_download_seq" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_fw_download_seq" 9 "nvme_fw_download_seq" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_fw_download_seq \- Firmware download sequence
 .SH SYNOPSIS
 .B "int" nvme_fw_download_seq
 .BI "(int fd "  ","
 .BI "__u32 size "  ","
 .BI "__u32 xfer "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_gen_dhchap_key.2` & `libnvme-1.9/doc/man/nvme_gen_dhchap_key.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_gen_dhchap_key" 9 "nvme_gen_dhchap_key" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_gen_dhchap_key" 9 "nvme_gen_dhchap_key" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_gen_dhchap_key \- DH-HMAC-CHAP key generation
 .SH SYNOPSIS
 .B "int" nvme_gen_dhchap_key
 .BI "(char *hostnqn "  ","
 .BI "enum nvme_hmac_alg hmac "  ","
 .BI "unsigned int key_len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_generate_tls_key_identity.2` & `libnvme-1.9/doc/man/nvme_generate_tls_key_identity.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_generate_tls_key_identity" 9 "nvme_generate_tls_key_identity" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_generate_tls_key_identity" 9 "nvme_generate_tls_key_identity" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_generate_tls_key_identity \- Generate the TLS key identity
 .SH SYNOPSIS
 .B "char *" nvme_generate_tls_key_identity
 .BI "(const char *hostnqn "  ","
 .BI "const char *subsysnqn "  ","
 .BI "int version "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_ctrl_telemetry.2` & `libnvme-1.9/doc/man/nvme_get_telemetry_log.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-.TH "nvme_get_ctrl_telemetry" 9 "nvme_get_ctrl_telemetry" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_telemetry_log" 9 "nvme_get_telemetry_log" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_ctrl_telemetry \- Get controller telemetry log
+nvme_get_telemetry_log \- Get specified telemetry log
 .SH SYNOPSIS
-.B "int" nvme_get_ctrl_telemetry
+.B "int" nvme_get_telemetry_log
 .BI "(int fd "  ","
+.BI "bool create "  ","
+.BI "bool ctrl "  ","
 .BI "bool rae "  ","
-.BI "struct nvme_telemetry_log **log "  ","
+.BI "size_t max_data_tx "  ","
 .BI "enum nvme_telemetry_da da "  ","
+.BI "struct nvme_telemetry_log **log "  ","
 .BI "size_t *size "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
+.IP "create" 12
+Generate new host initated telemetry capture
+.IP "ctrl" 12
+Get controller Initiated log
 .IP "rae" 12
 Retain asynchronous events
+.IP "max_data_tx" 12
+Set the max data transfer size to be used retrieving telemetry.
+.IP "da" 12
+Log page data area, valid values: \fIenum nvme_telemetry_da\fP.
 .IP "log" 12
 On success, set to the value of the allocated and retrieved log.
-.IP "da" 12
-Log page data area, valid values: \fIenum nvme_telemetry_da\fP
 .IP "size" 12
 Ptr to the telemetry log size, so it can be returned
 .SH "DESCRIPTION"
 The total size allocated can be calculated as:
 (nvme_telemetry_log da size  + 1) * NVME_LOG_TELEM_BLOCK_SIZE.
 .SH "RETURN"
 The nvme command status if a response was received (see
```

### Comparing `libnvme-1.8/doc/man/nvme_get_directive_receive_length.2` & `libnvme-1.9/doc/man/nvme_get_directive_receive_length.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_directive_receive_length" 9 "nvme_get_directive_receive_length" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_directive_receive_length" 9 "nvme_get_directive_receive_length" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_directive_receive_length \- Get directive receive length
 .SH SYNOPSIS
 .B "int" nvme_get_directive_receive_length
 .BI "(enum nvme_directive_dtype dtype "  ","
 .BI "enum nvme_directive_receive_doper doper "  ","
 .BI "__u32 *len "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_discovery_args.2` & `libnvme-1.9/doc/man/nvme_get_discovery_args.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_get_discovery_args" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_get_discovery_args" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_get_discovery_args \- Arguments for nvmf_get_discovery_wargs()
 .SH SYNOPSIS
 struct nvme_get_discovery_args {
 .br
 .BI "    nvme_ctrl_t c;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_get_feature_length.2` & `libnvme-1.9/doc/man/nvme_get_feature_length.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_feature_length" 9 "nvme_get_feature_length" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_feature_length" 9 "nvme_get_feature_length" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_feature_length \- Retreive the command payload length for a specific feature identifier
 .SH SYNOPSIS
 .B "int" nvme_get_feature_length
 .BI "(int fid "  ","
 .BI "__u32 cdw11 "  ","
 .BI "__u32 *len "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_arbitration.2` & `libnvme-1.9/doc/man/nvme_get_features_arbitration.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_arbitration" 9 "nvme_get_features_arbitration" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_arbitration" 9 "nvme_get_features_arbitration" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_arbitration \- Get arbitration feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_arbitration
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_async_event.2` & `libnvme-1.9/doc/man/nvme_get_features_power_mgmt.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_async_event" 9 "nvme_get_features_async_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_power_mgmt" 9 "nvme_get_features_power_mgmt" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_async_event \- Get asynchronous event feature
+nvme_get_features_power_mgmt \- Get power management feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_async_event
+.B "int" nvme_get_features_power_mgmt
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_auto_pst.2` & `libnvme-1.9/doc/man/nvme_get_features_auto_pst.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_auto_pst" 9 "nvme_get_features_auto_pst" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_auto_pst" 9 "nvme_get_features_auto_pst" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_auto_pst \- Get autonomous power state feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_auto_pst
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_feat_auto_pst *apst "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_data.2` & `libnvme-1.9/doc/man/nvme_get_features_data.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_data" 9 "nvme_get_features_data" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_data" 9 "nvme_get_features_data" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_data \- Helper function for @nvme_get_features()
 .SH SYNOPSIS
 .B "int" nvme_get_features_data
 .BI "(int fd "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_endurance_event_cfg.2` & `libnvme-1.9/doc/man/nvme_get_features_endurance_event_cfg.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_endurance_event_cfg" 9 "nvme_get_features_endurance_event_cfg" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_endurance_event_cfg" 9 "nvme_get_features_endurance_event_cfg" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_endurance_event_cfg \- Get endurance event config feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_endurance_event_cfg
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u16 endgid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_err_recovery.2` & `libnvme-1.9/doc/man/nvme_get_features_err_recovery2.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-.TH "nvme_get_features_err_recovery" 9 "nvme_get_features_err_recovery" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_err_recovery2" 9 "nvme_get_features_err_recovery2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_err_recovery \- Get error recovery feature
+nvme_get_features_err_recovery2 \- Get error recovery feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_err_recovery
+.B "int" nvme_get_features_err_recovery2
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
+.BI "__u32 nsid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "nsid" 12
+Namespace ID
 .IP "result" 12
 The command completion result from CQE dword0
-.SH "DESCRIPTION"
-
-Deprecated: doesn't support specifying a NSID.
-Use \fBnvme_get_features_err_recovery2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_err_recovery2.2` & `libnvme-1.9/doc/man/nvme_get_features_resv_persist2.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_err_recovery2" 9 "nvme_get_features_err_recovery2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_persist2" 9 "nvme_get_features_resv_persist2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_err_recovery2 \- Get error recovery feature
+nvme_get_features_resv_persist2 \- Get reservation persist feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_err_recovery2
+.B "int" nvme_get_features_resv_persist2
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_hctm.2` & `libnvme-1.9/doc/man/nvme_get_features_hctm.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_hctm" 9 "nvme_get_features_hctm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_hctm" 9 "nvme_get_features_hctm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_hctm \- Get thermal management feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_hctm
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_host_behavior.2` & `libnvme-1.9/doc/man/nvme_get_features_host_behavior.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_behavior" 9 "nvme_get_features_host_behavior" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_behavior" 9 "nvme_get_features_host_behavior" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_behavior \- Get host behavior feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_behavior
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_feat_host_behavior *data "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_host_id.2` & `libnvme-1.9/doc/man/nvme_get_features_host_id.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_id" 9 "nvme_get_features_host_id" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_id" 9 "nvme_get_features_host_id" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_id \- Get host id feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_id
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "bool exhid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_host_mem_buf.2` & `libnvme-1.9/doc/man/nvme_get_features_host_mem_buf.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_mem_buf" 9 "nvme_get_features_host_mem_buf" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_mem_buf" 9 "nvme_get_features_host_mem_buf" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_mem_buf \- Get host memory buffer feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_mem_buf
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_host_mem_buf2.2` & `libnvme-1.9/doc/man/nvme_get_features_host_mem_buf2.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_host_mem_buf2" 9 "nvme_get_features_host_mem_buf2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_host_mem_buf2" 9 "nvme_get_features_host_mem_buf2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_host_mem_buf2 \- Get host memory buffer feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_host_mem_buf2
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_host_mem_buf_attrs *attrs "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_iocs_profile.2` & `libnvme-1.9/doc/man/nvme_get_features_irq_config.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-.TH "nvme_get_features_iocs_profile" 9 "nvme_get_features_iocs_profile" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_irq_config" 9 "nvme_get_features_irq_config" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_iocs_profile \- Get IOCS profile feature
+nvme_get_features_irq_config \- Get IRQ config feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_iocs_profile
+.B "int" nvme_get_features_irq_config
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
+.BI "__u16 iv "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "iv" 12
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_irq_coalesce.2` & `libnvme-1.9/doc/man/nvme_get_features_kato.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_irq_coalesce" 9 "nvme_get_features_irq_coalesce" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_kato" 9 "nvme_get_features_kato" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_irq_coalesce \- Get IRQ coalesce feature
+nvme_get_features_kato \- Get keep alive timeout feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_irq_coalesce
+.B "int" nvme_get_features_kato
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_irq_config.2` & `libnvme-1.9/doc/man/nvme_get_features_plm_config.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-.TH "nvme_get_features_irq_config" 9 "nvme_get_features_irq_config" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_plm_config" 9 "nvme_get_features_plm_config" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_irq_config \- Get IRQ config feature
+nvme_get_features_plm_config \- Get predictable latency feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_irq_config
+.B "int" nvme_get_features_plm_config
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
-.BI "__u16 iv "  ","
+.BI "__u16 nvmsetid "  ","
+.BI "struct nvme_plm_config *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
-.IP "iv" 12
+.IP "nvmsetid" 12
+NVM set id
+.IP "data" 12
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_kato.2` & `libnvme-1.9/doc/man/nvme_get_features_sanitize.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_kato" 9 "nvme_get_features_kato" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_sanitize" 9 "nvme_get_features_sanitize" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_kato \- Get keep alive timeout feature
+nvme_get_features_sanitize \- Get sanitize feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_kato
+.B "int" nvme_get_features_sanitize
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_lba_range.2` & `libnvme-1.9/doc/man/nvme_get_features_lba_range.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_lba_range" 9 "nvme_get_features_lba_range" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_lba_range" 9 "nvme_get_features_lba_range" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_lba_range \- Get LBA range feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_lba_range
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_lba_range_type *data "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_lba_range2.2` & `libnvme-1.9/doc/man/nvme_get_features_lba_range2.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_lba_range2" 9 "nvme_get_features_lba_range2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_lba_range2" 9 "nvme_get_features_lba_range2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_lba_range2 \- Get LBA range feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_lba_range2
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_lba_sts_interval.2` & `libnvme-1.9/doc/man/nvme_get_features_lba_sts_interval.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_lba_sts_interval" 9 "nvme_get_features_lba_sts_interval" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_lba_sts_interval" 9 "nvme_get_features_lba_sts_interval" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_lba_sts_interval \- Get LBA status information feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_lba_sts_interval
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_nopsc.2` & `libnvme-1.9/doc/man/nvme_get_features_sw_progress.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_nopsc" 9 "nvme_get_features_nopsc" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_sw_progress" 9 "nvme_get_features_sw_progress" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_nopsc \- Get non-operational power state feature
+nvme_get_features_sw_progress \- Get software progress feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_nopsc
+.B "int" nvme_get_features_sw_progress
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_num_queues.2` & `libnvme-1.9/doc/man/nvme_get_features_num_queues.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_num_queues" 9 "nvme_get_features_num_queues" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_num_queues" 9 "nvme_get_features_num_queues" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_num_queues \- Get number of queues feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_num_queues
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_plm_config.2` & `libnvme-1.9/doc/man/nvme_get_features_temp_thresh.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-.TH "nvme_get_features_plm_config" 9 "nvme_get_features_plm_config" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_temp_thresh" 9 "nvme_get_features_temp_thresh" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_plm_config \- Get predictable latency feature
+nvme_get_features_temp_thresh \- Get temperature threshold feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_plm_config
+.B "int" nvme_get_features_temp_thresh
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
-.BI "__u16 nvmsetid "  ","
-.BI "struct nvme_plm_config *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
-.IP "nvmsetid" 12
-NVM set id
-.IP "data" 12
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_plm_window.2` & `libnvme-1.9/doc/man/nvme_set_features_plm_window.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-.TH "nvme_get_features_plm_window" 9 "nvme_get_features_plm_window" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_plm_window" 9 "nvme_set_features_plm_window" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_plm_window \- Get window select feature
+nvme_set_features_plm_window \- Set window select feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_plm_window
+.B "int" nvme_set_features_plm_window
 .BI "(int fd "  ","
-.BI "enum nvme_get_features_sel sel "  ","
+.BI "enum nvme_feat_plm_window_select sel "  ","
 .BI "__u16 nvmsetid "  ","
+.BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
-Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+Window Select
 .IP "nvmsetid" 12
-NVM set id
+NVM Set Identifier
+.IP "save" 12
+Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_power_mgmt.2` & `libnvme-1.9/doc/man/nvme_get_features_resv_mask.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-.TH "nvme_get_features_power_mgmt" 9 "nvme_get_features_power_mgmt" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_mask" 9 "nvme_get_features_resv_mask" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_power_mgmt \- Get power management feature
+nvme_get_features_resv_mask \- Get reservation mask feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_power_mgmt
+.B "int" nvme_get_features_resv_mask
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
 .IP "result" 12
 The command completion result from CQE dword0
+.SH "DESCRIPTION"
+
+Deprecated: doesn't support specifying a NSID.
+Use \fBnvme_get_features_resv_mask2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_resv_mask.2` & `libnvme-1.9/doc/man/nvme_get_features_resv_mask2.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-.TH "nvme_get_features_resv_mask" 9 "nvme_get_features_resv_mask" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_mask2" 9 "nvme_get_features_resv_mask2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_resv_mask \- Get reservation mask feature
+nvme_get_features_resv_mask2 \- Get reservation mask feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_resv_mask
+.B "int" nvme_get_features_resv_mask2
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
+.BI "__u32 nsid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "nsid" 12
+Namespace ID
 .IP "result" 12
 The command completion result from CQE dword0
-.SH "DESCRIPTION"
-
-Deprecated: doesn't support specifying a NSID.
-Use \fBnvme_get_features_resv_mask2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_resv_mask2.2` & `libnvme-1.9/doc/man/nvme_get_features_plm_window.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-.TH "nvme_get_features_resv_mask2" 9 "nvme_get_features_resv_mask2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_plm_window" 9 "nvme_get_features_plm_window" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_resv_mask2 \- Get reservation mask feature
+nvme_get_features_plm_window \- Get window select feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_resv_mask2
+.B "int" nvme_get_features_plm_window
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
-.BI "__u32 nsid "  ","
+.BI "__u16 nvmsetid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
-.IP "nsid" 12
-Namespace ID
+.IP "nvmsetid" 12
+NVM set id
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_resv_persist.2` & `libnvme-1.9/doc/man/nvme_get_features_resv_persist.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_resv_persist" 9 "nvme_get_features_resv_persist" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_resv_persist" 9 "nvme_get_features_resv_persist" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_resv_persist \- Get reservation persist feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_resv_persist
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_resv_persist2.2` & `libnvme-1.9/doc/man/nvme_get_features_write_atomic.2`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-.TH "nvme_get_features_resv_persist2" 9 "nvme_get_features_resv_persist2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_write_atomic" 9 "nvme_get_features_write_atomic" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_resv_persist2 \- Get reservation persist feature
+nvme_get_features_write_atomic \- Get write atomic feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_resv_persist2
+.B "int" nvme_get_features_write_atomic
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
-.BI "__u32 nsid "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
-.IP "nsid" 12
-Namespace ID
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_rrl.2` & `libnvme-1.9/doc/man/nvme_get_features_rrl.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_rrl" 9 "nvme_get_features_rrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_rrl" 9 "nvme_get_features_rrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_rrl \- Get read recovery level feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_rrl
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_sanitize.2` & `libnvme-1.9/doc/man/nvme_get_features_nopsc.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_sanitize" 9 "nvme_get_features_sanitize" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_nopsc" 9 "nvme_get_features_nopsc" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_sanitize \- Get sanitize feature
+nvme_get_features_nopsc \- Get non-operational power state feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_sanitize
+.B "int" nvme_get_features_nopsc
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_sel.2` & `libnvme-1.9/doc/man/nvme_get_features_sel.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_get_features_sel" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_get_features_sel" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_get_features_sel \- Get Features - Select
 .SH SYNOPSIS
 enum nvme_get_features_sel {
 .br
 .BI "    NVME_GET_FEATURES_SEL_CURRENT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_simple.2` & `libnvme-1.9/doc/man/nvme_get_features_simple.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_simple" 9 "nvme_get_features_simple" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_simple" 9 "nvme_get_features_simple" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_simple \- Helper function for @nvme_get_features()
 .SH SYNOPSIS
 .B "int" nvme_get_features_simple
 .BI "(int fd "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_sw_progress.2` & `libnvme-1.9/doc/man/nvme_get_features_volatile_wc.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_sw_progress" 9 "nvme_get_features_sw_progress" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_volatile_wc" 9 "nvme_get_features_volatile_wc" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_sw_progress \- Get software progress feature
+nvme_get_features_volatile_wc \- Get volatile write cache feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_sw_progress
+.B "int" nvme_get_features_volatile_wc
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_temp_thresh.2` & `libnvme-1.9/doc/man/nvme_get_features_irq_coalesce.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_get_features_temp_thresh" 9 "nvme_get_features_temp_thresh" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_irq_coalesce" 9 "nvme_get_features_irq_coalesce" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_temp_thresh \- Get temperature threshold feature
+nvme_get_features_irq_coalesce \- Get IRQ coalesce feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_temp_thresh
+.B "int" nvme_get_features_irq_coalesce
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "sel" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_timestamp.2` & `libnvme-1.9/doc/man/nvme_get_features_timestamp.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_features_timestamp" 9 "nvme_get_features_timestamp" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_timestamp" 9 "nvme_get_features_timestamp" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_features_timestamp \- Get timestamp feature
 .SH SYNOPSIS
 .B "int" nvme_get_features_timestamp
 .BI "(int fd "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "struct nvme_timestamp *ts "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_write_atomic.2` & `libnvme-1.9/doc/man/nvme_get_features_write_protect.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-.TH "nvme_get_features_write_atomic" 9 "nvme_get_features_write_atomic" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_features_write_protect" 9 "nvme_get_features_write_protect" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_write_atomic \- Get write atomic feature
+nvme_get_features_write_protect \- Get write protect feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_write_atomic
+.B "int" nvme_get_features_write_protect
 .BI "(int fd "  ","
+.BI "__u32 nsid "  ","
 .BI "enum nvme_get_features_sel sel "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
+.IP "nsid" 12
+Namespace ID
 .IP "sel" 12
 Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_features_write_protect.2` & `libnvme-1.9/doc/man/nvme_set_features_write_atomic.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-.TH "nvme_get_features_write_protect" 9 "nvme_get_features_write_protect" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_write_atomic" 9 "nvme_set_features_write_atomic" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_features_write_protect \- Get write protect feature
+nvme_set_features_write_atomic \- Set write atomic feature
 .SH SYNOPSIS
-.B "int" nvme_get_features_write_protect
+.B "int" nvme_set_features_write_atomic
 .BI "(int fd "  ","
-.BI "__u32 nsid "  ","
-.BI "enum nvme_get_features_sel sel "  ","
+.BI "bool dn "  ","
+.BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "nsid" 12
-Namespace ID
-.IP "sel" 12
-Select which type of attribute to return, see \fIenum nvme_get_features_sel\fP
+.IP "dn" 12
+Disable Normal
+.IP "save" 12
+Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_host_telemetry.2` & `libnvme-1.9/doc/man/nvme_get_host_telemetry.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_host_telemetry" 9 "nvme_get_host_telemetry" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_host_telemetry" 9 "nvme_get_host_telemetry" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_host_telemetry \- Get host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_host_telemetry
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log **log "  ","
 .BI "enum nvme_telemetry_da da "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_lba_status.2` & `libnvme-1.9/doc/man/nvme_get_lba_status.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_lba_status" 9 "nvme_get_lba_status" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_lba_status" 9 "nvme_get_lba_status" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_lba_status \- Retrieve information on possibly unrecoverable LBAs
 .SH SYNOPSIS
 .B "int" nvme_get_lba_status
 .BI "(struct nvme_get_lba_status_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_lba_status_log.2` & `libnvme-1.9/doc/man/nvme_get_lba_status_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_lba_status_log" 9 "nvme_get_lba_status_log" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_lba_status_log" 9 "nvme_get_lba_status_log" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_lba_status_log \- Retrieve the LBA Status log page
 .SH SYNOPSIS
 .B "int" nvme_get_lba_status_log
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_lba_status_log **log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_ana.2` & `libnvme-1.9/doc/man/nvme_get_log_ana.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_ana" 9 "nvme_get_log_ana" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_ana" 9 "nvme_get_log_ana" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_ana \- Retrieve Asymmetric Namespace Access log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_ana
 .BI "(int fd "  ","
 .BI "enum nvme_log_ana_lsp lsp "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_ana_groups.2` & `libnvme-1.9/doc/man/nvme_get_log_ana_groups.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_ana_groups" 9 "nvme_get_log_ana_groups" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_ana_groups" 9 "nvme_get_log_ana_groups" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_ana_groups \- Retrieve Asymmetric Namespace Access groups only log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_ana_groups
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_boot_partition.2` & `libnvme-1.9/doc/man/nvme_get_log_boot_partition.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_boot_partition" 9 "nvme_get_log_boot_partition" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_boot_partition" 9 "nvme_get_log_boot_partition" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_boot_partition \- Retrieve Boot Partition
 .SH SYNOPSIS
 .B "int" nvme_get_log_boot_partition
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u8 lsp "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_changed_ns_list.2` & `libnvme-1.9/doc/man/nvme_get_log_changed_ns_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_changed_ns_list" 9 "nvme_get_log_changed_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_changed_ns_list" 9 "nvme_get_log_changed_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_changed_ns_list \- Retrieve namespace changed list
 .SH SYNOPSIS
 .B "int" nvme_get_log_changed_ns_list
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_ns_list *ns_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_cmd_effects.2` & `libnvme-1.9/doc/man/nvme_get_log_cmd_effects.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_cmd_effects" 9 "nvme_get_log_cmd_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_cmd_effects" 9 "nvme_get_log_cmd_effects" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_cmd_effects \- Retrieve nvme command effects log
 .SH SYNOPSIS
 .B "int" nvme_get_log_cmd_effects
 .BI "(int fd "  ","
 .BI "enum nvme_csi csi "  ","
 .BI "struct nvme_cmd_effects_log *effects_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_create_telemetry_host.2` & `libnvme-1.9/doc/man/nvme_get_log_create_telemetry_host.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_create_telemetry_host" 9 "nvme_get_log_create_telemetry_host" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_create_telemetry_host" 9 "nvme_get_log_create_telemetry_host" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_create_telemetry_host \- Create host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_log_create_telemetry_host
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_device_self_test.2` & `libnvme-1.9/doc/man/nvme_get_log_device_self_test.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_device_self_test" 9 "nvme_get_log_device_self_test" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_device_self_test" 9 "nvme_get_log_device_self_test" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_device_self_test \- Retrieve the device self test log
 .SH SYNOPSIS
 .B "int" nvme_get_log_device_self_test
 .BI "(int fd "  ","
 .BI "struct nvme_self_test_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_discovery.2` & `libnvme-1.9/doc/man/nvme_get_log_discovery.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_discovery" 9 "nvme_get_log_discovery" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_discovery" 9 "nvme_get_log_discovery" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_discovery \- Retrieve Discovery log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_discovery
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_endurance_group.2` & `libnvme-1.9/doc/man/nvme_get_log_endurance_group.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_endurance_group" 9 "nvme_get_log_endurance_group" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_endurance_group" 9 "nvme_get_log_endurance_group" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_endurance_group \- Get Endurance Group log
 .SH SYNOPSIS
 .B "int" nvme_get_log_endurance_group
 .BI "(int fd "  ","
 .BI "__u16 endgid "  ","
 .BI "struct nvme_endurance_group_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_endurance_grp_evt.2` & `libnvme-1.9/doc/man/nvme_get_log_predictable_lat_event.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_get_log_endurance_grp_evt" 9 "nvme_get_log_endurance_grp_evt" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_predictable_lat_event" 9 "nvme_get_log_predictable_lat_event" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_endurance_grp_evt \- Retrieve Rotational Media Information
+nvme_get_log_predictable_lat_event \- Retrieve Predictable Latency Event Aggregate Log Page
 .SH SYNOPSIS
-.B "int" nvme_get_log_endurance_grp_evt
+.B "int" nvme_get_log_predictable_lat_event
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
 .BI "__u32 len "  ","
 .BI "void *log "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "rae" 12
 Retain asynchronous events
 .IP "offset" 12
-Offset to the start of the log page
+Offset into the predictable latency event
 .IP "len" 12
-The allocated length of the log page
+Length of provided user buffer to hold the log data in bytes
 .IP "log" 12
-User address to store the log page
+User address for log page data
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_error.2` & `libnvme-1.9/doc/man/nvme_get_log_error.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_error" 9 "nvme_get_log_error" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_error" 9 "nvme_get_log_error" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_error \- Retrieve nvme error log
 .SH SYNOPSIS
 .B "int" nvme_get_log_error
 .BI "(int fd "  ","
 .BI "unsigned int nr_entries "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_fdp_events.2` & `libnvme-1.9/doc/man/nvme_get_log_fdp_events.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fdp_events" 9 "nvme_get_log_fdp_events" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_fdp_events" 9 "nvme_get_log_fdp_events" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fdp_events \- Get Flexible Data Placement events
 .SH SYNOPSIS
 .B "int" nvme_get_log_fdp_events
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "bool host_events "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_fdp_stats.2` & `libnvme-1.9/doc/man/nvme_get_log_fdp_stats.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fdp_stats" 9 "nvme_get_log_fdp_stats" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_fdp_stats" 9 "nvme_get_log_fdp_stats" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fdp_stats \- Get Flexible Data Placement statistics
 .SH SYNOPSIS
 .B "int" nvme_get_log_fdp_stats
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_fid_supported_effects.2` & `libnvme-1.9/doc/man/nvme_get_log_fid_supported_effects.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fid_supported_effects" 9 "nvme_get_log_fid_supported_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_fid_supported_effects" 9 "nvme_get_log_fid_supported_effects" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fid_supported_effects \- Retrieve Feature Identifiers Supported and Effects
 .SH SYNOPSIS
 .B "int" nvme_get_log_fid_supported_effects
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_fid_supported_effects_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_fw_slot.2` & `libnvme-1.9/doc/man/nvme_get_log_fw_slot.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_fw_slot" 9 "nvme_get_log_fw_slot" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_fw_slot" 9 "nvme_get_log_fw_slot" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_fw_slot \- Retrieves the controller firmware log
 .SH SYNOPSIS
 .B "int" nvme_get_log_fw_slot
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_firmware_slot *fw_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_lba_status.2` & `libnvme-1.9/doc/man/nvme_get_log_lba_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_lba_status" 9 "nvme_get_log_lba_status" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_lba_status" 9 "nvme_get_log_lba_status" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_lba_status \- Retrieve LBA Status
 .SH SYNOPSIS
 .B "int" nvme_get_log_lba_status
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_media_unit_stat.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_media_unit_stat.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH "nvme_get_log_media_unit_stat" 9 "nvme_get_log_media_unit_stat" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_media_unit_stat" 9 "nvme_mi_admin_get_log_media_unit_stat" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_media_unit_stat \- Retrieve Media Unit Status
+nvme_mi_admin_get_log_media_unit_stat \- Retrieve Media Unit Status
 .SH SYNOPSIS
-.B "int" nvme_get_log_media_unit_stat
-.BI "(int fd "  ","
+.B "int" nvme_mi_admin_get_log_media_unit_stat
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_media_unit_stat_log *mus "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
+.IP "ctrl" 12
+Controller to query
 .IP "domid" 12
 Domain Identifier selection, if supported
 .IP "mus" 12
 User address to store the Media Unit statistics log
 .SH "RETURN"
 The nvme command status if a response was received (see
-\fIenum nvme_status_field\fP) or -1 with errno set otherwise
+\fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_mi_cmd_supported_effects.2` & `libnvme-1.9/doc/man/nvme_get_log_mi_cmd_supported_effects.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_mi_cmd_supported_effects" 9 "nvme_get_log_mi_cmd_supported_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_mi_cmd_supported_effects" 9 "nvme_get_log_mi_cmd_supported_effects" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_mi_cmd_supported_effects \- displays the MI Commands Supported by the controller
 .SH SYNOPSIS
 .B "int" nvme_get_log_mi_cmd_supported_effects
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_mi_cmd_supported_effects_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_page.2` & `libnvme-1.9/doc/man/nvme_get_log_page.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_page" 9 "nvme_get_log_page" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_page" 9 "nvme_get_log_page" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_page \- Get log page data
 .SH SYNOPSIS
 .B "int" nvme_get_log_page
 .BI "(int fd "  ","
 .BI "__u32 xfer_len "  ","
 .BI "struct nvme_get_log_args *args "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_persistent_event.2` & `libnvme-1.9/doc/man/nvme_get_log_persistent_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_persistent_event" 9 "nvme_get_log_persistent_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_persistent_event" 9 "nvme_get_log_persistent_event" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_persistent_event \- Retrieve Persistent Event Log
 .SH SYNOPSIS
 .B "int" nvme_get_log_persistent_event
 .BI "(int fd "  ","
 .BI "enum nvme_pevent_log_action action "  ","
 .BI "__u32 size "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_phy_rx_eom.2` & `libnvme-1.9/doc/man/nvme_get_log_phy_rx_eom.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_phy_rx_eom" 9 "nvme_get_log_phy_rx_eom" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_phy_rx_eom" 9 "nvme_get_log_phy_rx_eom" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_phy_rx_eom \- Retrieve Physical Interface Receiver Eye Opening Measurement Log
 .SH SYNOPSIS
 .B "int" nvme_get_log_phy_rx_eom
 .BI "(int fd "  ","
 .BI "__u8 lsp "  ","
 .BI "__u16 controller "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_predictable_lat_event.2` & `libnvme-1.9/doc/man/nvme_get_log_predictable_lat_nvmset.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-.TH "nvme_get_log_predictable_lat_event" 9 "nvme_get_log_predictable_lat_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_predictable_lat_nvmset" 9 "nvme_get_log_predictable_lat_nvmset" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_predictable_lat_event \- Retrieve Predictable Latency Event Aggregate Log Page
+nvme_get_log_predictable_lat_nvmset \- Predictable Latency Per NVM Set
 .SH SYNOPSIS
-.B "int" nvme_get_log_predictable_lat_event
+.B "int" nvme_get_log_predictable_lat_nvmset
 .BI "(int fd "  ","
-.BI "bool rae "  ","
-.BI "__u32 offset "  ","
-.BI "__u32 len "  ","
-.BI "void *log "  ");"
+.BI "__u16 nvmsetid "  ","
+.BI "struct nvme_nvmset_predictable_lat_log *log "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "rae" 12
-Retain asynchronous events
-.IP "offset" 12
-Offset into the predictable latency event
-.IP "len" 12
-Length of provided user buffer to hold the log data in bytes
+.IP "nvmsetid" 12
+NVM set id
 .IP "log" 12
-User address for log page data
+User address to store the predictable latency log
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_predictable_lat_nvmset.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_predictable_lat_nvmset.2`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH "nvme_get_log_predictable_lat_nvmset" 9 "nvme_get_log_predictable_lat_nvmset" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_predictable_lat_nvmset" 9 "nvme_mi_admin_get_log_predictable_lat_nvmset" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_log_predictable_lat_nvmset \- Predictable Latency Per NVM Set
+nvme_mi_admin_get_log_predictable_lat_nvmset \- Predictable Latency Per NVM Set
 .SH SYNOPSIS
-.B "int" nvme_get_log_predictable_lat_nvmset
-.BI "(int fd "  ","
+.B "int" nvme_mi_admin_get_log_predictable_lat_nvmset
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 nvmsetid "  ","
 .BI "struct nvme_nvmset_predictable_lat_log *log "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
+.IP "ctrl" 12
+Controller to query
 .IP "nvmsetid" 12
 NVM set id
 .IP "log" 12
 User address to store the predictable latency log
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_reclaim_unit_handle_usage.2` & `libnvme-1.9/doc/man/nvme_get_log_reclaim_unit_handle_usage.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_reclaim_unit_handle_usage" 9 "nvme_get_log_reclaim_unit_handle_usage" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_reclaim_unit_handle_usage" 9 "nvme_get_log_reclaim_unit_handle_usage" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_reclaim_unit_handle_usage \- Get reclaim unit handle usage
 .SH SYNOPSIS
 .B "int" nvme_get_log_reclaim_unit_handle_usage
 .BI "(int fd "  ","
 .BI "__u16 egid "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_reservation.2` & `libnvme-1.9/doc/man/nvme_get_log_reservation.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_reservation" 9 "nvme_get_log_reservation" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_reservation" 9 "nvme_get_log_reservation" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_reservation \- Retrieve Reservation Notification
 .SH SYNOPSIS
 .B "int" nvme_get_log_reservation
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_resv_notification_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_sanitize.2` & `libnvme-1.9/doc/man/nvme_get_log_sanitize.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_sanitize" 9 "nvme_get_log_sanitize" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_sanitize" 9 "nvme_get_log_sanitize" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_sanitize \- Retrieve Sanitize Status
 .SH SYNOPSIS
 .B "int" nvme_get_log_sanitize
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_sanitize_log_page *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_smart.2` & `libnvme-1.9/doc/man/nvme_get_log_smart.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_smart" 9 "nvme_get_log_smart" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_smart" 9 "nvme_get_log_smart" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_smart \- Retrieve nvme smart log
 .SH SYNOPSIS
 .B "int" nvme_get_log_smart
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_support_cap_config_list.2` & `libnvme-1.9/doc/man/nvme_get_log_support_cap_config_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_support_cap_config_list" 9 "nvme_get_log_support_cap_config_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_support_cap_config_list" 9 "nvme_get_log_support_cap_config_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_support_cap_config_list \- Retrieve Supported Capacity Configuration List
 .SH SYNOPSIS
 .B "int" nvme_get_log_support_cap_config_list
 .BI "(int fd "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_supported_cap_config_list_log *cap "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_supported_log_pages.2` & `libnvme-1.9/doc/man/nvme_get_log_supported_log_pages.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_supported_log_pages" 9 "nvme_get_log_supported_log_pages" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_supported_log_pages" 9 "nvme_get_log_supported_log_pages" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_supported_log_pages \- Retrieve nmve supported log pages
 .SH SYNOPSIS
 .B "int" nvme_get_log_supported_log_pages
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_supported_log_pages *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_telemetry_ctrl.2` & `libnvme-1.9/doc/man/nvme_get_log_telemetry_ctrl.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_telemetry_ctrl" 9 "nvme_get_log_telemetry_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_telemetry_ctrl" 9 "nvme_get_log_telemetry_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_telemetry_ctrl \- Get Telemetry Controller-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_telemetry_ctrl
 .BI "(int fd "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_telemetry_host.2` & `libnvme-1.9/doc/man/nvme_get_log_telemetry_host.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_telemetry_host" 9 "nvme_get_log_telemetry_host" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_telemetry_host" 9 "nvme_get_log_telemetry_host" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_telemetry_host \- Get Telemetry Host-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_get_log_telemetry_host
 .BI "(int fd "  ","
 .BI "__u64 offset "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_log_zns_changed_zones.2` & `libnvme-1.9/doc/man/nvme_get_log_zns_changed_zones.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_log_zns_changed_zones" 9 "nvme_get_log_zns_changed_zones" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_log_zns_changed_zones" 9 "nvme_get_log_zns_changed_zones" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_log_zns_changed_zones \- Retrieve list of zones that have changed
 .SH SYNOPSIS
 .B "int" nvme_get_log_zns_changed_zones
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_logical_block_size.2` & `libnvme-1.9/doc/man/nvme_get_logical_block_size.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_logical_block_size" 9 "nvme_get_logical_block_size" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_logical_block_size" 9 "nvme_get_logical_block_size" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_logical_block_size \- Retrieve block size
 .SH SYNOPSIS
 .B "int" nvme_get_logical_block_size
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "int *blksize "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_get_new_host_telemetry.2` & `libnvme-1.9/doc/man/nvme_get_new_host_telemetry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_new_host_telemetry" 9 "nvme_get_new_host_telemetry" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_new_host_telemetry" 9 "nvme_get_new_host_telemetry" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_new_host_telemetry \- Get new host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_get_new_host_telemetry
 .BI "(int fd "  ","
 .BI "struct nvme_telemetry_log **log "  ","
 .BI "enum nvme_telemetry_da da "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_get_nsid.2` & `libnvme-1.9/doc/man/nvme_get_nsid.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_nsid" 9 "nvme_get_nsid" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_nsid" 9 "nvme_get_nsid" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_nsid \- Retrieve the NSID from a namespace file descriptor
 .SH SYNOPSIS
 .B "int" nvme_get_nsid
 .BI "(int fd "  ","
 .BI "__u32 *nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_get_property.2` & `libnvme-1.9/doc/man/nvme_get_property.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_property" 9 "nvme_get_property" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_property" 9 "nvme_get_property" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_property \- Get a controller property
 .SH SYNOPSIS
 .B "int" nvme_get_property
 .BI "(struct nvme_get_property_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_get_telemetry_log.2` & `libnvme-1.9/doc/man/nvme_get_ctrl_telemetry.2`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-.TH "nvme_get_telemetry_log" 9 "nvme_get_telemetry_log" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_ctrl_telemetry" 9 "nvme_get_ctrl_telemetry" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_get_telemetry_log \- Get specified telemetry log
+nvme_get_ctrl_telemetry \- Get controller telemetry log
 .SH SYNOPSIS
-.B "int" nvme_get_telemetry_log
+.B "int" nvme_get_ctrl_telemetry
 .BI "(int fd "  ","
-.BI "bool create "  ","
-.BI "bool ctrl "  ","
 .BI "bool rae "  ","
-.BI "size_t max_data_tx "  ","
-.BI "enum nvme_telemetry_da da "  ","
 .BI "struct nvme_telemetry_log **log "  ","
+.BI "enum nvme_telemetry_da da "  ","
 .BI "size_t *size "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "create" 12
-Generate new host initated telemetry capture
-.IP "ctrl" 12
-Get controller Initiated log
 .IP "rae" 12
 Retain asynchronous events
-.IP "max_data_tx" 12
-Set the max data transfer size to be used retrieving telemetry.
-.IP "da" 12
-Log page data area, valid values: \fIenum nvme_telemetry_da\fP.
 .IP "log" 12
 On success, set to the value of the allocated and retrieved log.
+.IP "da" 12
+Log page data area, valid values: \fIenum nvme_telemetry_da\fP
 .IP "size" 12
 Ptr to the telemetry log size, so it can be returned
 .SH "DESCRIPTION"
 The total size allocated can be calculated as:
 (nvme_telemetry_log da size  + 1) * NVME_LOG_TELEM_BLOCK_SIZE.
 .SH "RETURN"
 The nvme command status if a response was received (see
```

### Comparing `libnvme-1.8/doc/man/nvme_get_telemetry_max.2` & `libnvme-1.9/doc/man/nvme_get_telemetry_max.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_get_telemetry_max" 9 "nvme_get_telemetry_max" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_get_telemetry_max" 9 "nvme_get_telemetry_max" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_get_telemetry_max \- Get telemetry limits
 .SH SYNOPSIS
 .B "int" nvme_get_telemetry_max
 .BI "(int fd "  ","
 .BI "enum nvme_telemetry_da *da "  ","
 .BI "size_t *max_data_tx "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_host_is_pdc_enabled.2` & `libnvme-1.9/doc/man/nvme_host_is_pdc_enabled.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_host_is_pdc_enabled" 9 "nvme_host_is_pdc_enabled" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_host_is_pdc_enabled" 9 "nvme_host_is_pdc_enabled" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_host_is_pdc_enabled \- Is Persistenct Discovery Controller enabled
 .SH SYNOPSIS
 .B "bool" nvme_host_is_pdc_enabled
 .BI "(nvme_host_t h "  ","
 .BI "bool fallback "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_host_mem_buf_attrs.2` & `libnvme-1.9/doc/man/nvme_host_mem_buf_attrs.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_host_mem_buf_attrs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_host_mem_buf_attrs" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_host_mem_buf_attrs \- Host Memory Buffer - Attributes Data Structure
 .SH SYNOPSIS
 struct nvme_host_mem_buf_attrs {
 .br
 .BI "    __le32 hsize;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_host_metadata.2` & `libnvme-1.9/doc/man/nvme_host_metadata.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_host_metadata" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_host_metadata" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_host_metadata \- Host Metadata Data Structure
 .SH SYNOPSIS
 struct nvme_host_metadata {
 .br
 .BI "    __u8 ndesc;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_host_set_pdc_enabled.2` & `libnvme-1.9/doc/man/nvme_host_set_pdc_enabled.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_host_set_pdc_enabled" 9 "nvme_host_set_pdc_enabled" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_host_set_pdc_enabled" 9 "nvme_host_set_pdc_enabled" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_host_set_pdc_enabled \- Set Persistent Discovery Controller flag
 .SH SYNOPSIS
 .B "void" nvme_host_set_pdc_enabled
 .BI "(nvme_host_t h "  ","
 .BI "bool enabled "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl.2` & `libnvme-1.9/doc/man/nvme_id_ctrl.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ctrl" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ctrl" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ctrl \- Identify Controller data structure
 .SH SYNOPSIS
 struct nvme_id_ctrl {
 .br
 .BI "    __le16 vid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_anacap.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_anacap.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_anacap" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_anacap" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_anacap \- This field indicates the capabilities associated with Asymmetric Namespace Access Reporting.
 .SH SYNOPSIS
 enum nvme_id_ctrl_anacap {
 .br
 .BI "    NVME_CTRL_ANACAP_OPT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_cmic.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_cmic.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_cmic" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_cmic" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_cmic \- Controller Multipath IO and Namespace Sharing Capabilities of the controller and NVM subsystem.
 .SH SYNOPSIS
 enum nvme_id_ctrl_cmic {
 .br
 .BI "    NVME_CTRL_CMIC_MULTI_PORT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_cqes.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_cqes.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_cqes" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_cqes" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_cqes \- Defines the required and maximum Completion Queue entry size when using the NVM Command Set.
 .SH SYNOPSIS
 enum nvme_id_ctrl_cqes {
 .br
 .BI "    NVME_CTRL_CQES_MIN"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_ctratt.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_ctratt.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_ctratt" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_ctratt" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_ctratt \- Controller attributes
 .SH SYNOPSIS
 enum nvme_id_ctrl_ctratt {
 .br
 .BI "    NVME_CTRL_CTRATT_128_ID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_dctype.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_dctype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_dctype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_dctype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_dctype \- Discovery Controller types
 .SH SYNOPSIS
 enum nvme_id_ctrl_dctype {
 .br
 .BI "    NVME_CTRL_DCTYPE_NOT_REPORTED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_fna.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_fna.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_fna" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_fna" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_fna \- This field indicates attributes for the Format NVM command.
 .SH SYNOPSIS
 enum nvme_id_ctrl_fna {
 .br
 .BI "    NVME_CTRL_FNA_FMT_ALL_NAMESPACES"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_frmw.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_frmw.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_frmw" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_frmw" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_frmw \- Flags and values indicates capabilities regarding firmware updates from &struct nvme_id_ctrl.frmw.
 .SH SYNOPSIS
 enum nvme_id_ctrl_frmw {
 .br
 .BI "    NVME_CTRL_FRMW_1ST_RO"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_lpa.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_lpa.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_lpa" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_lpa" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_lpa \- Flags indicating optional attributes for log pages that are accessed via the Get Log Page command.
 .SH SYNOPSIS
 enum nvme_id_ctrl_lpa {
 .br
 .BI "    NVME_CTRL_LPA_SMART_PER_NS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_mec.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_mec.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_mec" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_mec" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_mec \- Flags indicating the capabilities of the Management Endpoint in the Controller, &struct nvme_id_ctrl.mec.
 .SH SYNOPSIS
 enum nvme_id_ctrl_mec {
 .br
 .BI "    NVME_CTRL_MEC_SMBUSME"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_nvm.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ctrl_nvm" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ctrl_nvm" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ctrl_nvm \- I/O Command Set Specific Identify Controller data structure
 .SH SYNOPSIS
 struct nvme_id_ctrl_nvm {
 .br
 .BI "    __u8 vsl;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_nvmsr.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_nvmsr.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_nvmsr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_nvmsr" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_nvmsr \- This field reports information associated with the NVM Subsystem, see &struct nvme_id_ctrl.nvmsr.
 .SH SYNOPSIS
 enum nvme_id_ctrl_nvmsr {
 .br
 .BI "    NVME_CTRL_NVMSR_NVMESD"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_nwpc.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_nwpc.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_nwpc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_nwpc" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_nwpc \- This field indicates the optional namespace write protection capabilities supported by the controller.
 .SH SYNOPSIS
 enum nvme_id_ctrl_nwpc {
 .br
 .BI "    NVME_CTRL_NWPC_WRITE_PROTECT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_oacs.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_oacs.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oacs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oacs" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oacs \- Flags indicating the optional Admin commands and features supported by the controller, see &struct nvme_id_ctrl.oacs.
 .SH SYNOPSIS
 enum nvme_id_ctrl_oacs {
 .br
 .BI "    NVME_CTRL_OACS_SECURITY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_oaes.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_oaes.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oaes" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oaes" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oaes \- Optional Asynchronous Events Supported
 .SH SYNOPSIS
 enum nvme_id_ctrl_oaes {
 .br
 .BI "    NVME_CTRL_OAES_NA"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_oncs.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_oncs.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_oncs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_oncs" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_oncs \- This field indicates the optional NVM commands and features supported by the controller.
 .SH SYNOPSIS
 enum nvme_id_ctrl_oncs {
 .br
 .BI "    NVME_CTRL_ONCS_COMPARE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_rpmbs.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_rpmbs.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_rpmbs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_rpmbs" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_rpmbs \- This field indicates if the controller supports one or more Replay Protected Memory Blocks, from &struct nvme_id_ctrl.rpmbs.
 .SH SYNOPSIS
 enum nvme_id_ctrl_rpmbs {
 .br
 .BI "    NVME_CTRL_RPMBS_NR_UNITS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_sanicap.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_sanicap.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sanicap" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sanicap" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sanicap \- Indicates attributes for sanitize operations.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sanicap {
 .br
 .BI "    NVME_CTRL_SANICAP_CES"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_sgls.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_sgls.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sgls" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sgls" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sgls \- This field indicates if SGLs are supported for the NVM Command Set and the particular SGL types supported.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sgls {
 .br
 .BI "    NVME_CTRL_SGLS_SUPPORTED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_sqes.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_sqes.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_sqes" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_sqes" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_sqes \- Defines the required and maximum Submission Queue entry size when using the NVM Command Set.
 .SH SYNOPSIS
 enum nvme_id_ctrl_sqes {
 .br
 .BI "    NVME_CTRL_SQES_MIN"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_vwc.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_vwc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_vwc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_vwc" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_vwc \- Volatile write cache
 .SH SYNOPSIS
 enum nvme_id_ctrl_vwc {
 .br
 .BI "    NVME_CTRL_VWC_PRESENT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ctrl_vwci.2` & `libnvme-1.9/doc/man/nvme_id_ctrl_vwci.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ctrl_vwci" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ctrl_vwci" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ctrl_vwci \- This field indicates information about remaining number of times that VPD contents are able to be updated using the VPD Write command, see &struct nvme_id_ctrl.vwci.
 .SH SYNOPSIS
 enum nvme_id_ctrl_vwci {
 .br
 .BI "    NVME_CTRL_VWCI_VWCR"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_domain_attr.2` & `libnvme-1.9/doc/man/nvme_id_domain_attr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_domain_attr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_domain_attr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_domain_attr \- Domain Attributes Entry
 .SH SYNOPSIS
 struct nvme_id_domain_attr {
 .br
 .BI "    __le16 dom_id;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_independent_id_ns.2` & `libnvme-1.9/doc/man/nvme_id_independent_id_ns.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_independent_id_ns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_independent_id_ns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_independent_id_ns \- Identify - I/O Command Set Independent Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_id_independent_id_ns {
 .br
 .BI "    __u8 nsfeat;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns.2` & `libnvme-1.9/doc/man/nvme_id_ns.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ns \- Identify Namespace data structure
 .SH SYNOPSIS
 struct nvme_id_ns {
 .br
 .BI "    __le64 nsze;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_dlfeat.2` & `libnvme-1.9/doc/man/nvme_id_ns_dlfeat.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dlfeat" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dlfeat" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dlfeat \- This field indicates information about features that affect deallocating logical blocks for this namespace.
 .SH SYNOPSIS
 enum nvme_id_ns_dlfeat {
 .br
 .BI "    NVME_NS_DLFEAT_RB"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_dpc.2` & `libnvme-1.9/doc/man/nvme_id_ns_dpc.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dpc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dpc" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dpc \- This field indicates the capabilities for the end-to-end data protection feature.
 .SH SYNOPSIS
 enum nvme_id_ns_dpc {
 .br
 .BI "    NVME_NS_DPC_PI_TYPE1"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_dps.2` & `libnvme-1.9/doc/man/nvme_id_ns_dps.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_dps" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_dps" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_dps \- This field indicates the Type settings for the end-to-end data protection feature.
 .SH SYNOPSIS
 enum nvme_id_ns_dps {
 .br
 .BI "    NVME_NS_DPS_PI_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_flbas.2` & `libnvme-1.9/doc/man/nvme_id_ns_flbas.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_flbas" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_flbas" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_flbas \- This field indicates the LBA data size & metadata size combination that the namespace has been formatted with
 .SH SYNOPSIS
 enum nvme_id_ns_flbas {
 .br
 .BI "    NVME_NS_FLBAS_LOWER_MASK"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_granularity_list.2` & `libnvme-1.9/doc/man/nvme_id_ns_granularity_list.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_ns_granularity_list" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_ns_granularity_list" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_ns_granularity_list \- Namespace Granularity List
 .SH SYNOPSIS
 struct nvme_id_ns_granularity_list {
 .br
 .BI "    __le32 attributes;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_mc.2` & `libnvme-1.9/doc/man/nvme_id_ns_mc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_mc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_mc" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_mc \- This field indicates the capabilities for metadata.
 .SH SYNOPSIS
 enum nvme_id_ns_mc {
 .br
 .BI "    NVME_NS_MC_EXTENDED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_ns_rescap.2` & `libnvme-1.9/doc/man/nvme_id_ns_rescap.2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_ns_rescap" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_ns_rescap" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_ns_rescap \- This field indicates the reservation capabilities of the namespace.
 .SH SYNOPSIS
 enum nvme_id_ns_rescap {
 .br
 .BI "    NVME_NS_RESCAP_PTPL"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_nsfeat.2` & `libnvme-1.9/doc/man/nvme_id_nsfeat.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_nsfeat" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_nsfeat" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_nsfeat \- This field defines features of the namespace.
 .SH SYNOPSIS
 enum nvme_id_nsfeat {
 .br
 .BI "    NVME_NS_FEAT_THIN"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_id_psd.2` & `libnvme-1.9/doc/man/nvme_id_psd.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_id_psd" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_id_psd" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_id_psd \- Power Management data structure
 .SH SYNOPSIS
 struct nvme_id_psd {
 .br
 .BI "    __le16 mp;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_id_uuid.2` & `libnvme-1.9/doc/man/nvme_id_uuid.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_id_uuid" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_id_uuid" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_id_uuid \- Identifier Association
 .SH SYNOPSIS
 enum nvme_id_uuid {
 .br
 .BI "    NVME_ID_UUID_HDR_ASSOCIATION_MASK"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_identify.2` & `libnvme-1.9/doc/man/nvme_identify.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify" 9 "nvme_identify" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify" 9 "nvme_identify" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify \- Send the NVMe Identify command
 .SH SYNOPSIS
 .B "int" nvme_identify
 .BI "(struct nvme_identify_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_active_ns_list.2` & `libnvme-1.9/doc/man/nvme_identify_active_ns_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_active_ns_list" 9 "nvme_identify_active_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_active_ns_list" 9 "nvme_identify_active_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_active_ns_list \- Retrieves active namespaces id list
 .SH SYNOPSIS
 .B "int" nvme_identify_active_ns_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_active_ns_list_csi.2` & `libnvme-1.9/doc/man/nvme_identify_active_ns_list_csi.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_active_ns_list_csi" 9 "nvme_identify_active_ns_list_csi" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_active_ns_list_csi" 9 "nvme_identify_active_ns_list_csi" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_active_ns_list_csi \- Active namespace ID list associated with a specified I/O command set
 .SH SYNOPSIS
 .B "int" nvme_identify_active_ns_list_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "enum nvme_csi csi "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_allocated_ns.2` & `libnvme-1.9/doc/man/nvme_identify_allocated_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns" 9 "nvme_identify_allocated_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns" 9 "nvme_identify_allocated_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns \- Same as nvme_identify_ns, but only for allocated namespaces
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_allocated_ns_list.2` & `libnvme-1.9/doc/man/nvme_identify_allocated_ns_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns_list" 9 "nvme_identify_allocated_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns_list" 9 "nvme_identify_allocated_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns_list \- Retrieves allocated namespace id list
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns_list
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_allocated_ns_list_csi.2` & `libnvme-1.9/doc/man/nvme_identify_allocated_ns_list_csi.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_allocated_ns_list_csi" 9 "nvme_identify_allocated_ns_list_csi" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_allocated_ns_list_csi" 9 "nvme_identify_allocated_ns_list_csi" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_allocated_ns_list_csi \- Allocated namespace ID list associated with a specified I/O command set
 .SH SYNOPSIS
 .B "int" nvme_identify_allocated_ns_list_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "enum nvme_csi csi "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_cns.2` & `libnvme-1.9/doc/man/nvme_identify_cns.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_identify_cns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_identify_cns" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_identify_cns \- Identify - CNS Values
 .SH SYNOPSIS
 enum nvme_identify_cns {
 .br
 .BI "    NVME_IDENTIFY_CNS_NS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ctrl.2` & `libnvme-1.9/doc/man/nvme_identify_ctrl.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl" 9 "nvme_identify_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl" 9 "nvme_identify_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl \- Retrieves nvme identify controller
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ctrl_csi.2` & `libnvme-1.9/doc/man/nvme_identify_ctrl_csi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl_csi" 9 "nvme_identify_ctrl_csi" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl_csi" 9 "nvme_identify_ctrl_csi" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl_csi \- I/O command set specific Identify Controller data
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl_csi
 .BI "(int fd "  ","
 .BI "enum nvme_csi csi "  ","
 .BI "void *data "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_identify_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ctrl_list" 9 "nvme_identify_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ctrl_list" 9 "nvme_identify_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ctrl_list \- Retrieves identify controller list
 .SH SYNOPSIS
 .B "int" nvme_identify_ctrl_list
 .BI "(int fd "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_ctrl_list *cntlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_domain_list.2` & `libnvme-1.9/doc/man/nvme_identify_domain_list.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_domain_list" 9 "nvme_identify_domain_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_domain_list" 9 "nvme_identify_domain_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_domain_list \- Domain list data
 .SH SYNOPSIS
 .B "int" nvme_identify_domain_list
 .BI "(int fd "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_id_domain_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_endurance_group_list.2` & `libnvme-1.9/doc/man/nvme_identify_endurance_group_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_endurance_group_list" 9 "nvme_identify_endurance_group_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_endurance_group_list" 9 "nvme_identify_endurance_group_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_endurance_group_list \- Endurance group list data
 .SH SYNOPSIS
 .B "int" nvme_identify_endurance_group_list
 .BI "(int fd "  ","
 .BI "__u16 endgrp_id "  ","
 .BI "struct nvme_id_endurance_group_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_independent_identify_ns.2` & `libnvme-1.9/doc/man/nvme_identify_independent_identify_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_independent_identify_ns" 9 "nvme_identify_independent_identify_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_independent_identify_ns" 9 "nvme_identify_independent_identify_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_independent_identify_ns \- I/O command set independent Identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_identify_independent_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_independent_id_ns *ns "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_iocs.2` & `libnvme-1.9/doc/man/nvme_identify_iocs.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_iocs" 9 "nvme_identify_iocs" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_iocs" 9 "nvme_identify_iocs" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_iocs \- I/O command set data structure
 .SH SYNOPSIS
 .B "int" nvme_identify_iocs
 .BI "(int fd "  ","
 .BI "__u16 cntlid "  ","
 .BI "struct nvme_id_iocs *iocs "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2` & `libnvme-1.9/doc/man/nvme_identify_iocs_ns_csi_user_data_format.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_iocs_ns_csi_user_data_format" 9 "nvme_identify_iocs_ns_csi_user_data_format" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_iocs_ns_csi_user_data_format" 9 "nvme_identify_iocs_ns_csi_user_data_format" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_iocs_ns_csi_user_data_format \- Identify I/O command set namespace data structure
 .SH SYNOPSIS
 .B "int" nvme_identify_iocs_ns_csi_user_data_format
 .BI "(int fd "  ","
 .BI "__u16 user_data_format "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ns.2` & `libnvme-1.9/doc/man/nvme_identify_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns" 9 "nvme_identify_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ns" 9 "nvme_identify_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns \- Retrieves nvme identify namespace
 .SH SYNOPSIS
 .B "int" nvme_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ns_csi.2` & `libnvme-1.9/doc/man/nvme_identify_ns_csi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_csi" 9 "nvme_identify_ns_csi" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_csi" 9 "nvme_identify_ns_csi" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_csi \- I/O command set specific identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_csi
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ns_csi_user_data_format.2` & `libnvme-1.9/doc/man/nvme_identify_ns_csi_user_data_format.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_csi_user_data_format" 9 "nvme_identify_ns_csi_user_data_format" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_csi_user_data_format" 9 "nvme_identify_ns_csi_user_data_format" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_csi_user_data_format \- Identify namespace user data format
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_csi_user_data_format
 .BI "(int fd "  ","
 .BI "__u16 user_data_format "  ","
 .BI "__u8 uuidx "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ns_descs.2` & `libnvme-1.9/doc/man/nvme_identify_ns_descs.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_descs" 9 "nvme_identify_ns_descs" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_descs" 9 "nvme_identify_ns_descs" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_descs \- Retrieves namespace descriptor list
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_descs
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_id_desc *descs "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_ns_granularity.2` & `libnvme-1.9/doc/man/nvme_identify_ns_granularity.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_ns_granularity" 9 "nvme_identify_ns_granularity" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_ns_granularity" 9 "nvme_identify_ns_granularity" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_ns_granularity \- Retrieves namespace granularity identification
 .SH SYNOPSIS
 .B "int" nvme_identify_ns_granularity
 .BI "(int fd "  ","
 .BI "struct nvme_id_ns_granularity_list *gr_list "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_nsid_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_ctrl_list.2`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-.TH "nvme_identify_nsid_ctrl_list" 9 "nvme_identify_nsid_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ctrl_list" 9 "nvme_mi_admin_identify_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_identify_nsid_ctrl_list \- Retrieves controller list attached to an nsid
+nvme_mi_admin_identify_ctrl_list \- Perform an Admin identify for a controller list.
 .SH SYNOPSIS
-.B "int" nvme_identify_nsid_ctrl_list
-.BI "(int fd "  ","
-.BI "__u32 nsid "  ","
+.B "int" nvme_mi_admin_identify_ctrl_list
+.BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 cntid "  ","
-.BI "struct nvme_ctrl_list *cntlist "  ");"
+.BI "struct nvme_ctrl_list *list "  ");"
 .SH ARGUMENTS
-.IP "fd" 12
-File descriptor of nvme device
-.IP "nsid" 12
-Return controllers that are attached to this nsid
+.IP "ctrl" 12
+Controller to process identify command
 .IP "cntid" 12
-Starting CNTLID to return in the list
-.IP "cntlist" 12
-User space destination address to transfer the data
+Controller ID to specify list start
+.IP "list" 12
+List data to populate
 .SH "DESCRIPTION"
-Up to 2047 controller identifiers are returned containing a controller
-identifier greater than or equal to the controller identifier  specified in
-\fIcntid\fP attached to \fInsid\fP.
+Perform an Identify command, for the controller list starting with
+IDs greater than or equal to \fIcntid\fP.
 
-See \fIstruct nvme_ctrl_list\fP for a definition of the structure returned.
+Will return an error if the length of the response data (from the
+controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIid\fP will be
+fully populated on success.
+
+See: \fIstruct nvme_ctrl_list\fP
 .SH "RETURN"
 The nvme command status if a response was received (see
-\fIenum nvme_status_field\fP) or -1
+\fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_nvmset_list.2` & `libnvme-1.9/doc/man/nvme_identify_nvmset_list.2`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_nvmset_list" 9 "nvme_identify_nvmset_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_nvmset_list" 9 "nvme_identify_nvmset_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_nvmset_list \- Retrieves NVM Set List
 .SH SYNOPSIS
 .B "int" nvme_identify_nvmset_list
 .BI "(int fd "  ","
 .BI "__u16 nvmsetid "  ","
 .BI "struct nvme_id_nvmset_list *nvmset "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_primary_ctrl.2` & `libnvme-1.9/doc/man/nvme_identify_primary_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_primary_ctrl" 9 "nvme_identify_primary_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_primary_ctrl" 9 "nvme_identify_primary_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_primary_ctrl \- Retrieve NVMe Primary Controller identification
 .SH SYNOPSIS
 .B "int" nvme_identify_primary_ctrl
 .BI "(int fd "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_primary_ctrl_cap *cap "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_secondary_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_identify_secondary_ctrl_list.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_secondary_ctrl_list" 9 "nvme_identify_secondary_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_secondary_ctrl_list" 9 "nvme_identify_secondary_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_secondary_ctrl_list \- Retrieves secondary controller list
 .SH SYNOPSIS
 .B "int" nvme_identify_secondary_ctrl_list
 .BI "(int fd "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_secondary_ctrl_list *sc_list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_identify_uuid.2` & `libnvme-1.9/doc/man/nvme_identify_uuid.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_identify_uuid" 9 "nvme_identify_uuid" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_identify_uuid" 9 "nvme_identify_uuid" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_identify_uuid \- Retrieves device's UUIDs
 .SH SYNOPSIS
 .B "int" nvme_identify_uuid
 .BI "(int fd "  ","
 .BI "struct nvme_id_uuid_list *uuid_list "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_init_copy_range.2` & `libnvme-1.9/doc/man/nvme_init_copy_range.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range" 9 "nvme_init_copy_range" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range" 9 "nvme_init_copy_range" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range \- Constructs a copy range structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range
 .BI "(struct nvme_copy_range *copy "  ","
 .BI "__u16 *nlbs "  ","
 .BI "__u64 *slbas "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_init_copy_range_f1.2` & `libnvme-1.9/doc/man/nvme_init_copy_range_f1.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range_f1" 9 "nvme_init_copy_range_f1" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range_f1" 9 "nvme_init_copy_range_f1" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range_f1 \- Constructs a copy range f1 structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range_f1
 .BI "(struct nvme_copy_range_f1 *copy "  ","
 .BI "__u16 *nlbs "  ","
 .BI "__u64 *slbas "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_init_copy_range_f2.2` & `libnvme-1.9/doc/man/nvme_init_copy_range_f2.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range_f2" 9 "nvme_init_copy_range_f2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range_f2" 9 "nvme_init_copy_range_f2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range_f2 \- Constructs a copy range f2 structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range_f2
 .BI "(struct nvme_copy_range_f2 *copy "  ","
 .BI "__u32 *snsids "  ","
 .BI "__u16 *nlbs "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_init_copy_range_f3.2` & `libnvme-1.9/doc/man/nvme_init_copy_range_f3.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_copy_range_f3" 9 "nvme_init_copy_range_f3" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_copy_range_f3" 9 "nvme_init_copy_range_f3" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_copy_range_f3 \- Constructs a copy range f3 structure
 .SH SYNOPSIS
 .B "void" nvme_init_copy_range_f3
 .BI "(struct nvme_copy_range_f3 *copy "  ","
 .BI "__u32 *snsids "  ","
 .BI "__u16 *nlbs "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_init_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_init_ctrl_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_ctrl_list" 9 "nvme_init_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_ctrl_list" 9 "nvme_init_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_ctrl_list \- Initialize an nvme_ctrl_list structure from an array.
 .SH SYNOPSIS
 .B "void" nvme_init_ctrl_list
 .BI "(struct nvme_ctrl_list *cntlist "  ","
 .BI "__u16 num_ctrls "  ","
 .BI "__u16 *ctrlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_init_dsm_range.2` & `libnvme-1.9/doc/man/nvme_init_dsm_range.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_dsm_range" 9 "nvme_init_dsm_range" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_dsm_range" 9 "nvme_init_dsm_range" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_dsm_range \- Constructs a data set range structure
 .SH SYNOPSIS
 .B "void" nvme_init_dsm_range
 .BI "(struct nvme_dsm_range *dsm "  ","
 .BI "__u32 *ctx_attrs "  ","
 .BI "__u32 *llbas "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_init_logging.2` & `libnvme-1.9/doc/man/nvme_init_logging.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_init_logging" 9 "nvme_init_logging" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_init_logging" 9 "nvme_init_logging" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_init_logging \- Initialize logging
 .SH SYNOPSIS
 .B "void" nvme_init_logging
 .BI "(nvme_root_t r "  ","
 .BI "int lvl "  ","
 .BI "bool log_pid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_insert_tls_key.2` & `libnvme-1.9/doc/man/nvme_insert_tls_key.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_insert_tls_key" 9 "nvme_insert_tls_key" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_insert_tls_key" 9 "nvme_insert_tls_key" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_insert_tls_key \- Derive and insert TLS key
 .SH SYNOPSIS
 .B "long" nvme_insert_tls_key
 .BI "(const char *keyring "  ","
 .BI "const char *key_type "  ","
 .BI "const char *hostnqn "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_insert_tls_key_versioned.2` & `libnvme-1.9/doc/man/nvme_insert_tls_key_versioned.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_insert_tls_key_versioned" 9 "nvme_insert_tls_key_versioned" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_insert_tls_key_versioned" 9 "nvme_insert_tls_key_versioned" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_insert_tls_key_versioned \- Derive and insert TLS key
 .SH SYNOPSIS
 .B "long" nvme_insert_tls_key_versioned
 .BI "(const char *keyring "  ","
 .BI "const char *key_type "  ","
 .BI "const char *hostnqn "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_io_control_flags.2` & `libnvme-1.9/doc/man/nvme_io_control_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_control_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_control_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_io_control_flags \- I/O control flags
 .SH SYNOPSIS
 enum nvme_io_control_flags {
 .br
 .BI "    NVME_IO_DTYPE_STREAMS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_io_dsm_flags.2` & `libnvme-1.9/doc/man/nvme_io_dsm_flags.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_dsm_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_dsm_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_io_dsm_flags \- Dataset Management flags
 .SH SYNOPSIS
 enum nvme_io_dsm_flags {
 .br
 .BI "    NVME_IO_DSM_FREQ_UNSPEC"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_io_opcode.2` & `libnvme-1.9/doc/man/nvme_io_opcode.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_io_opcode" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_io_opcode" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_io_opcode \- Opcodes for I/O Commands
 .SH SYNOPSIS
 enum nvme_io_opcode {
 .br
 .BI "    nvme_cmd_flush"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_io_passthru.2` & `libnvme-1.9/doc/man/nvme_admin_passthru.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_io_passthru" 9 "nvme_io_passthru" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_admin_passthru" 9 "nvme_admin_passthru" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_io_passthru \- Submit an nvme io passthrough command
+nvme_admin_passthru \- Submit an nvme passthrough command
 .SH SYNOPSIS
-.B "int" nvme_io_passthru
+.B "int" nvme_admin_passthru
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_io_passthru\fP. This sets up and submits
-a \fIstruct nvme_passthru_cmd\fP.
+Parameterized form of \fBnvme_submit_admin_passthru\fP. This sets up and
+submits a \fIstruct nvme_passthru_cmd\fP.
 
-Known values for \fIopcode\fP are defined in \fIenum nvme_io_opcode\fP.
+Known values for \fIopcode\fP are defined in \fIenum nvme_admin_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_io_passthru64.2` & `libnvme-1.9/doc/man/nvme_io_passthru.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-.TH "nvme_io_passthru64" 9 "nvme_io_passthru64" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_io_passthru" 9 "nvme_io_passthru" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_io_passthru64 \- Submit an nvme io passthrough command
+nvme_io_passthru \- Submit an nvme io passthrough command
 .SH SYNOPSIS
-.B "int" nvme_io_passthru64
+.B "int" nvme_io_passthru
 .BI "(int fd "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
 .BI "__u16 rsvd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u32 cdw2 "  ","
 .BI "__u32 cdw3 "  ","
@@ -17,15 +17,15 @@
 .BI "__u32 cdw14 "  ","
 .BI "__u32 cdw15 "  ","
 .BI "__u32 data_len "  ","
 .BI "void *data "  ","
 .BI "__u32 metadata_len "  ","
 .BI "void *metadata "  ","
 .BI "__u32 timeout_ms "  ","
-.BI "__u64 *result "  ");"
+.BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "opcode" 12
 The nvme io command to send
 .IP "flags" 12
 NVMe command flags (not used)
@@ -58,14 +58,14 @@
 .IP "metadata" 12
 Pointer to user address of the metadata buffer
 .IP "timeout_ms" 12
 How long the kernel waits for the command to complete
 .IP "result" 12
 Optional field to return the result from the CQE dword 0
 .SH "DESCRIPTION"
-Parameterized form of \fBnvme_submit_io_passthru64\fP. This sets up and submits
-a \fIstruct nvme_passthru_cmd64\fP.
+Parameterized form of \fBnvme_submit_io_passthru\fP. This sets up and submits
+a \fIstruct nvme_passthru_cmd\fP.
 
 Known values for \fIopcode\fP are defined in \fIenum nvme_io_opcode\fP.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_is_64bit_reg.2` & `libnvme-1.9/doc/man/nvme_is_64bit_reg.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_is_64bit_reg" 9 "nvme_is_64bit_reg" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_is_64bit_reg" 9 "nvme_is_64bit_reg" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_is_64bit_reg \- Checks if offset of the controller register is a know 64bit value.
 .SH SYNOPSIS
 .B "bool" nvme_is_64bit_reg
 .BI "(__u32 offset "  ");"
 .SH ARGUMENTS
 .IP "offset" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_lba_range_type_entry.2` & `libnvme-1.9/doc/man/nvme_lba_range_type_entry.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_range_type_entry" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_range_type_entry" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_range_type_entry \- LBA Range Type - Data Structure Entry
 .SH SYNOPSIS
 struct nvme_lba_range_type_entry {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_lba_status_desc.2` & `libnvme-1.9/doc/man/nvme_lba_status_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_status_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_status_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_status_desc \- LBA Status Descriptor Entry
 .SH SYNOPSIS
 struct nvme_lba_status_desc {
 .br
 .BI "    __le64 dslba;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_lba_status_log.2` & `libnvme-1.9/doc/man/nvme_lba_status_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lba_status_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lba_status_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_lba_status_log \- LBA Status Information Log
 .SH SYNOPSIS
 struct nvme_lba_status_log {
 .br
 .BI "    __le32 lslplen;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_lbaf.2` & `libnvme-1.9/doc/man/nvme_lbaf.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lbaf" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lbaf" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_lbaf \- LBA Format Data Structure
 .SH SYNOPSIS
 struct nvme_lbaf {
 .br
 .BI "    __le16 ms;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_lbaf_rp.2` & `libnvme-1.9/doc/man/nvme_lbaf_rp.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_lbaf_rp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_lbaf_rp" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_lbaf_rp \- This field indicates the relative performance of the LBA format indicated relative to other LBA formats supported by the controller.
 .SH SYNOPSIS
 enum nvme_lbaf_rp {
 .br
 .BI "    NVME_LBAF_RP_BEST"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_lbart.2` & `libnvme-1.9/doc/man/nvme_lbart.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_lbart" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_lbart" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_lbart \- LBA Range Type - Data Structure Entry
 .SH SYNOPSIS
 enum nvme_lbart {
 .br
 .BI "    NVME_LBART_TYPE_GP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_lbas_ns_element.2` & `libnvme-1.9/doc/man/nvme_lbas_ns_element.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_lbas_ns_element" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_lbas_ns_element" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_lbas_ns_element \- LBA Status Log Namespace Element
 .SH SYNOPSIS
 struct nvme_lbas_ns_element {
 .br
 .BI "    __le32 neid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_log_phy_rx_eom_action.2` & `libnvme-1.9/doc/man/nvme_log_phy_rx_eom_action.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_log_phy_rx_eom_action" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_log_phy_rx_eom_action" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_log_phy_rx_eom_action \- Physical Interface Receiver Eye Opening Measurement Action
 .SH SYNOPSIS
 enum nvme_log_phy_rx_eom_action {
 .br
 .BI "    NVME_LOG_PHY_RX_EOM_READ"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_log_phy_rx_eom_quality.2` & `libnvme-1.9/doc/man/nvme_log_phy_rx_eom_quality.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_log_phy_rx_eom_quality" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_log_phy_rx_eom_quality" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_log_phy_rx_eom_quality \- Physical Interface Receiver Eye Opening Measurement Quality
 .SH SYNOPSIS
 enum nvme_log_phy_rx_eom_quality {
 .br
 .BI "    NVME_LOG_PHY_RX_EOM_GOOD"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_lookup_ctrl.2` & `libnvme-1.9/doc/man/nvme_lookup_ctrl.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_ctrl" 9 "nvme_lookup_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_lookup_ctrl" 9 "nvme_lookup_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_ctrl \- Lookup nvme_ctrl_t object
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvme_lookup_ctrl
 .BI "(nvme_subsystem_t s "  ","
 .BI "const char *transport "  ","
 .BI "const char *traddr "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_lookup_host.2` & `libnvme-1.9/doc/man/nvme_lookup_host.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_host" 9 "nvme_lookup_host" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_lookup_host" 9 "nvme_lookup_host" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_host \- Lookup nvme_host_t object
 .SH SYNOPSIS
 .B "nvme_host_t" nvme_lookup_host
 .BI "(nvme_root_t r "  ","
 .BI "const char *hostnqn "  ","
 .BI "const char *hostid "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_lookup_subsystem.2` & `libnvme-1.9/doc/man/nvme_lookup_subsystem.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_lookup_subsystem" 9 "nvme_lookup_subsystem" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_lookup_subsystem" 9 "nvme_lookup_subsystem" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_lookup_subsystem \- Lookup nvme_subsystem_t object
 .SH SYNOPSIS
 .B "nvme_subsystem_t" nvme_lookup_subsystem
 .BI "(struct nvme_host *h "  ","
 .BI "const char *name "  ","
 .BI "const char *subsysnqn "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_media_unit_stat_desc.2` & `libnvme-1.9/doc/man/nvme_media_unit_stat_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_media_unit_stat_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_media_unit_stat_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_media_unit_stat_desc \- Media Unit Status Descriptor
 .SH SYNOPSIS
 struct nvme_media_unit_stat_desc {
 .br
 .BI "    __le16 muid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_media_unit_stat_log.2` & `libnvme-1.9/doc/man/nvme_secondary_ctrl.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-.TH "libnvme" 9 "struct nvme_media_unit_stat_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_secondary_ctrl" "May 2024" "API Manual" LINUX
 .SH NAME
-struct nvme_media_unit_stat_log \- Media Unit Status
+struct nvme_secondary_ctrl \- Secondary Controller Entry
 .SH SYNOPSIS
-struct nvme_media_unit_stat_log {
+struct nvme_secondary_ctrl {
 .br
-.BI "    __le16 nmu;"
+.BI "    __le16 scid;"
 .br
-.BI "    __le16 cchans;"
+.BI "    __le16 pcid;"
 .br
-.BI "    __le16 sel_config;"
+.BI "    __u8 scs;"
 .br
-.BI "    __u8 rsvd6[10];"
+.BI "    __u8 rsvd5[3];"
 .br
-.BI "    struct nvme_media_unit_stat_desc mus_desc[];"
+.BI "    __le16 vfn;"
+.br
+.BI "    __le16 nvq;"
+.br
+.BI "    __le16 nvi;"
+.br
+.BI "    __u8 rsvd14[18];"
 .br
 .BI "
 };
 .br
 
 .SH Members
-.IP "nmu" 12
-Number unit status descriptor
-.IP "cchans" 12
-Number of Channels
-.IP "sel_config" 12
-Selected Configuration
-.IP "rsvd6" 12
+.IP "scid" 12
+Secondary Controller Identifier
+.IP "pcid" 12
+Primary Controller Identifier
+.IP "scs" 12
+Secondary Controller State
+.IP "rsvd5" 12
+Reserved
+.IP "vfn" 12
+Virtual Function Number
+.IP "nvq" 12
+Number of VQ Flexible Resources Assigned
+.IP "nvi" 12
+Number of VI Flexible Resources Assigned
+.IP "rsvd14" 12
 Reserved
-.IP "mus_desc" 12
-Media unit statistic descriptors
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_admin_passthru.2` & `libnvme-1.9/doc/man/nvme_mi_admin_admin_passthru.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_admin_passthru" 9 "nvme_mi_admin_admin_passthru" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_admin_passthru" 9 "nvme_mi_admin_admin_passthru" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_admin_passthru \- Submit an nvme admin passthrough command
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_admin_passthru
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u8 opcode "  ","
 .BI "__u8 flags "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_format_nvm.2` & `libnvme-1.9/doc/man/nvme_mi_admin_format_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_format_nvm" 9 "nvme_mi_admin_format_nvm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_format_nvm" 9 "nvme_mi_admin_format_nvm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_format_nvm \- Format NVMe namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_format_nvm
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_format_nvm_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_fw_commit.2` & `libnvme-1.9/doc/man/nvme_mi_admin_fw_commit.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_fw_commit" 9 "nvme_mi_admin_fw_commit" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_fw_commit" 9 "nvme_mi_admin_fw_commit" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_fw_commit \- Commit firmware using the specified action
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_fw_commit
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_fw_commit_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_fw_download.2` & `libnvme-1.9/doc/man/nvme_mi_admin_fw_download.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_fw_download" 9 "nvme_mi_admin_fw_download" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_fw_download" 9 "nvme_mi_admin_fw_download" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_fw_download \- Download part or all of a firmware image to the controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_fw_download
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_fw_download_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_features_data.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_features_data.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_features_data" 9 "nvme_mi_admin_get_features_data" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_features_data" 9 "nvme_mi_admin_get_features_data" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_features_data \- Helper function for &nvme_mi_admin_get_features()
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_features_data
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_features_id fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log" 9 "nvme_mi_admin_get_log" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log" 9 "nvme_mi_admin_get_log" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log \- Retrieve log page data from controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_get_log_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_ana.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_ana.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_ana" 9 "nvme_mi_admin_get_log_ana" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_ana" 9 "nvme_mi_admin_get_log_ana" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_ana \- Retrieve Asymmetric Namespace Access log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_ana
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_log_ana_lsp lsp "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_ana_groups.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_ana_groups.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_ana_groups" 9 "nvme_mi_admin_get_log_ana_groups" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_ana_groups" 9 "nvme_mi_admin_get_log_ana_groups" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_ana_groups \- Retrieve Asymmetric Namespace Access groups only log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_ana_groups
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_boot_partition.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_boot_partition.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_boot_partition" 9 "nvme_mi_admin_get_log_boot_partition" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_boot_partition" 9 "nvme_mi_admin_get_log_boot_partition" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_boot_partition \- Retrieve Boot Partition
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_boot_partition
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u8 lsp "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_changed_ns_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_changed_ns_list.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_changed_ns_list" 9 "nvme_mi_admin_get_log_changed_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_changed_ns_list" 9 "nvme_mi_admin_get_log_changed_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_changed_ns_list \- Retrieve namespace changed list
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_changed_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_ns_list *ns_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_cmd_effects.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_cmd_effects.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_cmd_effects" 9 "nvme_mi_admin_get_log_cmd_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_cmd_effects" 9 "nvme_mi_admin_get_log_cmd_effects" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_cmd_effects \- Retrieve nvme command effects log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_cmd_effects
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_csi csi "  ","
 .BI "struct nvme_cmd_effects_log *effects_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_create_telemetry_host.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_create_telemetry_host" 9 "nvme_mi_admin_get_log_create_telemetry_host" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_create_telemetry_host" 9 "nvme_mi_admin_get_log_create_telemetry_host" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_create_telemetry_host \- Create host telemetry log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_create_telemetry_host
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_telemetry_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_device_self_test.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_device_self_test.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_device_self_test" 9 "nvme_mi_admin_get_log_device_self_test" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_device_self_test" 9 "nvme_mi_admin_get_log_device_self_test" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_device_self_test \- Retrieve the device self test log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_device_self_test
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_self_test_log *log "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_discovery.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_discovery.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_discovery" 9 "nvme_mi_admin_get_log_discovery" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_discovery" 9 "nvme_mi_admin_get_log_discovery" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_discovery \- Retrieve Discovery log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_discovery
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_endurance_group.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_endurance_group.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_endurance_group" 9 "nvme_mi_admin_get_log_endurance_group" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_endurance_group" 9 "nvme_mi_admin_get_log_endurance_group" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_endurance_group \- Get Endurance Group log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_endurance_group
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 endgid "  ","
 .BI "struct nvme_endurance_group_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_endurance_grp_evt.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_endurance_grp_evt" 9 "nvme_mi_admin_get_log_endurance_grp_evt" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_endurance_grp_evt" 9 "nvme_mi_admin_get_log_endurance_grp_evt" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_endurance_grp_evt \- Retrieve Rotational Media Information
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_endurance_grp_evt
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_error.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_error.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_error" 9 "nvme_mi_admin_get_log_error" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_error" 9 "nvme_mi_admin_get_log_error" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_error \- Retrieve nvme error log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_error
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "unsigned int nr_entries "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_fid_supported_effects.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_fid_supported_effects" 9 "nvme_mi_admin_get_log_fid_supported_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_fid_supported_effects" 9 "nvme_mi_admin_get_log_fid_supported_effects" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_fid_supported_effects \- Retrieve Feature Identifiers Supported and Effects
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_fid_supported_effects
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_fid_supported_effects_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_fw_slot.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_fw_slot.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_fw_slot" 9 "nvme_mi_admin_get_log_fw_slot" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_fw_slot" 9 "nvme_mi_admin_get_log_fw_slot" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_fw_slot \- Retrieves the controller firmware log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_fw_slot
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_firmware_slot *fw_log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_lba_status.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_lba_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_lba_status" 9 "nvme_mi_admin_get_log_lba_status" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_lba_status" 9 "nvme_mi_admin_get_log_lba_status" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_lba_status \- Retrieve LBA Status
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_lba_status
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_mi_cmd_supported_effects.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_supported_log_pages.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-.TH "nvme_mi_admin_get_log_mi_cmd_supported_effects" 9 "nvme_mi_admin_get_log_mi_cmd_supported_effects" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_supported_log_pages" 9 "nvme_mi_admin_get_log_supported_log_pages" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_get_log_mi_cmd_supported_effects \- displays the MI Commands Supported by the controller
+nvme_mi_admin_get_log_supported_log_pages \- Retrieve nmve supported log pages
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_get_log_mi_cmd_supported_effects
+.B "int" nvme_mi_admin_get_log_supported_log_pages
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
-.BI "struct nvme_mi_cmd_supported_effects_log *log "  ");"
+.BI "struct nvme_supported_log_pages *log "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to query
 .IP "rae" 12
 Retain asynchronous events
 .IP "log" 12
-MI Command Supported and Effects data structure
+Array of LID supported and Effects data structures
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_page.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_page.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_page" 9 "nvme_mi_admin_get_log_page" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_page" 9 "nvme_mi_admin_get_log_page" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_page \- Retrieve log page data from controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_page
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 xfer_len "  ","
 .BI "struct nvme_get_log_args *args "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_persistent_event.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_persistent_event.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_persistent_event" 9 "nvme_mi_admin_get_log_persistent_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_persistent_event" 9 "nvme_mi_admin_get_log_persistent_event" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_persistent_event \- Retrieve Persistent Event Log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_persistent_event
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_pevent_log_action action "  ","
 .BI "__u32 size "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_phy_rx_eom.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_phy_rx_eom.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_phy_rx_eom" 9 "nvme_mi_admin_get_log_phy_rx_eom" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_phy_rx_eom" 9 "nvme_mi_admin_get_log_phy_rx_eom" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_phy_rx_eom \- Retrieve Physical Interface Receiver Eye Opening Measurement Log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_phy_rx_eom
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u8 lsp "  ","
 .BI "__u16 controller "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_predictable_lat_event.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_predictable_lat_event" 9 "nvme_mi_admin_get_log_predictable_lat_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_predictable_lat_event" 9 "nvme_mi_admin_get_log_predictable_lat_event" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_predictable_lat_event \- Retrieve Predictable Latency Event Aggregate Log Page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_predictable_lat_event
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u32 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_reservation.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_reservation.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_reservation" 9 "nvme_mi_admin_get_log_reservation" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_reservation" 9 "nvme_mi_admin_get_log_reservation" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_reservation \- Retrieve Reservation Notification
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_reservation
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_resv_notification_log *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_sanitize.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_sanitize.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_sanitize" 9 "nvme_mi_admin_get_log_sanitize" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_sanitize" 9 "nvme_mi_admin_get_log_sanitize" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_sanitize \- Retrieve Sanitize Status
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_sanitize
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "struct nvme_sanitize_log_page *log "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_simple.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_simple.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_simple" 9 "nvme_mi_admin_get_log_simple" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_simple" 9 "nvme_mi_admin_get_log_simple" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_simple \- Helper for Get Log Page functions with no NSID or RAE requirements
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_simple
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_cmd_get_log_lid lid "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_smart.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_smart.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_smart" 9 "nvme_mi_admin_get_log_smart" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_smart" 9 "nvme_mi_admin_get_log_smart" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_smart \- Retrieve nvme smart log
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_smart
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_support_cap_config_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_support_cap_config_list" 9 "nvme_mi_admin_get_log_support_cap_config_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_support_cap_config_list" 9 "nvme_mi_admin_get_log_support_cap_config_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_support_cap_config_list \- Retrieve Supported Capacity Configuration List
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_support_cap_config_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 domid "  ","
 .BI "struct nvme_supported_cap_config_list_log *cap "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_telemetry_ctrl.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_telemetry_ctrl" 9 "nvme_mi_admin_get_log_telemetry_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_telemetry_ctrl" 9 "nvme_mi_admin_get_log_telemetry_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_telemetry_ctrl \- Get Telemetry Controller-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_telemetry_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "__u64 offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_telemetry_host.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_telemetry_host.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_telemetry_host" 9 "nvme_mi_admin_get_log_telemetry_host" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_telemetry_host" 9 "nvme_mi_admin_get_log_telemetry_host" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_telemetry_host \- Get Telemetry Host-Initiated log page
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_telemetry_host
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u64 offset "  ","
 .BI "__u32 len "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_log_zns_changed_zones.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_log_zns_changed_zones" 9 "nvme_mi_admin_get_log_zns_changed_zones" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_log_zns_changed_zones" 9 "nvme_mi_admin_get_log_zns_changed_zones" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_log_zns_changed_zones \- Retrieve list of zones that have changed
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_log_zns_changed_zones
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "bool rae "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_get_nsid_log.2` & `libnvme-1.9/doc/man/nvme_mi_admin_get_nsid_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_get_nsid_log" 9 "nvme_mi_admin_get_nsid_log" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_get_nsid_log" 9 "nvme_mi_admin_get_nsid_log" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_get_nsid_log \- Helper for Get Log Page functions
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_get_nsid_log
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "bool rae "  ","
 .BI "enum nvme_cmd_get_log_lid lid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify" 9 "nvme_mi_admin_identify" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify" 9 "nvme_mi_admin_identify" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify \- Perform an Admin identify command.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_identify_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_active_ns_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_allocated_ns_list.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_mi_admin_identify_active_ns_list" 9 "nvme_mi_admin_identify_active_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_allocated_ns_list" 9 "nvme_mi_admin_identify_allocated_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_identify_active_ns_list \- Perform an Admin identify for an active namespace list
+nvme_mi_admin_identify_allocated_ns_list \- Perform an Admin identify for an allocated namespace list
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_identify_active_ns_list
+.B "int" nvme_mi_admin_identify_allocated_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to process identify command
 .IP "nsid" 12
 Namespace ID to specify list start
 .IP "list" 12
 List data to populate
 .SH "DESCRIPTION"
-Perform an Identify command, for the active namespace list starting with
+Perform an Identify command, for the allocated namespace list starting with
 IDs greater than or equal to \fInsid\fP. Specify \fINVME_NSID_NONE\fP for the start
 of the list.
 
 Will return an error if the length of the response data (from the
 controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIlist\fP will be
 be fully populated on success.
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_allocated_ns.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_allocated_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_allocated_ns" 9 "nvme_mi_admin_identify_allocated_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_allocated_ns" 9 "nvme_mi_admin_identify_allocated_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_allocated_ns \- Perform an Admin identify command for an allocated namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_allocated_ns
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_allocated_ns_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_active_ns_list.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_mi_admin_identify_allocated_ns_list" 9 "nvme_mi_admin_identify_allocated_ns_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_active_ns_list" 9 "nvme_mi_admin_identify_active_ns_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_identify_allocated_ns_list \- Perform an Admin identify for an allocated namespace list
+nvme_mi_admin_identify_active_ns_list \- Perform an Admin identify for an active namespace list
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_identify_allocated_ns_list
+.B "int" nvme_mi_admin_identify_active_ns_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_list *list "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to process identify command
 .IP "nsid" 12
 Namespace ID to specify list start
 .IP "list" 12
 List data to populate
 .SH "DESCRIPTION"
-Perform an Identify command, for the allocated namespace list starting with
+Perform an Identify command, for the active namespace list starting with
 IDs greater than or equal to \fInsid\fP. Specify \fINVME_NSID_NONE\fP for the start
 of the list.
 
 Will return an error if the length of the response data (from the
 controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIlist\fP will be
 be fully populated on success.
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_cns_nsid.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_cns_nsid.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_cns_nsid" 9 "nvme_mi_admin_identify_cns_nsid" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_cns_nsid" 9 "nvme_mi_admin_identify_cns_nsid" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_cns_nsid \- Perform an Admin identify command using specific CNS/NSID parameters.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_cns_nsid
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "enum nvme_identify_cns cns "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_ctrl.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ctrl" 9 "nvme_mi_admin_identify_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ctrl" 9 "nvme_mi_admin_identify_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ctrl \- Perform an Admin identify for a controller
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_nsid_ctrl_list.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-.TH "nvme_mi_admin_identify_ctrl_list" 9 "nvme_mi_admin_identify_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_nsid_ctrl_list" 9 "nvme_mi_admin_identify_nsid_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_mi_admin_identify_ctrl_list \- Perform an Admin identify for a controller list.
+nvme_mi_admin_identify_nsid_ctrl_list \- Perform an Admin identify for a controller list with specific namespace ID
 .SH SYNOPSIS
-.B "int" nvme_mi_admin_identify_ctrl_list
+.B "int" nvme_mi_admin_identify_nsid_ctrl_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
+.BI "__u32 nsid "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_ctrl_list *list "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
 Controller to process identify command
+.IP "nsid" 12
+Namespace identifier
 .IP "cntid" 12
 Controller ID to specify list start
 .IP "list" 12
 List data to populate
 .SH "DESCRIPTION"
-Perform an Identify command, for the controller list starting with
-IDs greater than or equal to \fIcntid\fP.
+Perform an Identify command, for the controller list for \fInsid\fP, starting
+with IDs greater than or equal to \fIcntid\fP.
 
 Will return an error if the length of the response data (from the
 controller) is not a full \fINVME_IDENTIFY_DATA_SIZE\fP, so \fIid\fP will be
 fully populated on success.
 
 See: \fIstruct nvme_ctrl_list\fP
 .SH "RETURN"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_ns.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ns" 9 "nvme_mi_admin_identify_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ns" 9 "nvme_mi_admin_identify_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ns \- Perform an Admin identify command for a namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ns
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_id_ns *ns "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_ns_descs.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_ns_descs.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_ns_descs" 9 "nvme_mi_admin_identify_ns_descs" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_ns_descs" 9 "nvme_mi_admin_identify_ns_descs" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_ns_descs \- Perform an Admin identify Namespace Identification Descriptor list command for a namespace
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_ns_descs
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ns_id_desc *descs "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_partial.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_partial.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_partial" 9 "nvme_mi_admin_identify_partial" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_partial" 9 "nvme_mi_admin_identify_partial" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_partial \- Perform an Admin identify command, and retrieve partial response data.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_partial
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_identify_args *args "  ","
 .BI "off_t offset "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_primary_ctrl.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_primary_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_primary_ctrl" 9 "nvme_mi_admin_identify_primary_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_primary_ctrl" 9 "nvme_mi_admin_identify_primary_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_primary_ctrl \- Perform an Admin identify for primary controller capabilities data structure.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_primary_ctrl
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_primary_ctrl_cap *cap "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_mi_admin_identify_secondary_ctrl_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_identify_secondary_ctrl_list" 9 "nvme_mi_admin_identify_secondary_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_identify_secondary_ctrl_list" 9 "nvme_mi_admin_identify_secondary_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_identify_secondary_ctrl_list \- Perform an Admin identify for a secondary controller list.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_identify_secondary_ctrl_list
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u16 cntid "  ","
 .BI "struct nvme_secondary_ctrl_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_ns_attach.2` & `libnvme-1.9/doc/man/nvme_mi_admin_ns_attach.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_attach" 9 "nvme_mi_admin_ns_attach" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_attach" 9 "nvme_mi_admin_ns_attach" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_attach \- Attach or detach namespace to controller(s)
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_attach
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_ns_attach_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_ns_attach_ctrls.2` & `libnvme-1.9/doc/man/nvme_mi_admin_ns_attach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_attach_ctrls" 9 "nvme_mi_admin_ns_attach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_attach_ctrls" 9 "nvme_mi_admin_ns_attach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_attach_ctrls \- Attach namespace to controllers
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_attach_ctrls
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_ns_detach_ctrls.2` & `libnvme-1.9/doc/man/nvme_mi_admin_ns_detach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_ns_detach_ctrls" 9 "nvme_mi_admin_ns_detach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_ns_detach_ctrls" 9 "nvme_mi_admin_ns_detach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_ns_detach_ctrls \- Detach namespace from controllers
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_ns_detach_ctrls
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_req_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_admin_req_hdr.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_admin_req_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_admin_req_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_admin_req_hdr \- Admin command request header.
 .SH SYNOPSIS
 struct nvme_mi_admin_req_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_resp_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_admin_resp_hdr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_admin_resp_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_admin_resp_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_admin_resp_hdr \- Admin command response header.
 .SH SYNOPSIS
 struct nvme_mi_admin_resp_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_sanitize_nvm.2` & `libnvme-1.9/doc/man/nvme_mi_admin_sanitize_nvm.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_sanitize_nvm" 9 "nvme_mi_admin_sanitize_nvm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_sanitize_nvm" 9 "nvme_mi_admin_sanitize_nvm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_sanitize_nvm \- Start a subsystem Sanitize operation
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_sanitize_nvm
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_sanitize_nvm_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_security_recv.2` & `libnvme-1.9/doc/man/nvme_mi_admin_security_recv.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_security_recv" 9 "nvme_mi_admin_security_recv" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_security_recv" 9 "nvme_mi_admin_security_recv" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_security_recv \- Perform a Security Receive command on a controller.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_security_recv
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_security_receive_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_security_send.2` & `libnvme-1.9/doc/man/nvme_mi_admin_security_send.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_security_send" 9 "nvme_mi_admin_security_send" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_security_send" 9 "nvme_mi_admin_security_send" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_security_send \- Perform a Security Send command on a controller.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_security_send
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_security_send_args *args "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_admin_xfer.2` & `libnvme-1.9/doc/man/nvme_mi_admin_xfer.2`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_admin_xfer" 9 "nvme_mi_admin_xfer" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_admin_xfer" 9 "nvme_mi_admin_xfer" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_admin_xfer \- Raw admin transfer interface.
 .SH SYNOPSIS
 .B "int" nvme_mi_admin_xfer
 .BI "(nvme_mi_ctrl_t ctrl "  ","
 .BI "struct nvme_mi_admin_req_hdr *admin_req "  ","
 .BI "size_t req_data_size "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_ccs.2` & `libnvme-1.9/doc/man/nvme_mi_ccs.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_ccs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_ccs" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_ccs \- Get State Control Primitive Success Response Fields - Control Primitive Specific Response
 .SH SYNOPSIS
 enum nvme_mi_ccs {
 .br
 .BI "    NVME_MI_CCS_RDY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_cmd_supported_effects.2` & `libnvme-1.9/doc/man/nvme_mi_cmd_supported_effects.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_cmd_supported_effects" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_cmd_supported_effects" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_cmd_supported_effects \- MI Command Supported and Effects Data Structure
 .SH SYNOPSIS
 enum nvme_mi_cmd_supported_effects {
 .br
 .BI "    NVME_MI_CMD_SUPPORTED_EFFECTS_CSUPP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_config_id.2` & `libnvme-1.9/doc/man/nvme_mi_config_id.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_config_id" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_config_id" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_config_id \- NVMe-MI Configuration identifier.
 .SH SYNOPSIS
 enum nvme_mi_config_id {
 .br
 .BI "    NVME_MI_CONFIG_SMBUS_FREQ"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_config_smbus_freq.2` & `libnvme-1.9/doc/man/nvme_mi_config_smbus_freq.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_config_smbus_freq" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_config_smbus_freq" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_config_smbus_freq \- SMBus/I2C frequency values
 .SH SYNOPSIS
 enum nvme_mi_config_smbus_freq {
 .br
 .BI "    NVME_MI_CONFIG_SMBUS_FREQ_100kHz"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_create_root.2` & `libnvme-1.9/doc/man/nvme_mi_create_root.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_create_root" 9 "nvme_mi_create_root" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_create_root" 9 "nvme_mi_create_root" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_create_root \- Create top-level MI (root) handle.
 .SH SYNOPSIS
 .B "nvme_root_t" nvme_mi_create_root
 .BI "(FILE *fp "  ","
 .BI "int log_level "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_csts.2` & `libnvme-1.9/doc/man/nvme_mi_csts.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_csts" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_csts" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_csts \- Controller Health Data Structure (CHDS) - Controller Status (CSTS)
 .SH SYNOPSIS
 enum nvme_mi_csts {
 .br
 .BI "    NVME_MI_CSTS_RDY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_ctrl_health_status.2` & `libnvme-1.9/doc/man/nvme_mi_ctrl_health_status.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_ctrl_health_status" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_ctrl_health_status" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_ctrl_health_status \- Controller Health Data Structure (CHDS)
 .SH SYNOPSIS
 struct nvme_mi_ctrl_health_status {
 .br
 .BI "    __le16 ctlid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_ctrl_id.2` & `libnvme-1.9/doc/man/nvme_mi_ctrl_id.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_ctrl_id" 9 "nvme_mi_ctrl_id" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_ctrl_id" 9 "nvme_mi_ctrl_id" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_ctrl_id \- get the ID of a controller
 .SH SYNOPSIS
 .B "__u16" nvme_mi_ctrl_id
 .BI "(nvme_mi_ctrl_t ctrl "  ");"
 .SH ARGUMENTS
 .IP "ctrl" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_cwarn.2` & `libnvme-1.9/doc/man/nvme_mi_cwarn.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_cwarn" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_cwarn" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_cwarn \- Controller Health Data Structure (CHDS) - Critical Warning (CWARN)
 .SH SYNOPSIS
 enum nvme_mi_cwarn {
 .br
 .BI "    NVME_MI_CWARN_ST"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_dtyp.2` & `libnvme-1.9/doc/man/nvme_mi_dtyp.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_dtyp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_dtyp" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_dtyp \- Data Structure Type field.
 .SH SYNOPSIS
 enum nvme_mi_dtyp {
 .br
 .BI "    nvme_mi_dtyp_subsys_info"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_elem.2` & `libnvme-1.9/doc/man/nvme_mi_elem.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_elem" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_elem" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_elem \- Element Descriptor Types
 .SH SYNOPSIS
 enum nvme_mi_elem {
 .br
 .BI "    NVME_MI_ELEM_EED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_init_ctrl.2` & `libnvme-1.9/doc/man/nvme_mi_init_ctrl.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_init_ctrl" 9 "nvme_mi_init_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_init_ctrl" 9 "nvme_mi_init_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_init_ctrl \- initialise a NVMe controller.
 .SH SYNOPSIS
 .B "nvme_mi_ctrl_t" nvme_mi_init_ctrl
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u16 ctrl_id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_message_type.2` & `libnvme-1.9/doc/man/nvme_mi_message_type.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_message_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_message_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_message_type \- NVMe-MI message type field.
 .SH SYNOPSIS
 enum nvme_mi_message_type {
 .br
 .BI "    NVME_MI_MT_CONTROL"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_opcode.2` & `libnvme-1.9/doc/man/nvme_mi_mi_opcode.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_mi_opcode" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_mi_opcode" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_mi_opcode \- Operation code for supported NVMe-MI commands.
 .SH SYNOPSIS
 enum nvme_mi_mi_opcode {
 .br
 .BI "    nvme_mi_mi_opcode_mi_data_read"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_ctrl.2` & `libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_ctrl.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_ctrl" 9 "nvme_mi_mi_read_mi_data_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_ctrl" 9 "nvme_mi_mi_read_mi_data_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_ctrl \- Perform a Read MI Data Structure command, retrieving controller information
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_ctrl
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u16 ctrl_id "  ","
 .BI "struct nvme_mi_read_ctrl_info *ctrl "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2` & `libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_ctrl_list.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_ctrl_list" 9 "nvme_mi_mi_read_mi_data_ctrl_list" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_ctrl_list" 9 "nvme_mi_mi_read_mi_data_ctrl_list" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_ctrl_list \- Perform a Read MI Data Structure command, retrieving the list of attached controllers.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_ctrl_list
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u8 start_ctrlid "  ","
 .BI "struct nvme_ctrl_list *list "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_port.2` & `libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_port.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_port" 9 "nvme_mi_mi_read_mi_data_port" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_port" 9 "nvme_mi_mi_read_mi_data_port" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_port \- Perform a Read MI Data Structure command, retrieving port data.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_port
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "__u8 portid "  ","
 .BI "struct nvme_mi_read_port_info *p "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_read_mi_data_subsys.2` & `libnvme-1.9/doc/man/nvme_mi_mi_read_mi_data_subsys.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_read_mi_data_subsys" 9 "nvme_mi_mi_read_mi_data_subsys" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_read_mi_data_subsys" 9 "nvme_mi_mi_read_mi_data_subsys" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_read_mi_data_subsys \- Perform a Read MI Data Structure command, retrieving subsystem data.
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_read_mi_data_subsys
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "struct nvme_mi_read_nvm_ss_info *s "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_req_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_mi_req_hdr.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_mi_req_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_mi_req_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_mi_req_hdr \- MI request message header.
 .SH SYNOPSIS
 struct nvme_mi_mi_req_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_resp_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_mi_resp_hdr.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_mi_resp_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_mi_resp_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_mi_resp_hdr \- MI response message header.
 .SH SYNOPSIS
 struct nvme_mi_mi_resp_hdr {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_mi_subsystem_health_status_poll.2` & `libnvme-1.9/doc/man/nvme_mi_mi_subsystem_health_status_poll.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_mi_subsystem_health_status_poll" 9 "nvme_mi_mi_subsystem_health_status_poll" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_mi_subsystem_health_status_poll" 9 "nvme_mi_mi_subsystem_health_status_poll" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_mi_subsystem_health_status_poll \- Read the Subsystem Health Data Structure from the NVM subsystem
 .SH SYNOPSIS
 .B "int" nvme_mi_mi_subsystem_health_status_poll
 .BI "(nvme_mi_ep_t ep "  ","
 .BI "bool clear "  ","
 .BI "struct nvme_mi_nvm_ss_health_status *nshds "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_msg_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_msg_hdr.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_msg_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_msg_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_msg_hdr \- General MI message header.
 .SH SYNOPSIS
 struct nvme_mi_msg_hdr {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_msg_resp.2` & `libnvme-1.9/doc/man/nvme_mi_msg_resp.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_msg_resp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_msg_resp" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_msg_resp \- Generic response type.
 .SH SYNOPSIS
 struct nvme_mi_msg_resp {
 .br
 .BI "    struct nvme_mi_msg_hdr hdr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_nvm_ss_health_status.2` & `libnvme-1.9/doc/man/nvme_mi_nvm_ss_health_status.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_nvm_ss_health_status" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_nvm_ss_health_status" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_nvm_ss_health_status \- Subsystem Management Data Structure
 .SH SYNOPSIS
 struct nvme_mi_nvm_ss_health_status {
 .br
 .BI "    __u8 nss;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_open_mctp.2` & `libnvme-1.9/doc/man/nvme_mi_open_mctp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_open_mctp" 9 "nvme_mi_open_mctp" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_open_mctp" 9 "nvme_mi_open_mctp" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_open_mctp \- Create an endpoint using a MCTP connection.
 .SH SYNOPSIS
 .B "nvme_mi_ep_t" nvme_mi_open_mctp
 .BI "(nvme_root_t root "  ","
 .BI "unsigned int netid "  ","
 .BI "uint8_t eid "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_port_pcie.2` & `libnvme-1.9/doc/man/nvme_mi_port_pcie.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_port_pcie" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_port_pcie" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_port_pcie \- PCIe Port Specific Data
 .SH SYNOPSIS
 struct nvme_mi_port_pcie {
 .br
 .BI "    __u8 mps;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_port_smb.2` & `libnvme-1.9/doc/man/nvme_mi_port_smb.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_port_smb" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_port_smb" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_port_smb \- SMBus Port Specific Data
 .SH SYNOPSIS
 struct nvme_mi_port_smb {
 .br
 .BI "    __u8 vpd_addr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_read_ctrl_info.2` & `libnvme-1.9/doc/man/nvme_mi_read_ctrl_info.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_read_ctrl_info" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_read_ctrl_info" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_read_ctrl_info \- Controller Information Data Structure
 .SH SYNOPSIS
 struct nvme_mi_read_ctrl_info {
 .br
 .BI "    __u8 portid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_read_port_info.2` & `libnvme-1.9/doc/man/nvme_mi_read_port_info.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_read_port_info" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_read_port_info" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_read_port_info \- Port Information Data Structure
 .SH SYNOPSIS
 struct nvme_mi_read_port_info {
 .br
 .BI "    __u8 portt;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_resp_status.2` & `libnvme-1.9/doc/man/nvme_mi_resp_status.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_mi_resp_status" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_mi_resp_status" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_mi_resp_status \- values for the response status field
 .SH SYNOPSIS
 enum nvme_mi_resp_status {
 .br
 .BI "    NVME_MI_RESP_SUCCESS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_set_probe_enabled.2` & `libnvme-1.9/doc/man/nvme_mi_set_probe_enabled.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_set_probe_enabled" 9 "nvme_mi_set_probe_enabled" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_set_probe_enabled" 9 "nvme_mi_set_probe_enabled" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_set_probe_enabled \- enable/disable the probe for new endpoints
 .SH SYNOPSIS
 .B "void" nvme_mi_set_probe_enabled
 .BI "(nvme_root_t root "  ","
 .BI "bool enabled "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_status_to_string.2` & `libnvme-1.9/doc/man/nvme_mi_status_to_string.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_mi_status_to_string" 9 "nvme_mi_status_to_string" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_mi_status_to_string" 9 "nvme_mi_status_to_string" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_mi_status_to_string \- return a string representation of the MI status.
 .SH SYNOPSIS
 .B "const char *" nvme_mi_status_to_string
 .BI "(int status "  ");"
 .SH ARGUMENTS
 .IP "status" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_vpd_hdr.2` & `libnvme-1.9/doc/man/nvme_mi_vpd_hdr.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_hdr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_hdr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_hdr \- Vital Product Data Common Header
 .SH SYNOPSIS
 struct nvme_mi_vpd_hdr {
 .br
 .BI "    __u8 ipmiver;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_vpd_mr_common.2` & `libnvme-1.9/doc/man/nvme_mi_vpd_mr_common.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_mr_common" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_mr_common" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_mr_common \- NVMe MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_mr_common {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_vpd_mra.2` & `libnvme-1.9/doc/man/nvme_mi_vpd_mra.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_mra" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_mra" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_mra \- NVMe MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_mra {
 .br
 .BI "    __u8 nmravn;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_vpd_ppmra.2` & `libnvme-1.9/doc/man/nvme_mi_vpd_ppmra.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_ppmra" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_ppmra" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_ppmra \- NVMe PCIe Port MultiRecord Area
 .SH SYNOPSIS
 struct nvme_mi_vpd_ppmra {
 .br
 .BI "    __u8 nppmravn;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_mi_vpd_telem.2` & `libnvme-1.9/doc/man/nvme_mi_vpd_telem.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_mi_vpd_telem" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_mi_vpd_telem" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_mi_vpd_telem \- Vital Product Data Element Descriptor
 .SH SYNOPSIS
 struct nvme_mi_vpd_telem {
 .br
 .BI "    __u8 type;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_namespace_attach_ctrls.2` & `libnvme-1.9/doc/man/nvme_namespace_attach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_namespace_attach_ctrls" 9 "nvme_namespace_attach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_namespace_attach_ctrls" 9 "nvme_namespace_attach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_namespace_attach_ctrls \- Attach namespace to controller(s)
 .SH SYNOPSIS
 .B "int" nvme_namespace_attach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 num_ctrls "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_namespace_detach_ctrls.2` & `libnvme-1.9/doc/man/nvme_namespace_detach_ctrls.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_namespace_detach_ctrls" 9 "nvme_namespace_detach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_namespace_detach_ctrls" 9 "nvme_namespace_detach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_namespace_detach_ctrls \- Detach namespace from controller(s)
 .SH SYNOPSIS
 .B "int" nvme_namespace_detach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 num_ctrls "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_nbft_read.2` & `libnvme-1.9/doc/man/nvme_nbft_read.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_nbft_read" 9 "nvme_nbft_read" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_nbft_read" 9 "nvme_nbft_read" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_nbft_read \- Read and parse contents of an ACPI NBFT table
 .SH SYNOPSIS
 .B "int" nvme_nbft_read
 .BI "(struct nbft_info **nbft "  ","
 .BI "const char *filename "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_nd_ns_fpi.2` & `libnvme-1.9/doc/man/nvme_nd_ns_fpi.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nd_ns_fpi" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nd_ns_fpi" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_nd_ns_fpi \- If a format operation is in progress, this field indicates the percentage of the namespace that remains to be formatted.
 .SH SYNOPSIS
 enum nvme_nd_ns_fpi {
 .br
 .BI "    NVME_NS_FPI_REMAINING"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_attach_ctrls.2` & `libnvme-1.9/doc/man/nvme_ns_attach_ctrls.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_attach_ctrls" 9 "nvme_ns_attach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ns_attach_ctrls" 9 "nvme_ns_attach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_attach_ctrls \- Attach namespace to controllers
 .SH SYNOPSIS
 .B "int" nvme_ns_attach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_detach_ctrls.2` & `libnvme-1.9/doc/man/nvme_ns_detach_ctrls.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_detach_ctrls" 9 "nvme_ns_detach_ctrls" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ns_detach_ctrls" 9 "nvme_ns_detach_ctrls" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_detach_ctrls \- Detach namespace from controllers
 .SH SYNOPSIS
 .B "int" nvme_ns_detach_ctrls
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_ctrl_list *ctrlist "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_get_fd.2` & `libnvme-1.9/doc/man/nvme_ns_get_fd.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_get_fd" 9 "nvme_ns_get_fd" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ns_get_fd" 9 "nvme_ns_get_fd" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_get_fd \- Get associated file descriptor
 .SH SYNOPSIS
 .B "int" nvme_ns_get_fd
 .BI "(nvme_ns_t n "  ");"
 .SH ARGUMENTS
 .IP "n" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_id_desc.2` & `libnvme-1.9/doc/man/nvme_ns_id_desc.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_ns_id_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_ns_id_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_ns_id_desc \- Namespace identifier type descriptor
 .SH SYNOPSIS
 struct nvme_ns_id_desc {
 .br
 .BI "    __u8 nidt;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_id_desc_nidt.2` & `libnvme-1.9/doc/man/nvme_ns_id_desc_nidt.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_id_desc_nidt" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_id_desc_nidt" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_id_desc_nidt \- Known namespace identifier types
 .SH SYNOPSIS
 enum nvme_ns_id_desc_nidt {
 .br
 .BI "    NVME_NIDT_EUI64"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_metadata_type.2` & `libnvme-1.9/doc/man/nvme_ns_metadata_type.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_metadata_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_metadata_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_metadata_type \- Namespace Metadata Element Types
 .SH SYNOPSIS
 enum nvme_ns_metadata_type {
 .br
 .BI "    NVME_NS_METADATA_OS_NS_NAME"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_mgmt_create.2` & `libnvme-1.9/doc/man/nvme_ns_mgmt_create.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_mgmt_create" 9 "nvme_ns_mgmt_create" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ns_mgmt_create" 9 "nvme_ns_mgmt_create" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_mgmt_create \- Create a non attached namespace
 .SH SYNOPSIS
 .B "int" nvme_ns_mgmt_create
 .BI "(int fd "  ","
 .BI "struct nvme_id_ns *ns "  ","
 .BI "__u32 *nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_mgmt_delete.2` & `libnvme-1.9/doc/man/nvme_ns_mgmt_delete.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_ns_mgmt_delete" 9 "nvme_ns_mgmt_delete" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_ns_mgmt_delete" 9 "nvme_ns_mgmt_delete" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_ns_mgmt_delete \- Delete a non attached namespace
 .SH SYNOPSIS
 .B "int" nvme_ns_mgmt_delete
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_mgmt_host_sw_specified.2` & `libnvme-1.9/doc/man/nvme_ns_mgmt_host_sw_specified.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_ns_mgmt_host_sw_specified" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_ns_mgmt_host_sw_specified" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_ns_mgmt_host_sw_specified \- Namespace management Host Software Specified Fields.
 .SH SYNOPSIS
 struct nvme_ns_mgmt_host_sw_specified {
 .br
 .BI "    __le64 nsze;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_ns_write_protect_cfg.2` & `libnvme-1.9/doc/man/nvme_ns_write_protect_cfg.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_ns_write_protect_cfg" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_ns_write_protect_cfg" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_ns_write_protect_cfg \- Write Protection - Write Protection State
 .SH SYNOPSIS
 enum nvme_ns_write_protect_cfg {
 .br
 .BI "    NVME_NS_WP_CFG_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_nvm_id_ns.2` & `libnvme-1.9/doc/man/nvme_nvm_id_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvm_id_ns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvm_id_ns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_nvm_id_ns \- NVME Command Set I/O Command Set Specific Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_nvm_id_ns {
 .br
 .BI "    __le64 lbstm;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_nvm_id_ns_elbaf.2` & `libnvme-1.9/doc/man/nvme_nvm_id_ns_elbaf.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvm_id_ns_elbaf" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvm_id_ns_elbaf" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_nvm_id_ns_elbaf \- This field indicates the extended LBA format
 .SH SYNOPSIS
 enum nvme_nvm_id_ns_elbaf {
 .br
 .BI "    NVME_NVM_ELBAF_STS_MASK"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_nvm_identify_ctrl.2` & `libnvme-1.9/doc/man/nvme_nvm_identify_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_nvm_identify_ctrl" 9 "nvme_nvm_identify_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_nvm_identify_ctrl" 9 "nvme_nvm_identify_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_nvm_identify_ctrl \- Identify controller data
 .SH SYNOPSIS
 .B "int" nvme_nvm_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_id_ctrl_nvm *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_nvmeset_pl_status.2` & `libnvme-1.9/doc/man/nvme_nvmeset_pl_status.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvmeset_pl_status" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvmeset_pl_status" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_nvmeset_pl_status \- Predictable Latency Per NVM Set Log - Status
 .SH SYNOPSIS
 enum nvme_nvmeset_pl_status {
 .br
 .BI "    NVME_NVMSET_PL_STATUS_DISABLED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_nvmset_attr.2` & `libnvme-1.9/doc/man/nvme_nvmset_attr.2`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvmset_attr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvmset_attr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_nvmset_attr \- NVM Set Attributes Entry
 .SH SYNOPSIS
 struct nvme_nvmset_attr {
 .br
 .BI "    __le16 nvmsetid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_nvmset_pl_events.2` & `libnvme-1.9/doc/man/nvme_nvmset_pl_events.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_nvmset_pl_events" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_nvmset_pl_events" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_nvmset_pl_events \- Predictable Latency Per NVM Set Log - Event Type
 .SH SYNOPSIS
 enum nvme_nvmset_pl_events {
 .br
 .BI "    NVME_NVMSET_PL_EVENT_DTWIN_READ_WARN"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_nvmset_predictable_lat_log.2` & `libnvme-1.9/doc/man/nvme_nvmset_predictable_lat_log.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_nvmset_predictable_lat_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_nvmset_predictable_lat_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_nvmset_predictable_lat_log \- Predictable Latency Mode - Deterministic Threshold Configuration Data
 .SH SYNOPSIS
 struct nvme_nvmset_predictable_lat_log {
 .br
 .BI "    __u8 status;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_passthru_cmd.2` & `libnvme-1.9/doc/man/nvme_passthru_cmd.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_passthru_cmd" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_passthru_cmd" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_passthru_cmd \- nvme passthrough command structure
 .SH SYNOPSIS
 struct nvme_passthru_cmd {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_passthru_cmd64.2` & `libnvme-1.9/doc/man/nvme_passthru_cmd64.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_passthru_cmd64" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_passthru_cmd64" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_passthru_cmd64 \- 64-bit nvme passthrough command structure
 .SH SYNOPSIS
 struct nvme_passthru_cmd64 {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_persistent_event_entry.2` & `libnvme-1.9/doc/man/nvme_persistent_event_entry.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_persistent_event_entry" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_persistent_event_entry" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_persistent_event_entry \- Persistent Event
 .SH SYNOPSIS
 struct nvme_persistent_event_entry {
 .br
 .BI "    __u8 etype;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_persistent_event_log.2` & `libnvme-1.9/doc/man/nvme_persistent_event_log.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_persistent_event_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_persistent_event_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_persistent_event_log \- Persistent Event Log
 .SH SYNOPSIS
 struct nvme_persistent_event_log {
 .br
 .BI "    __u8 lid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_persistent_event_types.2` & `libnvme-1.9/doc/man/nvme_persistent_event_types.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_persistent_event_types" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_persistent_event_types" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_persistent_event_types \- Persistent event log events
 .SH SYNOPSIS
 enum nvme_persistent_event_types {
 .br
 .BI "    NVME_PEL_SMART_HEALTH_EVENT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_pevent_log_action.2` & `libnvme-1.9/doc/man/nvme_pevent_log_action.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_pevent_log_action" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_pevent_log_action" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_pevent_log_action \- Persistent Event Log - Action
 .SH SYNOPSIS
 enum nvme_pevent_log_action {
 .br
 .BI "    NVME_PEVENT_LOG_READ"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_phy_rx_eom_log.2` & `libnvme-1.9/doc/man/nvme_phy_rx_eom_log.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_phy_rx_eom_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_phy_rx_eom_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_phy_rx_eom_log \- Physical Interface Receiver Eye Opening Measurement Log
 .SH SYNOPSIS
 struct nvme_phy_rx_eom_log {
 .br
 .BI "    __u8 lid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_plm_config.2` & `libnvme-1.9/doc/man/nvme_plm_config.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_plm_config" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_plm_config" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_plm_config \- Predictable Latency Mode - Deterministic Threshold Configuration Data Structure
 .SH SYNOPSIS
 struct nvme_plm_config {
 .br
 .BI "    __le16 ee;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_power_on_reset_info_list.2` & `libnvme-1.9/doc/man/nvme_power_on_reset_info_list.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_power_on_reset_info_list" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_power_on_reset_info_list" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_power_on_reset_info_list \- Controller Reset Information
 .SH SYNOPSIS
 struct nvme_power_on_reset_info_list {
 .br
 .BI "    __le16 cid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_primary_ctrl_cap.2` & `libnvme-1.9/doc/man/nvme_primary_ctrl_cap.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_primary_ctrl_cap" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_primary_ctrl_cap" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_primary_ctrl_cap \- Identify - Controller Capabilities Structure
 .SH SYNOPSIS
 struct nvme_primary_ctrl_cap {
 .br
 .BI "    __le16 cntlid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_psd_flags.2` & `libnvme-1.9/doc/man/nvme_psd_flags.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_flags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_flags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_flags \- Possible flag values in nvme power state descriptor
 .SH SYNOPSIS
 enum nvme_psd_flags {
 .br
 .BI "    NVME_PSD_FLAGS_MXPS"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_psd_ps.2` & `libnvme-1.9/doc/man/nvme_psd_ps.2`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_ps" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_ps" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_ps \- Known values for &struct nvme_psd %ips and %aps. Use with nvme_psd_power_scale() to extract the power scale field to match this enum.
 .SH SYNOPSIS
 enum nvme_psd_ps {
 .br
 .BI "    NVME_PSD_PS_NOT_REPORTED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_psd_workload.2` & `libnvme-1.9/doc/man/nvme_psd_workload.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_psd_workload" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_psd_workload" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_psd_workload \- Specifies a workload hint in the Power Management Feature (see &struct nvme_psd.apw) to inform the NVM subsystem or indicate the conditions for the active power level.
 .SH SYNOPSIS
 enum nvme_psd_workload {
 .br
 .BI "    NVME_PSD_WORKLOAD_NP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_register_offsets.2` & `libnvme-1.9/doc/man/nvme_register_offsets.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_register_offsets" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_register_offsets" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_register_offsets \- controller registers for all transports. This is the layout of BAR0/1 for PCIe, and properties for fabrics.
 .SH SYNOPSIS
 enum nvme_register_offsets {
 .br
 .BI "    NVME_REG_CAP"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_registered_ctrl.2` & `libnvme-1.9/doc/man/nvme_registered_ctrl.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_registered_ctrl" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_registered_ctrl" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_registered_ctrl \- Registered Controller Data Structure
 .SH SYNOPSIS
 struct nvme_registered_ctrl {
 .br
 .BI "    __le16 cntlid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_registered_ctrl_ext.2` & `libnvme-1.9/doc/man/nvme_registered_ctrl_ext.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_registered_ctrl_ext" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_registered_ctrl_ext" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_registered_ctrl_ext \- Registered Controller Extended Data Structure
 .SH SYNOPSIS
 struct nvme_registered_ctrl_ext {
 .br
 .BI "    __le16 cntlid;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_acquire.2` & `libnvme-1.9/doc/man/nvme_resv_acquire.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_acquire" 9 "nvme_resv_acquire" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_resv_acquire" 9 "nvme_resv_acquire" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_acquire \- Send an nvme reservation acquire
 .SH SYNOPSIS
 .B "int" nvme_resv_acquire
 .BI "(struct nvme_resv_acquire_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_cptpl.2` & `libnvme-1.9/doc/man/nvme_resv_cptpl.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_cptpl" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_cptpl" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_cptpl \- Reservation Register - Change Persist Through Power Loss State
 .SH SYNOPSIS
 enum nvme_resv_cptpl {
 .br
 .BI "    NVME_RESERVATION_CPTPL_NO_CHANGE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_notification_log.2` & `libnvme-1.9/doc/man/nvme_resv_notification_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_resv_notification_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_resv_notification_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_resv_notification_log \- Reservation Notification Log
 .SH SYNOPSIS
 struct nvme_resv_notification_log {
 .br
 .BI "    __le64 lpc;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_notify_rnlpt.2` & `libnvme-1.9/doc/man/nvme_resv_notify_rnlpt.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_notify_rnlpt" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_notify_rnlpt" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_notify_rnlpt \- Reservation Notification Log - Reservation Notification Log Page Type
 .SH SYNOPSIS
 enum nvme_resv_notify_rnlpt {
 .br
 .BI "    NVME_RESV_NOTIFY_RNLPT_EMPTY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_racqa.2` & `libnvme-1.9/doc/man/nvme_resv_racqa.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_racqa" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_racqa" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_racqa \- Reservation Acquire - Reservation Acquire Action
 .SH SYNOPSIS
 enum nvme_resv_racqa {
 .br
 .BI "    NVME_RESERVATION_RACQA_ACQUIRE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_register.2` & `libnvme-1.9/doc/man/nvme_resv_register.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_register" 9 "nvme_resv_register" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_resv_register" 9 "nvme_resv_register" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_register \- Send an nvme reservation register
 .SH SYNOPSIS
 .B "int" nvme_resv_register
 .BI "(struct nvme_resv_register_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_report.2` & `libnvme-1.9/doc/man/nvme_resv_report.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_resv_report" 9 "nvme_resv_report" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_resv_report" 9 "nvme_resv_report" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_resv_report \- Send an nvme reservation report
 .SH SYNOPSIS
 .B "int" nvme_resv_report
 .BI "(struct nvme_resv_report_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_rrega.2` & `libnvme-1.9/doc/man/nvme_resv_rrega.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_rrega" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_rrega" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_rrega \- Reservation Register - Reservation Register Action
 .SH SYNOPSIS
 enum nvme_resv_rrega {
 .br
 .BI "    NVME_RESERVATION_RREGA_REGISTER_KEY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_rtype.2` & `libnvme-1.9/doc/man/nvme_resv_rtype.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_resv_rtype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_resv_rtype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_resv_rtype \- Reservation Type Encoding
 .SH SYNOPSIS
 enum nvme_resv_rtype {
 .br
 .BI "    NVME_RESERVATION_RTYPE_WE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_resv_status.2` & `libnvme-1.9/doc/man/nvme_resv_status.2`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_resv_status" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_resv_status" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_resv_status \- Reservation Status Data Structure
 .SH SYNOPSIS
 struct nvme_resv_status {
 .br
 .BI "    __le32 gen;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_sanitize_log_page.2` & `libnvme-1.9/doc/man/nvme_sanitize_log_page.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_sanitize_log_page" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_sanitize_log_page" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_sanitize_log_page \- Sanitize Status (Log Identifier 81h)
 .SH SYNOPSIS
 struct nvme_sanitize_log_page {
 .br
 .BI "    __le16 sprog;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_sanitize_nvm.2` & `libnvme-1.9/doc/man/nvme_sanitize_nvm.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_sanitize_nvm" 9 "nvme_sanitize_nvm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_sanitize_nvm" 9 "nvme_sanitize_nvm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_sanitize_nvm \- Start a sanitize operation
 .SH SYNOPSIS
 .B "int" nvme_sanitize_nvm
 .BI "(struct nvme_sanitize_nvm_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_sanitize_sanact.2` & `libnvme-1.9/doc/man/nvme_sanitize_sanact.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_sanitize_sanact" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_sanitize_sanact" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_sanitize_sanact \- Sanitize Action
 .SH SYNOPSIS
 enum nvme_sanitize_sanact {
 .br
 .BI "    NVME_SANITIZE_SANACT_EXIT_FAILURE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_sanitize_sstat.2` & `libnvme-1.9/doc/man/nvme_sanitize_sstat.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_sanitize_sstat" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_sanitize_sstat" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_sanitize_sstat \- Sanitize Status (SSTAT)
 .SH SYNOPSIS
 enum nvme_sanitize_sstat {
 .br
 .BI "    NVME_SANITIZE_SSTAT_STATUS_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_scan_topology.2` & `libnvme-1.9/doc/man/nvme_scan_topology.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_scan_topology" 9 "nvme_scan_topology" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_scan_topology" 9 "nvme_scan_topology" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_scan_topology \- Scan NVMe topology and apply filter
 .SH SYNOPSIS
 .B "int" nvme_scan_topology
 .BI "(nvme_root_t r "  ","
 .BI "nvme_scan_filter_t f "  ","
 .BI "void *f_args "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_security_send.2` & `libnvme-1.9/doc/man/nvme_security_send.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_security_send" 9 "nvme_security_send" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_security_send" 9 "nvme_security_send" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_security_send \- Security Send command
 .SH SYNOPSIS
 .B "int" nvme_security_send
 .BI "(struct nvme_security_send_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_self_test_log.2` & `libnvme-1.9/doc/man/nvme_self_test_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_self_test_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_self_test_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_self_test_log \- Device Self-test (Log Identifier 06h)
 .SH SYNOPSIS
 struct nvme_self_test_log {
 .br
 .BI "    __u8 current_operation;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_arbitration.2` & `libnvme-1.9/doc/man/nvme_set_features_arbitration.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_arbitration" 9 "nvme_set_features_arbitration" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_arbitration" 9 "nvme_set_features_arbitration" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_arbitration \- Set arbitration features
 .SH SYNOPSIS
 .B "int" nvme_set_features_arbitration
 .BI "(int fd "  ","
 .BI "__u8 ab "  ","
 .BI "__u8 lpw "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_async_event.2` & `libnvme-1.9/doc/man/nvme_set_features_auto_pst.2`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-.TH "nvme_set_features_async_event" 9 "nvme_set_features_async_event" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_auto_pst" 9 "nvme_set_features_auto_pst" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_async_event \- Set asynchronous event feature
+nvme_set_features_auto_pst \- Set autonomous power state feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_async_event
+.B "int" nvme_set_features_auto_pst
 .BI "(int fd "  ","
-.BI "__u32 events "  ","
+.BI "bool apste "  ","
 .BI "bool save "  ","
+.BI "struct nvme_feat_auto_pst *apst "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "events" 12
-Events to enable
+.IP "apste" 12
+Autonomous Power State Transition Enable
 .IP "save" 12
 Save value across power states
+.IP "apst" 12
+Autonomous Power State Transition
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_auto_pst.2` & `libnvme-1.9/doc/man/nvme_set_features_write_protect2.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.TH "nvme_set_features_auto_pst" 9 "nvme_set_features_auto_pst" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_write_protect2" 9 "nvme_set_features_write_protect2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_auto_pst \- Set autonomous power state feature
+nvme_set_features_write_protect2 \- Set write protect feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_auto_pst
+.B "int" nvme_set_features_write_protect2
 .BI "(int fd "  ","
-.BI "bool apste "  ","
+.BI "__u32 nsid "  ","
+.BI "enum nvme_feat_nswpcfg_state state "  ","
 .BI "bool save "  ","
-.BI "struct nvme_feat_auto_pst *apst "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "apste" 12
-Autonomous Power State Transition Enable
+.IP "nsid" 12
+Namespace ID
+.IP "state" 12
+Write Protection State
 .IP "save" 12
 Save value across power states
-.IP "apst" 12
-Autonomous Power State Transition
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_data.2` & `libnvme-1.9/doc/man/nvme_set_features_data.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_data" 9 "nvme_set_features_data" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_data" 9 "nvme_set_features_data" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_data \- Helper function for @nvme_set_features()
 .SH SYNOPSIS
 .B "int" nvme_set_features_data
 .BI "(int fd "  ","
 .BI "__u8 fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_endurance_evt_cfg.2` & `libnvme-1.9/doc/man/nvme_set_features_lba_range.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-.TH "nvme_set_features_endurance_evt_cfg" 9 "nvme_set_features_endurance_evt_cfg" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_lba_range" 9 "nvme_set_features_lba_range" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_endurance_evt_cfg \- Set endurance event config feature
+nvme_set_features_lba_range \- Set LBA range feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_endurance_evt_cfg
+.B "int" nvme_set_features_lba_range
 .BI "(int fd "  ","
-.BI "__u16 endgid "  ","
-.BI "__u8 egwarn "  ","
+.BI "__u32 nsid "  ","
+.BI "__u8 nr_ranges "  ","
 .BI "bool save "  ","
+.BI "struct nvme_lba_range_type *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "endgid" 12
-Endurance Group Identifier
-.IP "egwarn" 12
-Flags to enable warning, see \fIenum nvme_eg_critical_warning_flags\fP
+.IP "nsid" 12
+Namespace ID
+.IP "nr_ranges" 12
+Number of ranges in \fIdata\fP
 .IP "save" 12
 Save value across power states
+.IP "data" 12
+User address of feature data
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_err_recovery.2` & `libnvme-1.9/doc/man/nvme_set_features_err_recovery.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_err_recovery" 9 "nvme_set_features_err_recovery" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_err_recovery" 9 "nvme_set_features_err_recovery" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_err_recovery \- Set error recovery feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_err_recovery
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u16 tler "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_hctm.2` & `libnvme-1.9/doc/man/nvme_set_features_hctm.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_hctm" 9 "nvme_set_features_hctm" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_hctm" 9 "nvme_set_features_hctm" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_hctm \- Set thermal management feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_hctm
 .BI "(int fd "  ","
 .BI "__u16 tmt2 "  ","
 .BI "__u16 tmt1 "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_host_behavior.2` & `libnvme-1.9/doc/man/nvme_set_features_host_behavior.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_host_behavior" 9 "nvme_set_features_host_behavior" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_host_behavior" 9 "nvme_set_features_host_behavior" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_host_behavior \- Set host behavior feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_host_behavior
 .BI "(int fd "  ","
 .BI "bool save "  ","
 .BI "struct nvme_feat_host_behavior *data "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_host_id.2` & `libnvme-1.9/doc/man/nvme_set_features_host_id.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_host_id" 9 "nvme_set_features_host_id" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_host_id" 9 "nvme_set_features_host_id" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_host_id \- Set enable extended host identifiers feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_host_id
 .BI "(int fd "  ","
 .BI "bool exhid "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_iocs_profile.2` & `libnvme-1.9/doc/man/nvme_set_features_iocs_profile.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_iocs_profile" 9 "nvme_set_features_iocs_profile" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_iocs_profile" 9 "nvme_set_features_iocs_profile" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_iocs_profile \- Set I/O command set profile feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_iocs_profile
 .BI "(int fd "  ","
 .BI "__u16 iocsi "  ","
 .BI "bool save "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_irq_coalesce.2` & `libnvme-1.9/doc/man/nvme_set_features_irq_coalesce.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_irq_coalesce" 9 "nvme_set_features_irq_coalesce" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_irq_coalesce" 9 "nvme_set_features_irq_coalesce" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_irq_coalesce \- Set IRQ coalesce feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_irq_coalesce
 .BI "(int fd "  ","
 .BI "__u8 thr "  ","
 .BI "__u8 time "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_irq_config.2` & `libnvme-1.9/doc/man/nvme_set_features_irq_config.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_irq_config" 9 "nvme_set_features_irq_config" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_irq_config" 9 "nvme_set_features_irq_config" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_irq_config \- Set IRQ config feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_irq_config
 .BI "(int fd "  ","
 .BI "__u16 iv "  ","
 .BI "bool cd "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_lba_range.2` & `libnvme-1.9/doc/man/nvme_set_features_nopsc.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-.TH "nvme_set_features_lba_range" 9 "nvme_set_features_lba_range" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_nopsc" 9 "nvme_set_features_nopsc" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_lba_range \- Set LBA range feature
+nvme_set_features_nopsc \- Set non-operational power state feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_lba_range
+.B "int" nvme_set_features_nopsc
 .BI "(int fd "  ","
-.BI "__u32 nsid "  ","
-.BI "__u8 nr_ranges "  ","
+.BI "bool noppme "  ","
 .BI "bool save "  ","
-.BI "struct nvme_lba_range_type *data "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "nsid" 12
-Namespace ID
-.IP "nr_ranges" 12
-Number of ranges in \fIdata\fP
+.IP "noppme" 12
+Non-Operational Power State Permissive Mode Enable
 .IP "save" 12
 Save value across power states
-.IP "data" 12
-User address of feature data
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_lba_sts_interval.2` & `libnvme-1.9/doc/man/nvme_set_features_lba_sts_interval.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_lba_sts_interval" 9 "nvme_set_features_lba_sts_interval" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_lba_sts_interval" 9 "nvme_set_features_lba_sts_interval" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_lba_sts_interval \- Set LBA status information feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_lba_sts_interval
 .BI "(int fd "  ","
 .BI "__u16 lsiri "  ","
 .BI "__u16 lsipi "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_nopsc.2` & `libnvme-1.9/doc/man/nvme_set_features_rrl.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-.TH "nvme_set_features_nopsc" 9 "nvme_set_features_nopsc" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_rrl" 9 "nvme_set_features_rrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_nopsc \- Set non-operational power state feature
+nvme_set_features_rrl \- Set read recovery level feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_nopsc
+.B "int" nvme_set_features_rrl
 .BI "(int fd "  ","
-.BI "bool noppme "  ","
+.BI "__u8 rrl "  ","
+.BI "__u16 nvmsetid "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "noppme" 12
-Non-Operational Power State Permissive Mode Enable
+.IP "rrl" 12
+Read recovery level setting
+.IP "nvmsetid" 12
+NVM set id
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_plm_config.2` & `libnvme-1.9/doc/man/nvme_set_features_plm_config.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_plm_config" 9 "nvme_set_features_plm_config" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_plm_config" 9 "nvme_set_features_plm_config" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_plm_config \- Set predictable latency feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_plm_config
 .BI "(int fd "  ","
 .BI "bool enable "  ","
 .BI "__u16 nvmsetid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_plm_window.2` & `libnvme-1.9/doc/man/nvme_set_features_resv_mask.2`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-.TH "nvme_set_features_plm_window" 9 "nvme_set_features_plm_window" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_mask" 9 "nvme_set_features_resv_mask" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_plm_window \- Set window select feature
+nvme_set_features_resv_mask \- Set reservation notification mask feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_plm_window
+.B "int" nvme_set_features_resv_mask
 .BI "(int fd "  ","
-.BI "enum nvme_feat_plm_window_select sel "  ","
-.BI "__u16 nvmsetid "  ","
+.BI "__u32 mask "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "sel" 12
-Window Select
-.IP "nvmsetid" 12
-NVM Set Identifier
+.IP "mask" 12
+Reservation Notification Mask Field
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
+.SH "DESCRIPTION"
+
+Deprecated: doesn't support specifying a NSID.
+Use \fBnvme_set_features_resv_mask2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_power_mgmt.2` & `libnvme-1.9/doc/man/nvme_set_features_power_mgmt.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_power_mgmt" 9 "nvme_set_features_power_mgmt" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_power_mgmt" 9 "nvme_set_features_power_mgmt" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_power_mgmt \- Set power management feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_power_mgmt
 .BI "(int fd "  ","
 .BI "__u8 ps "  ","
 .BI "__u8 wh "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_resv_mask.2` & `libnvme-1.9/doc/man/nvme_set_features_resv_mask2.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-.TH "nvme_set_features_resv_mask" 9 "nvme_set_features_resv_mask" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_mask2" 9 "nvme_set_features_resv_mask2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_resv_mask \- Set reservation notification mask feature
+nvme_set_features_resv_mask2 \- Set reservation notification mask feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_resv_mask
+.B "int" nvme_set_features_resv_mask2
 .BI "(int fd "  ","
+.BI "__u32 nsid "  ","
 .BI "__u32 mask "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
+.IP "nsid" 12
+Namespace ID
 .IP "mask" 12
 Reservation Notification Mask Field
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
-.SH "DESCRIPTION"
-
-Deprecated: doesn't support specifying a NSID.
-Use \fBnvme_set_features_resv_mask2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_resv_persist.2` & `libnvme-1.9/doc/man/nvme_set_features_resv_persist.2`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_resv_persist" 9 "nvme_set_features_resv_persist" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_persist" 9 "nvme_set_features_resv_persist" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_resv_persist \- Set persist through power loss feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_resv_persist
 .BI "(int fd "  ","
 .BI "bool ptpl "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_resv_persist2.2` & `libnvme-1.9/doc/man/nvme_set_features_resv_persist2.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_resv_persist2" 9 "nvme_set_features_resv_persist2" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_resv_persist2" 9 "nvme_set_features_resv_persist2" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_resv_persist2 \- Set persist through power loss feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_resv_persist2
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "bool ptpl "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_sanitize.2` & `libnvme-1.9/doc/man/nvme_set_features_sanitize.2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_sanitize" 9 "nvme_set_features_sanitize" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_sanitize" 9 "nvme_set_features_sanitize" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_sanitize \- Set sanitize feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_sanitize
 .BI "(int fd "  ","
 .BI "bool nodrm "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_simple.2` & `libnvme-1.9/doc/man/nvme_set_features_simple.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_simple" 9 "nvme_set_features_simple" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_simple" 9 "nvme_set_features_simple" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_simple \- Helper function for @nvme_set_features()
 .SH SYNOPSIS
 .B "int" nvme_set_features_simple
 .BI "(int fd "  ","
 .BI "__u8 fid "  ","
 .BI "__u32 nsid "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_sw_progress.2` & `libnvme-1.9/doc/man/nvme_set_features_sw_progress.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_sw_progress" 9 "nvme_set_features_sw_progress" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_sw_progress" 9 "nvme_set_features_sw_progress" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_sw_progress \- Set pre-boot software load count feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_sw_progress
 .BI "(int fd "  ","
 .BI "__u8 pbslc "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_temp_thresh.2` & `libnvme-1.9/doc/man/nvme_set_features_temp_thresh.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_temp_thresh" 9 "nvme_set_features_temp_thresh" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_temp_thresh" 9 "nvme_set_features_temp_thresh" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_temp_thresh \- Set temperature threshold feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_temp_thresh
 .BI "(int fd "  ","
 .BI "__u16 tmpth "  ","
 .BI "__u8 tmpsel "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_timestamp.2` & `libnvme-1.9/doc/man/nvme_set_features_timestamp.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_timestamp" 9 "nvme_set_features_timestamp" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_timestamp" 9 "nvme_set_features_timestamp" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_timestamp \- Set timestamp feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_timestamp
 .BI "(int fd "  ","
 .BI "bool save "  ","
 .BI "__u64 timestamp "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_volatile_wc.2` & `libnvme-1.9/doc/man/nvme_set_features_volatile_wc.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_features_volatile_wc" 9 "nvme_set_features_volatile_wc" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_volatile_wc" 9 "nvme_set_features_volatile_wc" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_features_volatile_wc \- Set volatile write cache feature
 .SH SYNOPSIS
 .B "int" nvme_set_features_volatile_wc
 .BI "(int fd "  ","
 .BI "bool wce "  ","
 .BI "bool save "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_write_atomic.2` & `libnvme-1.9/doc/man/nvme_set_features_write_protect.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-.TH "nvme_set_features_write_atomic" 9 "nvme_set_features_write_atomic" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_write_protect" 9 "nvme_set_features_write_protect" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_write_atomic \- Set write atomic feature
+nvme_set_features_write_protect \- Set write protect feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_write_atomic
+.B "int" nvme_set_features_write_protect
 .BI "(int fd "  ","
-.BI "bool dn "  ","
+.BI "enum nvme_feat_nswpcfg_state state "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "dn" 12
-Disable Normal
+.IP "state" 12
+Write Protection State
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
+.SH "DESCRIPTION"
+
+Deprecated: doesn't support specifying a NSID.
+Use \fBnvme_set_features_write_protect2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_features_write_protect.2` & `libnvme-1.9/doc/man/nvme_set_features_endurance_evt_cfg.2`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-.TH "nvme_set_features_write_protect" 9 "nvme_set_features_write_protect" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_features_endurance_evt_cfg" 9 "nvme_set_features_endurance_evt_cfg" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_set_features_write_protect \- Set write protect feature
+nvme_set_features_endurance_evt_cfg \- Set endurance event config feature
 .SH SYNOPSIS
-.B "int" nvme_set_features_write_protect
+.B "int" nvme_set_features_endurance_evt_cfg
 .BI "(int fd "  ","
-.BI "enum nvme_feat_nswpcfg_state state "  ","
+.BI "__u16 endgid "  ","
+.BI "__u8 egwarn "  ","
 .BI "bool save "  ","
 .BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
-.IP "state" 12
-Write Protection State
+.IP "endgid" 12
+Endurance Group Identifier
+.IP "egwarn" 12
+Flags to enable warning, see \fIenum nvme_eg_critical_warning_flags\fP
 .IP "save" 12
 Save value across power states
 .IP "result" 12
 The command completion result from CQE dword0
-.SH "DESCRIPTION"
-
-Deprecated: doesn't support specifying a NSID.
-Use \fBnvme_set_features_write_protect2\fP instead.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_set_property.2` & `libnvme-1.9/doc/man/nvme_set_property.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_property" 9 "nvme_set_property" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_property" 9 "nvme_set_property" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_property \- Set controller property
 .SH SYNOPSIS
 .B "int" nvme_set_property
 .BI "(struct nvme_set_property_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_set_root.2` & `libnvme-1.9/doc/man/nvme_set_root.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_set_root" 9 "nvme_set_root" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_set_root" 9 "nvme_set_root" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_set_root \- Set nvme_root_t context
 .SH SYNOPSIS
 .B "void" nvme_set_root
 .BI "(nvme_root_t r "  ");"
 .SH ARGUMENTS
 .IP "r" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_smart_crit.2` & `libnvme-1.9/doc/man/nvme_smart_crit.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_smart_crit" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_smart_crit" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_smart_crit \- Critical Warning
 .SH SYNOPSIS
 enum nvme_smart_crit {
 .br
 .BI "    NVME_SMART_CRIT_SPARE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_smart_egcw.2` & `libnvme-1.9/doc/man/nvme_smart_egcw.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_smart_egcw" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_smart_egcw" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_smart_egcw \- Endurance Group Critical Warning Summary
 .SH SYNOPSIS
 enum nvme_smart_egcw {
 .br
 .BI "    NVME_SMART_EGCW_SPARE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_smart_log.2` & `libnvme-1.9/doc/man/nvme_smart_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_smart_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_smart_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_smart_log \- SMART / Health Information Log (Log Identifier 02h)
 .SH SYNOPSIS
 struct nvme_smart_log {
 .br
 .BI "    __u8 critical_warning;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_st_code.2` & `libnvme-1.9/doc/man/nvme_st_code.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_code" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_code" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_st_code \- Self-test Code value
 .SH SYNOPSIS
 enum nvme_st_code {
 .br
 .BI "    NVME_ST_CODE_RESERVED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_st_curr_op.2` & `libnvme-1.9/doc/man/nvme_st_curr_op.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_curr_op" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_curr_op" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_st_curr_op \- Current Device Self-Test Operation
 .SH SYNOPSIS
 enum nvme_st_curr_op {
 .br
 .BI "    NVME_ST_CURR_OP_NOT_RUNNING"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_st_result.2` & `libnvme-1.9/doc/man/nvme_st_result.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_st_result" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_st_result" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_st_result \- Self-test Result
 .SH SYNOPSIS
 struct nvme_st_result {
 .br
 .BI "    __u8 dsts;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_st_valid_diag_info.2` & `libnvme-1.9/doc/man/nvme_st_valid_diag_info.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_st_valid_diag_info" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_st_valid_diag_info" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_st_valid_diag_info \- Valid Diagnostic Information
 .SH SYNOPSIS
 enum nvme_st_valid_diag_info {
 .br
 .BI "    NVME_ST_VALID_DIAG_INFO_NSID"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_status_equals.2` & `libnvme-1.9/doc/man/nvme_status_equals.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_equals" 9 "nvme_status_equals" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_status_equals" 9 "nvme_status_equals" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_equals \- helper to check a status against a type and value
 .SH SYNOPSIS
 .B "__u32" nvme_status_equals
 .BI "(int status "  ","
 .BI "enum nvme_status_type type "  ","
 .BI "unsigned int value "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_status_field.2` & `libnvme-1.9/doc/man/nvme_status_field.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_field" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_field" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_status_field \- Defines all parts of the nvme status field: status code, status code type, and additional flags.
 .SH SYNOPSIS
 enum nvme_status_field {
 .br
 .BI "    NVME_SCT_GENERIC"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_status_result.2` & `libnvme-1.9/doc/man/nvme_status_result.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_result" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_result" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_status_result \- Result of the device self-test operation
 .SH SYNOPSIS
 enum nvme_status_result {
 .br
 .BI "    NVME_ST_RESULT_NO_ERR"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_status_to_errno.2` & `libnvme-1.9/doc/man/nvme_status_to_errno.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_to_errno" 9 "nvme_status_to_errno" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_status_to_errno" 9 "nvme_status_to_errno" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_to_errno \- Converts nvme return status to errno
 .SH SYNOPSIS
 .B "__u8" nvme_status_to_errno
 .BI "(int status "  ","
 .BI "bool fabrics "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_status_to_string.2` & `libnvme-1.9/doc/man/nvme_status_to_string.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_status_to_string" 9 "nvme_status_to_string" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_status_to_string" 9 "nvme_status_to_string" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_status_to_string \- Returns string describing nvme return status.
 .SH SYNOPSIS
 .B "const char *" nvme_status_to_string
 .BI "(int status "  ","
 .BI "bool fabrics "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_status_type.2` & `libnvme-1.9/doc/man/nvme_status_type.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_status_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_status_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_status_type \- type encoding for NVMe return values, when represented as an int.
 .SH SYNOPSIS
 enum nvme_status_type {
 .br
 .BI "    NVME_STATUS_TYPE_SHIFT"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_streams_directive_params.2` & `libnvme-1.9/doc/man/nvme_streams_directive_params.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_streams_directive_params" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_streams_directive_params" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_streams_directive_params \- Streams Directive - Return Parameters Data Structure
 .SH SYNOPSIS
 struct nvme_streams_directive_params {
 .br
 .BI "    __le16 msl;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_submit_admin_passthru.2` & `libnvme-1.9/doc/man/nvme_submit_admin_passthru64.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.TH "nvme_submit_admin_passthru" 9 "nvme_submit_admin_passthru" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_submit_admin_passthru64" 9 "nvme_submit_admin_passthru64" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_submit_admin_passthru \- Submit an nvme passthrough admin command
+nvme_submit_admin_passthru64 \- Submit a 64-bit nvme passthrough admin command
 .SH SYNOPSIS
-.B "int" nvme_submit_admin_passthru
+.B "int" nvme_submit_admin_passthru64
 .BI "(int fd "  ","
-.BI "struct nvme_passthru_cmd *cmd "  ","
-.BI "__u32 *result "  ");"
+.BI "struct nvme_passthru_cmd64 *cmd "  ","
+.BI "__u64 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "cmd" 12
 The nvme admin command to send
 .IP "result" 12
-Optional field to return the result from the CQE DW0
+Optional field to return the result from the CQE DW0-1
 .SH "DESCRIPTION"
-Uses NVME_IOCTL_ADMIN_CMD for the ioctl request.
+Uses NVME_IOCTL_ADMIN64_CMD for the ioctl request.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_submit_admin_passthru64.2` & `libnvme-1.9/doc/man/nvme_submit_admin_passthru.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-.TH "nvme_submit_admin_passthru64" 9 "nvme_submit_admin_passthru64" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_submit_admin_passthru" 9 "nvme_submit_admin_passthru" "May 2024" "libnvme API manual" LINUX
 .SH NAME
-nvme_submit_admin_passthru64 \- Submit a 64-bit nvme passthrough admin command
+nvme_submit_admin_passthru \- Submit an nvme passthrough admin command
 .SH SYNOPSIS
-.B "int" nvme_submit_admin_passthru64
+.B "int" nvme_submit_admin_passthru
 .BI "(int fd "  ","
-.BI "struct nvme_passthru_cmd64 *cmd "  ","
-.BI "__u64 *result "  ");"
+.BI "struct nvme_passthru_cmd *cmd "  ","
+.BI "__u32 *result "  ");"
 .SH ARGUMENTS
 .IP "fd" 12
 File descriptor of nvme device
 .IP "cmd" 12
 The nvme admin command to send
 .IP "result" 12
-Optional field to return the result from the CQE DW0-1
+Optional field to return the result from the CQE DW0
 .SH "DESCRIPTION"
-Uses NVME_IOCTL_ADMIN64_CMD for the ioctl request.
+Uses NVME_IOCTL_ADMIN_CMD for the ioctl request.
 .SH "RETURN"
 The nvme command status if a response was received (see
 \fIenum nvme_status_field\fP) or -1 with errno set otherwise.
```

### Comparing `libnvme-1.8/doc/man/nvme_submit_io_passthru.2` & `libnvme-1.9/doc/man/nvme_submit_io_passthru.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_submit_io_passthru" 9 "nvme_submit_io_passthru" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_submit_io_passthru" 9 "nvme_submit_io_passthru" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_submit_io_passthru \- Submit an nvme passthrough command
 .SH SYNOPSIS
 .B "int" nvme_submit_io_passthru
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd *cmd "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_submit_io_passthru64.2` & `libnvme-1.9/doc/man/nvme_submit_io_passthru64.2`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_submit_io_passthru64" 9 "nvme_submit_io_passthru64" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_submit_io_passthru64" 9 "nvme_submit_io_passthru64" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_submit_io_passthru64 \- Submit a 64-bit nvme passthrough command
 .SH SYNOPSIS
 .B "int" nvme_submit_io_passthru64
 .BI "(int fd "  ","
 .BI "struct nvme_passthru_cmd64 *cmd "  ","
 .BI "__u64 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_subsys_type.2` & `libnvme-1.9/doc/man/nvme_subsys_type.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_subsys_type" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_subsys_type" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_subsys_type \- Type of the NVM subsystem.
 .SH SYNOPSIS
 enum nvme_subsys_type {
 .br
 .BI "    NVME_NQN_DISC"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_supported_cap_config_list_log.2` & `libnvme-1.9/doc/man/nvme_supported_cap_config_list_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_supported_cap_config_list_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_supported_cap_config_list_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_supported_cap_config_list_log \- Supported Capacity Configuration list log page
 .SH SYNOPSIS
 struct nvme_supported_cap_config_list_log {
 .br
 .BI "    __u8 sccn;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_telemetry_log.2` & `libnvme-1.9/doc/man/nvme_telemetry_log.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_telemetry_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_telemetry_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_telemetry_log \- Retrieve internal data specific to the manufacturer.
 .SH SYNOPSIS
 struct nvme_telemetry_log {
 .br
 .BI "    __u8 lpi;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_uring_cmd.2` & `libnvme-1.9/doc/man/nvme_uring_cmd.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_uring_cmd" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_uring_cmd" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_uring_cmd \- nvme uring command structure
 .SH SYNOPSIS
 struct nvme_uring_cmd {
 .br
 .BI "    __u8 opcode;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_verify.2` & `libnvme-1.9/doc/man/nvme_verify.2`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_verify" 9 "nvme_verify" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_verify" 9 "nvme_verify" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_verify \- Send an nvme verify command
 .SH SYNOPSIS
 .B "int" nvme_verify
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_virt_mgmt_act.2` & `libnvme-1.9/doc/man/nvme_virt_mgmt_act.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_virt_mgmt_act" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_virt_mgmt_act" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_virt_mgmt_act \- Virtualization Management - Action
 .SH SYNOPSIS
 enum nvme_virt_mgmt_act {
 .br
 .BI "    NVME_VIRT_MGMT_ACT_PRIM_CTRL_FLEX_ALLOC"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_virtual_mgmt.2` & `libnvme-1.9/doc/man/nvme_virtual_mgmt.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_virtual_mgmt" 9 "nvme_virtual_mgmt" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_virtual_mgmt" 9 "nvme_virtual_mgmt" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_virtual_mgmt \- Virtualization resource management
 .SH SYNOPSIS
 .B "int" nvme_virtual_mgmt
 .BI "(struct nvme_virtual_mgmt_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_write_uncorrectable.2` & `libnvme-1.9/doc/man/nvme_write_uncorrectable.2`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_write_uncorrectable" 9 "nvme_write_uncorrectable" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_write_uncorrectable" 9 "nvme_write_uncorrectable" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_write_uncorrectable \- Submit an nvme write uncorrectable command
 .SH SYNOPSIS
 .B "int" nvme_write_uncorrectable
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_write_zeros.2` & `libnvme-1.9/doc/man/nvme_write_zeros.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_write_zeros" 9 "nvme_write_zeros" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_write_zeros" 9 "nvme_write_zeros" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_write_zeros \- Submit an nvme write zeroes command
 .SH SYNOPSIS
 .B "int" nvme_write_zeros
 .BI "(struct nvme_io_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_desc.2` & `libnvme-1.9/doc/man/nvme_zns_desc.2`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_zns_desc" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_zns_desc" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_zns_desc \- Zone Descriptor Data Structure
 .SH SYNOPSIS
 struct nvme_zns_desc {
 .br
 .BI "    __u8 zt;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_id_ns.2` & `libnvme-1.9/doc/man/nvme_zns_id_ns.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvme_zns_id_ns" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvme_zns_id_ns" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvme_zns_id_ns \- Zoned Namespace Command Set Specific Identify Namespace Data Structure
 .SH SYNOPSIS
 struct nvme_zns_id_ns {
 .br
 .BI "    __le16 zoc;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_identify_ctrl.2` & `libnvme-1.9/doc/man/nvme_zns_identify_ctrl.2`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_identify_ctrl" 9 "nvme_zns_identify_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_zns_identify_ctrl" 9 "nvme_zns_identify_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_identify_ctrl \- ZNS identify controller data
 .SH SYNOPSIS
 .B "int" nvme_zns_identify_ctrl
 .BI "(int fd "  ","
 .BI "struct nvme_zns_id_ctrl *id "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_identify_ns.2` & `libnvme-1.9/doc/man/nvme_zns_identify_ns.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_identify_ns" 9 "nvme_zns_identify_ns" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_zns_identify_ns" 9 "nvme_zns_identify_ns" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_identify_ns \- ZNS identify namespace data
 .SH SYNOPSIS
 .B "int" nvme_zns_identify_ns
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "struct nvme_zns_id_ns *data "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_report_options.2` & `libnvme-1.9/doc/man/nvme_zns_report_options.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_report_options" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_report_options" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_report_options \- Zone Management Receive - Zone Receive Action Specific Field
 .SH SYNOPSIS
 enum nvme_zns_report_options {
 .br
 .BI "    NVME_ZNS_ZRAS_REPORT_ALL"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_report_zones.2` & `libnvme-1.9/doc/man/nvme_zns_report_zones.2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvme_zns_report_zones" 9 "nvme_zns_report_zones" "February 2024" "libnvme API manual" LINUX
+.TH "nvme_zns_report_zones" 9 "nvme_zns_report_zones" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvme_zns_report_zones \- Return the list of zones
 .SH SYNOPSIS
 .B "int" nvme_zns_report_zones
 .BI "(int fd "  ","
 .BI "__u32 nsid "  ","
 .BI "__u64 slba "  ","
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_send_action.2` & `libnvme-1.9/doc/man/nvme_zns_send_action.2`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_send_action" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_send_action" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_send_action \- Zone Management Send - Zone Send Action
 .SH SYNOPSIS
 enum nvme_zns_send_action {
 .br
 .BI "    NVME_ZNS_ZSA_CLOSE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_za.2` & `libnvme-1.9/doc/man/nvme_zns_za.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_za" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_za" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_za \- Zone Descriptor Data Structure
 .SH SYNOPSIS
 enum nvme_zns_za {
 .br
 .BI "    NVME_ZNS_ZA_ZFC"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvme_zns_zs.2` & `libnvme-1.9/doc/man/nvme_zns_zs.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvme_zns_zs" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvme_zns_zs" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvme_zns_zs \- Zone Descriptor Data Structure - Zone State
 .SH SYNOPSIS
 enum nvme_zns_zs {
 .br
 .BI "    NVME_ZNS_ZS_EMPTY"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_add_ctrl.2` & `libnvme-1.9/doc/man/nvmf_add_ctrl.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_add_ctrl" 9 "nvmf_add_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_add_ctrl" 9 "nvmf_add_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_add_ctrl \- Connect a controller and update topology
 .SH SYNOPSIS
 .B "int" nvmf_add_ctrl
 .BI "(nvme_host_t h "  ","
 .BI "nvme_ctrl_t c "  ","
 .BI "const struct nvme_fabrics_config *cfg "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvmf_addr_family.2` & `libnvme-1.9/doc/man/nvmf_addr_family.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_addr_family" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_addr_family" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_addr_family \- Address Family codes for Discovery Log Page entry ADRFAM field
 .SH SYNOPSIS
 enum nvmf_addr_family {
 .br
 .BI "    NVMF_ADDR_FAMILY_PCI"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_connect_data.2` & `libnvme-1.9/doc/man/nvmf_connect_data.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_connect_data" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_connect_data" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_connect_data \- Data payload for the 'connect' command
 .SH SYNOPSIS
 struct nvmf_connect_data {
 .br
 .BI "    __u8 hostid[16];"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_connect_disc_entry.2` & `libnvme-1.9/doc/man/nvmf_connect_disc_entry.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_connect_disc_entry" 9 "nvmf_connect_disc_entry" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_connect_disc_entry" 9 "nvmf_connect_disc_entry" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_connect_disc_entry \- Connect controller based on the discovery log page entry
 .SH SYNOPSIS
 .B "nvme_ctrl_t" nvmf_connect_disc_entry
 .BI "(nvme_host_t h "  ","
 .BI "struct nvmf_disc_log_entry *e "  ","
 .BI "const struct nvme_fabrics_config *defcfg "  ","
```

### Comparing `libnvme-1.8/doc/man/nvmf_dim_data.2` & `libnvme-1.9/doc/man/nvmf_dim_data.2`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_dim_data" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_dim_data" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_dim_data \- Discovery Information Management (DIM) - Data
 .SH SYNOPSIS
 struct nvmf_dim_data {
 .br
 .BI "    __le32 tdl;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_disc_eflags.2` & `libnvme-1.9/doc/man/nvmf_disc_eflags.2`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_disc_eflags" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_disc_eflags" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_disc_eflags \- Discovery Log Page entry flags.
 .SH SYNOPSIS
 enum nvmf_disc_eflags {
 .br
 .BI "    NVMF_DISC_EFLAGS_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_disc_log_entry.2` & `libnvme-1.9/doc/man/nvmf_disc_log_entry.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_disc_log_entry" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_disc_log_entry" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_disc_log_entry \- Discovery Log Page entry
 .SH SYNOPSIS
 struct nvmf_disc_log_entry {
 .br
 .BI "    __u8 trtype;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_discovery_log.2` & `libnvme-1.9/doc/man/nvmf_discovery_log.2`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_discovery_log" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_discovery_log" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_discovery_log \- Discovery Log Page (Log Identifier 70h)
 .SH SYNOPSIS
 struct nvmf_discovery_log {
 .br
 .BI "    __le64 genctr;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_ext_attr.2` & `libnvme-1.9/doc/man/nvmf_ext_attr.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_ext_attr" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_ext_attr" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_ext_attr \- Extended Attribute (EXAT)
 .SH SYNOPSIS
 struct nvmf_ext_attr {
 .br
 .BI "    __le16 exattype;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_ext_die.2` & `libnvme-1.9/doc/man/nvmf_ext_die.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "struct nvmf_ext_die" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "struct nvmf_ext_die" "May 2024" "API Manual" LINUX
 .SH NAME
 struct nvmf_ext_die \- Extended Discovery Information Entry (DIE)
 .SH SYNOPSIS
 struct nvmf_ext_die {
 .br
 .BI "    __u8 trtype;"
 .br
```

### Comparing `libnvme-1.8/doc/man/nvmf_get_discovery_log.2` & `libnvme-1.9/doc/man/nvmf_get_discovery_log.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_get_discovery_log" 9 "nvmf_get_discovery_log" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_get_discovery_log" 9 "nvmf_get_discovery_log" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_get_discovery_log \- Return the discovery log page
 .SH SYNOPSIS
 .B "int" nvmf_get_discovery_log
 .BI "(nvme_ctrl_t c "  ","
 .BI "struct nvmf_discovery_log **logp "  ","
 .BI "int max_retries "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvmf_get_discovery_wargs.2` & `libnvme-1.9/doc/man/nvmf_get_discovery_wargs.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_get_discovery_wargs" 9 "nvmf_get_discovery_wargs" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_get_discovery_wargs" 9 "nvmf_get_discovery_wargs" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_get_discovery_wargs \- Get the discovery log page with args
 .SH SYNOPSIS
 .B "struct nvmf_discovery_log *" nvmf_get_discovery_wargs
 .BI "(struct nvme_get_discovery_args *args "  ");"
 .SH ARGUMENTS
 .IP "args" 12
```

### Comparing `libnvme-1.8/doc/man/nvmf_log_discovery_lid_support.2` & `libnvme-1.9/doc/man/nvmf_log_discovery_lid_support.2`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_log_discovery_lid_support" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_log_discovery_lid_support" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_log_discovery_lid_support \- Discovery log specific support
 .SH SYNOPSIS
 enum nvmf_log_discovery_lid_support {
 .br
 .BI "    NVMF_LOG_DISC_LID_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_log_discovery_lsp.2` & `libnvme-1.9/doc/man/nvmf_log_discovery_lsp.2`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_log_discovery_lsp" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_log_discovery_lsp" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_log_discovery_lsp \- Discovery log specific field
 .SH SYNOPSIS
 enum nvmf_log_discovery_lsp {
 .br
 .BI "    NVMF_LOG_DISC_LSP_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_rdma_prtype.2` & `libnvme-1.9/doc/man/nvmf_rdma_prtype.2`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_rdma_prtype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_rdma_prtype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_rdma_prtype \- RDMA Provider Type codes for Discovery Log Page entry TSAS RDMA_PRTYPE field
 .SH SYNOPSIS
 enum nvmf_rdma_prtype {
 .br
 .BI "    NVMF_RDMA_PRTYPE_NOT_SPECIFIED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_register_ctrl.2` & `libnvme-1.9/doc/man/nvmf_register_ctrl.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_register_ctrl" 9 "nvmf_register_ctrl" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_register_ctrl" 9 "nvmf_register_ctrl" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_register_ctrl \- Perform registration task with a DC
 .SH SYNOPSIS
 .B "int" nvmf_register_ctrl
 .BI "(nvme_ctrl_t c "  ","
 .BI "enum nvmf_dim_tas tas "  ","
 .BI "__u32 *result "  ");"
```

### Comparing `libnvme-1.8/doc/man/nvmf_tcp_sectype.2` & `libnvme-1.9/doc/man/nvmf_tcp_sectype.2`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_tcp_sectype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_tcp_sectype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_tcp_sectype \- Transport Specific Address Subtype Definition for NVMe/TCP Transport
 .SH SYNOPSIS
 enum nvmf_tcp_sectype {
 .br
 .BI "    NVMF_TCP_SECTYPE_NONE"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_treq.2` & `libnvme-1.9/doc/man/nvmf_treq.2`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_treq" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_treq" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_treq \- Transport Requirements codes for Discovery Log Page entry TREQ field
 .SH SYNOPSIS
 enum nvmf_treq {
 .br
 .BI "    NVMF_TREQ_NOT_SPECIFIED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_trtype.2` & `libnvme-1.9/doc/man/nvmf_trtype.2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "libnvme" 9 "enum nvmf_trtype" "February 2024" "API Manual" LINUX
+.TH "libnvme" 9 "enum nvmf_trtype" "May 2024" "API Manual" LINUX
 .SH NAME
 enum nvmf_trtype \- Transport Type codes for Discovery Log Page entry TRTYPE field
 .SH SYNOPSIS
 enum nvmf_trtype {
 .br
 .BI "    NVMF_TRTYPE_UNSPECIFIED"
 ,
```

### Comparing `libnvme-1.8/doc/man/nvmf_update_config.2` & `libnvme-1.9/doc/man/nvmf_update_config.2`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "nvmf_update_config" 9 "nvmf_update_config" "February 2024" "libnvme API manual" LINUX
+.TH "nvmf_update_config" 9 "nvmf_update_config" "May 2024" "libnvme API manual" LINUX
 .SH NAME
 nvmf_update_config \- Update fabrics configuration values
 .SH SYNOPSIS
 .B "void" nvmf_update_config
 .BI "(nvme_ctrl_t c "  ","
 .BI "const struct nvme_fabrics_config *cfg "  ");"
 .SH ARGUMENTS
```

### Comparing `libnvme-1.8/doc/meson.build` & `libnvme-1.9/doc/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/mi.rst.in` & `libnvme-1.9/doc/mi.rst.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/rst/fabrics.rst` & `libnvme-1.9/doc/rst/fabrics.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     int reconnect_delay;
     int ctrl_loss_tmo;
     int fast_io_fail_tmo;
     int keep_alive_tmo;
     int nr_write_queues;
     int nr_poll_queues;
     int tos;
-    int keyring;
-    int tls_key;
+    long keyring;
+    long tls_key;
     bool duplicate_connect;
     bool disable_sqflow;
     bool hdr_digest;
     bool data_digest;
     bool tls;
     bool concat;
   };
```

### Comparing `libnvme-1.8/doc/rst/filters.rst` & `libnvme-1.9/doc/rst/filters.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/rst/ioctl.rst` & `libnvme-1.9/doc/rst/ioctl.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4214,14 +4214,42 @@
 
 **Return**
 
 The nvme command status if a response was received (see
 :c:type:`enum nvme_status_field <nvme_status_field>`) or -1 with errno set otherwise.
 
 
+.. c:function:: int nvme_ns_mgmt_delete_timeout (int fd, __u32 nsid, __u32 timeout)
+
+   Delete a non attached namespace with timeout
+
+**Parameters**
+
+``int fd``
+  File descriptor of nvme device
+
+``__u32 nsid``
+  Namespace identifier to delete
+
+``__u32 timeout``
+  Override the default timeout to this value in milliseconds;
+  set to 0 to use the system default.
+
+**Description**
+
+It is recommended that a namespace being deleted is not attached to any
+controller. Use the nvme_ns_detach_ctrls() first if the namespace is still
+attached.
+
+**Return**
+
+The nvme command status if a response was received (see
+:c:type:`enum nvme_status_field <nvme_status_field>`) or -1 with errno set otherwise.
+
+
 .. c:function:: int nvme_ns_mgmt_delete (int fd, __u32 nsid)
 
    Delete a non attached namespace
 
 **Parameters**
 
 ``int fd``
@@ -5197,31 +5225,7 @@
 
 **Return**
 
 The nvme command status if a response was received (see
 :c:type:`enum nvme_status_field <nvme_status_field>`) or -1 with errno set otherwise.
 
 
-.. c:function:: void nvme_set_debug (bool debug)
-
-   Set NVMe command debugging output
-
-**Parameters**
-
-``bool debug``
-  true to enable or false to disable
-
-
-.. c:function:: bool nvme_get_debug (void)
-
-   Get NVMe command debugging output
-
-**Parameters**
-
-``void``
-  no arguments
-
-**Return**
-
-false if disabled or true if enabled.
-
-
```

### Comparing `libnvme-1.8/doc/rst/linux.rst` & `libnvme-1.9/doc/rst/linux.rst`

 * *Files 22% similar despite different names*

```diff
@@ -459,14 +459,135 @@
 
 **Return**
 
 0 on success, a negative number on error
 with errno set.
 
 
+.. c:function:: unsigned char * nvme_read_key (long keyring_id, long key_id, int *len)
+
+   Read key raw data
+
+**Parameters**
+
+``long keyring_id``
+  Id of the keyring holding ``key_id``
+
+``long key_id``
+  Key id
+
+``int *len``
+  Length of the returned data
+
+**Description**
+
+Links the keyring specified by **keyring_id** into the session
+keyring and reads the payload of the key specified by **key_id**.
+**len** holds the size of the returned buffer.
+If **keyring** is 0 the default keyring '.nvme' is used.
+
+**Return**
+
+Pointer to the payload on success,
+or NULL with errno set otherwise.
+
+
+.. c:function:: long nvme_update_key (long keyring_id, const char *key_type, const char *identity, unsigned char *key_data, int key_len)
+
+   Update key raw data
+
+**Parameters**
+
+``long keyring_id``
+  Id of the keyring holding ``key_id``
+
+``const char *key_type``
+  Type of the key to insert
+
+``const char *identity``
+  Key identity string
+
+``unsigned char *key_data``
+  Raw data of the key
+
+``int key_len``
+  Length of **key_data**
+
+**Description**
+
+Links the keyring specified by **keyring_id** into the session
+keyring and updates the key reference by **identity** with **key_data**.
+The old key with identity **identity** will be revoked to make it
+inaccessible.
+
+**Return**
+
+Key id of the new key or 0 with errno set otherwise.
+
+
+.. c:macro:: nvme_scan_tls_keys_cb_t
+
+   **Typedef**: Callback for iterating TLS keys
+
+
+**Syntax**
+
+  ``void nvme_scan_tls_keys_cb_t (long keyring, long key, char *desc, int desc_len, void *data)``
+
+**Parameters**
+
+``long keyring``
+  Keyring which has been iterated
+
+``long key``
+  Key for which the callback has been invoked
+
+``char *desc``
+  Description of the key
+
+``int desc_len``
+  Length of **desc**
+
+``void *data``
+  Pointer for caller data
+
+**Description**
+
+Called for each TLS PSK in the keyring.
+
+
+.. c:function:: int nvme_scan_tls_keys (const char *keyring, nvme_scan_tls_keys_cb_t cb, void *data)
+
+   Iterate over TLS keys in a keyring
+
+**Parameters**
+
+``const char *keyring``
+  Keyring holding TLS keys
+
+``nvme_scan_tls_keys_cb_t cb``
+  Callback function
+
+``void *data``
+  Pointer for data to be passed to **cb**
+
+**Description**
+
+Iterates **keyring** and call **cb** for each TLS key. When **keyring** is NULL
+the default '.nvme' keyring is used.
+A TLS key must be of type 'psk' and the description must be of the
+form 'NVMe<0|1><R|G>0<1|2> <identity>', otherwise it will be skipped
+during iteration.
+
+**Return**
+
+Number of keys for which **cb** was called, or -1 with errno set
+on error.
+
+
 .. c:function:: long nvme_insert_tls_key (const char *keyring, const char *key_type, const char *hostnqn, const char *subsysnqn, int hmac, unsigned char *configured_key, int key_len)
 
    Derive and insert TLS key
 
 **Parameters**
 
 ``const char *keyring``
@@ -574,7 +695,115 @@
 
 **Return**
 
 The string containing the TLS identity. It is the responsibility
 of the caller to free the returned string.
 
 
+.. c:function:: char * nvme_export_tls_key (const unsigned char *key_data, int key_len)
+
+   Export a TLS key
+
+**Parameters**
+
+``const unsigned char *key_data``
+  Raw data of the key
+
+``int key_len``
+  Length of **key_data**
+
+**Description**
+
+Returns **key_data** in the PSK Interchange format as defined in section
+3.6.1.5 of the NVMe TCP Transport specification.
+
+**Return**
+
+The string containing the TLS identity or NULL with errno set
+on error. It is the responsibility of the caller to free the returned
+string.
+
+
+.. c:function:: unsigned char * nvme_import_tls_key (const char *encoded_key, int *key_len, unsigned int *hmac)
+
+   Import a TLS key
+
+**Parameters**
+
+``const char *encoded_key``
+  TLS key in PSK interchange format
+
+``int *key_len``
+  Length of the resulting key data
+
+``unsigned int *hmac``
+  HMAC algorithm
+
+**Description**
+
+Imports **key_data** in the PSK Interchange format as defined in section
+3.6.1.5 of the NVMe TCP Transport specification.
+
+**Return**
+
+The raw data of the PSK or NULL with errno set on error. It is
+the responsibility of the caller to free the returned string.
+
+
+.. c:function:: int nvme_submit_passthru (int fd, unsigned long ioctl_cmd, struct nvme_passthru_cmd *cmd, __u32 *result)
+
+   Low level ioctl wrapper for passthru commands
+
+**Parameters**
+
+``int fd``
+  File descriptor of the nvme device
+
+``unsigned long ioctl_cmd``
+  IOCTL command id
+
+``struct nvme_passthru_cmd *cmd``
+  Passhtru command
+
+``__u32 *result``
+  Optional field to return the result
+
+**Description**
+
+This is a low level library function which should not be used directly. It is
+exposed as weak symbol so that the user application is able to provide their own
+implementation of this function with additional debugging or logging code.
+
+**Return**
+
+The value from the ioctl system call (see ioctl documentation)
+
+
+.. c:function:: int nvme_submit_passthru64 (int fd, unsigned long ioctl_cmd, struct nvme_passthru_cmd64 *cmd, __u64 *result)
+
+   Low level ioctl wrapper for passthru commands
+
+**Parameters**
+
+``int fd``
+  File descriptor of the nvme device
+
+``unsigned long ioctl_cmd``
+  IOCTL command id
+
+``struct nvme_passthru_cmd64 *cmd``
+  Passhtru command
+
+``__u64 *result``
+  Optional field to return the result
+
+**Description**
+
+This is a low level library function which should not be used directly. It is
+exposed as weak symbol so that the user application is able to provide their own
+implementation of this function with additional debugging or logging code.
+
+**Return**
+
+The value from the ioctl system call (see ioctl documentation)
+
+
```

### Comparing `libnvme-1.8/doc/rst/meson.build` & `libnvme-1.9/doc/rst/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/rst/mi.rst` & `libnvme-1.9/doc/rst/mi.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/doc/rst/nbft.rst` & `libnvme-1.9/doc/rst/nbft.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+.. _nbft.h:
+
+**nbft.h**
+
+
+NVM Express Boot Specification, Revision 1.0
+
+Note: this API is currently unstable, subject to further additions.
+
 
 
 .. c:enum:: nbft_desc_type
 
    NBFT Elements - Descriptor Types (Figure 5)
 
 **Constants**
@@ -1712,14 +1721,16 @@
     __u8 *nid;
     char *subsys_nqn;
     bool pdu_header_digest_required;
     bool data_digest_required;
     int controller_id;
     int asqsz;
     char *dhcp_root_path_string;
+    bool discovered;
+    bool unavailable;
   };
 
 **Members**
 
 ``index``
   SSNS Descriptor Index in the descriptor list.
 
@@ -1781,14 +1792,22 @@
   Admin Submission Queue Size (SSNS Extended Information
   Descriptor) or 0 if not supported.
 
 ``dhcp_root_path_string``
   DHCP Root Path Override string (SSNS Extended
   Information Descriptor).
 
+``discovered``
+  Indicates that this namespace was acquired
+  through discovery.
+
+``unavailable``
+  Namespace is unavailable as indicated by
+  the pre-OS driver.
+
 
 
 
 
 .. c:struct:: nbft_info
 
    The parsed NBFT table data.
```

### Comparing `libnvme-1.8/doc/rst/tree.rst` & `libnvme-1.9/doc/rst/tree.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1725,14 +1725,28 @@
   Controller to be checked
 
 **Return**
 
 DH-HMAC-CHAP host key or NULL if not set
 
 
+.. c:function:: const char * nvme_ctrl_get_cntlid (nvme_ctrl_t c)
+
+   Controller id
+
+**Parameters**
+
+``nvme_ctrl_t c``
+  Controller to be checked
+
+**Return**
+
+Controller id of **c**
+
+
 .. c:function:: void nvme_ctrl_set_dhchap_host_key (nvme_ctrl_t c, const char *key)
 
    Set host key
 
 **Parameters**
 
 ``nvme_ctrl_t c``
```

### Comparing `libnvme-1.8/doc/rst/types.rst` & `libnvme-1.9/doc/rst/types.rst`

 * *Files 5% similar despite different names*

```diff
@@ -292,42 +292,936 @@
 Location) register is not supported by fabrics, but it can be checked here.
 
 **Return**
 
 true if given offset is 64bit register, otherwise it returns false.
 
 
+
+
+.. c:enum:: nvme_cap
+
+   This field indicates the controller capabilities register
+
+**Constants**
+
+``NVME_CAP_MQES_SHIFT``
+  Shift amount to get the maximum queue entries supported
+
+``NVME_CAP_CQR_SHIFT``
+  Shift amount to get the contiguous queues required
+
+``NVME_CAP_AMS_SHIFT``
+  Shift amount to get the arbitration mechanism supported
+
+``NVME_CAP_TO_SHIFT``
+  Shift amount to get the timeout
+
+``NVME_CAP_DSTRD_SHIFT``
+  Shift amount to get the doorbell stride
+
+``NVME_CAP_NSSRC_SHIFT``
+  Shift amount to get the NVM subsystem reset supported
+
+``NVME_CAP_CSS_SHIFT``
+  Shift amount to get the command sets supported
+
+``NVME_CAP_BPS_SHIFT``
+  Shift amount to get the boot partition support
+
+``NVME_CAP_CPS_SHIFT``
+  Shift amount to get the controller power scope
+
+``NVME_CAP_MPSMIN_SHIFT``
+  Shift amount to get the memory page size minimum
+
+``NVME_CAP_MPSMAX_SHIFT``
+  Shift amount to get the memory page size maximum
+
+``NVME_CAP_PMRS_SHIFT``
+  Shift amount to get the persistent memory region supported
+
+``NVME_CAP_CMBS_SHIFT``
+  Shift amount to get the controller memory buffer supported
+
+``NVME_CAP_NSSS_SHIFT``
+  Shift amount to get the NVM subsystem shutdown supported
+
+``NVME_CAP_CRMS_SHIFT``
+  Shift amount to get the controller ready modes supported
+
+``NVME_CAP_MQES_MASK``
+  Mask to get the maximum queue entries supported
+
+``NVME_CAP_CQR_MASK``
+  Mask to get the contiguous queues required
+
+``NVME_CAP_AMS_MASK``
+  Mask to get the arbitration mechanism supported
+
+``NVME_CAP_TO_MASK``
+  Mask to get the timeout
+
+``NVME_CAP_DSTRD_MASK``
+  Mask to get the doorbell stride
+
+``NVME_CAP_NSSRC_MASK``
+  Mask to get the NVM subsystem reset supported
+
+``NVME_CAP_CSS_MASK``
+  Mask to get the command sets supported
+
+``NVME_CAP_BPS_MASK``
+  Mask to get the boot partition support
+
+``NVME_CAP_CPS_MASK``
+  Mask to get the controller power scope
+
+``NVME_CAP_MPSMIN_MASK``
+  Mask to get the memory page size minimum
+
+``NVME_CAP_MPSMAX_MASK``
+  Mask to get the memory page size maximum
+
+``NVME_CAP_PMRS_MASK``
+  Mask to get the persistent memory region supported
+
+``NVME_CAP_CMBS_MASK``
+  Mask to get the controller memory buffer supported
+
+``NVME_CAP_NSSS_MASK``
+  Mask to get the NVM subsystem shutdown supported
+
+``NVME_CAP_CRMS_MASK``
+  Mask to get the controller ready modes supported
+
+``NVME_CAP_AMS_WRR``
+  Weighted round robin with urgent priority class
+
+``NVME_CAP_AMS_VS``
+  Vendor specific
+
+``NVME_CAP_CSS_NVM``
+  NVM command set or a discovery controller
+
+``NVME_CAP_CSS_CSI``
+  Controller supports one or more I/O command sets
+
+``NVME_CAP_CSS_ADMIN``
+  No I/O command set is supported
+
+``NVME_CAP_CPS_NONE``
+  Not reported
+
+``NVME_CAP_CPS_CTRL``
+  Controller scope
+
+``NVME_CAP_CPS_DOMAIN``
+  Domain scope
+
+``NVME_CAP_CPS_NVMS``
+  NVM subsystem scope
+
+``NVME_CAP_CRWMS``
+  Controller ready with media support
+
+``NVME_CAP_CRIMS``
+  Controller ready independent of media support
+
+
+
+
+.. c:enum:: nvme_vs
+
+   This field indicates the version
+
+**Constants**
+
+``NVME_VS_TER_SHIFT``
+  Shift amount to get the tertiary version
+
+``NVME_VS_MNR_SHIFT``
+  Shift amount to get the minor version
+
+``NVME_VS_MJR_SHIFT``
+  Shift amount to get the major version
+
+``NVME_VS_TER_MASK``
+  Mask to get the tertiary version
+
+``NVME_VS_MNR_MASK``
+  Mask to get the minor version
+
+``NVME_VS_MJR_MASK``
+  Mask to get the major version
+
+
+
+
+.. c:enum:: nvme_cc
+
+   This field indicates the controller configuration
+
+**Constants**
+
+``NVME_CC_EN_SHIFT``
+  Shift amount to get the enable
+
+``NVME_CC_CSS_SHIFT``
+  Shift amount to get the I/O command set selected
+
+``NVME_CC_MPS_SHIFT``
+  Shift amount to get the memory page size
+
+``NVME_CC_AMS_SHIFT``
+  Shift amount to get the arbitration mechanism selected
+
+``NVME_CC_SHN_SHIFT``
+  Shift amount to get the shutdown notification
+
+``NVME_CC_IOSQES_SHIFT``
+  Shift amount to get the I/O submission queue entry size
+
+``NVME_CC_IOCQES_SHIFT``
+  Shift amount to get the I/O completion queue entry size
+
+``NVME_CC_CRIME_SHIFT``
+  Shift amount to get the controller ready independent of media enable
+
+``NVME_CC_EN_MASK``
+  Mask to get the enable
+
+``NVME_CC_CSS_MASK``
+  Mask to get the I/O command set selected
+
+``NVME_CC_MPS_MASK``
+  Mask to get the memory page size
+
+``NVME_CC_AMS_MASK``
+  Mask to get the arbitration mechanism selected
+
+``NVME_CC_SHN_MASK``
+  Mask to get the shutdown notification
+
+``NVME_CC_CRIME_MASK``
+  Mask to get the I/O submission queue entry size
+
+``NVME_CC_IOSQES_MASK``
+  Mask to get the I/O completion queue entry size
+
+``NVME_CC_IOCQES_MASK``
+  Mask to get the controller ready independent of media enable
+
+``NVME_CC_CSS_NVM``
+  NVM command set
+
+``NVME_CC_CSS_CSI``
+  All supported I/O command sets
+
+``NVME_CC_CSS_ADMIN``
+  Admin command set only
+
+``NVME_CC_AMS_RR``
+  Round robin
+
+``NVME_CC_AMS_WRRU``
+  Weighted round robin with urgent priority class
+
+``NVME_CC_AMS_VS``
+  Vendor specific
+
+``NVME_CC_SHN_NONE``
+  No notification; no effect
+
+``NVME_CC_SHN_NORMAL``
+  Normal shutdown notification
+
+``NVME_CC_SHN_ABRUPT``
+  Abrupt shutdown notification
+
+``NVME_CC_CRWME``
+  Controller ready with media enable
+
+``NVME_CC_CRIME``
+  Controller ready independent of media enable
+
+
+
+
+.. c:enum:: nvme_csts
+
+   This field indicates the controller status register
+
+**Constants**
+
+``NVME_CSTS_RDY_SHIFT``
+  Shift amount to get the ready
+
+``NVME_CSTS_CFS_SHIFT``
+  Shift amount to get the controller fatal status
+
+``NVME_CSTS_SHST_SHIFT``
+  Shift amount to get the shutdown status
+
+``NVME_CSTS_NSSRO_SHIFT``
+  Shift amount to get the NVM subsystem reset occurred
+
+``NVME_CSTS_PP_SHIFT``
+  Shift amount to get the processing paused
+
+``NVME_CSTS_ST_SHIFT``
+  Shift amount to get the shutdown type
+
+``NVME_CSTS_RDY_MASK``
+  Mask to get the ready
+
+``NVME_CSTS_CFS_MASK``
+  Mask to get the controller fatal status
+
+``NVME_CSTS_SHST_MASK``
+  Mask to get the shutdown status
+
+``NVME_CSTS_NSSRO_MASK``
+  Mask to get the NVM subsystem reset occurred
+
+``NVME_CSTS_PP_MASK``
+  Mask to get the processing paused
+
+``NVME_CSTS_ST_MASK``
+  Mask to get the shutdown type
+
+``NVME_CSTS_SHST_NORMAL``
+  Normal operation
+
+``NVME_CSTS_SHST_OCCUR``
+  Shutdown processing occurring
+
+``NVME_CSTS_SHST_CMPLT``
+  Shutdown processing complete
+
+``NVME_CSTS_SHN_MASK``
+  Deprecated mask to get the shutdown status
+
+
+
+
+.. c:enum:: nvme_aqa
+
+   This field indicates the admin queue attributes
+
+**Constants**
+
+``NVME_AQA_ASQS_SHIFT``
+  Shift amount to get the admin submission queue size
+
+``NVME_AQA_ACQS_SHIFT``
+  Shift amount to get the admin completion queue size
+
+``NVME_AQA_ASQS_MASK``
+  Mask to get the admin submission queue size
+
+``NVME_AQA_ACQS_MASK``
+  Mask to get the admin completion queue size
+
+
+
+
+.. c:enum:: nvme_asq
+
+   This field indicates the admin submission queue base address
+
+**Constants**
+
+``NVME_ASQ_ASQB_SHIFT``
+  Shift amount to get the admin submission queue base
+
+
+
+
+.. c:enum:: nvme_acq
+
+   This field indicates the admin completion queue base address
+
+**Constants**
+
+``NVME_ACQ_ACQB_SHIFT``
+  Shift amount to get the admin completion queue base
+
+
+
+
+.. c:enum:: nvme_cmbloc
+
+   This field indicates the controller memory buffer location
+
+**Constants**
+
+``NVME_CMBLOC_BIR_SHIFT``
+  Shift amount to get the base indicator register
+
+``NVME_CMBLOC_CQMMS_SHIFT``
+  Shift amount to get the CMB queue mixed memory support
+
+``NVME_CMBLOC_CQPDS_SHIFT``
+  Shift amount to get the CMB queue physically discontiguous support
+
+``NVME_CMBLOC_CDPLMS_SHIFT``
+  Shift amount to get the CMB data pointer mixed locations support
+
+``NVME_CMBLOC_CDPCILS_SHIFT``
+  Shift amount to get the CMB data pointer and command independent locations support
+
+``NVME_CMBLOC_CDMMMS_SHIFT``
+  Shift amount to get the CMB data metadata mixed memory support
+
+``NVME_CMBLOC_CQDA_SHIFT``
+  Shift amount to get the CMB queue dword alignment
+
+``NVME_CMBLOC_OFST_SHIFT``
+  Shift amount to get the offset
+
+``NVME_CMBLOC_BIR_MASK``
+  Mask to get the base indicator register
+
+``NVME_CMBLOC_CQMMS_MASK``
+  Mask to get the CMB queue mixed memory support
+
+``NVME_CMBLOC_CQPDS_MASK``
+  Mask to get the CMB queue physically discontiguous support
+
+``NVME_CMBLOC_CDPLMS_MASK``
+  Mask to get the CMB data pointer mixed locations support
+
+``NVME_CMBLOC_CDPCILS_MASK``
+  Mask to get the CMB data pointer and command independent locations support
+
+``NVME_CMBLOC_CDMMMS_MASK``
+  Mask to get the CMB data metadata mixed memory support
+
+``NVME_CMBLOC_CQDA_MASK``
+  Mask to get the CMB queue dword alignment
+
+``NVME_CMBLOC_OFST_MASK``
+  Mask to get the offset
+
+
+
+
+.. c:enum:: nvme_cmbsz
+
+   This field indicates the controller memory buffer size
+
+**Constants**
+
+``NVME_CMBSZ_SQS_SHIFT``
+  Shift amount to get the submission queue support
+
+``NVME_CMBSZ_CQS_SHIFT``
+  Shift amount to get the completion queue support
+
+``NVME_CMBSZ_LISTS_SHIFT``
+  Shift amount to get the PLP SGL list support
+
+``NVME_CMBSZ_RDS_SHIFT``
+  Shift amount to get the read data support
+
+``NVME_CMBSZ_WDS_SHIFT``
+  Shift amount to get the write data support
+
+``NVME_CMBSZ_SZU_SHIFT``
+  Shift amount to get the size units
+
+``NVME_CMBSZ_SZ_SHIFT``
+  Shift amount to get the size
+
+``NVME_CMBSZ_SQS_MASK``
+  Mask to get the submission queue support
+
+``NVME_CMBSZ_CQS_MASK``
+  Mask to get the completion queue support
+
+``NVME_CMBSZ_LISTS_MASK``
+  Mask to get the PLP SGL list support
+
+``NVME_CMBSZ_RDS_MASK``
+  Mask to get the read data support
+
+``NVME_CMBSZ_WDS_MASK``
+  Mask to get the write data support
+
+``NVME_CMBSZ_SZU_MASK``
+  Mask to get the size units
+
+``NVME_CMBSZ_SZ_MASK``
+  Mask to get the size
+
+``NVME_CMBSZ_SZU_4K``
+  4 KiB
+
+``NVME_CMBSZ_SZU_64K``
+  64 KiB
+
+``NVME_CMBSZ_SZU_1M``
+  1 MiB
+
+``NVME_CMBSZ_SZU_16M``
+  16 MiB
+
+``NVME_CMBSZ_SZU_256M``
+  256 MiB
+
+``NVME_CMBSZ_SZU_4G``
+  4 GiB
+
+``NVME_CMBSZ_SZU_64G``
+  64 GiB
+
+
 .. c:function:: __u64 nvme_cmb_size (__u32 cmbsz)
 
    Calculate size of the controller memory buffer
 
 **Parameters**
 
 ``__u32 cmbsz``
   Value from controller register ``NVME_REG_CMBSZ``
 
 **Return**
 
 size of controller memory buffer in bytes
 
 
+
+
+.. c:enum:: nvme_bpinfo
+
+   This field indicates the boot partition information
+
+**Constants**
+
+``NVME_BPINFO_BPSZ_SHIFT``
+  Shift amount to get the boot partition size
+
+``NVME_BPINFO_BRS_SHIFT``
+  Shift amount to get the boot read status
+
+``NVME_BPINFO_ABPID_SHIFT``
+  Shift amount to get the active boot partition ID
+
+``NVME_BPINFO_BPSZ_MASK``
+  Mask to get the boot partition size
+
+``NVME_BPINFO_BRS_MASK``
+  Mask to get the boot read status
+
+``NVME_BPINFO_ABPID_MASK``
+  Mask to get the active boot partition ID
+
+``NVME_BPINFO_BRS_NONE``
+  No boot partition read operation requested
+
+``NVME_BPINFO_BRS_READ_IN_PROGRESS``
+  Boot partition read in progress
+
+``NVME_BPINFO_BRS_READ_SUCCESS``
+  Boot partition read completed successfully
+
+``NVME_BPINFO_BRS_READ_ERROR``
+  Error completing boot partition read
+
+
+
+
+.. c:enum:: nvme_bprsel
+
+   This field indicates the boot partition read select
+
+**Constants**
+
+``NVME_BPRSEL_BPRSZ_SHIFT``
+  Shift amount to get the boot partition read size
+
+``NVME_BPRSEL_BPROF_SHIFT``
+  Shift amount to get the boot partition read offset
+
+``NVME_BPRSEL_BPID_SHIFT``
+  Shift amount to get the boot partition identifier
+
+``NVME_BPRSEL_BPRSZ_MASK``
+  Mask to get the boot partition read size
+
+``NVME_BPRSEL_BPROF_MASK``
+  Mask to get the boot partition read offset
+
+``NVME_BPRSEL_BPID_MASK``
+  Mask to get the boot partition identifier
+
+
+
+
+.. c:enum:: nvme_bpmbl
+
+   This field indicates the boot partition memory buffer location
+
+**Constants**
+
+``NVME_BPMBL_BMBBA_SHIFT``
+  Shift amount to get the boot partition memory buffer base address
+
+
+
+
+.. c:enum:: nvme_cmbmsc
+
+   This field indicates the controller memory buffer memory space control
+
+**Constants**
+
+``NVME_CMBMSC_CRE_SHIFT``
+  Shift amount to get the capabilities registers enabled
+
+``NVME_CMBMSC_CMSE_SHIFT``
+  Shift amount to get the controller memory space enable
+
+``NVME_CMBMSC_CBA_SHIFT``
+  Shift amount to get the controller base address
+
+``NVME_CMBMSC_CRE_MASK``
+  Mask to get the capabilities registers enabled
+
+``NVME_CMBMSC_CMSE_MASK``
+  Mask to get the controller memory space enable
+
+
+
+
+.. c:enum:: nvme_cmbsts
+
+   This field indicates the controller memory buffer status
+
+**Constants**
+
+``NVME_CMBSTS_CBAI_SHIFT``
+  Shift amount to get the controller base address invalid
+
+``NVME_CMBSTS_CBAI_MASK``
+  Mask to get the controller base address invalid
+
+
+
+
+.. c:enum:: nvme_unit
+
+   Defined buffer size and write throughput granularity units
+
+**Constants**
+
+``NVME_UNIT_B``
+  Bytes or Bytes/second
+
+``NVME_UNIT_1K``
+  1 KiB or 1 KiB/second
+
+``NVME_UNIT_1M``
+  1 MiB or 1 MiB/second
+
+``NVME_UNIT_1G``
+  1 GiB or 1 GiB/second
+
+
+
+
+.. c:enum:: nvme_cmbebs
+
+   This field indicates the controller memory buffer elasticity buffer size
+
+**Constants**
+
+``NVME_CMBEBS_CMBSZU_SHIFT``
+  Shift amount to get the CMB elasticity buffer size units
+
+``NVME_CMBEBS_RBB_SHIFT``
+  Shift amount to get the read bypass behavior
+
+``NVME_CMBEBS_CMBWBZ_SHIFT``
+  Shift amount to get the CMB elasiticity buffer size base
+
+``NVME_CMBEBS_CMBSZU_MASK``
+  Mask to get the CMB elasticity buffer size units
+
+``NVME_CMBEBS_RBB_MASK``
+  Mask to get the read bypass behavior
+
+``NVME_CMBEBS_CMBWBZ_MASK``
+  Mask to get the CMB elasiticity buffer size base
+
+``NVME_CMBEBS_CMBSZU_B``
+  Bytes granularity
+
+``NVME_CMBEBS_CMBSZU_1K``
+  1 KiB granularity
+
+``NVME_CMBEBS_CMBSZU_1M``
+  1 MiB granularity
+
+``NVME_CMBEBS_CMBSZU_1G``
+  1 GiB granularity
+
+
+
+
+.. c:enum:: nvme_cmbswtp
+
+   This field indicates the controller memory buffer sustained write throughput
+
+**Constants**
+
+``NVME_CMBSWTP_CMBSWTU_SHIFT``
+  Shift amount to get the CMB sustained write throughput units
+
+``NVME_CMBSWTP_CMBSWTV_SHIFT``
+  Shift amount to get the CMB sustained write throughput
+
+``NVME_CMBSWTP_CMBSWTU_MASK``
+  Mask to get the CMB sustained write throughput units
+
+``NVME_CMBSWTP_CMBSWTV_MASK``
+  Mask to get the CMB sustained write throughput
+
+``NVME_CMBSWTP_CMBSWTU_B``
+  Bytes/second granularity
+
+``NVME_CMBSWTP_CMBSWTU_1K``
+  1 KiB/second granularity
+
+``NVME_CMBSWTP_CMBSWTU_1M``
+  1 MiB/second granularity
+
+``NVME_CMBSWTP_CMBSWTU_1G``
+  1 GiB/second granularity
+
+
+
+
+.. c:enum:: nvme_crto
+
+   This field indicates the controller ready timeouts
+
+**Constants**
+
+``NVME_CRTO_CRWMT_SHIFT``
+  Shift amount to get the  controller ready with media timeout
+
+``NVME_CRTO_CRIMT_SHIFT``
+  Shift amount to get the controller ready independent of media timeout
+
+``NVME_CRTO_CRWMT_MASK``
+  Mask to get the controller ready with media timeout
+
+``NVME_CRTO_CRIMT_MASK``
+  Mask to get the controller ready independent of media timeout
+
+
+
+
+.. c:enum:: nvme_pmrcap
+
+   This field indicates the persistent memory region capabilities
+
+**Constants**
+
+``NVME_PMRCAP_RDS_SHIFT``
+  Shift amount to get the read data support
+
+``NVME_PMRCAP_WDS_SHIFT``
+  Shift amount to get the write data support
+
+``NVME_PMRCAP_BIR_SHIFT``
+  Shift amount to get the base indicator register
+
+``NVME_PMRCAP_PMRTU_SHIFT``
+  Shift amount to get the persistent memory region time units
+
+``NVME_PMRCAP_PMRWBM_SHIFT``
+  Shift amount to get the persistent memory region write barrier mechanisms
+
+``NVME_PMRCAP_PMRTO_SHIFT``
+  Shift amount to get the persistent memory region timeout
+
+``NVME_PMRCAP_CMSS_SHIFT``
+  Shift amount to get the controller memory space supported
+
+``NVME_PMRCAP_PMRWMB_SHIFT``
+  Deprecated shift amount to get the persistent memory region write barrier mechanisms
+
+``NVME_PMRCAP_RDS_MASK``
+  Mask to get the read data support
+
+``NVME_PMRCAP_WDS_MASK``
+  Mask to get the write data support
+
+``NVME_PMRCAP_BIR_MASK``
+  Mask to get the base indicator register
+
+``NVME_PMRCAP_PMRTU_MASK``
+  Mask to get the persistent memory region time units
+
+``NVME_PMRCAP_PMRWBM_MASK``
+  Mask to get the persistent memory region write barrier mechanisms
+
+``NVME_PMRCAP_PMRTO_MASK``
+  Mask to get the persistent memory region timeout
+
+``NVME_PMRCAP_CMSS_MASK``
+  Mask to get the controller memory space supported
+
+``NVME_PMRCAP_PMRWMB_MASK``
+  Deprecated mask to get the persistent memory region write barrier mechanisms
+
+``NVME_PMRCAP_PMRTU_500MS``
+  500 milliseconds
+
+``NVME_PMRCAP_PMRTU_60S``
+  minutes
+
+
+
+
+.. c:enum:: nvme_pmrctl
+
+   This field indicates the persistent memory region control
+
+**Constants**
+
+``NVME_PMRCTL_EN_SHIFT``
+  Shift amount to get the enable
+
+``NVME_PMRCTL_EN_MASK``
+  Mask to get the enable
+
+
+
+
+.. c:enum:: nvme_pmrsts
+
+   This field indicates the persistent memory region status
+
+**Constants**
+
+``NVME_PMRSTS_ERR_SHIFT``
+  Shift amount to get the error
+
+``NVME_PMRSTS_NRDY_SHIFT``
+  Shift amount to get the not ready
+
+``NVME_PMRSTS_HSTS_SHIFT``
+  Shift amount to get the health status
+
+``NVME_PMRSTS_CBAI_SHIFT``
+  Shift amount to get the controller base address invalid
+
+``NVME_PMRSTS_ERR_MASK``
+  Mask to get the error
+
+``NVME_PMRSTS_NRDY_MASK``
+  Mask to get the not ready
+
+``NVME_PMRSTS_HSTS_MASK``
+  Mask to get the health status
+
+``NVME_PMRSTS_CBAI_MASK``
+  Mask to get the controller base address invalid
+
+
+
+
+.. c:enum:: nvme_pmrebs
+
+   This field indicates the persistent memory region elasticity buffer size
+
+**Constants**
+
+``NVME_PMREBS_PMRSZU_SHIFT``
+  Shift amount to get the PMR elasticity buffer size units
+
+``NVME_PMREBS_RBB_SHIFT``
+  Shift amount to get the read bypass behavior
+
+``NVME_PMREBS_PMRWBZ_SHIFT``
+  Shift amount to get the PMR elasticity buffer size base
+
+``NVME_PMREBS_PMRSZU_MASK``
+  Mask to get the PMR elasticity buffer size units
+
+``NVME_PMREBS_RBB_MASK``
+  Mask to get the read bypass behavior
+
+``NVME_PMREBS_PMRWBZ_MASK``
+  Mask to get the PMR elasticity buffer size base
+
+``NVME_PMREBS_PMRSZU_B``
+  Bytes
+
+``NVME_PMREBS_PMRSZU_1K``
+  1 KiB
+
+``NVME_PMREBS_PMRSZU_1M``
+  1 MiB
+
+``NVME_PMREBS_PMRSZU_1G``
+  1 GiB
+
+
 .. c:function:: __u64 nvme_pmr_size (__u32 pmrebs)
 
    Calculate size of persistent memory region elasticity buffer
 
 **Parameters**
 
 ``__u32 pmrebs``
   Value from controller register ``NVME_REG_PMREBS``
 
 **Return**
 
 size of controller persistent memory buffer in bytes
 
 
+
+
+.. c:enum:: nvme_pmrswtp
+
+   This field indicates the persistent memory region sustained write throughput
+
+**Constants**
+
+``NVME_PMRSWTP_PMRSWTU_SHIFT``
+  Shift amount to get the PMR sustained write throughput units
+
+``NVME_PMRSWTP_PMRSWTV_SHIFT``
+  Shift amount to get the PMR sustained write throughput
+
+``NVME_PMRSWTP_PMRSWTU_MASK``
+  Mask to get the PMR sustained write throughput units
+
+``NVME_PMRSWTP_PMRSWTV_MASK``
+  Mask to get the PMR sustained write throughput
+
+``NVME_PMRSWTP_PMRSWTU_BPS``
+  Bytes per second
+
+``NVME_PMRSWTP_PMRSWTU_KBPS``
+  1 KiB / s
+
+``NVME_PMRSWTP_PMRSWTU_MBPS``
+  1 MiB / s
+
+``NVME_PMRSWTP_PMRSWTU_GBPS``
+  1 GiB / s
+
+
 .. c:function:: __u64 nvme_pmr_throughput (__u32 pmrswtp)
 
    Calculate throughput of persistent memory buffer
 
 **Parameters**
 
 ``__u32 pmrswtp``
@@ -336,14 +1230,59 @@
 **Return**
 
 throughput of controller persistent memory buffer in bytes/second
 
 
 
 
+.. c:enum:: nvme_pmrmsc
+
+   This field indicates the persistent memory region memory space control
+
+**Constants**
+
+``NVME_PMRMSC_CMSE_SHIFT``
+  Shift amount to get the controller memory space enable
+
+``NVME_PMRMSC_CBA_SHIFT``
+  Shift amount to get the controller base address
+
+``NVME_PMRMSC_CMSE_MASK``
+  Mask to get the controller memory space enable
+
+
+
+
+.. c:enum:: nvme_flbas
+
+   This field indicates the formatted LBA size
+
+**Constants**
+
+``NVME_FLBAS_LOWER_SHIFT``
+  Shift amount to get the format index least significant 4 bits
+
+``NVME_FLBAS_META_EXT_SHIFT``
+  Shift amount to get the metadata transferred
+
+``NVME_FLBAS_HIGHER_SHIFT``
+  Shift amount to get the format index most significant 2 bits
+
+``NVME_FLBAS_LOWER_MASK``
+  Mask to get the format index least significant 4 bits
+
+``NVME_FLBAS_META_EXT_MASK``
+  Mask to get the metadata transferred
+
+``NVME_FLBAS_HIGHER_MASK``
+  Mask to get the format index most significant 2 bits
+
+
+
+
 .. c:enum:: nvme_psd_flags
 
    Possible flag values in nvme power state descriptor
 
 **Constants**
 
 ``NVME_PSD_FLAGS_MXPS``
@@ -1038,14 +1977,53 @@
 ``vs``
   Vendor Specific
 
 
 
 
 
+.. c:enum:: nvme_cmic
+
+   This field indicates the controller multi-path I/O and NS sharing capabilities
+
+**Constants**
+
+``NVME_CMIC_MULTI_PORT_SHIFT``
+  Shift amount to get the NVM subsystem port
+
+``NVME_CMIC_MULTI_CTRL_SHIFT``
+  Shift amount to get the controllers
+
+``NVME_CMIC_MULTI_SRIOV_SHIFT``
+  Shift amount to get the SR-IOV virtual function
+
+``NVME_CMIC_MULTI_ANA_SHIFT``
+  Shift amount to get the asymmetric namespace access reporting
+
+``NVME_CMIC_MULTI_RSVD_SHIFT``
+  Shift amount to get the reserved
+
+``NVME_CMIC_MULTI_PORT_MASK``
+  Mask to get the NVM subsystem port
+
+``NVME_CMIC_MULTI_CTRL_MASK``
+  Mask to get the controllers
+
+``NVME_CMIC_MULTI_SRIOV_MASK``
+  Mask to get the SR-IOV virtual function
+
+``NVME_CMIC_MULTI_ANA_MASK``
+  Mask to get the asymmetric namespace access reporting
+
+``NVME_CMIC_MULTI_RSVD_MASK``
+  Mask to get the reserved
+
+
+
+
 .. c:enum:: nvme_id_ctrl_cmic
 
    Controller Multipath IO and Namespace Sharing Capabilities of the controller and NVM subsystem.
 
 **Constants**
 
 ``NVME_CTRL_CMIC_MULTI_PORT``
@@ -4678,14 +5656,73 @@
 ``seb``
   Supported Events Bitmap
 
 
 
 
 
+.. c:enum:: nvme_pel_rci
+
+   This field indicates the persistent event log reporting context
+
+**Constants**
+
+``NVME_PEL_RCI_RCPID_SHIFT``
+  Shift amount to get the reporting context port identifier
+  from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RCPIT_SHIFT``
+  Shift amount to get the reporting context port identifier
+  type from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RCE_SHIFT``
+  Shift amount to get the reporting context exists
+  from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RSVD_SHIFT``
+  Shift amount to get the reserved reporting context
+  from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RCPID_MASK``
+  Mask to get the reporting context port identifier from
+  the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RCPIT_MASK``
+  Mask to get the reporting context port identifier type from
+  the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RCE_MASK``
+  Mask to get the reporting context exists from
+  the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_RCI_RSVD_MASK``
+  Mask to get the reserved reporting context from
+  the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+
+
+
+.. c:enum:: nvme_pel_rci_rcpit
+
+   Persistent Event Log Reporting Context - Port Identifier Type
+
+**Constants**
+
+``NVME_PEL_RCI_RCPIT_NOT_EXIST``
+  Does not already exist
+
+``NVME_PEL_RCI_RCPIT_EST_PORT``
+  Established by an NVM subsystem port
+
+``NVME_PEL_RCI_RCPIT_EST_ME``
+  Established by a Management Endpoint
+
+
+
+
 .. c:struct:: nvme_persistent_event_entry
 
    Persistent Event
 
 **Definition**
 
 ::
@@ -4783,14 +5820,60 @@
 
 ``NVME_PEL_THERMAL_EXCURSION_EVENT``
   Thermal Excursion Event
 
 
 
 
+.. c:enum:: nvme_pel_ehai
+
+   This field indicates the persistent event header additional information
+
+**Constants**
+
+``NVME_PEL_EHAI_PIT_SHIFT``
+  Shift amount to get the reporting context port identifier
+  from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_EHAI_RSVD_SHIFT``
+  Shift amount to get the reserved reporting context
+  from the :c:type:`struct nvme_persistent_event_log <nvme_persistent_event_log>`.rci field.
+
+``NVME_PEL_EHAI_PIT_MASK``
+  Mask to get the reporting context port identifier from
+  the :c:type:`struct nvme_st_result <nvme_st_result>`.dsts field.
+
+``NVME_PEL_EHAI_RSVD_MASK``
+  Mask to get the reserved reporting context from
+  the :c:type:`struct nvme_st_result <nvme_st_result>`.dsts field.
+
+
+
+
+.. c:enum:: nvme_pel_ehai_pit
+
+   Persistent Event Header Additional Information - Port Identifier Type
+
+**Constants**
+
+``NVME_PEL_EHAI_PIT_NOT_REPORTED``
+  PIT not reported and PELPID does not apply
+
+``NVME_PEL_EHAI_PIT_NSS_PORT``
+  NVM subsystem port
+
+``NVME_PEL_EHAI_PIT_NMI_PORT``
+  NVMe-MI port
+
+``NVME_PEL_EHAI_PIT_NOT_ASSOCIATED``
+  Event not associated with any port and PELPID does not apply
+
+
+
+
 .. c:struct:: nvme_fw_commit_event
 
    Firmware Commit Event Data
 
 **Definition**
 
 ::
@@ -5182,14 +6265,47 @@
 ``cdw_mem``
   Command Dwords Memory buffer
 
 
 
 
 
+.. c:enum:: nvme_set_feat_event_layout
+
+   This field indicates the set feature event layout
+
+**Constants**
+
+``NVME_SET_FEAT_EVENT_DW_COUNT_SHIFT``
+  Shift amount to get the Dword count from the
+  :c:type:`struct nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+``NVME_SET_FEAT_EVENT_CC_DW0_SHIFT``
+  Shift amount to get the logged command completion Dword 0
+  from the :c:type:`struct nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+``NVME_SET_FEAT_EVENT_MB_COUNT_SHIFT``
+  Shift amount to get the memory buffer count from
+  the :c:type:`struct nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+``NVME_SET_FEAT_EVENT_DW_COUNT_MASK``
+  Mask to get the Dword count from the :c:type:`struct
+  nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+``NVME_SET_FEAT_EVENT_CC_DW0_MASK``
+  Mask to get the logged command completion Dword 0 from
+  the :c:type:`struct nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+``NVME_SET_FEAT_EVENT_MB_COUNT_MASK``
+  Mask to get the memory buffer count from the :c:type:`struct
+  nvme_set_feature_event <nvme_set_feature_event>`.layout field.
+
+
+
+
 .. c:struct:: nvme_thermal_exc_event
 
    Thermal Excursion Event Data
 
 **Definition**
 
 ::
@@ -5538,14 +6654,39 @@
   Contains the contents of the
   specified Boot Partition
 
 
 
 
 
+.. c:enum:: nvme_boot_partition_info
+
+   This field indicates the boot partition information
+
+**Constants**
+
+``NVME_BOOT_PARTITION_INFO_BPSZ_SHIFT``
+  Shift amount to get the boot partition size from
+  the :c:type:`struct nvme_boot_partition <nvme_boot_partition>`.bpinfo field.
+
+``NVME_BOOT_PARTITION_INFO_ABPID_SHIFT``
+  Shift amount to get the active boot partition ID
+  from the :c:type:`struct nvme_boot_partition <nvme_boot_partition>`.bpinfo field.
+
+``NVME_BOOT_PARTITION_INFO_BPSZ_MASK``
+  Mask to get the boot partition size from the
+  :c:type:`struct nvme_boot_partition <nvme_boot_partition>`.bpinfo field.
+
+``NVME_BOOT_PARTITION_INFO_ABPID_MASK``
+  Mask to get the active boot partition ID from the
+  :c:type:`struct nvme_boot_partition <nvme_boot_partition>`.bpinfo field.
+
+
+
+
 .. c:struct:: nvme_eom_lane_desc
 
    EOM Lane Descriptor
 
 **Definition**
 
 ::
@@ -5712,26 +6853,59 @@
 ``descs``
   EOM Lane Descriptors
 
 
 
 
 
-.. c:enum:: nvme_eom_optional_data
+.. c:enum:: nvme_eom_optional_data_present
 
    EOM Optional Data Present Fields
 
 **Constants**
 
-``NVME_EOM_EYE_DATA_PRESENT``
-  Eye Data Present
+``NVME_EOM_ODP_PEFP_SHIFT``
+  Shift amount to get the printable eye field present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+``NVME_EOM_ODP_EDFP_SHIFT``
+  Shift amount to get the eye data field present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+``NVME_EOM_ODP_RSVD_SHIFT``
+  Shift amount to get the reserved optional data present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+``NVME_EOM_ODP_PEFP_MASK``
+  Mask to get the printable eye field present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+``NVME_EOM_ODP_EDFP_MASK``
+  Mask to get the eye data field present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+``NVME_EOM_ODP_RSVD_MASK``
+  Mask to get the reserved data present
+  from the :c:type:`struct nvme_phy_rx_eom_log <nvme_phy_rx_eom_log>`.odp field.
+
+
+
+
+.. c:enum:: nvme_eom_optional_data
+
+   EOM Optional Data Present Fields (Deprecated)
+
+**Constants**
 
 ``NVME_EOM_PRINTABLE_EYE_PRESENT``
   Printable Eye Present
 
+``NVME_EOM_EYE_DATA_PRESENT``
+  Eye Data Present
+
 
 
 
 .. c:enum:: nvme_phy_rx_eom_progress
 
    EOM In Progress Values
 
@@ -10910,14 +12084,17 @@
 
 ``NVME_LOG_LID_FID_SUPPORTED_EFFECTS``
   Feature Identifiers Supported and Effects
 
 ``NVME_LOG_LID_MI_CMD_SUPPORTED_EFFECTS``
   NVMe-MI Commands Supported and Effects
 
+``NVME_LOG_LID_CMD_AND_FEAT_LOCKDOWN``
+  Command and Feature Lockdown
+
 ``NVME_LOG_LID_BOOT_PARTITION``
   Boot Partition
 
 ``NVME_LOG_LID_PHY_RX_EOM``
   Physical Interface Receiver Eye Opening Measurement
 
 ``NVME_LOG_LID_FDP_CONFIGS``
```

### Comparing `libnvme-1.8/doc/rst/util.rst` & `libnvme-1.9/doc/rst/util.rst`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/discover-loop.c` & `libnvme-1.9/examples/discover-loop.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/discover-loop.py` & `libnvme-1.9/examples/discover-loop.py`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/display-columnar.c` & `libnvme-1.9/examples/display-columnar.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/display-tree.c` & `libnvme-1.9/examples/display-tree.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/meson.build` & `libnvme-1.9/examples/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/mi-conf.c` & `libnvme-1.9/examples/mi-conf.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/examples/mi-mctp.c` & `libnvme-1.9/examples/mi-mctp.c`

 * *Files 1% similar despite different names*

```diff
@@ -673,16 +673,16 @@
 
 int main(int argc, char **argv)
 {
 	enum action action;
 	nvme_root_t root;
 	nvme_mi_ep_t ep;
 	bool dbus = false, usage = true;
-	uint8_t eid;
-	int rc = 0, net;
+	uint8_t eid = 0;
+	int rc = 0, net = 0;
 
 	if (argc >= 2 && strcmp(argv[1], "dbus") == 0) {
 		usage = false;
 		dbus= true;
 		argv += 1;
 		argc -= 1;
 	} else if (argc >= 3) {
```

### Comparing `libnvme-1.8/examples/telemetry-listen.c` & `libnvme-1.9/examples/telemetry-listen.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/internal/meson.build` & `libnvme-1.9/internal/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/README.md` & `libnvme-1.9/libnvme/README.md`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/meson.build` & `libnvme-1.9/libnvme/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/nvme.i` & `libnvme-1.9/libnvme/nvme.i`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/tests/NBFT` & `libnvme-1.9/libnvme/tests/NBFT`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/tests/gc.py` & `libnvme-1.9/libnvme/tests/gc.py`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme/tests/test-nbft.py` & `libnvme-1.9/libnvme/tests/test-nbft.py`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/libnvme.spec.in` & `libnvme-1.9/libnvme.spec.in`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/meson.build` & `libnvme-1.9/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 # Copyright (c) 2021 Dell Inc.
 #
 # Authors: Martin Belanger <Martin.Belanger@dell.com>
 #
 project(
     'libnvme', ['c'],
     meson_version: '>= 0.50.0',
-    version: '1.8',
+    version: '1.9',
     license: 'LGPL-2.1-or-later',
     default_options: [
         'c_std=gnu99',
         'warning_level=1',
-        'buildtype=debug',
+        'buildtype=debugoptimized',
         'prefix=/usr/local',
         'sysconfdir=etc',
         'wrap_mode=nofallback'
     ]
 )
 
 vstr = meson.project_version().split('-rc')[0]
```

### Comparing `libnvme-1.8/meson_options.txt` & `libnvme-1.9/meson_options.txt`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/pyproject.toml` & `libnvme-1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/scripts/build.sh` & `libnvme-1.9/scripts/build.sh`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/scripts/kernel-doc` & `libnvme-1.9/scripts/kernel-doc`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/scripts/meson-vcs-tag.sh` & `libnvme-1.9/scripts/meson-vcs-tag.sh`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/scripts/release.sh` & `libnvme-1.9/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/scripts/update-docs.sh` & `libnvme-1.9/scripts/update-docs.sh`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/libnvme-mi.map` & `libnvme-1.9/src/libnvme-mi.map`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/libnvme.h` & `libnvme-1.9/src/libnvme.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/libnvme.map` & `libnvme-1.9/src/libnvme.map`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 # SPDX-License-Identifier: LGPL-2.1-or-later
+LIBNVME_1.9 {
+	global:
+		nvme_export_tls_key;
+		nvme_get_logging_level;
+		nvme_import_tls_key;
+		nvme_read_key;
+		nvme_scan_tls_keys;
+		nvme_submit_passthru;
+		nvme_submit_passthru64;
+		nvme_update_key;
+		nvme_ctrl_get_cntlid;
+};
+
 LIBNVME_1_8 {
 	global:
 		nvme_uuid_find;
 };
 
 LIBNVME_1_7 {
 	global:
```

### Comparing `libnvme-1.8/src/meson.build` & `libnvme-1.9/src/meson.build`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 sources = [
     'nvme/nbft.c',
     'nvme/fabrics.c',
     'nvme/filters.c',
     'nvme/ioctl.c',
     'nvme/linux.c',
     'nvme/log.c',
+    'nvme/sysfs.c',
     'nvme/tree.c',
     'nvme/util.c',
-    'nvme/base64.c'
+    'nvme/base64.c',
+    'nvme/crc32.c'
 ]
 
 mi_sources = [
     'nvme/log.c',
     'nvme/mi.c',
     'nvme/mi-mctp.c',
 ]
```

### Comparing `libnvme-1.8/src/nvme/api-types.h` & `libnvme-1.9/src/nvme/api-types.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/base64.c` & `libnvme-1.9/src/nvme/base64.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/cleanup.h` & `libnvme-1.9/src/nvme/cleanup.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/fabrics.c` & `libnvme-1.9/src/nvme/fabrics.c`

 * *Files 1% similar despite different names*

```diff
@@ -1182,64 +1182,31 @@
 
 	for (int i = 0; i < le64_to_cpu(log->numrec); i++)
 		sanitize_discovery_log_entry(&log->entries[i]);
 
 	return log;
 }
 
-#define PATH_UUID_IBM	"/proc/device-tree/ibm,partition-uuid"
-
-static char *uuid_ibm_filename(void)
-{
-	char *basepath = getenv("LIBNVME_SYSFS_PATH");
-	char *str;
-
-	if (!basepath)
-		return strdup(PATH_UUID_IBM);
-
-	if (!asprintf(&str, "%s" PATH_UUID_IBM, basepath))
-		return NULL;
-
-	return str;
-}
-
 static int uuid_from_device_tree(char *system_uuid)
 {
-	_cleanup_free_ char *filename = uuid_ibm_filename();
 	_cleanup_fd_ int f = -1;
 	ssize_t len;
 
-	f = open(filename, O_RDONLY);
+	f = open(nvme_uuid_ibm_filename(), O_RDONLY);
 	if (f < 0)
 		return -ENXIO;
 
 	memset(system_uuid, 0, NVME_UUID_LEN_STRING);
 	len = read(f, system_uuid, NVME_UUID_LEN_STRING - 1);
 	if (len < 0)
 		return -ENXIO;
 
 	return strlen(system_uuid) ? 0 : -ENXIO;
 }
 
-#define PATH_DMI_ENTRIES       "/sys/firmware/dmi/entries"
-
-static char *dmi_entries_dir(void)
-{
-	char *basepath = getenv("LIBNVME_SYSFS_PATH");
-	char *str;
-
-	if (!basepath)
-		return strdup(PATH_DMI_ENTRIES);
-
-	if (!asprintf(&str, "%s" PATH_DMI_ENTRIES, basepath))
-		return NULL;
-
-	return str;
-}
-
 /*
  * See System Management BIOS (SMBIOS) Reference Specification
  * https://www.dmtf.org/sites/default/files/standards/documents/DSP0134_3.2.0.pdf
  */
 #define DMI_SYSTEM_INFORMATION	1
 
 static bool is_dmi_uuid_valid(const char *buf, size_t len)
@@ -1260,15 +1227,15 @@
 
 	return true;
 }
 
 static int uuid_from_dmi_entries(char *system_uuid)
 {
 	_cleanup_dir_ DIR *d = NULL;
-	_cleanup_free_ char *entries_dir = dmi_entries_dir();
+	const char *entries_dir = nvme_dmi_entries_dir();
 	int f;
 	struct dirent *de;
 	char buf[512] = {0};
 
 	system_uuid[0] = '\0';
 	d = opendir(entries_dir);
 	if (!d)
@@ -1293,14 +1260,16 @@
 			continue;
 		sprintf(filename, "%s/%s/raw", entries_dir, de->d_name);
 		f = open(filename, O_RDONLY);
 		if (f < 0)
 			continue;
 		len = read(f, buf, 512);
 		close(f);
+		if (len <= 0)
+			continue;
 
 		if (!is_dmi_uuid_valid(buf, len))
 			continue;
 
 		/* Sigh. https://en.wikipedia.org/wiki/Overengineering */
 		/* DMTF SMBIOS 3.0 Section 7.2.1 System UUID */
 		sprintf(system_uuid,
```

### Comparing `libnvme-1.8/src/nvme/fabrics.h` & `libnvme-1.9/src/nvme/fabrics.h`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 	int reconnect_delay;
 	int ctrl_loss_tmo;
 	int fast_io_fail_tmo;
 	int keep_alive_tmo;
 	int nr_write_queues;
 	int nr_poll_queues;
 	int tos;
-	int keyring;
-	int tls_key;
+	long keyring;
+	long tls_key;
 
 	bool duplicate_connect;
 	bool disable_sqflow;
 	bool hdr_digest;
 	bool data_digest;
 	bool tls;
 	bool concat;
```

### Comparing `libnvme-1.8/src/nvme/filters.h` & `libnvme-1.9/src/nvme/filters.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/ioctl.c` & `libnvme-1.9/src/nvme/ioctl.c`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 #include <sys/time.h>
 
 #include <ccan/build_assert/build_assert.h>
 #include <ccan/endian/endian.h>
 
 #include "ioctl.h"
 #include "util.h"
-
-static bool nvme_debug;
+#include "log.h"
 
 static int nvme_verify_chr(int fd)
 {
 	static struct stat nvme_stat;
 	int err = fstat(fd, &nvme_stat);
 
 	if (err < 0)
@@ -75,81 +74,34 @@
 int nvme_get_nsid(int fd, __u32 *nsid)
 {
 	errno = 0;
 	*nsid = ioctl(fd, NVME_IOCTL_ID);
 	return -1 * (errno != 0);
 }
 
-static int nvme_submit_passthru64(int fd, unsigned long ioctl_cmd,
-				  struct nvme_passthru_cmd64 *cmd,
-				  __u64 *result)
+__attribute__((weak))
+int nvme_submit_passthru64(int fd, unsigned long ioctl_cmd,
+			   struct nvme_passthru_cmd64 *cmd,
+			   __u64 *result)
 {
 	int err = ioctl(fd, ioctl_cmd, cmd);
 
 	if (err >= 0 && result)
 		*result = cmd->result;
 	return err;
 }
 
-static void nvme_show_command(struct nvme_passthru_cmd *cmd, int err, struct timeval start,
-			      struct timeval end)
+__attribute__((weak))
+int nvme_submit_passthru(int fd, unsigned long ioctl_cmd,
+			 struct nvme_passthru_cmd *cmd, __u32 *result)
 {
-	printf("opcode       : %02x\n", cmd->opcode);
-	printf("flags        : %02x\n", cmd->flags);
-	printf("rsvd1        : %04x\n", cmd->rsvd1);
-	printf("nsid         : %08x\n", cmd->nsid);
-	printf("cdw2         : %08x\n", cmd->cdw2);
-	printf("cdw3         : %08x\n", cmd->cdw3);
-	printf("data_len     : %08x\n", cmd->data_len);
-	printf("metadata_len : %08x\n", cmd->metadata_len);
-	printf("addr         : %"PRIx64"\n", (uint64_t)(uintptr_t)cmd->addr);
-	printf("metadata     : %"PRIx64"\n", (uint64_t)(uintptr_t)cmd->metadata);
-	printf("cdw10        : %08x\n", cmd->cdw10);
-	printf("cdw11        : %08x\n", cmd->cdw11);
-	printf("cdw12        : %08x\n", cmd->cdw12);
-	printf("cdw13        : %08x\n", cmd->cdw13);
-	printf("cdw14        : %08x\n", cmd->cdw14);
-	printf("cdw15        : %08x\n", cmd->cdw15);
-	printf("timeout_ms   : %08x\n", cmd->timeout_ms);
-	printf("result       : %08x\n", cmd->result);
-	printf("err          : %d\n", err);
-	printf("latency      : %lu us\n",
-	       (end.tv_sec - start.tv_sec) * 1000000 + (end.tv_usec - start.tv_usec));
-}
-
-void nvme_set_debug(bool debug)
-{
-	nvme_debug = debug;
-}
-
-bool nvme_get_debug(void)
-{
-	return nvme_debug;
-}
-
-static int nvme_submit_passthru(int fd, unsigned long ioctl_cmd,
-				struct nvme_passthru_cmd *cmd, __u32 *result)
-{
-	struct timeval start;
-	struct timeval end;
-	int err;
-
-	if (nvme_get_debug())
-		gettimeofday(&start, NULL);
-
-	err = ioctl(fd, ioctl_cmd, cmd);
-
-	if (nvme_get_debug()) {
-		gettimeofday(&end, NULL);
-		nvme_show_command(cmd, err, start, end);
-	}
+	int err = ioctl(fd, ioctl_cmd, cmd);
 
 	if (err >= 0 && result)
 		*result = cmd->result;
-
 	return err;
 }
 
 static int nvme_passthru64(int fd, unsigned long ioctl_cmd, __u8 opcode,
 			   __u8 flags, __u16 rsvd, __u32 nsid, __u32 cdw2,
 			   __u32 cdw3, __u32 cdw10, __u32 cdw11, __u32 cdw12,
 			   __u32 cdw13, __u32 cdw14, __u32 cdw15,
@@ -242,133 +194,14 @@
 {
 	return nvme_passthru(fd, NVME_IOCTL_ADMIN_CMD, opcode, flags, rsvd,
 			     nsid, cdw2, cdw3, cdw10, cdw11, cdw12, cdw13,
 			     cdw14, cdw15, data_len, data, metadata_len,
 			     metadata, timeout_ms, result);
 }
 
-enum nvme_cmd_dword_fields {
-	NVME_DEVICE_SELF_TEST_CDW10_STC_SHIFT			= 0,
-	NVME_DEVICE_SELF_TEST_CDW10_STC_MASK			= 0xf,
-	NVME_DIRECTIVE_CDW11_DOPER_SHIFT			= 0,
-	NVME_DIRECTIVE_CDW11_DTYPE_SHIFT			= 8,
-	NVME_DIRECTIVE_CDW11_DPSEC_SHIFT			= 16,
-	NVME_DIRECTIVE_CDW11_DOPER_MASK				= 0xff,
-	NVME_DIRECTIVE_CDW11_DTYPE_MASK				= 0xff,
-	NVME_DIRECTIVE_CDW11_DPSEC_MASK				= 0xffff,
-	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_ENDIR_SHIFT		= 0,
-	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_DTYPE_SHIFT		= 1,
-	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_ENDIR_MASK		= 0x1,
-	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_DTYPE_MASK		= 0x1,
-	NVME_FW_COMMIT_CDW10_FS_SHIFT				= 0,
-	NVME_FW_COMMIT_CDW10_CA_SHIFT				= 3,
-	NVME_FW_COMMIT_CDW10_BPID_SHIFT				= 31,
-	NVME_FW_COMMIT_CDW10_FS_MASK				= 0x7,
-	NVME_FW_COMMIT_CDW10_CA_MASK				= 0x7,
-	NVME_FW_COMMIT_CDW10_BPID_MASK				= 0x1,
-	NVME_GET_FEATURES_CDW10_SEL_SHIFT			= 8,
-	NVME_GET_FEATURES_CDW10_SEL_MASK			= 0x7,
-	NVME_SET_FEATURES_CDW10_SAVE_SHIFT			= 31,
-	NVME_SET_FEATURES_CDW10_SAVE_MASK			= 0x1,
-	NVME_FEATURES_CDW10_FID_SHIFT				= 0,
-	NVME_FEATURES_CDW14_UUID_SHIFT				= 0,
-	NVME_FEATURES_CDW10_FID_MASK				= 0xff,
-	NVME_FEATURES_CDW14_UUID_MASK				= 0x7f,
-	NVME_LOG_CDW10_LID_SHIFT				= 0,
-	NVME_LOG_CDW10_LSP_SHIFT				= 8,
-	NVME_LOG_CDW10_RAE_SHIFT				= 15,
-	NVME_LOG_CDW10_NUMDL_SHIFT				= 16,
-	NVME_LOG_CDW11_NUMDU_SHIFT				= 0,
-	NVME_LOG_CDW11_LSI_SHIFT				= 16,
-	NVME_LOG_CDW14_UUID_SHIFT				= 0,
-	NVME_LOG_CDW14_CSI_SHIFT				= 24,
-	NVME_LOG_CDW14_OT_SHIFT					= 23,
-	NVME_LOG_CDW10_LID_MASK					= 0xff,
-	NVME_LOG_CDW10_LSP_MASK					= 0x7f,
-	NVME_LOG_CDW10_RAE_MASK					= 0x1,
-	NVME_LOG_CDW10_NUMDL_MASK				= 0xffff,
-	NVME_LOG_CDW11_NUMDU_MASK				= 0xffff,
-	NVME_LOG_CDW11_LSI_MASK					= 0xffff,
-	NVME_LOG_CDW14_UUID_MASK				= 0x7f,
-	NVME_LOG_CDW14_CSI_MASK					= 0xff,
-	NVME_LOG_CDW14_OT_MASK					= 0x1,
-	NVME_IDENTIFY_CDW10_CNS_SHIFT				= 0,
-	NVME_IDENTIFY_CDW10_CNTID_SHIFT				= 16,
-	NVME_IDENTIFY_CDW11_CNSSPECID_SHIFT			= 0,
-	NVME_IDENTIFY_CDW14_UUID_SHIFT				= 0,
-	NVME_IDENTIFY_CDW11_CSI_SHIFT				= 24,
-	NVME_IDENTIFY_CDW10_CNS_MASK				= 0xff,
-	NVME_IDENTIFY_CDW10_CNTID_MASK				= 0xffff,
-	NVME_IDENTIFY_CDW11_CNSSPECID_MASK			= 0xffff,
-	NVME_IDENTIFY_CDW14_UUID_MASK				= 0x7f,
-	NVME_IDENTIFY_CDW11_CSI_MASK				= 0xff,
-	NVME_NAMESPACE_ATTACH_CDW10_SEL_SHIFT			= 0,
-	NVME_NAMESPACE_ATTACH_CDW10_SEL_MASK			= 0xf,
-	NVME_NAMESPACE_MGMT_CDW10_SEL_SHIFT			= 0,
-	NVME_NAMESPACE_MGMT_CDW10_SEL_MASK			= 0xf,
-	NVME_NAMESPACE_MGMT_CDW11_CSI_SHIFT			= 24,
-	NVME_NAMESPACE_MGMT_CDW11_CSI_MASK			= 0xff,
-	NVME_VIRT_MGMT_CDW10_ACT_SHIFT				= 0,
-	NVME_VIRT_MGMT_CDW10_RT_SHIFT				= 8,
-	NVME_VIRT_MGMT_CDW10_CNTLID_SHIFT			= 16,
-	NVME_VIRT_MGMT_CDW11_NR_SHIFT				= 0,
-	NVME_VIRT_MGMT_CDW10_ACT_MASK				= 0xf,
-	NVME_VIRT_MGMT_CDW10_RT_MASK				= 0x7,
-	NVME_VIRT_MGMT_CDW10_CNTLID_MASK			= 0xffff,
-	NVME_VIRT_MGMT_CDW11_NR_MASK				= 0xffff,
-	NVME_FORMAT_CDW10_LBAF_SHIFT				= 0,
-	NVME_FORMAT_CDW10_MSET_SHIFT				= 4,
-	NVME_FORMAT_CDW10_PI_SHIFT				= 5,
-	NVME_FORMAT_CDW10_PIL_SHIFT				= 8,
-	NVME_FORMAT_CDW10_SES_SHIFT				= 9,
-	NVME_FORMAT_CDW10_LBAFU_SHIFT				= 12,
-	NVME_FORMAT_CDW10_LBAF_MASK				= 0xf,
-	NVME_FORMAT_CDW10_MSET_MASK				= 0x1,
-	NVME_FORMAT_CDW10_PI_MASK				= 0x7,
-	NVME_FORMAT_CDW10_PIL_MASK				= 0x1,
-	NVME_FORMAT_CDW10_SES_MASK				= 0x7,
-	NVME_FORMAT_CDW10_LBAFU_MASK				= 0x3,
-	NVME_SANITIZE_CDW10_SANACT_SHIFT			= 0,
-	NVME_SANITIZE_CDW10_AUSE_SHIFT				= 3,
-	NVME_SANITIZE_CDW10_OWPASS_SHIFT			= 4,
-	NVME_SANITIZE_CDW10_OIPBP_SHIFT				= 8,
-	NVME_SANITIZE_CDW10_NODAS_SHIFT				= 9,
-	NVME_SANITIZE_CDW10_SANACT_MASK				= 0x7,
-	NVME_SANITIZE_CDW10_AUSE_MASK				= 0x1,
-	NVME_SANITIZE_CDW10_OWPASS_MASK				= 0xf,
-	NVME_SANITIZE_CDW10_OIPBP_MASK				= 0x1,
-	NVME_SANITIZE_CDW10_NODAS_MASK				= 0x1,
-	NVME_SECURITY_NSSF_SHIFT				= 0,
-	NVME_SECURITY_SPSP0_SHIFT				= 8,
-	NVME_SECURITY_SPSP1_SHIFT				= 16,
-	NVME_SECURITY_SECP_SHIFT				= 24,
-	NVME_SECURITY_NSSF_MASK					= 0xff,
-	NVME_SECURITY_SPSP0_MASK				= 0xff,
-	NVME_SECURITY_SPSP1_MASK				= 0xff,
-	NVME_SECURITY_SECP_MASK					= 0xffff,
-	NVME_GET_LBA_STATUS_CDW13_RL_SHIFT			= 0,
-	NVME_GET_LBA_STATUS_CDW13_ATYPE_SHIFT			= 24,
-	NVME_GET_LBA_STATUS_CDW13_RL_MASK			= 0xffff,
-	NVME_GET_LBA_STATUS_CDW13_ATYPE_MASK			= 0xff,
-	NVME_ZNS_MGMT_SEND_ZSASO_SHIFT				= 9,
-	NVME_ZNS_MGMT_SEND_ZSASO_MASK				= 0x1,
-	NVME_ZNS_MGMT_SEND_SEL_SHIFT				= 8,
-	NVME_ZNS_MGMT_SEND_SEL_MASK				= 0x1,
-	NVME_ZNS_MGMT_SEND_ZSA_SHIFT				= 0,
-	NVME_ZNS_MGMT_SEND_ZSA_MASK				= 0xff,
-	NVME_ZNS_MGMT_RECV_ZRA_SHIFT				= 0,
-	NVME_ZNS_MGMT_RECV_ZRA_MASK				= 0xff,
-	NVME_ZNS_MGMT_RECV_ZRASF_SHIFT				= 8,
-	NVME_ZNS_MGMT_RECV_ZRASF_MASK				= 0xff,
-	NVME_ZNS_MGMT_RECV_ZRAS_FEAT_SHIFT			= 16,
-	NVME_ZNS_MGMT_RECV_ZRAS_FEAT_MASK			= 0x1,
-	NVME_DIM_TAS_SHIFT					= 0,
-	NVME_DIM_TAS_MASK					= 0xF,
-};
-
 enum features {
 	NVME_FEATURES_ARBITRATION_BURST_SHIFT			= 0,
 	NVME_FEATURES_ARBITRATION_LPW_SHIFT			= 8,
 	NVME_FEATURES_ARBITRATION_MPW_SHIFT			= 16,
 	NVME_FEATURES_ARBITRATION_HPW_SHIFT			= 24,
 	NVME_FEATURES_ARBITRATION_BURST_MASK			= 0x7,
 	NVME_FEATURES_ARBITRATION_LPW_MASK			= 0xff,
```

### Comparing `libnvme-1.8/src/nvme/ioctl.h` & `libnvme-1.9/src/nvme/ioctl.h`

 * *Files 7% similar despite different names*

```diff
@@ -195,14 +195,133 @@
 ({										\
 	type s;									\
 	size_t t = offsetof(type, member) + sizeof(s.member);			\
 	size_t p = (sizeof(align) - (t % sizeof(align))) % sizeof(align);	\
 	t + p;									\
 })
 
+enum nvme_cmd_dword_fields {
+	NVME_DEVICE_SELF_TEST_CDW10_STC_SHIFT			= 0,
+	NVME_DEVICE_SELF_TEST_CDW10_STC_MASK			= 0xf,
+	NVME_DIRECTIVE_CDW11_DOPER_SHIFT			= 0,
+	NVME_DIRECTIVE_CDW11_DTYPE_SHIFT			= 8,
+	NVME_DIRECTIVE_CDW11_DPSEC_SHIFT			= 16,
+	NVME_DIRECTIVE_CDW11_DOPER_MASK				= 0xff,
+	NVME_DIRECTIVE_CDW11_DTYPE_MASK				= 0xff,
+	NVME_DIRECTIVE_CDW11_DPSEC_MASK				= 0xffff,
+	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_ENDIR_SHIFT		= 0,
+	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_DTYPE_SHIFT		= 1,
+	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_ENDIR_MASK		= 0x1,
+	NVME_DIRECTIVE_SEND_IDENTIFY_CDW12_DTYPE_MASK		= 0x1,
+	NVME_FW_COMMIT_CDW10_FS_SHIFT				= 0,
+	NVME_FW_COMMIT_CDW10_CA_SHIFT				= 3,
+	NVME_FW_COMMIT_CDW10_BPID_SHIFT				= 31,
+	NVME_FW_COMMIT_CDW10_FS_MASK				= 0x7,
+	NVME_FW_COMMIT_CDW10_CA_MASK				= 0x7,
+	NVME_FW_COMMIT_CDW10_BPID_MASK				= 0x1,
+	NVME_GET_FEATURES_CDW10_SEL_SHIFT			= 8,
+	NVME_GET_FEATURES_CDW10_SEL_MASK			= 0x7,
+	NVME_SET_FEATURES_CDW10_SAVE_SHIFT			= 31,
+	NVME_SET_FEATURES_CDW10_SAVE_MASK			= 0x1,
+	NVME_FEATURES_CDW10_FID_SHIFT				= 0,
+	NVME_FEATURES_CDW14_UUID_SHIFT				= 0,
+	NVME_FEATURES_CDW10_FID_MASK				= 0xff,
+	NVME_FEATURES_CDW14_UUID_MASK				= 0x7f,
+	NVME_LOG_CDW10_LID_SHIFT				= 0,
+	NVME_LOG_CDW10_LSP_SHIFT				= 8,
+	NVME_LOG_CDW10_RAE_SHIFT				= 15,
+	NVME_LOG_CDW10_NUMDL_SHIFT				= 16,
+	NVME_LOG_CDW11_NUMDU_SHIFT				= 0,
+	NVME_LOG_CDW11_LSI_SHIFT				= 16,
+	NVME_LOG_CDW14_UUID_SHIFT				= 0,
+	NVME_LOG_CDW14_CSI_SHIFT				= 24,
+	NVME_LOG_CDW14_OT_SHIFT					= 23,
+	NVME_LOG_CDW10_LID_MASK					= 0xff,
+	NVME_LOG_CDW10_LSP_MASK					= 0x7f,
+	NVME_LOG_CDW10_RAE_MASK					= 0x1,
+	NVME_LOG_CDW10_NUMDL_MASK				= 0xffff,
+	NVME_LOG_CDW11_NUMDU_MASK				= 0xffff,
+	NVME_LOG_CDW11_LSI_MASK					= 0xffff,
+	NVME_LOG_CDW14_UUID_MASK				= 0x7f,
+	NVME_LOG_CDW14_CSI_MASK					= 0xff,
+	NVME_LOG_CDW14_OT_MASK					= 0x1,
+	NVME_IDENTIFY_CDW10_CNS_SHIFT				= 0,
+	NVME_IDENTIFY_CDW10_CNTID_SHIFT				= 16,
+	NVME_IDENTIFY_CDW11_CNSSPECID_SHIFT			= 0,
+	NVME_IDENTIFY_CDW14_UUID_SHIFT				= 0,
+	NVME_IDENTIFY_CDW11_CSI_SHIFT				= 24,
+	NVME_IDENTIFY_CDW10_CNS_MASK				= 0xff,
+	NVME_IDENTIFY_CDW10_CNTID_MASK				= 0xffff,
+	NVME_IDENTIFY_CDW11_CNSSPECID_MASK			= 0xffff,
+	NVME_IDENTIFY_CDW14_UUID_MASK				= 0x7f,
+	NVME_IDENTIFY_CDW11_CSI_MASK				= 0xff,
+	NVME_NAMESPACE_ATTACH_CDW10_SEL_SHIFT			= 0,
+	NVME_NAMESPACE_ATTACH_CDW10_SEL_MASK			= 0xf,
+	NVME_NAMESPACE_MGMT_CDW10_SEL_SHIFT			= 0,
+	NVME_NAMESPACE_MGMT_CDW10_SEL_MASK			= 0xf,
+	NVME_NAMESPACE_MGMT_CDW11_CSI_SHIFT			= 24,
+	NVME_NAMESPACE_MGMT_CDW11_CSI_MASK			= 0xff,
+	NVME_VIRT_MGMT_CDW10_ACT_SHIFT				= 0,
+	NVME_VIRT_MGMT_CDW10_RT_SHIFT				= 8,
+	NVME_VIRT_MGMT_CDW10_CNTLID_SHIFT			= 16,
+	NVME_VIRT_MGMT_CDW11_NR_SHIFT				= 0,
+	NVME_VIRT_MGMT_CDW10_ACT_MASK				= 0xf,
+	NVME_VIRT_MGMT_CDW10_RT_MASK				= 0x7,
+	NVME_VIRT_MGMT_CDW10_CNTLID_MASK			= 0xffff,
+	NVME_VIRT_MGMT_CDW11_NR_MASK				= 0xffff,
+	NVME_FORMAT_CDW10_LBAF_SHIFT				= 0,
+	NVME_FORMAT_CDW10_MSET_SHIFT				= 4,
+	NVME_FORMAT_CDW10_PI_SHIFT				= 5,
+	NVME_FORMAT_CDW10_PIL_SHIFT				= 8,
+	NVME_FORMAT_CDW10_SES_SHIFT				= 9,
+	NVME_FORMAT_CDW10_LBAFU_SHIFT				= 12,
+	NVME_FORMAT_CDW10_LBAF_MASK				= 0xf,
+	NVME_FORMAT_CDW10_MSET_MASK				= 0x1,
+	NVME_FORMAT_CDW10_PI_MASK				= 0x7,
+	NVME_FORMAT_CDW10_PIL_MASK				= 0x1,
+	NVME_FORMAT_CDW10_SES_MASK				= 0x7,
+	NVME_FORMAT_CDW10_LBAFU_MASK				= 0x3,
+	NVME_SANITIZE_CDW10_SANACT_SHIFT			= 0,
+	NVME_SANITIZE_CDW10_AUSE_SHIFT				= 3,
+	NVME_SANITIZE_CDW10_OWPASS_SHIFT			= 4,
+	NVME_SANITIZE_CDW10_OIPBP_SHIFT				= 8,
+	NVME_SANITIZE_CDW10_NODAS_SHIFT				= 9,
+	NVME_SANITIZE_CDW10_SANACT_MASK				= 0x7,
+	NVME_SANITIZE_CDW10_AUSE_MASK				= 0x1,
+	NVME_SANITIZE_CDW10_OWPASS_MASK				= 0xf,
+	NVME_SANITIZE_CDW10_OIPBP_MASK				= 0x1,
+	NVME_SANITIZE_CDW10_NODAS_MASK				= 0x1,
+	NVME_SECURITY_NSSF_SHIFT				= 0,
+	NVME_SECURITY_SPSP0_SHIFT				= 8,
+	NVME_SECURITY_SPSP1_SHIFT				= 16,
+	NVME_SECURITY_SECP_SHIFT				= 24,
+	NVME_SECURITY_NSSF_MASK					= 0xff,
+	NVME_SECURITY_SPSP0_MASK				= 0xff,
+	NVME_SECURITY_SPSP1_MASK				= 0xff,
+	NVME_SECURITY_SECP_MASK					= 0xffff,
+	NVME_GET_LBA_STATUS_CDW13_RL_SHIFT			= 0,
+	NVME_GET_LBA_STATUS_CDW13_ATYPE_SHIFT			= 24,
+	NVME_GET_LBA_STATUS_CDW13_RL_MASK			= 0xffff,
+	NVME_GET_LBA_STATUS_CDW13_ATYPE_MASK			= 0xff,
+	NVME_ZNS_MGMT_SEND_ZSASO_SHIFT				= 9,
+	NVME_ZNS_MGMT_SEND_ZSASO_MASK				= 0x1,
+	NVME_ZNS_MGMT_SEND_SEL_SHIFT				= 8,
+	NVME_ZNS_MGMT_SEND_SEL_MASK				= 0x1,
+	NVME_ZNS_MGMT_SEND_ZSA_SHIFT				= 0,
+	NVME_ZNS_MGMT_SEND_ZSA_MASK				= 0xff,
+	NVME_ZNS_MGMT_RECV_ZRA_SHIFT				= 0,
+	NVME_ZNS_MGMT_RECV_ZRA_MASK				= 0xff,
+	NVME_ZNS_MGMT_RECV_ZRASF_SHIFT				= 8,
+	NVME_ZNS_MGMT_RECV_ZRASF_MASK				= 0xff,
+	NVME_ZNS_MGMT_RECV_ZRAS_FEAT_SHIFT			= 16,
+	NVME_ZNS_MGMT_RECV_ZRAS_FEAT_MASK			= 0x1,
+	NVME_DIM_TAS_SHIFT					= 0,
+	NVME_DIM_TAS_MASK					= 0xF,
+};
+
 /**
  * nvme_submit_admin_passthru64() - Submit a 64-bit nvme passthrough admin
  *				    command
  * @fd:		File descriptor of nvme device
  * @cmd:	The nvme admin command to send
  * @result:	Optional field to return the result from the CQE DW0-1
  *
@@ -3229,45 +3348,64 @@
 		.data = data,
 	};
 
 	return nvme_ns_mgmt(&args);
 }
 
 /**
- * nvme_ns_mgmt_delete() - Delete a non attached namespace
+ * nvme_ns_mgmt_delete_timeout() - Delete a non attached namespace with timeout
  * @fd:		File descriptor of nvme device
  * @nsid:	Namespace identifier to delete
+ * @timeout:	Override the default timeout to this value in milliseconds;
+ *		set to 0 to use the system default.
  *
  * It is recommended that a namespace being deleted is not attached to any
  * controller. Use the nvme_ns_detach_ctrls() first if the namespace is still
  * attached.
  *
  * Return: The nvme command status if a response was received (see
  * &enum nvme_status_field) or -1 with errno set otherwise.
  */
-static inline int nvme_ns_mgmt_delete(int fd, __u32 nsid)
+static inline int nvme_ns_mgmt_delete_timeout(int fd, __u32 nsid, __u32 timeout)
 {
 	struct nvme_ns_mgmt_args args = {
 		.result = NULL,
 		.ns = NULL,
 		.args_size = sizeof(args),
 		.fd = fd,
-		.timeout = 0,
+		.timeout = timeout,
 		.nsid = nsid,
 		.sel = NVME_NS_MGMT_SEL_DELETE,
 		.csi = 0,
 		.rsvd1 = { 0, },
 		.rsvd2 = NULL,
 		.data = NULL,
 	};
 
 	return nvme_ns_mgmt(&args);
 }
 
 /**
+ * nvme_ns_mgmt_delete() - Delete a non attached namespace
+ * @fd:		File descriptor of nvme device
+ * @nsid:	Namespace identifier to delete
+ *
+ * It is recommended that a namespace being deleted is not attached to any
+ * controller. Use the nvme_ns_detach_ctrls() first if the namespace is still
+ * attached.
+ *
+ * Return: The nvme command status if a response was received (see
+ * &enum nvme_status_field) or -1 with errno set otherwise.
+ */
+static inline int nvme_ns_mgmt_delete(int fd, __u32 nsid)
+{
+	return nvme_ns_mgmt_delete_timeout(fd, nsid, 0);
+}
+
+/**
  * nvme_ns_attach() - Attach or detach namespace to controller(s)
  * @args:	&struct nvme_ns_attach_args Argument structure
  *
  * Return: The nvme command status if a response was received (see
  * &enum nvme_status_field) or -1 with errno set otherwise.
  */
 int nvme_ns_attach(struct nvme_ns_attach_args *args);
@@ -4043,20 +4181,8 @@
  * @args:	&struct nvme_dim_args argument structure
  *
  * Return: The nvme command status if a response was received (see
  * &enum nvme_status_field) or -1 with errno set otherwise.
  */
 int nvme_dim_send(struct nvme_dim_args *args);
 
-/**
- * nvme_set_debug - Set NVMe command debugging output
- * @debug:	true to enable or false to disable
- */
-void nvme_set_debug(bool debug);
-
-/**
- * nvme_get_debug - Get NVMe command debugging output
- *
- * Return: false if disabled or true if enabled.
- */
-bool nvme_get_debug(void);
 #endif /* _LIBNVME_IOCTL_H */
```

### Comparing `libnvme-1.8/src/nvme/json.c` & `libnvme-1.9/src/nvme/json.c`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,70 @@
 #include "linux.h"
 
 #define JSON_UPDATE_INT_OPTION(c, k, a, o)				\
 	if (!strcmp(# a, k ) && !c->a) c->a = json_object_get_int(o);
 #define JSON_UPDATE_BOOL_OPTION(c, k, a, o)				\
 	if (!strcmp(# a, k ) && !c->a) c->a = json_object_get_boolean(o);
 
+static void json_import_nvme_tls_key(nvme_ctrl_t c, const char *keyring_str,
+				     const char *encoded_key)
+{
+	struct nvme_fabrics_config *cfg = nvme_ctrl_get_config(c);
+	const char *hostnqn = nvme_host_get_hostnqn(c->s->h);
+	const char *subsysnqn = nvme_ctrl_get_subsysnqn(c);
+	int key_len;
+	unsigned int hmac;
+	long key_id;
+	_cleanup_free_ unsigned char *key_data = NULL;
+
+	if (!hostnqn || !subsysnqn) {
+		nvme_msg(NULL, LOG_ERR, "Invalid NQNs (%s, %s)\n",
+			 hostnqn, subsysnqn);
+		return;
+	}
+	key_data = nvme_import_tls_key(encoded_key, &key_len, &hmac);
+	if (!key_data) {
+		nvme_msg(NULL, LOG_ERR, "Failed to decode TLS Key '%s'\n",
+			encoded_key);
+		return;
+	}
+	key_id = nvme_insert_tls_key_versioned(keyring_str, "psk",
+					       hostnqn, subsysnqn,
+					       0, hmac, key_data, key_len);
+	if (key_id <= 0)
+		nvme_msg(NULL, LOG_ERR, "Failed to insert TLS KEY, error %d\n",
+			 errno);
+	else {
+		cfg->tls_key = key_id;
+		cfg->tls = true;
+	}
+}
+
+static void json_export_nvme_tls_key(long keyring_id, long tls_key,
+				     struct json_object *obj)
+{
+	int key_len;
+	_cleanup_free_ unsigned char *key_data = NULL;
+
+	key_data = nvme_read_key(keyring_id, tls_key, &key_len);
+	if (key_data) {
+		_cleanup_free_ char *tls_str = NULL;
+
+		tls_str = nvme_export_tls_key(key_data, key_len);
+		if (tls_str)
+			json_object_object_add(obj, "tls_key",
+					       json_object_new_string(tls_str));
+	}
+}
+
 static void json_update_attributes(nvme_ctrl_t c,
 				   struct json_object *ctrl_obj)
 {
 	struct nvme_fabrics_config *cfg = nvme_ctrl_get_config(c);
+	const char *keyring_str = NULL, *encoded_key = NULL;
 
 	json_object_object_foreach(ctrl_obj, key_str, val_obj) {
 		JSON_UPDATE_INT_OPTION(cfg, key_str,
 				       nr_io_queues, val_obj);
 		JSON_UPDATE_INT_OPTION(cfg, key_str,
 				       nr_write_queues, val_obj);
 		JSON_UPDATE_INT_OPTION(cfg, key_str,
@@ -71,29 +123,32 @@
 		/*
 		 * The JSON configuration holds the keyring description
 		 * which needs to be converted into the keyring serial number.
 		 */
 		if (!strcmp("keyring", key_str) && cfg->keyring == 0) {
 			long keyring;
 
-			keyring = nvme_lookup_keyring(json_object_get_string(val_obj));
+			keyring_str = json_object_get_string(val_obj);
+			keyring = nvme_lookup_keyring(keyring_str);
 			if (keyring) {
 				cfg->keyring = keyring;
 				nvme_set_keyring(cfg->keyring);
 			}
 		}
-		if (!strcmp("tls_key", key_str) && cfg->tls_key == 0) {
-			long key;
-
-			key = nvme_lookup_key("psk",
-					      json_object_get_string(val_obj));
-			if (key)
-				cfg->tls_key = key;
-		}
+		if (!strcmp("tls_key", key_str) && cfg->tls_key == 0)
+			encoded_key = json_object_get_string(val_obj);
 	}
+
+	/*
+	 * We might need the keyring information from the above loop,
+	 * so we can only import the TLS key once all entries are
+	 * processed.
+	 */
+	if (encoded_key)
+		json_import_nvme_tls_key(c, keyring_str, encoded_key);
 }
 
 static void json_parse_port(nvme_subsystem_t s, struct json_object *port_obj)
 {
 	nvme_ctrl_t c;
 	struct json_object *attr_obj;
 	const char *transport, *traddr = NULL;
@@ -342,23 +397,19 @@
 			nvme_describe_key_serial(cfg->keyring);
 
 		if (desc) {
 			json_object_object_add(port_obj, "keyring",
 					       json_object_new_string(desc));
 		}
 	}
-	if (cfg->tls_key) {
-		_cleanup_free_ char *desc =
-			nvme_describe_key_serial(cfg->tls_key);
-
-		if (desc) {
-			json_object_object_add(port_obj, "tls_key",
-					       json_object_new_string(desc));
-		}
-	}
+	/*
+	 * Store the TLS key in PSK interchange format
+	 */
+	if (cfg->tls_key)
+		json_export_nvme_tls_key(cfg->keyring, cfg->tls_key, port_obj);
 
 	json_object_array_add(ctrl_array, port_obj);
 }
 
 static void json_update_subsys(struct json_object *subsys_array,
 			       nvme_subsystem_t s)
 {
@@ -499,15 +550,21 @@
 		JSON_INT_OPTION(cfg, ctrl_obj, fast_io_fail_tmo, 0);
 	}
 	JSON_INT_OPTION(cfg, ctrl_obj, tos, -1);
 	JSON_BOOL_OPTION(cfg, ctrl_obj, duplicate_connect);
 	JSON_BOOL_OPTION(cfg, ctrl_obj, disable_sqflow);
 	JSON_BOOL_OPTION(cfg, ctrl_obj, hdr_digest);
 	JSON_BOOL_OPTION(cfg, ctrl_obj, data_digest);
-	JSON_BOOL_OPTION(cfg, ctrl_obj, tls);
+	if (!strcmp(transport, "tcp")) {
+		JSON_BOOL_OPTION(cfg, ctrl_obj, tls);
+
+		if (cfg->tls_key)
+			json_export_nvme_tls_key(cfg->keyring, cfg->tls_key,
+						 ctrl_obj);
+	}
 	JSON_BOOL_OPTION(cfg, ctrl_obj, concat);
 	if (nvme_ctrl_is_persistent(c))
 		json_object_object_add(ctrl_obj, "persistent",
 				       json_object_new_boolean(true));
 	if (nvme_ctrl_is_discovery_ctrl(c))
 		json_object_object_add(ctrl_obj, "discovery",
 				       json_object_new_boolean(true));
```

### Comparing `libnvme-1.8/src/nvme/linux.c` & `libnvme-1.9/src/nvme/linux.c`

 * *Files 10% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 #include <openssl/core_names.h>
 #include <openssl/params.h>
 #endif
 #endif
 
 #ifdef CONFIG_KEYUTILS
 #include <keyutils.h>
+
+#define NVME_TLS_DEFAULT_KEYRING ".nvme"
 #endif
 
 #include <ccan/endian/endian.h>
 
 #include "cleanup.h"
 #include "linux.h"
 #include "tree.h"
 #include "log.h"
 #include "private.h"
 #include "base64.h"
+#include "crc32.h"
 
 static int __nvme_open(const char *name)
 {
 	_cleanup_free_ char *path = NULL;
 	int ret;
 
 	ret = asprintf(&path, "%s/%s", "/dev", name);
@@ -179,15 +182,15 @@
 		.csi = NVME_CSI_NVM,
 		.rae = rae,
 		.ot = false,
 	};
 
 	*size = 0;
 
-	log = malloc(xfer);
+	log = __nvme_alloc(xfer);
 	if (!log) {
 		errno = ENOMEM;
 		return -1;
 	}
 
 	if (ctrl) {
 		err = nvme_get_log_telemetry_ctrl(fd, true, 0, xfer, log);
@@ -232,15 +235,15 @@
 
 	if (dalb == 0) {
 		errno = ENOENT;
 		return -1;
 	}
 
 	*size = (dalb + 1) * xfer;
-	tmp = realloc(log, *size);
+	tmp = __nvme_realloc(log, *size);
 	if (!tmp) {
 		errno = ENOMEM;
 		return -1;
 	}
 	log = tmp;
 
 	args.lid = lid;
@@ -1154,14 +1157,16 @@
 }
 
 #ifdef CONFIG_KEYUTILS
 long nvme_lookup_keyring(const char *keyring)
 {
 	key_serial_t keyring_id;
 
+	if (!keyring)
+		keyring = NVME_TLS_DEFAULT_KEYRING;
 	keyring_id = find_key_by_type_and_desc("keyring", keyring, 0);
 	if (keyring_id < 0)
 		return 0;
 	return keyring_id;
 }
 
 char *nvme_describe_key_serial(long key_id)
@@ -1183,66 +1188,174 @@
 	return key;
 }
 
 int nvme_set_keyring(long key_id)
 {
 	long err;
 
+	if (key_id == 0) {
+		key_id = nvme_lookup_keyring(NULL);
+		if (key_id == 0) {
+			errno = ENOKEY;
+			return -1;
+		}
+	}
+
 	err = keyctl_link(key_id, KEY_SPEC_SESSION_KEYRING);
 	if (err < 0)
 		return -1;
 	return 0;
 }
 
+unsigned char *nvme_read_key(long keyring_id, long key_id, int *len)
+{
+	void *buffer;
+	int ret;
+
+	ret = nvme_set_keyring(keyring_id);
+	if (ret < 0) {
+		errno = -ret;
+		return NULL;
+	}
+	ret = keyctl_read_alloc(key_id, &buffer);
+	if (ret < 0) {
+		errno = -ret;
+		buffer = NULL;
+	} else
+		*len = ret;
+
+	return buffer;
+}
+
+long nvme_update_key(long keyring_id, const char *key_type,
+		     const char *identity, unsigned char *key_data,
+		     int key_len)
+{
+	long key;
+
+	key = keyctl_search(keyring_id, key_type, identity, 0);
+	if (key > 0) {
+		if (keyctl_revoke(key) < 0)
+			return 0;
+	}
+	key = add_key(key_type, identity,
+		      key_data, key_len, keyring_id);
+	if (key < 0)
+		key = 0;
+	return key;
+}
+
+struct __scan_keys_data {
+	nvme_scan_tls_keys_cb_t cb;
+	key_serial_t keyring;
+	void *data;
+};
+
+int __scan_keys_cb(key_serial_t parent, key_serial_t key,
+		   char *desc, int desc_len, void *data)
+{
+	struct __scan_keys_data *d = data;
+	int ver, hmac, uid, gid, perm;
+	char type, *ptr;
+
+	if (desc_len < 6)
+		return 0;
+	if (sscanf(desc, "psk;%d;%d;%08x;NVMe%01d%c%02d %*s",
+		   &uid, &gid, &perm, &ver, &type, &hmac) != 6)
+		return 0;
+	/* skip key type */
+	ptr = strchr(desc, ';');
+	if (!ptr)
+		return 0;
+	/* skip key uid */
+	ptr = strchr(ptr + 1, ';');
+	if (!ptr)
+		return 0;
+	/* skip key gid */
+	ptr = strchr(ptr + 1, ';');
+	if (!ptr)
+		return 0;
+	/* skip key permissions */
+	ptr = strchr(ptr + 1, ';');
+	if (!ptr)
+		return 0;
+	/* Only use the key description for the callback */
+	(d->cb)(d->keyring, key, ptr + 1, strlen(ptr) - 1, d->data);
+	return 1;
+}
+
+int nvme_scan_tls_keys(const char *keyring, nvme_scan_tls_keys_cb_t cb,
+		       void *data)
+{
+	struct __scan_keys_data d;
+	key_serial_t keyring_id = nvme_lookup_keyring(keyring);
+	int ret;
+
+	if (!keyring_id) {
+		errno = EINVAL;
+		return -1;
+	}
+	ret = nvme_set_keyring(keyring_id);
+	if (ret < 0)
+		return ret;
+
+	d.keyring = keyring_id;
+	d.cb = cb;
+	d.data = data;
+	ret = recursive_key_scan(keyring_id, __scan_keys_cb, &d);
+	return ret;
+}
+
 long nvme_insert_tls_key_versioned(const char *keyring, const char *key_type,
 				   const char *hostnqn, const char *subsysnqn,
 				   int version, int hmac,
 				   unsigned char *configured_key, int key_len)
 {
 	key_serial_t keyring_id, key;
 	_cleanup_free_ char *identity = NULL;
 	size_t identity_len;
 	_cleanup_free_ unsigned char *psk = NULL;
-	int ret = -1;
+	int ret;
 
 	keyring_id = nvme_lookup_keyring(keyring);
-	if (keyring_id == 0)
-		return -1;
+	if (keyring_id == 0) {
+		errno = ENOKEY;
+		return 0;
+	}
+
+	ret = nvme_set_keyring(keyring_id);
+	if (ret < 0)
+		return 0;
 
 	identity_len = nvme_identity_len(hmac, version, hostnqn, subsysnqn);
 	if (identity_len < 0)
-		return -1;
+		return 0;
 
 	identity = malloc(identity_len);
 	if (!identity) {
 		errno = ENOMEM;
-		return -1;
+		return 0;
 	}
+	memset(identity, 0, identity_len);
 
 	psk = malloc(key_len);
 	if (!psk) {
 		errno = ENOMEM;
 		return 0;
 	}
 	memset(psk, 0, key_len);
 	ret = derive_nvme_keys(hostnqn, subsysnqn, identity, version, hmac,
 			       configured_key, psk, key_len);
-	if (ret != key_len)
+	if (ret != key_len) {
+		errno = ENOKEY;
 		return 0;
-
-	key = keyctl_search(keyring_id, key_type, identity, 0);
-	if (key > 0) {
-		if (keyctl_update(key, psk, key_len) < 0)
-			key = 0;
-	} else {
-		key = add_key(key_type, identity,
-			      psk, key_len, keyring_id);
-		if (key < 0)
-			key = 0;
 	}
+
+	key = nvme_update_key(keyring_id, key_type, identity,
+			      psk, key_len);
 	return key;
 }
 
 #else
 long nvme_lookup_keyring(const char *keyring)
 {
 	nvme_msg(NULL, LOG_ERR, "key operations not supported; "\
@@ -1271,14 +1384,35 @@
 {
 	nvme_msg(NULL, LOG_ERR, "key operations not supported; "\
 		 "recompile with keyutils support.\n");
 	errno = ENOTSUP;
 	return -1;
 }
 
+unsigned char *nvme_read_key(long keyring_id, long key_id, int *len)
+{
+	errno = ENOTSUP;
+	return NULL;
+}
+
+long nvme_update_key(long keyring_id, const char *key_type,
+		     const char *identity, unsigned char *key_data,
+		     int key_len)
+{
+	errno = ENOTSUP;
+	return 0;
+}
+
+int nvme_scan_tls_keys(const char *keyring, nvme_scan_tls_keys_cb_t cb,
+		       void *data)
+{
+	errno = ENOTSUP;
+	return -1;
+}
+
 long nvme_insert_tls_key_versioned(const char *keyring, const char *key_type,
 				   const char *hostnqn, const char *subsysnqn,
 				   int version, int hmac,
 				   unsigned char *configured_key, int key_len)
 {
 	nvme_msg(NULL, LOG_ERR, "key operations not supported; "
 		 "recompile with keyutils support.\n");
@@ -1291,7 +1425,112 @@
 			 const char *hostnqn, const char *subsysnqn, int hmac,
 			 unsigned char *configured_key, int key_len)
 {
 	return nvme_insert_tls_key_versioned(keyring, key_type,
 					     hostnqn, subsysnqn, 0, hmac,
 					     configured_key, key_len);
 }
+
+char *nvme_export_tls_key(const unsigned char *key_data, int key_len)
+{
+	unsigned char raw_secret[52];
+	char *encoded_key;
+	unsigned int raw_len, encoded_len, len;
+	unsigned long crc = crc32(0L, NULL, 0);
+
+	if (key_len == 32) {
+		raw_len = 32;
+	} else if (key_len == 48) {
+		raw_len = 48;
+	} else {
+		errno = EINVAL;
+		return NULL;
+	}
+
+	memcpy(raw_secret, key_data, raw_len);
+	crc = crc32(crc, raw_secret, raw_len);
+	raw_secret[raw_len++] = crc & 0xff;
+	raw_secret[raw_len++] = (crc >> 8) & 0xff;
+	raw_secret[raw_len++] = (crc >> 16) & 0xff;
+	raw_secret[raw_len++] = (crc >> 24) & 0xff;
+
+	encoded_len = (raw_len * 2) + 20;
+	encoded_key = malloc(encoded_len);
+	if (!encoded_key) {
+		errno = ENOMEM;
+		return NULL;
+	}
+	memset(encoded_key, 0, encoded_len);
+	len = sprintf(encoded_key, "NVMeTLSkey-1:%02x:",
+		      key_len == 32 ? 1 : 2);
+	len += base64_encode(raw_secret, raw_len, encoded_key + len);
+	encoded_key[len++] = ':';
+	encoded_key[len++] = '\0';
+
+	return encoded_key;
+}
+
+unsigned char *nvme_import_tls_key(const char *encoded_key, int *key_len,
+				   unsigned int *hmac)
+{
+	unsigned char decoded_key[128], *key_data;
+	unsigned int crc = crc32(0L, NULL, 0);
+	unsigned int key_crc;
+	int err, decoded_len;
+
+	if (sscanf(encoded_key, "NVMeTLSkey-1:%02x:*s", &err) != 1) {
+		errno = EINVAL;
+		return NULL;
+	}
+	switch (err) {
+	case 1:
+		if (strlen(encoded_key) != 65) {
+			errno = EINVAL;
+			return NULL;
+		}
+		break;
+	case 2:
+		if (strlen(encoded_key) != 89) {
+			errno = EINVAL;
+			return NULL;
+		}
+		break;
+	default:
+		errno = EINVAL;
+		return NULL;
+	}
+
+	*hmac = err;
+	err = base64_decode(encoded_key + 16, strlen(encoded_key) - 17,
+			    decoded_key);
+	if (err < 0) {
+		errno = ENOKEY;
+		return NULL;
+	}
+	decoded_len = err;
+	decoded_len -= 4;
+	if (decoded_len != 32 && decoded_len != 48) {
+		errno = ENOKEY;
+		return NULL;
+	}
+	crc = crc32(crc, decoded_key, decoded_len);
+	key_crc = ((u_int32_t)decoded_key[decoded_len]) |
+		((u_int32_t)decoded_key[decoded_len + 1] << 8) |
+		((u_int32_t)decoded_key[decoded_len + 2] << 16) |
+		((u_int32_t)decoded_key[decoded_len + 3] << 24);
+	if (key_crc != crc) {
+		nvme_msg(NULL, LOG_ERR, "CRC mismatch (key %08x, crc %08x)",
+			 key_crc, crc);
+		errno = ENOKEY;
+		return NULL;
+	}
+
+	key_data = malloc(decoded_len);
+	if (!key_data) {
+		errno = ENOMEM;
+		return NULL;
+	}
+	memcpy(key_data, decoded_key, decoded_len);
+
+	*key_len = decoded_len;
+	return key_data;
+}
```

### Comparing `libnvme-1.8/src/nvme/linux.h` & `libnvme-1.9/src/nvme/linux.h`

 * *Files 20% similar despite different names*

```diff
@@ -270,14 +270,80 @@
  *
  * Return: 0 on success, a negative number on error
  * with errno set.
  */
 int nvme_set_keyring(long keyring_id);
 
 /**
+ * nvme_read_key() - Read key raw data
+ * @keyring_id:     Id of the keyring holding %key_id
+ * @key_id:      Key id
+ * @len:         Length of the returned data
+ *
+ * Links the keyring specified by @keyring_id into the session
+ * keyring and reads the payload of the key specified by @key_id.
+ * @len holds the size of the returned buffer.
+ * If @keyring is 0 the default keyring '.nvme' is used.
+ *
+ * Return: Pointer to the payload on success,
+ * or NULL with errno set otherwise.
+ */
+unsigned char *nvme_read_key(long keyring_id, long key_id, int *len);
+
+/**
+ * nvme_update_key() - Update key raw data
+ * @keyring_id:  Id of the keyring holding %key_id
+ * @key_type:    Type of the key to insert
+ * @identity:    Key identity string
+ * @key_data:    Raw data of the key
+ * @key_len:     Length of @key_data
+ *
+ * Links the keyring specified by @keyring_id into the session
+ * keyring and updates the key reference by @identity with @key_data.
+ * The old key with identity @identity will be revoked to make it
+ * inaccessible.
+ *
+ * Return: Key id of the new key or 0 with errno set otherwise.
+ */
+long nvme_update_key(long keyring_id, const char *key_type,
+		     const char *identity, unsigned char *key_data,
+		     int key_len);
+
+/**
+ * typedef nvme_scan_tls_keys_cb_t - Callback for iterating TLS keys
+ * @keyring:	Keyring which has been iterated
+ * @key:	Key for which the callback has been invoked
+ * @desc:	Description of the key
+ * @desc_len:	Length of @desc
+ * @data:	Pointer for caller data
+ *
+ * Called for each TLS PSK in the keyring.
+ */
+typedef void (*nvme_scan_tls_keys_cb_t)(long keyring, long key,
+					char *desc, int desc_len, void *data);
+
+/**
+ * nvme_scan_tls_keys() - Iterate over TLS keys in a keyring
+ * @keyring:	Keyring holding TLS keys
+ * @cb:		Callback function
+ * @data:	Pointer for data to be passed to @cb
+ *
+ * Iterates @keyring and call @cb for each TLS key. When @keyring is NULL
+ * the default '.nvme' keyring is used.
+ * A TLS key must be of type 'psk' and the description must be of the
+ * form 'NVMe<0|1><R|G>0<1|2> <identity>', otherwise it will be skipped
+ * during iteration.
+ *
+ * Return: Number of keys for which @cb was called, or -1 with errno set
+ * on error.
+ */
+int nvme_scan_tls_keys(const char *keyring, nvme_scan_tls_keys_cb_t cb,
+		       void *data);
+
+/**
  * nvme_insert_tls_key() - Derive and insert TLS key
  * @keyring:    Keyring to use
  * @key_type:	Type of the resulting key
  * @hostnqn:	Host NVMe Qualified Name
  * @subsysnqn:	Subsystem NVMe Qualified Name
  * @hmac:	HMAC algorithm
  * @configured_key:	Configured key data to derive the key from
@@ -331,8 +397,72 @@
  * Return: The string containing the TLS identity. It is the responsibility
  * of the caller to free the returned string.
  */
 char *nvme_generate_tls_key_identity(const char *hostnqn, const char *subsysnqn,
 				     int version, int hmac,
 				     unsigned char *configured_key, int key_len);
 
+/**
+ * nvme_export_tls_key() - Export a TLS key
+ * @key_data:	Raw data of the key
+ * @key_len:	Length of @key_data
+ *
+ * Returns @key_data in the PSK Interchange format as defined in section
+ * 3.6.1.5 of the NVMe TCP Transport specification.
+ *
+ * Return: The string containing the TLS identity or NULL with errno set
+ * on error. It is the responsibility of the caller to free the returned
+ * string.
+ */
+char *nvme_export_tls_key(const unsigned char *key_data, int key_len);
+
+/**
+ * nvme_import_tls_key() - Import a TLS key
+ * @encoded_key:	TLS key in PSK interchange format
+ * @key_len:		Length of the resulting key data
+ * @hmac:		HMAC algorithm
+ *
+ * Imports @key_data in the PSK Interchange format as defined in section
+ * 3.6.1.5 of the NVMe TCP Transport specification.
+ *
+ * Return: The raw data of the PSK or NULL with errno set on error. It is
+ * the responsibility of the caller to free the returned string.
+ */
+unsigned char *nvme_import_tls_key(const char *encoded_key, int *key_len,
+				   unsigned int *hmac);
+
+/**
+ * nvme_submit_passthru - Low level ioctl wrapper for passthru commands
+ * @fd:		File descriptor of the nvme device
+ * @ioctl_cmd:	IOCTL command id
+ * @cmd:	Passhtru command
+ * @result:	Optional field to return the result
+ *
+ * This is a low level library function which should not be used directly. It is
+ * exposed as weak symbol so that the user application is able to provide their own
+ * implementation of this function with additional debugging or logging code.
+ *
+ * Return: The value from the ioctl system call (see ioctl documentation)
+ */
+__attribute__((weak))
+int nvme_submit_passthru(int fd, unsigned long ioctl_cmd,
+			 struct nvme_passthru_cmd *cmd, __u32 *result);
+
+/**
+ * nvme_submit_passthru64 - Low level ioctl wrapper for passthru commands
+ * @fd:		File descriptor of the nvme device
+ * @ioctl_cmd:	IOCTL command id
+ * @cmd:	Passhtru command
+ * @result:	Optional field to return the result
+ *
+ * This is a low level library function which should not be used directly. It is
+ * exposed as weak symbol so that the user application is able to provide their own
+ * implementation of this function with additional debugging or logging code.
+ *
+ * Return: The value from the ioctl system call (see ioctl documentation)
+ */
+__attribute__((weak))
+int nvme_submit_passthru64(int fd, unsigned long ioctl_cmd,
+			   struct nvme_passthru_cmd64 *cmd,
+			   __u64 *result);
+
 #endif /* _LIBNVME_LINUX_H */
```

### Comparing `libnvme-1.8/src/nvme/log.c` & `libnvme-1.9/src/nvme/log.c`

 * *Files 14% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 		r = root;
 
 	if (r)
 		fp = r->fp;
 
 	if (r && lvl > r->log_level)
 		return;
+	if (!r && lvl > DEFAULT_LOGLEVEL)
+		return;
 
 	if (r && r->log_timestamp) {
 		struct timespec now;
 
 		clock_gettime(LOG_CLOCK, &now);
 		snprintf(timebuf, sizeof(timebuf), "%6ld.%06ld",
 			 (long)now.tv_sec, now.tv_nsec / 1000);
@@ -95,11 +97,34 @@
 void nvme_init_logging(nvme_root_t r, int lvl, bool log_pid, bool log_tstamp)
 {
 	r->log_level = lvl;
 	r->log_pid = log_pid;
 	r->log_timestamp = log_tstamp;
 }
 
+int nvme_get_logging_level(nvme_root_t r, bool *log_pid, bool *log_tstamp)
+{
+	if (!r)
+		r = root;
+	if (!r)
+		return DEFAULT_LOGLEVEL;
+	if (log_pid)
+		*log_pid = r->log_pid;
+	if (log_tstamp)
+		*log_tstamp = r->log_timestamp;
+	return r->log_level;
+}
+
 void nvme_set_root(nvme_root_t r)
 {
 	root = r;
 }
+
+void nvme_set_debug(bool debug)
+{
+	root->log_level = debug ? LOG_DEBUG : DEFAULT_LOGLEVEL;
+}
+
+bool nvme_get_debug(void)
+{
+	return root->log_level == LOG_DEBUG;
+}
```

### Comparing `libnvme-1.8/src/nvme/mi-mctp.c` & `libnvme-1.9/src/nvme/mi-mctp.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/mi.c` & `libnvme-1.9/src/nvme/mi.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/mi.h` & `libnvme-1.9/src/nvme/mi.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/src/nvme/nbft.c` & `libnvme-1.9/src/nvme/nbft.c`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,20 @@
 	ssns->subsys_port_id = le16_to_cpu(raw_ssns->subsys_port_id);
 
 	/* NSID, NID type, & NID */
 	ssns->nsid = le32_to_cpu(raw_ssns->nsid);
 	ssns->nid_type = raw_ssns->nidt;
 	ssns->nid = raw_ssns->nid;
 
+	/* flags */
+	ssns->unavailable = !!(le16_to_cpu(raw_ssns->flags) &
+			       NBFT_SSNS_UNAVAIL_NAMESPACE_UNAVAIL);
+	ssns->discovered = !!(le16_to_cpu(raw_ssns->flags) &
+			      NBFT_SSNS_DISCOVERED_NAMESPACE);
+
 	/* security profile */
 	if (raw_ssns->security_desc_index) {
 		ssns->security = security_from_index(nbft, raw_ssns->security_desc_index);
 		if (!ssns->security)
 			nvme_msg(NULL, LOG_DEBUG,
 				 "file %s: namespace %d security controller not found\n",
 				 nbft->filename, ssns->index);
```

### Comparing `libnvme-1.8/src/nvme/nbft.h` & `libnvme-1.9/src/nvme/nbft.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
  */
 #ifndef _NBFT_H
 #define _NBFT_H
 
 #include <sys/types.h>
 #include "util.h"
 
+/**
+ * DOC: nbft.h
+ *
+ * NVM Express Boot Specification, Revision 1.0
+ *
+ * Note: this API is currently unstable, subject to further additions.
+ */
+
 /*
  *  ACPI NBFT table structures (TP8012 Boot Specification rev. 1.0)
  */
 
 /**
  * enum nbft_desc_type - NBFT Elements - Descriptor Types (Figure 5)
  * @NBFT_DESC_HEADER:	     Header: an ACPI structure header with some additional
@@ -990,87 +998,87 @@
 /*
  *  Convenient NBFT table parser ('nbft_info' prefix)
  */
 
 /**
  * enum nbft_info_primary_admin_host_flag - Primary Administrative Host Descriptor Flags
  * @NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_NOT_INDICATED: Not Indicated by Driver: The driver
- * 						     that created this NBFT provided no
- * 						     administrative priority hint for
- * 						     this NBFT.
+ *						     that created this NBFT provided no
+ *						     administrative priority hint for
+ *						     this NBFT.
  * @NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_UNSELECTED:    Unselected: The driver that created
- * 						     this NBFT explicitly indicated that
- * 						     this NBFT should not be prioritized
- * 						     over any other NBFT.
+ *						     this NBFT explicitly indicated that
+ *						     this NBFT should not be prioritized
+ *						     over any other NBFT.
  * @NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_SELECTED:	     Selected: The driver that created
- * 						     this NBFT explicitly indicated that
- * 						     this NBFT should be prioritized over
- * 						     any other NBFT.
+ *						     this NBFT explicitly indicated that
+ *						     this NBFT should be prioritized over
+ *						     any other NBFT.
  * @NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_RESERVED:	     Reserved.
  */
 enum nbft_info_primary_admin_host_flag {
 	NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_NOT_INDICATED,
 	NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_UNSELECTED,
 	NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_SELECTED,
 	NBFT_INFO_PRIMARY_ADMIN_HOST_FLAG_RESERVED,
 };
 
 /**
  * struct nbft_info_host - Host Descriptor
  * @id:			 Host ID (raw UUID, length = 16 bytes).
  * @nqn:		 Host NQN.
  * @host_id_configured:	 HostID Configured Flag: value of True indicates that @id
- * 			 contains administratively-configured value, or driver
- * 			 default value if False.
+ *			 contains administratively-configured value, or driver
+ *			 default value if False.
  * @host_nqn_configured: Host NQN Configured Flag: value of True indicates that
- * 			 @nqn contains administratively-configured value,
- * 			 or driver default value if False.
+ *			 @nqn contains administratively-configured value,
+ *			 or driver default value if False.
  * @primary:		 Primary Administrative Host Descriptor, see
- * 			 &enum nbft_info_primary_admin_host_flag.
+ *			 &enum nbft_info_primary_admin_host_flag.
  */
 struct nbft_info_host {
 	unsigned char *id;
 	char *nqn;
 	bool host_id_configured;
 	bool host_nqn_configured;
 	enum nbft_info_primary_admin_host_flag primary;
 };
 
 /**
  * struct nbft_info_hfi_info_tcp - HFI Transport Info Descriptor - NVMe/TCP
  * @pci_sbdf:		       PCI Express Routing ID for the HFI Transport Function.
  * @mac_addr:		       MAC Address: The MAC address of this HFI,
- * 			       in EUI-48TM format.
+ *			       in EUI-48TM format.
  * @vlan:		       The VLAN identifier if the VLAN is associated with
- * 			       this HFI, as defined in IEEE 802.1q-2018 or zeroes
- * 			       if no VLAN is associated with this HFI.
+ *			       this HFI, as defined in IEEE 802.1q-2018 or zeroes
+ *			       if no VLAN is associated with this HFI.
  * @ip_origin:		       The source of Ethernet L3 configuration information
- * 			       used by the driver or 0 if not used.
+ *			       used by the driver or 0 if not used.
  * @ipaddr:		       The IPv4 or IPv6 address of this HFI.
  * @subnet_mask_prefix:	       The IPv4 or IPv6 subnet mask in CIDR routing prefix
- * 			       notation.
+ *			       notation.
  * @gateway_ipaddr:	       The IPv4 or IPv6 address of the IP gateway for this
- * 			       HFI or zeroes if no IP gateway is specified.
+ *			       HFI or zeroes if no IP gateway is specified.
  * @route_metric:	       The cost value for the route indicated by this HFI.
  * @primary_dns_ipaddr:	       The IPv4 or IPv6 address of the Primary DNS server
- * 			       for this HFI.
+ *			       for this HFI.
  * @secondary_dns_ipaddr:      The IPv4 or IPv6 address of the Secondary DNS server
- * 			       for this HFI.
+ *			       for this HFI.
  * @dhcp_server_ipaddr:	       The IPv4 or IPv6 address of the DHCP server used
- * 			       to assign this HFI address.
+ *			       to assign this HFI address.
  * @host_name:		       The Host Name string.
  * @this_hfi_is_default_route: If True, then the BIOS utilized this interface
- * 			       described by HFI to be the default route with highest
- * 			       priority. If False, then routes are local to their
- * 			       own scope.
+ *			       described by HFI to be the default route with highest
+ *			       priority. If False, then routes are local to their
+ *			       own scope.
  * @dhcp_override:	       If True, then HFI information was populated
- * 			       by consuming the DHCP on this interface. If False,
- * 			       then the HFI information was set administratively
- * 			       by a configuration interface to the driver and
- * 			       pre-OS envrionment.
+ *			       by consuming the DHCP on this interface. If False,
+ *			       then the HFI information was set administratively
+ *			       by a configuration interface to the driver and
+ *			       pre-OS envrionment.
  */
 struct nbft_info_hfi_info_tcp {
 	__u32 pci_sbdf;
 	__u8 mac_addr[6];
 	__u16 vlan;
 	__u8 ip_origin;
 	char ipaddr[40];
@@ -1084,47 +1092,47 @@
 	bool this_hfi_is_default_route;
 	bool dhcp_override;
 };
 
 /**
  * struct nbft_info_hfi - Host Fabric Interface (HFI) Descriptor
  * @index:     HFI Descriptor Index: indicates the number of this HFI Descriptor
- * 	       in the Host Fabric Interface Descriptor List.
+ *	       in the Host Fabric Interface Descriptor List.
  * @transport: Transport Type string (e.g. 'tcp').
  * @tcp_info:  The HFI Transport Info Descriptor, see &struct nbft_info_hfi_info_tcp.
  */
 struct nbft_info_hfi {
 	int index;
 	char transport[8];
 	struct nbft_info_hfi_info_tcp tcp_info;
 };
 
 /**
  * struct nbft_info_discovery - Discovery Descriptor
  * @index:    The number of this Discovery Descriptor in the Discovery
- * 	      Descriptor List.
+ *	      Descriptor List.
  * @security: The Security Profile Descriptor, see &struct nbft_info_security.
  * @hfi:      The HFI Descriptor associated with this Discovery Descriptor.
- * 	      See &struct nbft_info_hfi.
+ *	      See &struct nbft_info_hfi.
  * @uri:      A URI which indicates an NVMe Discovery controller associated
- * 	      with this Discovery Descriptor.
+ *	      with this Discovery Descriptor.
  * @nqn:      An NVMe Discovery controller NQN.
  */
 struct nbft_info_discovery {
 	int index;
 	struct nbft_info_security *security;
 	struct nbft_info_hfi *hfi;
 	char *uri;
 	char *nqn;
 };
 
 /**
  * struct nbft_info_security - Security Profile Descriptor
  * @index: The number of this Security Profile Descriptor in the Security
- * 	   Profile Descriptor List.
+ *	   Profile Descriptor List.
  */
 struct nbft_info_security {
 	int index;
 	/* TODO add fields */
 };
 
 /**
@@ -1139,43 +1147,47 @@
 	NBFT_INFO_NID_TYPE_EUI64	= 1,
 	NBFT_INFO_NID_TYPE_NGUID	= 2,
 	NBFT_INFO_NID_TYPE_NS_UUID	= 3,
 };
 
 /**
  * struct nbft_info_subsystem_ns - Subsystem Namespace (SSNS) info
- * @index: 			SSNS Descriptor Index in the descriptor list.
+ * @index:			SSNS Descriptor Index in the descriptor list.
  * @discovery:			Primary Discovery Controller associated with
- * 				this SSNS Descriptor.
+ *				this SSNS Descriptor.
  * @security:			Security Profile Descriptor associated with
- * 				this namespace.
+ *				this namespace.
  * @num_hfis:			Number of HFIs.
  * @hfis:			List of HFIs associated with this namespace.
- * 				Includes the primary HFI at the first position
- * 				and all secondary HFIs. This array is null-terminated.
+ *				Includes the primary HFI at the first position
+ *				and all secondary HFIs. This array is null-terminated.
  * @transport:			Transport Type string (e.g. 'tcp').
  * @traddr:			Subsystem Transport Address.
  * @trsvcid:			Subsystem Transport Service Identifier.
  * @subsys_port_id:		The Subsystem Port ID.
  * @nsid:			The Namespace ID of this descriptor or when @nid
- * 				should be used instead.
+ *				should be used instead.
  * @nid_type:			Namespace Identifier Type, see &enum nbft_info_nid_type.
  * @nid:			The Namespace Identifier value.
  * @subsys_nqn:			Subsystem and Namespace NQN.
  * @pdu_header_digest_required:	PDU Header Digest (HDGST) Flag: the use of NVM Header
- * 				Digest Enabled is required.
- * @data_digest_required: 	Data Digest (DDGST) Flag: the use of NVM Data Digest
- * 				Enabled is required.
+ *				Digest Enabled is required.
+ * @data_digest_required:	Data Digest (DDGST) Flag: the use of NVM Data Digest
+ *				Enabled is required.
  * @controller_id:		Controller ID (SSNS Extended Information Descriptor):
- * 				The controller ID associated with the Admin Queue
- * 				or 0 if not supported.
+ *				The controller ID associated with the Admin Queue
+ *				or 0 if not supported.
  * @asqsz:			Admin Submission Queue Size (SSNS Extended Information
- * 				Descriptor) or 0 if not supported.
+ *				Descriptor) or 0 if not supported.
  * @dhcp_root_path_string:	DHCP Root Path Override string (SSNS Extended
- * 				Information Descriptor).
+ *				Information Descriptor).
+ * @discovered:			Indicates that this namespace was acquired
+ *				through discovery.
+ * @unavailable:		Namespace is unavailable as indicated by
+ *				the pre-OS driver.
  */
 struct nbft_info_subsystem_ns {
 	int index;
 	struct nbft_info_discovery *discovery;
 	struct nbft_info_security *security;
 	int num_hfis;
 	struct nbft_info_hfi **hfis;
@@ -1188,14 +1200,16 @@
 	__u8 *nid;
 	char *subsys_nqn;
 	bool pdu_header_digest_required;
 	bool data_digest_required;
 	int controller_id;
 	int asqsz;
 	char *dhcp_root_path_string;
+	bool discovered;
+	bool unavailable;
 };
 
 /**
  * struct nbft_info - The parsed NBFT table data.
  * @filename:	       Path to the NBFT table.
  * @raw_nbft:	       The original NBFT table contents.
  * @raw_nbft_size:     Size of @raw_nbft.
```

### Comparing `libnvme-1.8/src/nvme/private.h` & `libnvme-1.9/src/nvme/private.h`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 #include <poll.h>
 #include <sys/socket.h>
 
 #include "fabrics.h"
 #include "mi.h"
 
 
-char *nvme_ctrl_sysfs_dir(void);
-char *nvme_subsys_sysfs_dir(void);
-char *nvme_ns_sysfs_dir(void);
+const char *nvme_subsys_sysfs_dir(void);
+const char *nvme_ctrl_sysfs_dir(void);
+const char *nvme_ns_sysfs_dir(void);
+const char *nvme_slots_sysfs_dir(void);
+const char *nvme_uuid_ibm_filename(void);
+const char *nvme_dmi_entries_dir(void);
 
 struct nvme_path {
 	struct list_node entry;
 	struct list_node nentry;
 
 	struct nvme_ctrl *c;
 	struct nvme_ns *n;
@@ -79,14 +82,15 @@
 	char *transport;
 	char *subsysnqn;
 	char *traddr;
 	char *trsvcid;
 	char *dhchap_key;
 	char *dhchap_ctrl_key;
 	char *cntrltype;
+	char *cntlid;
 	char *dctype;
 	char *phy_slot;
 	bool discovery_ctrl;
 	bool unique_discovery_ctrl;
 	bool discovered;
 	bool persistent;
 	struct nvme_fabrics_config cfg;
@@ -181,14 +185,16 @@
 nvme_ctrl_t __nvme_lookup_ctrl(nvme_subsystem_t s, const char *transport,
 			       const char *traddr, const char *host_traddr,
 			       const char *host_iface, const char *trsvcid,
 			       const char *subsysnqn, nvme_ctrl_t p);
 
 void *__nvme_alloc(size_t len);
 
+void *__nvme_realloc(void *p, size_t len);
+
 #if (LOG_FUNCNAME == 1)
 #define __nvme_log_func __func__
 #else
 #define __nvme_log_func NULL
 #endif
 
 void __attribute__((format(printf, 4, 5)))
@@ -282,8 +288,11 @@
 	ssize_t (*sendmsg)(int, const struct msghdr *, int);
 	ssize_t (*recvmsg)(int, struct msghdr *, int);
 	int (*poll)(struct pollfd *, nfds_t, int);
 	int (*ioctl_tag)(int, unsigned long, struct mctp_ioc_tag_ctl *);
 };
 void __nvme_mi_mctp_set_ops(const struct __mi_mctp_socket_ops *newops);
 
+#define SECTOR_SIZE	512
+#define SECTOR_SHIFT	9
+
 #endif /* _LIBNVME_PRIVATE_H */
```

### Comparing `libnvme-1.8/src/nvme/tree.c` & `libnvme-1.9/src/nvme/tree.c`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,14 @@
 	const char *host_iface;
 	struct ifaddrs *iface_list;
 	bool (*addreq)(const char *, const char *);
 	bool well_known_nqn;
 };
 typedef bool (*ctrl_match_t)(struct nvme_ctrl *c, struct candidate_args *candidate);
 
-#define PATH_SYSFS_SLOTS "/sys/bus/pci/slots"
-
-static char *nvme_slots_sysfs_dir(void)
-{
-	char *basepath = getenv("LIBNVME_SYSFS_PATH");
-	char *str;
-
-	if (!basepath)
-		return strdup(PATH_SYSFS_SLOTS);
-
-	if (!asprintf(&str, "%s" PATH_SYSFS_SLOTS, basepath))
-		return NULL;
-
-	return str;
-}
-
 static struct nvme_host *default_host;
 
 static void __nvme_free_host(nvme_host_t h);
 static void __nvme_free_ctrl(nvme_ctrl_t c);
 static int nvme_subsystem_scan_namespace(nvme_root_t r,
 		struct nvme_subsystem *s, char *name,
 		nvme_scan_filter_t f, void *f_args);
@@ -668,18 +652,17 @@
 	}
 
 	return 0;
 }
 
 static int nvme_init_subsystem(nvme_subsystem_t s, const char *name)
 {
-	_cleanup_free_ char *subsys_dir = nvme_subsys_sysfs_dir();
 	char *path;
 
-	if (asprintf(&path, "%s/%s", subsys_dir, name) < 0)
+	if (asprintf(&path, "%s/%s", nvme_subsys_sysfs_dir(), name) < 0)
 		return -1;
 
 	s->model = nvme_get_attr(path, "model");
 	if (!s->model)
 		s->model = strdup("undefined");
 	s->serial = nvme_get_attr(path, "serial");
 	s->firmware = nvme_get_attr(path, "firmware_rev");
@@ -712,20 +695,19 @@
 }
 
 static int nvme_scan_subsystem(struct nvme_root *r, const char *name,
 		nvme_scan_filter_t f, void *f_args)
 {
 	struct nvme_subsystem *s = NULL, *_s;
 	_cleanup_free_ char *path = NULL, *subsysnqn = NULL;
-	_cleanup_free_ char *subsys_dir = nvme_subsys_sysfs_dir();
 	nvme_host_t h = NULL;
 	int ret;
 
 	nvme_msg(r, LOG_DEBUG, "scan subsystem %s\n", name);
-	ret = asprintf(&path, "%s/%s", subsys_dir, name);
+	ret = asprintf(&path, "%s/%s", nvme_subsys_sysfs_dir(), name);
 	if (ret < 0)
 		return ret;
 
 	subsysnqn = nvme_get_attr(path, "subsysnqn");
 	if (!subsysnqn) {
 		errno = ENODEV;
 		return -1;
@@ -1022,14 +1004,19 @@
 }
 
 const char *nvme_ctrl_get_dhchap_host_key(nvme_ctrl_t c)
 {
 	return c->dhchap_key;
 }
 
+const char *nvme_ctrl_get_cntlid(nvme_ctrl_t c)
+{
+	return c->cntlid;
+}
+
 void nvme_ctrl_set_dhchap_host_key(nvme_ctrl_t c, const char *key)
 {
 	if (c->dhchap_key) {
 		free(c->dhchap_key);
 		c->dhchap_key = NULL;
 	}
 	if (key)
@@ -1131,14 +1118,15 @@
 	FREE_CTRL_ATTR(c->serial);
 	FREE_CTRL_ATTR(c->sqsize);
 	FREE_CTRL_ATTR(c->dhchap_key);
 	FREE_CTRL_ATTR(c->dhchap_ctrl_key);
 	FREE_CTRL_ATTR(c->address);
 	FREE_CTRL_ATTR(c->dctype);
 	FREE_CTRL_ATTR(c->cntrltype);
+	FREE_CTRL_ATTR(c->cntlid);
 	FREE_CTRL_ATTR(c->phy_slot);
 }
 
 int nvme_disconnect_ctrl(nvme_ctrl_t c)
 {
 	nvme_root_t r = c->s && c->s->h ? c->s->h->r : NULL;
 	int ret;
@@ -1699,15 +1687,15 @@
 
 	return 0;
 }
 
 static char *nvme_ctrl_lookup_subsystem_name(nvme_root_t r,
 					     const char *ctrl_name)
 {
-	_cleanup_free_ char *subsys_dir = nvme_subsys_sysfs_dir();
+	const char *subsys_dir = nvme_subsys_sysfs_dir();
 	_cleanup_dirents_ struct dirents subsys = {};
 	int i;
 
 	subsys.num = nvme_scan_subsystems(&subsys.ents);
 	if (subsys.num < 0)
 		return NULL;
 	for (i = 0; i < subsys.num; i++) {
@@ -1726,15 +1714,15 @@
 		return strdup(subsys.ents[i]->d_name);
 	}
 	return NULL;
 }
 
 static char *nvme_ctrl_lookup_phy_slot(nvme_root_t r, const char *address)
 {
-	_cleanup_free_ char *slots_sysfs_dir = nvme_slots_sysfs_dir();
+	const char *slots_sysfs_dir = nvme_slots_sysfs_dir();
 	_cleanup_free_ char *target_addr = NULL;
 	_cleanup_dir_ DIR *slots_dir = NULL;
 	int ret;
 	struct dirent *entry;
 
 	if (!address)
 		return NULL;
@@ -1743,15 +1731,15 @@
 	if (!slots_dir) {
 		nvme_msg(r, LOG_WARNING, "failed to open slots dir %s\n",
 		slots_sysfs_dir);
 		return NULL;
 	}
 
 	target_addr = strndup(address, 10);
-	while (!(entry = readdir(slots_dir))) {
+	while ((entry = readdir(slots_dir))) {
 		if (entry->d_type == DT_DIR &&
 		    strncmp(entry->d_name, ".", 1) != 0 &&
 		    strncmp(entry->d_name, "..", 2) != 0) {
 			_cleanup_free_ char *path = NULL;
 			_cleanup_free_ char *addr = NULL;
 
 			ret = asprintf(&path, "%s/%s",
@@ -1768,15 +1756,15 @@
 	return NULL;
 }
 
 static int nvme_configure_ctrl(nvme_root_t r, nvme_ctrl_t c, const char *path,
 			       const char *name)
 {
 	DIR *d;
-	char *host_key;
+	char *host_key, *tls_psk;
 
 	d = opendir(path);
 	if (!d) {
 		nvme_msg(r, LOG_ERR, "Failed to open ctrl dir %s, error %d\n",
 			 path, errno);
 		errno = ENODEV;
 		return -1;
@@ -1803,37 +1791,47 @@
 	if (host_key)
 		c->dhchap_key = host_key;
 	c->dhchap_ctrl_key = nvme_get_ctrl_attr(c, "dhchap_ctrl_secret");
 	if (c->dhchap_ctrl_key && !strcmp(c->dhchap_ctrl_key, "none")) {
 		free(c->dhchap_ctrl_key);
 		c->dhchap_ctrl_key = NULL;
 	}
+	tls_psk = nvme_get_ctrl_attr(c, "tls_key");
+	if (tls_psk) {
+		char *endptr;
+		long key_id = strtol(tls_psk, &endptr, 16);
+
+		if (endptr != tls_psk) {
+			c->cfg.tls_key = key_id;
+			c->cfg.tls = true;
+		}
+	}
 	c->cntrltype = nvme_get_ctrl_attr(c, "cntrltype");
+	c->cntlid = nvme_get_ctrl_attr(c, "cntlid");
 	c->dctype = nvme_get_ctrl_attr(c, "dctype");
 	c->phy_slot = nvme_ctrl_lookup_phy_slot(r, c->address);
 
 	errno = 0; /* cleanup after nvme_get_ctrl_attr() */
 	return 0;
 }
 
 int nvme_init_ctrl(nvme_host_t h, nvme_ctrl_t c, int instance)
 {
-	_cleanup_free_ char *ctrl_dir = nvme_ctrl_sysfs_dir();
 	_cleanup_free_ char *subsys_name = NULL;
 	_cleanup_free_ char *name = NULL;
 	nvme_subsystem_t s;
 	char *path;
 	int ret;
 
 	ret = asprintf(&name, "nvme%d", instance);
 	if (ret < 0) {
 		errno = ENOMEM;
 		return -1;
 	}
-	ret = asprintf(&path, "%s/nvme%d", ctrl_dir, instance);
+	ret = asprintf(&path, "%s/%s", nvme_ctrl_sysfs_dir(), name);
 	if (ret < 0) {
 		errno = ENOMEM;
 		return ret;
 	}
 
 	ret = nvme_configure_ctrl(h->r, c, path, name);
 	if (ret < 0) {
@@ -1868,15 +1866,15 @@
 }
 
 static nvme_ctrl_t nvme_ctrl_alloc(nvme_root_t r, nvme_subsystem_t s,
 				   const char *path, const char *name)
 {
 	nvme_ctrl_t c, p;
 	_cleanup_free_ char *addr = NULL, *address = NULL;
-	char *a, *e;
+	char *a = NULL, *e = NULL;
 	_cleanup_free_ char *transport = NULL;
 	char *traddr = NULL, *trsvcid = NULL;
 	char *host_traddr = NULL, *host_iface = NULL;
 	int ret;
 
 	transport = nvme_get_attr(path, "transport");
 	if (!transport) {
@@ -1969,19 +1967,18 @@
 {
 	nvme_host_t h;
 	nvme_subsystem_t s;
 	nvme_ctrl_t c;
 	_cleanup_free_ char *path = NULL;
 	_cleanup_free_ char *hostnqn = NULL, *hostid = NULL;
 	_cleanup_free_ char *subsysnqn = NULL, *subsysname = NULL;
-	_cleanup_free_ char *ctrl_dir = nvme_ctrl_sysfs_dir();
 	int ret;
 
 	nvme_msg(r, LOG_DEBUG, "scan controller %s\n", name);
-	ret = asprintf(&path, "%s/%s", ctrl_dir, name);
+	ret = asprintf(&path, "%s/%s", nvme_ctrl_sysfs_dir(), name);
 	if (ret < 0) {
 		errno = ENOMEM;
 		return NULL;
 	}
 
 	hostnqn = nvme_get_attr(path, "hostnqn");
 	hostid = nvme_get_attr(path, "hostid");
@@ -2448,30 +2445,36 @@
 	return 0;
 }
 
 static int nvme_ns_init(const char *path, struct nvme_ns *ns)
 {
 	_cleanup_free_ char *attr = NULL;
 	struct stat sb;
+	uint64_t size;
 	int ret;
 
 	struct sysfs_attr_table base[] = {
 		{ &ns->nsid,      nvme_strtou32,  true, "nsid" },
-		{ &ns->lba_count, nvme_strtou64,  true, "size" },
-		{ &ns->lba_size,  nvme_strtou64,  true, "queue/logical_block_size" },
+		{ &size,          nvme_strtou64,  true, "size" },
+		{ &ns->lba_size,  nvme_strtou32,  true, "queue/logical_block_size" },
 		{ ns->eui64,      nvme_strtoeuid, false, "eui" },
 		{ ns->nguid,      nvme_strtouuid, false, "nguid" },
 		{ ns->uuid,       nvme_strtouuid, false, "uuid" }
 	};
 
 	ret = parse_attrs(path, base, ARRAY_SIZE(base));
 	if (ret)
 		return ret;
 
 	ns->lba_shift = GETSHIFT(ns->lba_size);
+	/*
+	 * size is in 512 bytes units and lba_count is in lba_size which are not
+	 * necessarily the same.
+	 */
+	ns->lba_count = size >> (ns->lba_shift -  SECTOR_SHIFT);
 
 	if (asprintf(&attr, "%s/csi", path) < 0)
 		return -errno;
 	ret = stat(attr, &sb);
 	if (ret == 0) {
 		/* only available on kernels >= 6.8 */
 		struct sysfs_attr_table ext[] = {
@@ -2481,15 +2484,15 @@
 
 		};
 
 		ret = parse_attrs(path, ext, ARRAY_SIZE(ext));
 		if (ret)
 			return ret;
 	} else {
-		struct nvme_id_ns *id;
+		_cleanup_free_ struct nvme_id_ns *id = NULL;
 		uint8_t flbas;
 
 		id = __nvme_alloc(sizeof(*ns));
 		if (!id)
 			return -ENOMEM;
 
 		ret = nvme_ns_identify(ns, id);
@@ -2601,17 +2604,15 @@
 	path = NULL;
 
 	return n;
 }
 
 nvme_ns_t nvme_scan_namespace(const char *name)
 {
-	_cleanup_free_ char *ns_dir = nvme_ns_sysfs_dir();
-
-	return __nvme_scan_namespace(ns_dir, name);
+	return __nvme_scan_namespace(nvme_ns_sysfs_dir(), name);
 }
 
 static int nvme_ctrl_scan_namespace(nvme_root_t r, struct nvme_ctrl *c,
 				    char *name)
 {
 	struct nvme_ns *n, *_n, *__n;
```

### Comparing `libnvme-1.8/src/nvme/tree.h` & `libnvme-1.9/src/nvme/tree.h`

 * *Files 1% similar despite different names*

```diff
@@ -1022,14 +1022,22 @@
  * @c:	Controller to be checked
  *
  * Return: DH-HMAC-CHAP host key or NULL if not set
  */
 const char *nvme_ctrl_get_dhchap_host_key(nvme_ctrl_t c);
 
 /**
+ *  nvme_ctrl_get_cntlid() - Controller id
+ *  @c:	Controller to be checked
+ *
+ *  Return : Controller id of @c
+ */
+const char *nvme_ctrl_get_cntlid(nvme_ctrl_t c);
+
+/**
  * nvme_ctrl_set_dhchap_host_key() - Set host key
  * @c:		Host for which the key should be set
  * @key:	DH-HMAC-CHAP Key to set or NULL to clear existing key
  */
 void nvme_ctrl_set_dhchap_host_key(nvme_ctrl_t c, const char *key);
 
 /**
```

### Comparing `libnvme-1.8/src/nvme/types.h` & `libnvme-1.9/src/nvme/types.h`

 * *Files 4% similar despite different names*

```diff
@@ -226,64 +226,127 @@
 	case NVME_REG_CMBMSC:
 		return true;
 	default:
 		return false;
 	}
 }
 
+/**
+ * enum nvme_cap - This field indicates the controller capabilities register
+ * @NVME_CAP_MQES_SHIFT:	Shift amount to get the maximum queue entries supported
+ * @NVME_CAP_CQR_SHIFT:		Shift amount to get the contiguous queues required
+ * @NVME_CAP_AMS_SHIFT:		Shift amount to get the arbitration mechanism supported
+ * @NVME_CAP_TO_SHIFT:		Shift amount to get the timeout
+ * @NVME_CAP_DSTRD_SHIFT:	Shift amount to get the doorbell stride
+ * @NVME_CAP_NSSRC_SHIFT:	Shift amount to get the NVM subsystem reset supported
+ * @NVME_CAP_CSS_SHIFT:		Shift amount to get the command sets supported
+ * @NVME_CAP_BPS_SHIFT:		Shift amount to get the boot partition support
+ * @NVME_CAP_CPS_SHIFT:		Shift amount to get the controller power scope
+ * @NVME_CAP_MPSMIN_SHIFT:	Shift amount to get the memory page size minimum
+ * @NVME_CAP_MPSMAX_SHIFT:	Shift amount to get the memory page size maximum
+ * @NVME_CAP_PMRS_SHIFT:	Shift amount to get the persistent memory region supported
+ * @NVME_CAP_CMBS_SHIFT:	Shift amount to get the controller memory buffer supported
+ * @NVME_CAP_NSSS_SHIFT:	Shift amount to get the NVM subsystem shutdown supported
+ * @NVME_CAP_CRMS_SHIFT:	Shift amount to get the controller ready modes supported
+ * @NVME_CAP_MQES_MASK:		Mask to get the maximum queue entries supported
+ * @NVME_CAP_CQR_MASK:		Mask to get the contiguous queues required
+ * @NVME_CAP_AMS_MASK:		Mask to get the arbitration mechanism supported
+ * @NVME_CAP_TO_MASK:		Mask to get the timeout
+ * @NVME_CAP_DSTRD_MASK:	Mask to get the doorbell stride
+ * @NVME_CAP_NSSRC_MASK:	Mask to get the NVM subsystem reset supported
+ * @NVME_CAP_CSS_MASK:		Mask to get the command sets supported
+ * @NVME_CAP_BPS_MASK:		Mask to get the boot partition support
+ * @NVME_CAP_CPS_MASK:		Mask to get the controller power scope
+ * @NVME_CAP_MPSMIN_MASK:	Mask to get the memory page size minimum
+ * @NVME_CAP_MPSMAX_MASK:	Mask to get the memory page size maximum
+ * @NVME_CAP_PMRS_MASK:		Mask to get the persistent memory region supported
+ * @NVME_CAP_CMBS_MASK:		Mask to get the controller memory buffer supported
+ * @NVME_CAP_NSSS_MASK:		Mask to get the NVM subsystem shutdown supported
+ * @NVME_CAP_CRMS_MASK:		Mask to get the controller ready modes supported
+ * @NVME_CAP_AMS_WRR:		Weighted round robin with urgent priority class
+ * @NVME_CAP_AMS_VS:		Vendor specific
+ * @NVME_CAP_CSS_NVM:		NVM command set or a discovery controller
+ * @NVME_CAP_CSS_CSI:		Controller supports one or more I/O command sets
+ * @NVME_CAP_CSS_ADMIN:		No I/O command set is supported
+ * @NVME_CAP_CPS_NONE:		Not reported
+ * @NVME_CAP_CPS_CTRL:		Controller scope
+ * @NVME_CAP_CPS_DOMAIN:	Domain scope
+ * @NVME_CAP_CPS_NVMS:		NVM subsystem scope
+ * @NVME_CAP_CRWMS:		Controller ready with media support
+ * @NVME_CAP_CRIMS:		Controller ready independent of media support
+ */
 enum nvme_cap {
 	NVME_CAP_MQES_SHIFT		= 0,
 	NVME_CAP_CQR_SHIFT		= 16,
 	NVME_CAP_AMS_SHIFT		= 17,
 	NVME_CAP_TO_SHIFT		= 24,
 	NVME_CAP_DSTRD_SHIFT		= 32,
 	NVME_CAP_NSSRC_SHIFT		= 36,
 	NVME_CAP_CSS_SHIFT		= 37,
 	NVME_CAP_BPS_SHIFT		= 45,
+	NVME_CAP_CPS_SHIFT		= 46,
 	NVME_CAP_MPSMIN_SHIFT		= 48,
 	NVME_CAP_MPSMAX_SHIFT		= 52,
 	NVME_CAP_PMRS_SHIFT		= 56,
 	NVME_CAP_CMBS_SHIFT		= 57,
+	NVME_CAP_NSSS_SHIFT		= 58,
 	NVME_CAP_CRMS_SHIFT		= 59,
 	NVME_CAP_MQES_MASK		= 0xffff,
 	NVME_CAP_CQR_MASK		= 0x1,
 	NVME_CAP_AMS_MASK		= 0x3,
 	NVME_CAP_TO_MASK		= 0xff,
 	NVME_CAP_DSTRD_MASK		= 0xf,
 	NVME_CAP_NSSRC_MASK		= 0x1,
 	NVME_CAP_CSS_MASK		= 0xff,
 	NVME_CAP_BPS_MASK		= 0x1,
+	NVME_CAP_CPS_MASK		= 0x3,
 	NVME_CAP_MPSMIN_MASK		= 0xf,
 	NVME_CAP_MPSMAX_MASK		= 0xf,
 	NVME_CAP_PMRS_MASK		= 0x1,
 	NVME_CAP_CMBS_MASK		= 0x1,
+	NVME_CAP_NSSS_MASK		= 0x1,
 	NVME_CAP_CRMS_MASK		= 0x3,
 	NVME_CAP_AMS_WRR		= 1 << 0,
 	NVME_CAP_AMS_VS			= 1 << 1,
 	NVME_CAP_CSS_NVM		= 1 << 0,
 	NVME_CAP_CSS_CSI		= 1 << 6,
 	NVME_CAP_CSS_ADMIN		= 1 << 7,
+	NVME_CAP_CPS_NONE		= 0,
+	NVME_CAP_CPS_CTRL		= 1,
+	NVME_CAP_CPS_DOMAIN		= 2,
+	NVME_CAP_CPS_NVMS		= 3,
 	NVME_CAP_CRWMS			= 1 << 0,
 	NVME_CAP_CRIMS			= 1 << 1,
 };
 
 #define NVME_CAP_MQES(cap)	NVME_GET(cap, CAP_MQES)
 #define NVME_CAP_CQR(cap)	NVME_GET(cap, CAP_CQR)
 #define NVME_CAP_AMS(cap)	NVME_GET(cap, CAP_AMS)
 #define NVME_CAP_TO(cap)	NVME_GET(cap, CAP_TO)
 #define NVME_CAP_DSTRD(cap)	NVME_GET(cap, CAP_DSTRD)
 #define NVME_CAP_NSSRC(cap)	NVME_GET(cap, CAP_NSSRC)
 #define NVME_CAP_CSS(cap)	NVME_GET(cap, CAP_CSS)
 #define NVME_CAP_BPS(cap)	NVME_GET(cap, CAP_BPS)
+#define NVME_CAP_CPS(cap)	NVME_GET(cap, CAP_CPS)
 #define NVME_CAP_MPSMIN(cap)	NVME_GET(cap, CAP_MPSMIN)
 #define NVME_CAP_MPSMAX(cap)	NVME_GET(cap, CAP_MPSMAX)
 #define NVME_CAP_PMRS(cap)	NVME_GET(cap, CAP_PMRS)
 #define NVME_CAP_CMBS(cap)	NVME_GET(cap, CAP_CMBS)
+#define NVME_CAP_NSSS(cap)	NVME_GET(cap, CAP_NSSS)
 #define NVME_CAP_CRMS(cap)	NVME_GET(cap, CAP_CRMS)
 
+/**
+ * enum nvme_vs - This field indicates the version
+ * @NVME_VS_TER_SHIFT:	Shift amount to get the tertiary version
+ * @NVME_VS_MNR_SHIFT:	Shift amount to get the minor version
+ * @NVME_VS_MJR_SHIFT:	Shift amount to get the major version
+ * @NVME_VS_TER_MASK:	Mask to get the tertiary version
+ * @NVME_VS_MNR_MASK:	Mask to get the minor version
+ * @NVME_VS_MJR_MASK:	Mask to get the major version
+ */
 enum nvme_vs {
 	NVME_VS_TER_SHIFT		= 0,
 	NVME_VS_MNR_SHIFT		= 8,
 	NVME_VS_MJR_SHIFT		= 16,
 	NVME_VS_TER_MASK		= 0xff,
 	NVME_VS_MNR_MASK		= 0xff,
 	NVME_VS_MJR_MASK		= 0xffff,
@@ -293,14 +356,44 @@
 #define NVME_VS_MNR(vs)		NVME_GET(vs, VS_MNR)
 #define NVME_VS_MJR(vs)		NVME_GET(vs, VS_MJR)
 
 #define NVME_MAJOR(ver)		NVME_VS_MJR(ver)
 #define NVME_MINOR(ver)		NVME_VS_MNR(ver)
 #define NVME_TERTIARY(ver)	NVME_VS_TER(ver)
 
+/**
+ * enum nvme_cc - This field indicates the controller configuration
+ * @NVME_CC_EN_SHIFT:		Shift amount to get the enable
+ * @NVME_CC_CSS_SHIFT:		Shift amount to get the I/O command set selected
+ * @NVME_CC_MPS_SHIFT:		Shift amount to get the memory page size
+ * @NVME_CC_AMS_SHIFT:		Shift amount to get the arbitration mechanism selected
+ * @NVME_CC_SHN_SHIFT:		Shift amount to get the shutdown notification
+ * @NVME_CC_IOSQES_SHIFT:	Shift amount to get the I/O submission queue entry size
+ * @NVME_CC_IOCQES_SHIFT:	Shift amount to get the I/O completion queue entry size
+ * @NVME_CC_CRIME_SHIFT:	Shift amount to get the controller ready independent of media enable
+ * @NVME_CC_EN_MASK:		Mask to get the enable
+ * @NVME_CC_CSS_MASK:		Mask to get the I/O command set selected
+ * @NVME_CC_MPS_MASK:		Mask to get the memory page size
+ * @NVME_CC_AMS_MASK:		Mask to get the arbitration mechanism selected
+ * @NVME_CC_SHN_MASK:		Mask to get the shutdown notification
+ * @NVME_CC_CRIME_MASK:		Mask to get the I/O submission queue entry size
+ * @NVME_CC_IOSQES_MASK:	Mask to get the I/O completion queue entry size
+ * @NVME_CC_IOCQES_MASK:	Mask to get the controller ready independent of media enable
+ * @NVME_CC_CSS_NVM:		NVM command set
+ * @NVME_CC_CSS_CSI:		All supported I/O command sets
+ * @NVME_CC_CSS_ADMIN:		Admin command set only
+ * @NVME_CC_AMS_RR:		Round robin
+ * @NVME_CC_AMS_WRRU:		Weighted round robin with urgent priority class
+ * @NVME_CC_AMS_VS:		Vendor specific
+ * @NVME_CC_SHN_NONE:		No notification; no effect
+ * @NVME_CC_SHN_NORMAL:		Normal shutdown notification
+ * @NVME_CC_SHN_ABRUPT:		Abrupt shutdown notification
+ * @NVME_CC_CRWME:		Controller ready with media enable
+ * @NVME_CC_CRIME:		Controller ready independent of media enable
+ */
 enum nvme_cc {
 	NVME_CC_EN_SHIFT	= 0,
 	NVME_CC_CSS_SHIFT	= 4,
 	NVME_CC_MPS_SHIFT	= 7,
 	NVME_CC_AMS_SHIFT	= 11,
 	NVME_CC_SHN_SHIFT	= 14,
 	NVME_CC_IOSQES_SHIFT	= 16,
@@ -332,47 +425,117 @@
 #define NVME_CC_MPS(cc)		NVME_GET(cc, CC_MPS)
 #define NVME_CC_AMS(cc)		NVME_GET(cc, CC_AMS)
 #define NVME_CC_SHN(cc)		NVME_GET(cc, CC_SHN)
 #define NVME_CC_IOSQES(cc)	NVME_GET(cc, CC_IOSQES)
 #define NVME_CC_IOCQES(cc)	NVME_GET(cc, CC_IOCQES)
 #define NVME_CC_CRIME(cc)	NVME_GET(cc, CC_CRIME)
 
+/**
+ * enum nvme_csts - This field indicates the controller status register
+ * @NVME_CSTS_RDY_SHIFT:	Shift amount to get the ready
+ * @NVME_CSTS_CFS_SHIFT:	Shift amount to get the controller fatal status
+ * @NVME_CSTS_SHST_SHIFT:	Shift amount to get the shutdown status
+ * @NVME_CSTS_NSSRO_SHIFT:	Shift amount to get the NVM subsystem reset occurred
+ * @NVME_CSTS_PP_SHIFT:		Shift amount to get the processing paused
+ * @NVME_CSTS_ST_SHIFT:		Shift amount to get the shutdown type
+ * @NVME_CSTS_RDY_MASK:		Mask to get the ready
+ * @NVME_CSTS_CFS_MASK:		Mask to get the controller fatal status
+ * @NVME_CSTS_SHST_MASK:	Mask to get the shutdown status
+ * @NVME_CSTS_NSSRO_MASK:	Mask to get the NVM subsystem reset occurred
+ * @NVME_CSTS_PP_MASK:		Mask to get the processing paused
+ * @NVME_CSTS_ST_MASK:		Mask to get the shutdown type
+ * @NVME_CSTS_SHST_NORMAL:	Normal operation
+ * @NVME_CSTS_SHST_OCCUR:	Shutdown processing occurring
+ * @NVME_CSTS_SHST_CMPLT:	Shutdown processing complete
+ * @NVME_CSTS_SHN_MASK:		Deprecated mask to get the shutdown status
+ */
 enum nvme_csts {
 	NVME_CSTS_RDY_SHIFT	= 0,
 	NVME_CSTS_CFS_SHIFT	= 1,
 	NVME_CSTS_SHST_SHIFT	= 2,
 	NVME_CSTS_NSSRO_SHIFT	= 4,
 	NVME_CSTS_PP_SHIFT	= 5,
+	NVME_CSTS_ST_SHIFT	= 6,
 	NVME_CSTS_RDY_MASK	= 0x1,
 	NVME_CSTS_CFS_MASK	= 0x1,
-	NVME_CSTS_SHN_MASK	= 0x3,
+	NVME_CSTS_SHST_MASK	= 0x3,
 	NVME_CSTS_NSSRO_MASK	= 0x1,
 	NVME_CSTS_PP_MASK	= 0x1,
+	NVME_CSTS_ST_MASK	= 0x1,
 	NVME_CSTS_SHST_NORMAL	= 0,
 	NVME_CSTS_SHST_OCCUR	= 1,
 	NVME_CSTS_SHST_CMPLT	= 2,
-	NVME_CSTS_SHST_MASK	= 3,
+	NVME_CSTS_SHN_MASK	= NVME_CSTS_SHST_MASK, /* Deprecated */
 };
 
 #define NVME_CSTS_RDY(csts)	NVME_GET(csts, CSTS_RDY)
 #define NVME_CSTS_CFS(csts)	NVME_GET(csts, CSTS_CFS)
 #define NVME_CSTS_SHST(csts)	NVME_GET(csts, CSTS_SHST)
 #define NVME_CSTS_NSSRO(csts)	NVME_GET(csts, CSTS_NSSRO)
 #define NVME_CSTS_PP(csts)	NVME_GET(csts, CSTS_PP)
+#define NVME_CSTS_ST(csts)	NVME_GET(csts, CSTS_ST)
 
+/**
+ * enum nvme_aqa - This field indicates the admin queue attributes
+ * @NVME_AQA_ASQS_SHIFT:	Shift amount to get the admin submission queue size
+ * @NVME_AQA_ACQS_SHIFT:	Shift amount to get the admin completion queue size
+ * @NVME_AQA_ASQS_MASK:		Mask to get the admin submission queue size
+ * @NVME_AQA_ACQS_MASK:		Mask to get the admin completion queue size
+ */
 enum nvme_aqa {
 	NVME_AQA_ASQS_SHIFT	= 0,
 	NVME_AQA_ACQS_SHIFT	= 16,
 	NVME_AQA_ASQS_MASK	= 0xfff,
 	NVME_AQA_ACQS_MASK	= 0xfff,
 };
 
 #define NVME_AQA_ASQS(aqa)	NVME_GET(aqa, AQA_ASQS)
 #define NVME_AQA_ACQS(aqa)	NVME_GET(aqa, AQA_ACQS)
 
+/**
+ * enum nvme_asq - This field indicates the admin submission queue base address
+ * @NVME_ASQ_ASQB_SHIFT:	Shift amount to get the admin submission queue base
+ */
+enum nvme_asq {
+	NVME_ASQ_ASQB_SHIFT		= 12,
+};
+static const __u64 NVME_ASQ_ASQB_MASK = 0xfffffffffffffull;
+
+#define NVME_ASQ_ASQB(asq)		NVME_GET(asq, ASQ_ASQB)
+
+/**
+ * enum nvme_acq - This field indicates the admin completion queue base address
+ * @NVME_ACQ_ACQB_SHIFT:	Shift amount to get the admin completion queue base
+ */
+enum nvme_acq {
+	NVME_ACQ_ACQB_SHIFT		= 12,
+};
+static const __u64 NVME_ACQ_ACQB_MASK = 0xfffffffffffffull;
+
+#define NVME_ACQ_ACQB(acq)		NVME_GET(acq, ACQ_ACQB)
+
+/**
+ * enum nvme_cmbloc - This field indicates the controller memory buffer location
+ * @NVME_CMBLOC_BIR_SHIFT:	Shift amount to get the base indicator register
+ * @NVME_CMBLOC_CQMMS_SHIFT:	Shift amount to get the CMB queue mixed memory support
+ * @NVME_CMBLOC_CQPDS_SHIFT:	Shift amount to get the CMB queue physically discontiguous support
+ * @NVME_CMBLOC_CDPLMS_SHIFT:	Shift amount to get the CMB data pointer mixed locations support
+ * @NVME_CMBLOC_CDPCILS_SHIFT:	Shift amount to get the CMB data pointer and command independent locations support
+ * @NVME_CMBLOC_CDMMMS_SHIFT:	Shift amount to get the CMB data metadata mixed memory support
+ * @NVME_CMBLOC_CQDA_SHIFT:	Shift amount to get the CMB queue dword alignment
+ * @NVME_CMBLOC_OFST_SHIFT:	Shift amount to get the offset
+ * @NVME_CMBLOC_BIR_MASK:	Mask to get the base indicator register
+ * @NVME_CMBLOC_CQMMS_MASK:	Mask to get the CMB queue mixed memory support
+ * @NVME_CMBLOC_CQPDS_MASK:	Mask to get the CMB queue physically discontiguous support
+ * @NVME_CMBLOC_CDPLMS_MASK:	Mask to get the CMB data pointer mixed locations support
+ * @NVME_CMBLOC_CDPCILS_MASK:	Mask to get the CMB data pointer and command independent locations support
+ * @NVME_CMBLOC_CDMMMS_MASK:	Mask to get the CMB data metadata mixed memory support
+ * @NVME_CMBLOC_CQDA_MASK:	Mask to get the CMB queue dword alignment
+ * @NVME_CMBLOC_OFST_MASK:	Mask to get the offset
+ */
 enum nvme_cmbloc {
 	NVME_CMBLOC_BIR_SHIFT		= 0,
 	NVME_CMBLOC_CQMMS_SHIFT		= 3,
 	NVME_CMBLOC_CQPDS_SHIFT		= 4,
 	NVME_CMBLOC_CDPLMS_SHIFT	= 5,
 	NVME_CMBLOC_CDPCILS_SHIFT	= 6,
 	NVME_CMBLOC_CDMMMS_SHIFT	= 7,
@@ -393,14 +556,38 @@
 #define NVME_CMBLOC_CQPDS(cmbloc)	NVME_GET(cmbloc, CMBLOC_CQPDS)
 #define NVME_CMBLOC_CDPLMS(cmbloc)	NVME_GET(cmbloc, CMBLOC_CDPLMS)
 #define NVME_CMBLOC_CDPCILS(cmbloc)	NVME_GET(cmbloc, CMBLOC_CDPCILS)
 #define NVME_CMBLOC_CDMMMS(cmbloc)	NVME_GET(cmbloc, CMBLOC_CDMMMS)
 #define NVME_CMBLOC_CQDA(cmbloc)	NVME_GET(cmbloc, CMBLOC_CQDA)
 #define NVME_CMBLOC_OFST(cmbloc)	NVME_GET(cmbloc, CMBLOC_OFST)
 
+/**
+ * enum nvme_cmbsz - This field indicates the controller memory buffer size
+ * @NVME_CMBSZ_SQS_SHIFT:	Shift amount to get the submission queue support
+ * @NVME_CMBSZ_CQS_SHIFT:	Shift amount to get the completion queue support
+ * @NVME_CMBSZ_LISTS_SHIFT:	Shift amount to get the PLP SGL list support
+ * @NVME_CMBSZ_RDS_SHIFT:	Shift amount to get the read data support
+ * @NVME_CMBSZ_WDS_SHIFT:	Shift amount to get the write data support
+ * @NVME_CMBSZ_SZU_SHIFT:	Shift amount to get the size units
+ * @NVME_CMBSZ_SZ_SHIFT:	Shift amount to get the size
+ * @NVME_CMBSZ_SQS_MASK:	Mask to get the submission queue support
+ * @NVME_CMBSZ_CQS_MASK:	Mask to get the completion queue support
+ * @NVME_CMBSZ_LISTS_MASK:	Mask to get the PLP SGL list support
+ * @NVME_CMBSZ_RDS_MASK:	Mask to get the read data support
+ * @NVME_CMBSZ_WDS_MASK:	Mask to get the write data support
+ * @NVME_CMBSZ_SZU_MASK:	Mask to get the size units
+ * @NVME_CMBSZ_SZ_MASK:		Mask to get the size
+ * @NVME_CMBSZ_SZU_4K:		4 KiB
+ * @NVME_CMBSZ_SZU_64K:		64 KiB
+ * @NVME_CMBSZ_SZU_1M:		1 MiB
+ * @NVME_CMBSZ_SZU_16M:		16 MiB
+ * @NVME_CMBSZ_SZU_256M:	256 MiB
+ * @NVME_CMBSZ_SZU_4G:		4 GiB
+ * @NVME_CMBSZ_SZU_64G:		64 GiB
+ */
 enum nvme_cmbsz {
 	NVME_CMBSZ_SQS_SHIFT	= 0,
 	NVME_CMBSZ_CQS_SHIFT	= 1,
 	NVME_CMBSZ_LISTS_SHIFT	= 2,
 	NVME_CMBSZ_RDS_SHIFT	= 3,
 	NVME_CMBSZ_WDS_SHIFT	= 4,
 	NVME_CMBSZ_SZU_SHIFT	= 8,
@@ -437,14 +624,27 @@
  */
 static inline __u64 nvme_cmb_size(__u32 cmbsz)
 {
 	return ((__u64)NVME_CMBSZ_SZ(cmbsz)) *
 		(1ULL << (12 + 4 * NVME_CMBSZ_SZU(cmbsz)));
 }
 
+/**
+ * enum nvme_bpinfo - This field indicates the boot partition information
+ * @NVME_BPINFO_BPSZ_SHIFT:		Shift amount to get the boot partition size
+ * @NVME_BPINFO_BRS_SHIFT:		Shift amount to get the boot read status
+ * @NVME_BPINFO_ABPID_SHIFT:		Shift amount to get the active boot partition ID
+ * @NVME_BPINFO_BPSZ_MASK:		Mask to get the boot partition size
+ * @NVME_BPINFO_BRS_MASK:		Mask to get the boot read status
+ * @NVME_BPINFO_ABPID_MASK:		Mask to get the active boot partition ID
+ * @NVME_BPINFO_BRS_NONE:		No boot partition read operation requested
+ * @NVME_BPINFO_BRS_READ_IN_PROGRESS:	Boot partition read in progress
+ * @NVME_BPINFO_BRS_READ_SUCCESS:	Boot partition read completed successfully
+ * @NVME_BPINFO_BRS_READ_ERROR:		Error completing boot partition read
+ */
 enum nvme_bpinfo {
 	NVME_BPINFO_BPSZ_SHIFT			= 0,
 	NVME_BPINFO_BRS_SHIFT			= 24,
 	NVME_BPINFO_ABPID_SHIFT			= 31,
 	NVME_BPINFO_BPSZ_MASK			= 0x7fff,
 	NVME_BPINFO_BRS_MASK			= 0x3,
 	NVME_BPINFO_ABPID_MASK			= 0x1,
@@ -454,91 +654,240 @@
 	NVME_BPINFO_BRS_READ_ERROR		= 3,
 };
 
 #define NVME_BPINFO_BPSZ(bpinfo)	NVME_GET(bpinfo, BPINFO_BPSZ)
 #define NVME_BPINFO_BRS(bpinfo)		NVME_GET(bpinfo, BPINFO_BRS)
 #define NVME_BPINFO_ABPID(bpinfo)	NVME_GET(bpinfo, BPINFO_ABPID)
 
+/**
+ * enum nvme_bprsel - This field indicates the boot partition read select
+ * @NVME_BPRSEL_BPRSZ_SHIFT:	Shift amount to get the boot partition read size
+ * @NVME_BPRSEL_BPROF_SHIFT:	Shift amount to get the boot partition read offset
+ * @NVME_BPRSEL_BPID_SHIFT:	Shift amount to get the boot partition identifier
+ * @NVME_BPRSEL_BPRSZ_MASK:	Mask to get the boot partition read size
+ * @NVME_BPRSEL_BPROF_MASK:	Mask to get the boot partition read offset
+ * @NVME_BPRSEL_BPID_MASK:	Mask to get the boot partition identifier
+ */
 enum nvme_bprsel {
 	NVME_BPRSEL_BPRSZ_SHIFT		= 0,
 	NVME_BPRSEL_BPROF_SHIFT		= 10,
 	NVME_BPRSEL_BPID_SHIFT		= 31,
 	NVME_BPRSEL_BPRSZ_MASK		= 0x3ff,
-	NVME_BPRSEL_BPROF_MASK		= 0xfff,
+	NVME_BPRSEL_BPROF_MASK		= 0xfffff,
 	NVME_BPRSEL_BPID_MASK		= 0x1,
 };
 
 #define NVME_BPRSEL_BPRSZ(bprsel)	NVME_GET(bprsel, BPRSEL_BPRSZ)
 #define NVME_BPRSEL_BPROF(bprsel)	NVME_GET(bprsel, BPRSEL_BPROF)
 #define NVME_BPRSEL_BPID(bprsel)	NVME_GET(bprsel, BPRSEL_BPID)
 
+/**
+ * enum nvme_bpmbl - This field indicates the boot partition memory buffer location
+ * @NVME_BPMBL_BMBBA_SHIFT:	Shift amount to get the boot partition memory buffer base address
+ */
+enum nvme_bpmbl {
+	NVME_BPMBL_BMBBA_SHIFT		= 12,
+};
+static const __u64 NVME_BPMBL_BMBBA_MASK = 0xfffffffffffffull;
+
+#define NVME_BPMBL_BMBBA(bpmbl)		NVME_GET(bpmbl, BPMBL_BMBBA)
+
+/**
+ * enum nvme_cmbmsc - This field indicates the controller memory buffer memory space control
+ * @NVME_CMBMSC_CRE_SHIFT:	Shift amount to get the capabilities registers enabled
+ * @NVME_CMBMSC_CMSE_SHIFT:	Shift amount to get the controller memory space enable
+ * @NVME_CMBMSC_CBA_SHIFT:	Shift amount to get the controller base address
+ * @NVME_CMBMSC_CRE_MASK:	Mask to get the capabilities registers enabled
+ * @NVME_CMBMSC_CMSE_MASK:	Mask to get the controller memory space enable
+ */
 enum nvme_cmbmsc {
 	NVME_CMBMSC_CRE_SHIFT		= 0,
 	NVME_CMBMSC_CMSE_SHIFT		= 1,
 	NVME_CMBMSC_CBA_SHIFT		= 12,
 	NVME_CMBMSC_CRE_MASK		= 0x1,
 	NVME_CMBMSC_CMSE_MASK		= 0x1,
 };
 static const __u64 NVME_CMBMSC_CBA_MASK = 0xfffffffffffffull;
 
 #define NVME_CMBMSC_CRE(cmbmsc)		NVME_GET(cmbmsc, CMBMSC_CRE)
 #define NVME_CMBMSC_CMSE(cmbmsc)	NVME_GET(cmbmsc, CMBMSC_CMSE)
 #define NVME_CMBMSC_CBA(cmbmsc)		NVME_GET(cmbmsc, CMBMSC_CBA)
 
+/**
+ * enum nvme_cmbsts - This field indicates the controller memory buffer status
+ * @NVME_CMBSTS_CBAI_SHIFT:	Shift amount to get the controller base address invalid
+ * @NVME_CMBSTS_CBAI_MASK:	Mask to get the controller base address invalid
+ */
 enum nvme_cmbsts {
 	NVME_CMBSTS_CBAI_SHIFT	= 0,
 	NVME_CMBSTS_CBAI_MASK	= 0x1,
 };
 
 #define NVME_CMBSTS_CBAI(cmbsts)	NVME_GET(cmbsts, CMBSTS_CBAI)
 
+/**
+ * enum nvme_unit - Defined buffer size and write throughput granularity units
+ * @NVME_UNIT_B:	Bytes or Bytes/second
+ * @NVME_UNIT_1K:	1 KiB or 1 KiB/second
+ * @NVME_UNIT_1M:	1 MiB or 1 MiB/second
+ * @NVME_UNIT_1G:	1 GiB or 1 GiB/second
+ */
+enum nvme_unit {
+	NVME_UNIT_B	= 0,
+	NVME_UNIT_1K	= 1,
+	NVME_UNIT_1M	= 2,
+	NVME_UNIT_1G	= 3,
+};
+
+/**
+ * enum nvme_cmbebs - This field indicates the controller memory buffer elasticity buffer size
+ * @NVME_CMBEBS_CMBSZU_SHIFT:	Shift amount to get the CMB elasticity buffer size units
+ * @NVME_CMBEBS_RBB_SHIFT:	Shift amount to get the read bypass behavior
+ * @NVME_CMBEBS_CMBWBZ_SHIFT:	Shift amount to get the CMB elasiticity buffer size base
+ * @NVME_CMBEBS_CMBSZU_MASK:	Mask to get the CMB elasticity buffer size units
+ * @NVME_CMBEBS_RBB_MASK:	Mask to get the read bypass behavior
+ * @NVME_CMBEBS_CMBWBZ_MASK:	Mask to get the CMB elasiticity buffer size base
+ * @NVME_CMBEBS_CMBSZU_B:	Bytes granularity
+ * @NVME_CMBEBS_CMBSZU_1K:	1 KiB granularity
+ * @NVME_CMBEBS_CMBSZU_1M:	1 MiB granularity
+ * @NVME_CMBEBS_CMBSZU_1G:	1 GiB granularity
+ */
+enum nvme_cmbebs {
+	NVME_CMBEBS_CMBSZU_SHIFT	= 0,
+	NVME_CMBEBS_RBB_SHIFT		= 4,
+	NVME_CMBEBS_CMBWBZ_SHIFT	= 8,
+	NVME_CMBEBS_CMBSZU_MASK		= 0xf,
+	NVME_CMBEBS_RBB_MASK		= 0x1,
+	NVME_CMBEBS_CMBWBZ_MASK		= 0xffffff,
+	NVME_CMBEBS_CMBSZU_B		= NVME_UNIT_B,
+	NVME_CMBEBS_CMBSZU_1K		= NVME_UNIT_1K,
+	NVME_CMBEBS_CMBSZU_1M		= NVME_UNIT_1M,
+	NVME_CMBEBS_CMBSZU_1G		= NVME_UNIT_1G,
+};
+
+#define NVME_CMBEBS_CMBSZU(cmbebs)	NVME_GET(cmbebs, CMBEBS_CMBSZU)
+#define NVME_CMBEBS_RBB(cmbebs)		NVME_GET(cmbebs, CMBEBS_RBB)
+#define NVME_CMBEBS_CMBWBZ(cmbebs)	NVME_GET(cmbebs, CMBEBS_CMBWBZ)
+
+/**
+ * enum nvme_cmbswtp - This field indicates the controller memory buffer sustained write throughput
+ * @NVME_CMBSWTP_CMBSWTU_SHIFT:	Shift amount to get the CMB sustained write throughput units
+ * @NVME_CMBSWTP_CMBSWTV_SHIFT:	Shift amount to get the CMB sustained write throughput
+ * @NVME_CMBSWTP_CMBSWTU_MASK:	Mask to get the CMB sustained write throughput units
+ * @NVME_CMBSWTP_CMBSWTV_MASK:	Mask to get the CMB sustained write throughput
+ * @NVME_CMBSWTP_CMBSWTU_B:	Bytes/second granularity
+ * @NVME_CMBSWTP_CMBSWTU_1K:	1 KiB/second granularity
+ * @NVME_CMBSWTP_CMBSWTU_1M:	1 MiB/second granularity
+ * @NVME_CMBSWTP_CMBSWTU_1G:	1 GiB/second granularity
+ */
+enum nvme_cmbswtp {
+	NVME_CMBSWTP_CMBSWTU_SHIFT	= 0,
+	NVME_CMBSWTP_CMBSWTV_SHIFT	= 8,
+	NVME_CMBSWTP_CMBSWTU_MASK	= 0xf,
+	NVME_CMBSWTP_CMBSWTV_MASK	= 0xffffff,
+	NVME_CMBSWTP_CMBSWTU_B		= NVME_UNIT_B,
+	NVME_CMBSWTP_CMBSWTU_1K		= NVME_UNIT_1K,
+	NVME_CMBSWTP_CMBSWTU_1M		= NVME_UNIT_1M,
+	NVME_CMBSWTP_CMBSWTU_1G		= NVME_UNIT_1G,
+};
+
+#define NVME_CMBSWTP_CMBSWTU(cmbswtp)	NVME_GET(cmbswtp, CMBSWTP_CMBSWTU)
+#define NVME_CMBSWTP_CMBSWTV(cmbswtp)	NVME_GET(cmbswtp, CMBSWTP_CMBSWTV)
+
+/**
+ * enum nvme_crto - This field indicates the controller ready timeouts
+ * @NVME_CRTO_CRWMT_SHIFT:	Shift amount to get the  controller ready with media timeout
+ * @NVME_CRTO_CRIMT_SHIFT:	Shift amount to get the controller ready independent of media timeout
+ * @NVME_CRTO_CRWMT_MASK:	Mask to get the controller ready with media timeout
+ * @NVME_CRTO_CRIMT_MASK:	Mask to get the controller ready independent of media timeout
+ */
 enum nvme_crto {
-	NVME_CRTO_CRIMT_SHIFT	= 16,
-	NVME_CRTO_CRIMT_MASK	= 0xffff0000,
 	NVME_CRTO_CRWMT_SHIFT	= 0,
-	NVME_CRTO_CRWMT_MASK	= 0x0000ffff,
+	NVME_CRTO_CRIMT_SHIFT	= 16,
+	NVME_CRTO_CRWMT_MASK	= 0xffff,
+	NVME_CRTO_CRIMT_MASK	= 0xffff,
 };
 
 #define NVME_CRTO_CRIMT(crto)	NVME_GET(crto, CRTO_CRIMT)
 #define NVME_CRTO_CRWMT(crto)	NVME_GET(crto, CRTO_CRWMT)
 
+/**
+ * enum nvme_pmrcap - This field indicates the persistent memory region capabilities
+ * @NVME_PMRCAP_RDS_SHIFT:	Shift amount to get the read data support
+ * @NVME_PMRCAP_WDS_SHIFT:	Shift amount to get the write data support
+ * @NVME_PMRCAP_BIR_SHIFT:	Shift amount to get the base indicator register
+ * @NVME_PMRCAP_PMRTU_SHIFT:	Shift amount to get the persistent memory region time units
+ * @NVME_PMRCAP_PMRWBM_SHIFT:	Shift amount to get the persistent memory region write barrier mechanisms
+ * @NVME_PMRCAP_PMRTO_SHIFT:	Shift amount to get the persistent memory region timeout
+ * @NVME_PMRCAP_CMSS_SHIFT:	Shift amount to get the controller memory space supported
+ * @NVME_PMRCAP_PMRWMB_SHIFT:	Deprecated shift amount to get the persistent memory region write barrier mechanisms
+ * @NVME_PMRCAP_RDS_MASK:	Mask to get the read data support
+ * @NVME_PMRCAP_WDS_MASK:	Mask to get the write data support
+ * @NVME_PMRCAP_BIR_MASK:	Mask to get the base indicator register
+ * @NVME_PMRCAP_PMRTU_MASK:	Mask to get the persistent memory region time units
+ * @NVME_PMRCAP_PMRWBM_MASK:	Mask to get the persistent memory region write barrier mechanisms
+ * @NVME_PMRCAP_PMRTO_MASK:	Mask to get the persistent memory region timeout
+ * @NVME_PMRCAP_CMSS_MASK:	Mask to get the controller memory space supported
+ * @NVME_PMRCAP_PMRWMB_MASK:	Deprecated mask to get the persistent memory region write barrier mechanisms
+ * @NVME_PMRCAP_PMRTU_500MS:	500 milliseconds
+ * @NVME_PMRCAP_PMRTU_60S:	minutes
+ */
 enum nvme_pmrcap {
 	NVME_PMRCAP_RDS_SHIFT		= 3,
 	NVME_PMRCAP_WDS_SHIFT		= 4,
 	NVME_PMRCAP_BIR_SHIFT		= 5,
 	NVME_PMRCAP_PMRTU_SHIFT		= 8,
-	NVME_PMRCAP_PMRWMB_SHIFT	= 10,
+	NVME_PMRCAP_PMRWBM_SHIFT	= 10,
 	NVME_PMRCAP_PMRTO_SHIFT		= 16,
 	NVME_PMRCAP_CMSS_SHIFT		= 24,
+	NVME_PMRCAP_PMRWMB_SHIFT	= NVME_PMRCAP_PMRWBM_SHIFT, /* Deprecated */
 	NVME_PMRCAP_RDS_MASK		= 0x1,
 	NVME_PMRCAP_WDS_MASK		= 0x1,
 	NVME_PMRCAP_BIR_MASK		= 0x7,
 	NVME_PMRCAP_PMRTU_MASK		= 0x3,
-	NVME_PMRCAP_PMRWMB_MASK		= 0xf,
+	NVME_PMRCAP_PMRWBM_MASK		= 0xf,
 	NVME_PMRCAP_PMRTO_MASK		= 0xff,
 	NVME_PMRCAP_CMSS_MASK		= 0x1,
+	NVME_PMRCAP_PMRWMB_MASK		= NVME_PMRCAP_PMRWBM_MASK, /* Deprecated */
 	NVME_PMRCAP_PMRTU_500MS		= 0,
 	NVME_PMRCAP_PMRTU_60S		= 1,
 };
 
 #define NVME_PMRCAP_RDS(pmrcap)		NVME_GET(pmrcap, PMRCAP_RDS)
 #define NVME_PMRCAP_WDS(pmrcap)		NVME_GET(pmrcap, PMRCAP_WDS)
 #define NVME_PMRCAP_BIR(pmrcap)		NVME_GET(pmrcap, PMRCAP_BIR)
 #define NVME_PMRCAP_PMRTU(pmrcap)	NVME_GET(pmrcap, PMRCAP_PMRTU)
-#define NVME_PMRCAP_PMRWMB(pmrcap)	NVME_GET(pmrcap, PMRCAP_PMRWMB)
+#define NVME_PMRCAP_PMRWBM(pmrcap)	NVME_GET(pmrcap, PMRCAP_PMRWBM)
 #define NVME_PMRCAP_PMRTO(pmrcap)	NVME_GET(pmrcap, PMRCAP_PMRTO)
 #define NVME_PMRCAP_CMSS(pmrcap)	NVME_GET(pmrcap, PMRCAP_CMSS)
+#define NVME_PMRCAP_PMRWMB(pmrcap)	NVME_GET(pmrcap, PMRCAP_PMRWMB) /* Deprecated */
 
+/**
+ * enum nvme_pmrctl - This field indicates the persistent memory region control
+ * @NVME_PMRCTL_EN_SHIFT:	Shift amount to get the enable
+ * @NVME_PMRCTL_EN_MASK:	Mask to get the enable
+ */
 enum nvme_pmrctl {
 	NVME_PMRCTL_EN_SHIFT	= 0,
 	NVME_PMRCTL_EN_MASK	= 0x1,
 };
 
 #define NVME_PMRCTL_EN(pmrctl)		NVME_GET(pmrctl, PMRCTL_EN)
 
+/**
+ * enum nvme_pmrsts - This field indicates the persistent memory region status
+ * @NVME_PMRSTS_ERR_SHIFT:	Shift amount to get the error
+ * @NVME_PMRSTS_NRDY_SHIFT:	Shift amount to get the not ready
+ * @NVME_PMRSTS_HSTS_SHIFT:	Shift amount to get the health status
+ * @NVME_PMRSTS_CBAI_SHIFT:	Shift amount to get the controller base address invalid
+ * @NVME_PMRSTS_ERR_MASK:	Mask to get the error
+ * @NVME_PMRSTS_NRDY_MASK:	Mask to get the not ready
+ * @NVME_PMRSTS_HSTS_MASK:	Mask to get the health status
+ * @NVME_PMRSTS_CBAI_MASK:	Mask to get the controller base address invalid
+ */
 enum nvme_pmrsts {
 	NVME_PMRSTS_ERR_SHIFT		= 0,
 	NVME_PMRSTS_NRDY_SHIFT		= 8,
 	NVME_PMRSTS_HSTS_SHIFT		= 9,
 	NVME_PMRSTS_CBAI_SHIFT		= 12,
 	NVME_PMRSTS_ERR_MASK		= 0xff,
 	NVME_PMRSTS_NRDY_MASK		= 0x1,
@@ -547,25 +896,38 @@
 };
 
 #define NVME_PMRSTS_ERR(pmrsts)		NVME_GET(pmrsts, PMRSTS_ERR)
 #define NVME_PMRSTS_NRDY(pmrsts)	NVME_GET(pmrsts, PMRSTS_NRDY)
 #define NVME_PMRSTS_HSTS(pmrsts)	NVME_GET(pmrsts, PMRSTS_HSTS)
 #define NVME_PMRSTS_CBAI(pmrsts)	NVME_GET(pmrsts, PMRSTS_CBAI)
 
+/**
+ * enum nvme_pmrebs - This field indicates the persistent memory region elasticity buffer size
+ * @NVME_PMREBS_PMRSZU_SHIFT:	Shift amount to get the PMR elasticity buffer size units
+ * @NVME_PMREBS_RBB_SHIFT:	Shift amount to get the read bypass behavior
+ * @NVME_PMREBS_PMRWBZ_SHIFT:	Shift amount to get the PMR elasticity buffer size base
+ * @NVME_PMREBS_PMRSZU_MASK:	Mask to get the PMR elasticity buffer size units
+ * @NVME_PMREBS_RBB_MASK:	Mask to get the read bypass behavior
+ * @NVME_PMREBS_PMRWBZ_MASK:	Mask to get the PMR elasticity buffer size base
+ * @NVME_PMREBS_PMRSZU_B:	Bytes
+ * @NVME_PMREBS_PMRSZU_1K:	1 KiB
+ * @NVME_PMREBS_PMRSZU_1M:	1 MiB
+ * @NVME_PMREBS_PMRSZU_1G:	1 GiB
+ */
 enum nvme_pmrebs {
 	NVME_PMREBS_PMRSZU_SHIFT	= 0,
 	NVME_PMREBS_RBB_SHIFT		= 4,
 	NVME_PMREBS_PMRWBZ_SHIFT	= 8,
 	NVME_PMREBS_PMRSZU_MASK		= 0xf,
 	NVME_PMREBS_RBB_MASK		= 0x1,
 	NVME_PMREBS_PMRWBZ_MASK		= 0xffffff,
-	NVME_PMREBS_PMRSZU_B		= 0,
-	NVME_PMREBS_PMRSZU_1K		= 1,
-	NVME_PMREBS_PMRSZU_1M		= 2,
-	NVME_PMREBS_PMRSZU_1G		= 3,
+	NVME_PMREBS_PMRSZU_B		= NVME_UNIT_B,
+	NVME_PMREBS_PMRSZU_1K		= NVME_UNIT_1K,
+	NVME_PMREBS_PMRSZU_1M		= NVME_UNIT_1M,
+	NVME_PMREBS_PMRSZU_1G		= NVME_UNIT_1G,
 };
 
 #define NVME_PMREBS_PMRSZU(pmrebs)	NVME_GET(pmrebs, PMREBS_PMRSZU)
 #define NVME_PMREBS_RBB(pmrebs)		NVME_GET(pmrebs, PMREBS_RBB)
 #define NVME_PMREBS_PMRWBZ(pmrebs)	NVME_GET(pmrebs, PMREBS_PMRWBZ)
 
 /**
@@ -577,23 +939,34 @@
  */
 static inline __u64 nvme_pmr_size(__u32 pmrebs)
 {
 	return ((__u64)NVME_PMREBS_PMRWBZ(pmrebs)) *
 		(1ULL << (10 * NVME_PMREBS_PMRSZU(pmrebs)));
 }
 
+/**
+ * enum nvme_pmrswtp - This field indicates the persistent memory region sustained write throughput
+ * @NVME_PMRSWTP_PMRSWTU_SHIFT:	Shift amount to get the PMR sustained write throughput units
+ * @NVME_PMRSWTP_PMRSWTV_SHIFT:	Shift amount to get the PMR sustained write throughput
+ * @NVME_PMRSWTP_PMRSWTU_MASK:	Mask to get the PMR sustained write throughput units
+ * @NVME_PMRSWTP_PMRSWTV_MASK:	Mask to get the PMR sustained write throughput
+ * @NVME_PMRSWTP_PMRSWTU_BPS:	Bytes per second
+ * @NVME_PMRSWTP_PMRSWTU_KBPS:	1 KiB / s
+ * @NVME_PMRSWTP_PMRSWTU_MBPS:	1 MiB / s
+ * @NVME_PMRSWTP_PMRSWTU_GBPS:	1 GiB / s
+ */
 enum nvme_pmrswtp {
 	NVME_PMRSWTP_PMRSWTU_SHIFT	= 0,
 	NVME_PMRSWTP_PMRSWTV_SHIFT	= 8,
 	NVME_PMRSWTP_PMRSWTU_MASK	= 0xf,
 	NVME_PMRSWTP_PMRSWTV_MASK	= 0xffffff,
-	NVME_PMRSWTP_PMRSWTU_BPS	= 0,
-	NVME_PMRSWTP_PMRSWTU_KBPS	= 1,
-	NVME_PMRSWTP_PMRSWTU_MBPS	= 2,
-	NVME_PMRSWTP_PMRSWTU_GBPS	= 3,
+	NVME_PMRSWTP_PMRSWTU_BPS	= NVME_UNIT_B,
+	NVME_PMRSWTP_PMRSWTU_KBPS	= NVME_UNIT_1K,
+	NVME_PMRSWTP_PMRSWTU_MBPS	= NVME_UNIT_1M,
+	NVME_PMRSWTP_PMRSWTU_GBPS	= NVME_UNIT_1G,
 };
 
 #define NVME_PMRSWTP_PMRSWTU(pmrswtp)	NVME_GET(pmrswtp, PMRSWTP_PMRSWTU)
 #define NVME_PMRSWTP_PMRSWTV(pmrswtp)	NVME_GET(pmrswtp, PMRSWTP_PMRSWTU)
 
 /**
  * nvme_pmr_throughput() - Calculate throughput of persistent memory buffer
@@ -603,24 +976,39 @@
  */
 static inline __u64 nvme_pmr_throughput(__u32 pmrswtp)
 {
 	return ((__u64)NVME_PMRSWTP_PMRSWTV(pmrswtp)) *
 		(1ULL << (10 * NVME_PMRSWTP_PMRSWTU(pmrswtp)));
 }
 
+/**
+ * enum nvme_pmrmsc - This field indicates the persistent memory region memory space control
+ * @NVME_PMRMSC_CMSE_SHIFT:	Shift amount to get the controller memory space enable
+ * @NVME_PMRMSC_CBA_SHIFT:	Shift amount to get the controller base address
+ * @NVME_PMRMSC_CMSE_MASK:	Mask to get the controller memory space enable
+ */
 enum nvme_pmrmsc {
 	NVME_PMRMSC_CMSE_SHIFT	= 1,
 	NVME_PMRMSC_CBA_SHIFT	= 12,
 	NVME_PMRMSC_CMSE_MASK	= 0x1,
 };
 static const __u64 NVME_PMRMSC_CBA_MASK = 0xfffffffffffffull;
 
 #define NVME_PMRMSC_CMSE(pmrmsc)	NVME_GET(pmrmsc, PMRMSC_CMSE)
 #define NVME_PMRMSC_CBA(pmrmsc)		NVME_GET(pmrmsc, PMRMSC_CBA)
 
+/**
+ * enum nvme_flbas - This field indicates the formatted LBA size
+ * @NVME_FLBAS_LOWER_SHIFT:	Shift amount to get the format index least significant 4 bits
+ * @NVME_FLBAS_META_EXT_SHIFT:	Shift amount to get the metadata transferred
+ * @NVME_FLBAS_HIGHER_SHIFT:	Shift amount to get the format index most significant 2 bits
+ * @NVME_FLBAS_LOWER_MASK:	Mask to get the format index least significant 4 bits
+ * @NVME_FLBAS_META_EXT_MASK:	Mask to get the metadata transferred
+ * @NVME_FLBAS_HIGHER_MASK:	Mask to get the format index most significant 2 bits
+ */
 enum nvme_flbas {
 	NVME_FLBAS_LOWER_SHIFT		= 0,
 	NVME_FLBAS_META_EXT_SHIFT	= 4,
 	NVME_FLBAS_HIGHER_SHIFT		= 5,
 	NVME_FLBAS_LOWER_MASK		= 0xf,
 	NVME_FLBAS_META_EXT_MASK	= 0x1,
 	NVME_FLBAS_HIGHER_MASK		= 0x3,
@@ -1073,14 +1461,46 @@
 	__u8			rsvd1807[241];
 
 	struct nvme_id_psd	psd[32];
 	__u8			vs[1024];
 };
 
 /**
+ * enum nvme_cmic - This field indicates the controller multi-path I/O and NS sharing capabilities
+ * @NVME_CMIC_MULTI_PORT_SHIFT:		Shift amount to get the NVM subsystem port
+ * @NVME_CMIC_MULTI_CTRL_SHIFT:		Shift amount to get the controllers
+ * @NVME_CMIC_MULTI_SRIOV_SHIFT:	Shift amount to get the SR-IOV virtual function
+ * @NVME_CMIC_MULTI_ANA_SHIFT:		Shift amount to get the asymmetric namespace access reporting
+ * @NVME_CMIC_MULTI_RSVD_SHIFT:		Shift amount to get the reserved
+ * @NVME_CMIC_MULTI_PORT_MASK:		Mask to get the NVM subsystem port
+ * @NVME_CMIC_MULTI_CTRL_MASK:		Mask to get the controllers
+ * @NVME_CMIC_MULTI_SRIOV_MASK:		Mask to get the SR-IOV virtual function
+ * @NVME_CMIC_MULTI_ANA_MASK:		Mask to get the asymmetric namespace access reporting
+ * @NVME_CMIC_MULTI_RSVD_MASK:		Mask to get the reserved
+ */
+enum nvme_cmic {
+	NVME_CMIC_MULTI_PORT_SHIFT	= 0,
+	NVME_CMIC_MULTI_CTRL_SHIFT	= 1,
+	NVME_CMIC_MULTI_SRIOV_SHIFT	= 2,
+	NVME_CMIC_MULTI_ANA_SHIFT	= 3,
+	NVME_CMIC_MULTI_RSVD_SHIFT	= 4,
+	NVME_CMIC_MULTI_PORT_MASK	= 0x1,
+	NVME_CMIC_MULTI_CTRL_MASK	= 0x1,
+	NVME_CMIC_MULTI_SRIOV_MASK	= 0x1,
+	NVME_CMIC_MULTI_ANA_MASK	= 0x1,
+	NVME_CMIC_MULTI_RSVD_MASK	= 0xf,
+};
+
+#define NVME_CMIC_MULTI_PORT(cmic)	NVME_GET(cmic, CMIC_MULTI_PORT)
+#define NVME_CMIC_MULTI_CTRL(cmic)	NVME_GET(cmic, CMIC_MULTI_CTRL)
+#define NVME_CMIC_MULTI_SRIOV(cmic)	NVME_GET(cmic, CMIC_MULTI_SRIOV)
+#define NVME_CMIC_MULTI_ANA(cmic)	NVME_GET(cmic, CMIC_MULTI_ANA)
+#define NVME_CMIC_MULTI_RSVD(cmic)	NVME_GET(cmic, CMIC_MULTI_RSVD)
+
+/**
  * enum nvme_id_ctrl_cmic - Controller Multipath IO and Namespace Sharing
  *			    Capabilities of the controller and NVM subsystem.
  * @NVME_CTRL_CMIC_MULTI_PORT:		If set, then the NVM subsystem may contain
  *					more than one NVM subsystem port, otherwise
  *					the NVM subsystem contains only a single
  *					NVM subsystem port.
  * @NVME_CTRL_CMIC_MULTI_CTRL:		If set, then the NVM subsystem may contain
@@ -3336,14 +3756,61 @@
 	__le16	gen_number;
 	__le32	rci;
 	__u8	rsvd378[102];
 	__u8	seb[32];
 } __attribute__((packed));
 
 /**
+ * enum nvme_pel_rci - This field indicates the persistent event log reporting context
+ * @NVME_PEL_RCI_RCPID_SHIFT:	Shift amount to get the reporting context port identifier
+ *				from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RCPIT_SHIFT:	Shift amount to get the reporting context port identifier
+ *				type from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RCE_SHIFT:	Shift amount to get the reporting context exists
+ *				from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RSVD_SHIFT:	Shift amount to get the reserved reporting context
+ *				from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RCPID_MASK:	Mask to get the reporting context port identifier from
+ *				the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RCPIT_MASK:	Mask to get the reporting context port identifier type from
+ *				the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RCE_MASK:	Mask to get the reporting context exists from
+ *				the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_RCI_RSVD_MASK:	Mask to get the reserved reporting context from
+ *				the &struct nvme_persistent_event_log.rci field.
+ */
+enum nvme_pel_rci {
+	NVME_PEL_RCI_RCPID_SHIFT	= 0,
+	NVME_PEL_RCI_RCPIT_SHIFT	= 16,
+	NVME_PEL_RCI_RCE_SHIFT		= 18,
+	NVME_PEL_RCI_RSVD_SHIFT		= 19,
+	NVME_PEL_RCI_RCPID_MASK		= 0xffff,
+	NVME_PEL_RCI_RCPIT_MASK		= 0x3,
+	NVME_PEL_RCI_RCE_MASK		= 0x1,
+	NVME_PEL_RCI_RSVD_MASK		= 0x1fff,
+};
+
+#define NVME_PEL_RCI_RCPID(rci)	NVME_GET(rci, PEL_RCI_RCPID)
+#define NVME_PEL_RCI_RCPIT(rci)	NVME_GET(rci, PEL_RCI_RCPIT)
+#define NVME_PEL_RCI_RCE(rci)	NVME_GET(rci, PEL_RCI_RCE)
+#define NVME_PEL_RCI_RSVD(rci)	NVME_GET(rci, PEL_RCI_RSVD)
+
+/**
+ * enum nvme_pel_rci_rcpit - Persistent Event Log Reporting Context - Port Identifier Type
+ * @NVME_PEL_RCI_RCPIT_NOT_EXIST:	Does not already exist
+ * @NVME_PEL_RCI_RCPIT_EST_PORT:	Established by an NVM subsystem port
+ * @NVME_PEL_RCI_RCPIT_EST_ME:		Established by a Management Endpoint
+ */
+enum nvme_pel_rci_rcpit {
+	NVME_PEL_RCI_RCPIT_NOT_EXIST	= 0,
+	NVME_PEL_RCI_RCPIT_EST_PORT	= 1,
+	NVME_PEL_RCI_RCPIT_EST_ME	= 2,
+};
+
+/**
  * struct nvme_persistent_event_entry - Persistent Event
  * @etype:	Event Type
  * @etype_rev:	Event Type Revision
  * @ehl:	Event Header Length
  * @ehai:	Event Header Additional Info
  * @cntlid:	Controller Identifier
  * @ets:	Event Timestamp
@@ -3394,14 +3861,49 @@
 	NVME_PEL_SANITIZE_COMPLETION_EVENT	= 0x0a,
 	NVME_PEL_SET_FEATURE_EVENT		= 0x0b,
 	NVME_PEL_TELEMETRY_CRT			= 0x0c,
 	NVME_PEL_THERMAL_EXCURSION_EVENT	= 0x0d,
 };
 
 /**
+ * enum nvme_pel_ehai - This field indicates the persistent event header additional information
+ * @NVME_PEL_EHAI_PIT_SHIFT:	Shift amount to get the reporting context port identifier
+ *				from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_EHAI_RSVD_SHIFT:	Shift amount to get the reserved reporting context
+ *				from the &struct nvme_persistent_event_log.rci field.
+ * @NVME_PEL_EHAI_PIT_MASK:	Mask to get the reporting context port identifier from
+ *				the &struct nvme_st_result.dsts field.
+ * @NVME_PEL_EHAI_RSVD_MASK:	Mask to get the reserved reporting context from
+ *				the &struct nvme_st_result.dsts field.
+ */
+enum nvme_pel_ehai {
+	NVME_PEL_EHAI_PIT_SHIFT		= 0,
+	NVME_PEL_EHAI_RSVD_SHIFT	= 2,
+	NVME_PEL_EHAI_PIT_MASK		= 0x3,
+	NVME_PEL_EHAI_RSVD_MASK		= 0x3f,
+};
+
+#define NVME_PEL_EHAI_PIT(ehai)		NVME_GET(ehai, PEL_EHAI_PIT)
+#define NVME_PEL_EHAI_RSVD(ehai)	NVME_GET(ehai, PEL_EHAI_RSVD)
+
+/**
+ * enum nvme_pel_ehai_pit - Persistent Event Header Additional Information - Port Identifier Type
+ * @NVME_PEL_EHAI_PIT_NOT_REPORTED:	PIT not reported and PELPID does not apply
+ * @NVME_PEL_EHAI_PIT_NSS_PORT:		NVM subsystem port
+ * @NVME_PEL_EHAI_PIT_NMI_PORT:		NVMe-MI port
+ * @NVME_PEL_EHAI_PIT_NOT_ASSOCIATED:	Event not associated with any port and PELPID does not apply
+ */
+enum nvme_pel_ehai_pit {
+	NVME_PEL_EHAI_PIT_NOT_REPORTED		= 0,
+	NVME_PEL_EHAI_PIT_NSS_PORT		= 1,
+	NVME_PEL_EHAI_PIT_NMI_PORT		= 2,
+	NVME_PEL_EHAI_PIT_NOT_ASSOCIATED	= 3,
+};
+
+/**
  * struct nvme_fw_commit_event - Firmware Commit Event Data
  * @old_fw_rev:			Old Firmware Revision
  * @new_fw_rev:			New Firmware Revision
  * @fw_commit_action:		Firmware Commit Action
  * @fw_slot:			Firmware Slot
  * @sct_fw:			Status Code Type for Firmware Commit Command
  * @sc_fw:			Status Returned for Firmware Commit Command
@@ -3566,14 +4068,42 @@
  */
 struct nvme_set_feature_event {
 	__le32	layout;
 	__le32	cdw_mem[0];
 };
 
 /**
+ * enum nvme_set_feat_event_layout - This field indicates the set feature event layout
+ * @NVME_SET_FEAT_EVENT_DW_COUNT_SHIFT:	Shift amount to get the Dword count from the
+ *					&struct nvme_set_feature_event.layout field.
+ * @NVME_SET_FEAT_EVENT_CC_DW0_SHIFT:	Shift amount to get the logged command completion Dword 0
+ *					from the &struct nvme_set_feature_event.layout field.
+ * @NVME_SET_FEAT_EVENT_MB_COUNT_SHIFT:	Shift amount to get the memory buffer count from
+ *					the &struct nvme_set_feature_event.layout field.
+ * @NVME_SET_FEAT_EVENT_DW_COUNT_MASK:	Mask to get the Dword count from the &struct
+ *					nvme_set_feature_event.layout field.
+ * @NVME_SET_FEAT_EVENT_CC_DW0_MASK:	Mask to get the logged command completion Dword 0 from
+ *					the &struct nvme_set_feature_event.layout field.
+ * @NVME_SET_FEAT_EVENT_MB_COUNT_MASK:	Mask to get the memory buffer count from the &struct
+ *					nvme_set_feature_event.layout field.
+ */
+enum nvme_set_feat_event_layout {
+	NVME_SET_FEAT_EVENT_DW_COUNT_SHIFT	= 0,
+	NVME_SET_FEAT_EVENT_CC_DW0_SHIFT	= 3,
+	NVME_SET_FEAT_EVENT_MB_COUNT_SHIFT	= 16,
+	NVME_SET_FEAT_EVENT_DW_COUNT_MASK	= 0x7,
+	NVME_SET_FEAT_EVENT_CC_DW0_MASK		= 0x1,
+	NVME_SET_FEAT_EVENT_MB_COUNT_MASK	= 0xffff,
+};
+
+#define NVME_SET_FEAT_EVENT_DW_COUNT(layout)	NVME_GET(layout, SET_FEAT_EVENT_DW_COUNT)
+#define NVME_SET_FEAT_EVENT_CC_DW0(layout)	NVME_GET(layout, SET_FEAT_EVENT_CC_DW0)
+#define NVME_SET_FEAT_EVENT_MB_COUNT(layout)	NVME_GET(layout, SET_FEAT_EVENT_MB_COUNT)
+
+/**
  * struct nvme_thermal_exc_event -  Thermal Excursion Event Data
  * @over_temp:	Over Temperature
  * @threshold:	temperature threshold
  */
 struct nvme_thermal_exc_event {
 	__u8	over_temp;
 	__u8	threshold;
@@ -3745,14 +4275,35 @@
 	__u8	rsvd1[3];
 	__le32	bpinfo;
 	__u8	rsvd8[8];
 	__u8	boot_partition_data[];
 };
 
 /**
+ * enum nvme_boot_partition_info - This field indicates the boot partition information
+ * @NVME_BOOT_PARTITION_INFO_BPSZ_SHIFT:	Shift amount to get the boot partition size from
+ *						the &struct nvme_boot_partition.bpinfo field.
+ * @NVME_BOOT_PARTITION_INFO_ABPID_SHIFT:	Shift amount to get the active boot partition ID
+ *						from the &struct nvme_boot_partition.bpinfo field.
+ * @NVME_BOOT_PARTITION_INFO_BPSZ_MASK:		Mask to get the boot partition size from the
+ *						&struct nvme_boot_partition.bpinfo field.
+ * @NVME_BOOT_PARTITION_INFO_ABPID_MASK:	Mask to get the active boot partition ID from the
+ *						&struct nvme_boot_partition.bpinfo field.
+ */
+enum nvme_boot_partition_info {
+	NVME_BOOT_PARTITION_INFO_BPSZ_SHIFT	= 0,
+	NVME_BOOT_PARTITION_INFO_ABPID_SHIFT	= 31,
+	NVME_BOOT_PARTITION_INFO_BPSZ_MASK	= 0x7fff,
+	NVME_BOOT_PARTITION_INFO_ABPID_MASK	= 0x1,
+};
+
+#define NVME_BOOT_PARTITION_INFO_BPSZ(bpinfo)	NVME_GET(bpinfo, BOOT_PARTITION_INFO_BPSZ)
+#define NVME_BOOT_PARTITION_INFO_ABPID(bpinfo)	NVME_GET(bpinfo, BOOT_PARTITION_INFO_ABPID)
+
+/**
  * struct nvme_eom_lane_desc - EOM Lane Descriptor
  * @rsvd0:	Reserved
  * @mstatus:	Measurement Status
  * @lane:	Lane number
  * @eye:	Eye number
  * @top:	Absolute number of rows from center to top edge of eye
  * @bottom:	Absolute number of rows from center to bottom edge of eye
@@ -3827,21 +4378,49 @@
 	__le16	etbetter;
 	__le16	etbest;
 	__u8	rsvd36[28];
 	struct nvme_eom_lane_desc descs[];
 };
 
 /**
- * enum nvme_eom_optional_data - EOM Optional Data Present Fields
- * @NVME_EOM_EYE_DATA_PRESENT:		Eye Data Present
+ * enum nvme_eom_optional_data_present - EOM Optional Data Present Fields
+ * @NVME_EOM_ODP_PEFP_SHIFT:	Shift amount to get the printable eye field present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ * @NVME_EOM_ODP_EDFP_SHIFT:	Shift amount to get the eye data field present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ * @NVME_EOM_ODP_RSVD_SHIFT:	Shift amount to get the reserved optional data present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ * @NVME_EOM_ODP_PEFP_MASK:	Mask to get the printable eye field present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ * @NVME_EOM_ODP_EDFP_MASK:	Mask to get the eye data field present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ * @NVME_EOM_ODP_RSVD_MASK:	Mask to get the reserved data present
+ *				from the &struct nvme_phy_rx_eom_log.odp field.
+ */
+enum nvme_eom_optional_data_present {
+	NVME_EOM_ODP_PEFP_SHIFT	= 0,
+	NVME_EOM_ODP_EDFP_SHIFT	= 1,
+	NVME_EOM_ODP_RSVD_SHIFT	= 2,
+	NVME_EOM_ODP_PEFP_MASK	= 0x1,
+	NVME_EOM_ODP_EDFP_MASK	= 0x1,
+	NVME_EOM_ODP_RSVD_MASK	= 0x3f,
+};
+
+#define NVME_EOM_ODP_PEFP(odp)	NVME_GET(odp, EOM_ODP_PEFP)
+#define NVME_EOM_ODP_EDFP(odp)	NVME_GET(odp, EOM_ODP_EDFP)
+#define NVME_EOM_ODP_RSVD(odp)	NVME_GET(odp, EOM_ODP_RSVD)
+
+/**
+ * enum nvme_eom_optional_data - EOM Optional Data Present Fields (Deprecated)
  * @NVME_EOM_PRINTABLE_EYE_PRESENT:	Printable Eye Present
+ * @NVME_EOM_EYE_DATA_PRESENT:		Eye Data Present
  */
 enum nvme_eom_optional_data {
-	NVME_EOM_EYE_DATA_PRESENT	= 1,
-	NVME_EOM_PRINTABLE_EYE_PRESENT	= 1 << 1,
+	NVME_EOM_PRINTABLE_EYE_PRESENT	= NVME_EOM_ODP_PEFP_MASK << NVME_EOM_ODP_PEFP_SHIFT,
+	NVME_EOM_EYE_DATA_PRESENT	= NVME_EOM_ODP_EDFP_MASK << NVME_EOM_ODP_EDFP_SHIFT,
 };
 
 /**
  * enum nvme_phy_rx_eom_progress - EOM In Progress Values
  * @NVME_PHY_RX_EOM_NOT_STARTED:	EOM Not Started
  * @NVME_PHY_RX_EOM_IN_PROGRESS:	EOM In Progress
  * @NVME_PHY_RX_EOM_COMPLETED:		EOM Completed
@@ -6913,14 +7492,15 @@
  * @NVME_LOG_LID_PERSISTENT_EVENT:		Persistent Event Log
  * @NVME_LOG_LID_LBA_STATUS:			LBA Status Information
  * @NVME_LOG_LID_ENDURANCE_GRP_EVT:		Endurance Group Event Aggregate
  * @NVME_LOG_LID_MEDIA_UNIT_STATUS:		Media Unit Status
  * @NVME_LOG_LID_SUPPORTED_CAP_CONFIG_LIST:	Supported Capacity Configuration Lis
  * @NVME_LOG_LID_FID_SUPPORTED_EFFECTS:		Feature Identifiers Supported and Effects
  * @NVME_LOG_LID_MI_CMD_SUPPORTED_EFFECTS:	NVMe-MI Commands Supported and Effects
+ * @NVME_LOG_LID_CMD_AND_FEAT_LOCKDOWN:		Command and Feature Lockdown
  * @NVME_LOG_LID_BOOT_PARTITION:		Boot Partition
  * @NVME_LOG_LID_PHY_RX_EOM:			Physical Interface Receiver Eye Opening Measurement
  * @NVME_LOG_LID_FDP_CONFIGS:			FDP Configurations
  * @NVME_LOG_LID_FDP_RUH_USAGE:			Reclaim Unit Handle Usage
  * @NVME_LOG_LID_FDP_STATS:			FDP Statistics
  * @NVME_LOG_LID_FDP_EVENTS:			FDP Events
  * @NVME_LOG_LID_DISCOVER:			Discovery
@@ -6945,14 +7525,15 @@
 	NVME_LOG_LID_PERSISTENT_EVENT				= 0x0d,
 	NVME_LOG_LID_LBA_STATUS					= 0x0e,
 	NVME_LOG_LID_ENDURANCE_GRP_EVT				= 0x0f,
 	NVME_LOG_LID_MEDIA_UNIT_STATUS				= 0x10,
 	NVME_LOG_LID_SUPPORTED_CAP_CONFIG_LIST			= 0x11,
 	NVME_LOG_LID_FID_SUPPORTED_EFFECTS			= 0x12,
 	NVME_LOG_LID_MI_CMD_SUPPORTED_EFFECTS			= 0x13,
+	NVME_LOG_LID_CMD_AND_FEAT_LOCKDOWN			= 0x14,
 	NVME_LOG_LID_BOOT_PARTITION				= 0x15,
 	NVME_LOG_LID_PHY_RX_EOM					= 0x19,
 	NVME_LOG_LID_FDP_CONFIGS				= 0x20,
 	NVME_LOG_LID_FDP_RUH_USAGE				= 0x21,
 	NVME_LOG_LID_FDP_STATS					= 0x22,
 	NVME_LOG_LID_FDP_EVENTS					= 0x23,
 	NVME_LOG_LID_DISCOVER					= 0x70,
```

### Comparing `libnvme-1.8/src/nvme/util.c` & `libnvme-1.9/src/nvme/util.c`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  */
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <stdbool.h>
 #include <string.h>
 #include <errno.h>
+#include <malloc.h>
 
 #include <sys/stat.h>
 #include <fcntl.h>
 #include <sys/param.h>
 #include <sys/types.h>
 #include <arpa/inet.h>
 #include <netdb.h>
@@ -615,14 +616,15 @@
 	[ENVME_CONNECT_ALREADY] = "already connected",
 	[ENVME_CONNECT_INVAL] = "invalid arguments/configuration",
 	[ENVME_CONNECT_ADDRINUSE] = "hostnqn already in use",
 	[ENVME_CONNECT_NODEV] = "invalid interface",
 	[ENVME_CONNECT_OPNOTSUPP] = "not supported",
 	[ENVME_CONNECT_CONNREFUSED] = "connection refused",
 	[ENVME_CONNECT_ADDRNOTAVAIL] = "cannot assign requested address",
+	[ENVME_CONNECT_IGNORED] = "connection ignored",
 };
 
 const char *nvme_errno_to_string(int status)
 {
 	const char *s = ARGSTR(libnvme_status, status);
 
 	return s;
@@ -1131,7 +1133,21 @@
 
 	if (posix_memalign((void *)&p, getpagesize(), _len))
 		return NULL;
 
 	memset(p, 0, _len);
 	return p;
 }
+
+void *__nvme_realloc(void *p, size_t len)
+{
+	size_t old_len = malloc_usable_size(p);
+
+	void *result = __nvme_alloc(len);
+
+	if (p) {
+		memcpy(result, p, min(old_len, len));
+		free(p);
+	}
+
+	return result;
+}
```

### Comparing `libnvme-1.8/src/nvme/util.h` & `libnvme-1.9/src/nvme/util.h`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
 							       __u8 *wps)
 {
 	*wps	= NVME_FEAT_WP_WPS(value);
 }
 
 static inline void nvme_id_ns_flbas_to_lbaf_inuse(__u8 flbas, __u8 *lbaf_inuse)
 {
-	*lbaf_inuse = ((NVME_FLBAS_HIGHER(flbas) >> 1) |
+	*lbaf_inuse = ((NVME_FLBAS_HIGHER(flbas) << 4) |
 			NVME_FLBAS_LOWER(flbas));
 }
 
 struct nvme_root;
 
 char *hostname2traddr(struct nvme_root *r, const char *traddr);
 
@@ -554,14 +554,16 @@
  * @prefix: A string that @s could be starting with
  *
  * Return: If @s starts with @prefix, then return a pointer within @s at
  * the first character after the matched @prefix. NULL otherwise.
  */
 char *startswith(const char *s, const char *prefix);
 
+#define min(x, y) ((x) > (y) ? (y) : (x))
+
 #define __round_mask(val, mult) ((__typeof__(val))((mult)-1))
 
 /**
  * round_up - Round a value @val to the next multiple specified by @mult.
  * @val:  Value to round
  * @mult: Multiple to round to.
  *
```

### Comparing `libnvme-1.8/subprojects/json-c.wrap` & `libnvme-1.9/subprojects/json-c.wrap`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/subprojects/openssl.wrap` & `libnvme-1.9/subprojects/openssl.wrap`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/cpp.cc` & `libnvme-1.9/test/cpp.cc`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/discovery.c` & `libnvme-1.9/test/ioctl/discovery.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/features.c` & `libnvme-1.9/test/ioctl/features.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/identify.c` & `libnvme-1.9/test/ioctl/identify.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/meson.build` & `libnvme-1.9/test/ioctl/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/mock.c` & `libnvme-1.9/test/ioctl/mock.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/mock.h` & `libnvme-1.9/test/ioctl/mock.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/util.c` & `libnvme-1.9/test/ioctl/util.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/ioctl/util.h` & `libnvme-1.9/test/ioctl/util.h`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/meson.build` & `libnvme-1.9/test/meson.build`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/mi-mctp.c` & `libnvme-1.9/test/mi-mctp.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/mi.c` & `libnvme-1.9/test/mi.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/mock-ifaddrs.c` & `libnvme-1.9/test/mock-ifaddrs.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/README` & `libnvme-1.9/test/nbft/README`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-Dell.PowerEdge.R660-fw1.5.5-single` & `libnvme-1.9/test/nbft/diffs/NBFT-Dell.PowerEdge.R660-fw1.5.5-single`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 subsystem_ns_list[0]->nid=5380b42fc0c5de718ccf9680be3ca7
 subsystem_ns_list[0]->subsys_nqn=nqn.1988-11.com.dell:powerstore:00:88b402df2d762AA7AF94
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=4105
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
 subsystem_ns_list[1]->index=2
 subsystem_ns_list[1]->num_hfis=1
 subsystem_ns_list[1]->hfis[0]->index=1
 subsystem_ns_list[1]->transport=tcp
 subsystem_ns_list[1]->traddr=172.18.240.60
 subsystem_ns_list[1]->trsvcid=4420
 subsystem_ns_list[1]->subsys_port_id=0
@@ -48,7 +50,9 @@
 subsystem_ns_list[1]->nid=f4c66fce74afdb8ccf96807eaeae
 subsystem_ns_list[1]->subsys_nqn=nqn.1988-11.com.dell:powerstore:00:88b402df2d762AA7AF94
 subsystem_ns_list[1]->pdu_header_digest_required=0
 subsystem_ns_list[1]->data_digest_required=0
 subsystem_ns_list[1]->controller_id=4105
 subsystem_ns_list[1]->asqsz=0
 subsystem_ns_list[1]->dhcp_root_path_string=(null)
+subsystem_ns_list[1]->discovered=0
+subsystem_ns_list[1]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-Dell.PowerEdge.R760` & `libnvme-1.9/test/nbft/diffs/NBFT-Dell.PowerEdge.R760`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 subsystem_ns_list[0]->nid=c8244ed9c15f53b8ccf96802efca
 subsystem_ns_list[0]->subsys_nqn=nqn.1988-11.com.dell:powerstore:00:2a64abf1c5b81F6C4549
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=5
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=1
+subsystem_ns_list[0]->unavailable=0
 subsystem_ns_list[1]->index=2
 subsystem_ns_list[1]->discovery->index=1
 subsystem_ns_list[1]->num_hfis=1
 subsystem_ns_list[1]->hfis[0]->index=1
 subsystem_ns_list[1]->transport=tcp
 subsystem_ns_list[1]->traddr=100.71.103.49
 subsystem_ns_list[1]->trsvcid=4420
@@ -54,7 +56,9 @@
 subsystem_ns_list[1]->nid=c8244ed9c15f53b8ccf96802efca
 subsystem_ns_list[1]->subsys_nqn=nqn.1988-11.com.dell:powerstore:00:2a64abf1c5b81F6C4549
 subsystem_ns_list[1]->pdu_header_digest_required=0
 subsystem_ns_list[1]->data_digest_required=0
 subsystem_ns_list[1]->controller_id=4166
 subsystem_ns_list[1]->asqsz=0
 subsystem_ns_list[1]->dhcp_root_path_string=(null)
+subsystem_ns_list[1]->discovered=1
+subsystem_ns_list[1]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-auto-ipv6` & `libnvme-1.9/test/nbft/diffs/NBFT-auto-ipv6`

 * *Files 4% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 subsystem_ns_list[0]->nid=848f4dc06d394968bf180569b8eea97
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.de.suse.mwilck:zeus.vagrant-nvmet.subsys04
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=1
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-dhcp-ipv4` & `libnvme-1.9/test/nbft/diffs/NBFT-dhcp-ipv4`

 * *Files 1% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 subsystem_ns_list[0]->nid=df669a88bd6f4dd68a505f97eb55c835
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.org.nvmexpress.boot.poc:bremer.vagrant-nvmet.subsys02
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=7
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=1
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-dhcp-ipv6` & `libnvme-1.9/test/nbft/diffs/NBFT-dhcp-ipv6`

 * *Files 2% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 subsystem_ns_list[0]->nid=df669a88bd6f4dd68a505f97eb55c835
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.org.nvmexpress.boot.poc:bremer.vagrant-nvmet.subsys02
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=34
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-rhpoc` & `libnvme-1.9/test/nbft/diffs/NBFT-rhpoc`

 * *Files 2% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 subsystem_ns_list[0]->nid=bee9c2b7176144b5a4e6f69498a94b
 subsystem_ns_list[0]->subsys_nqn=nqn.2014-08.org.nvmexpress:uuid:0c468c4d-a385-47e0-8299-6e95051277db
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=12
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-static-ipv4` & `libnvme-1.9/test/nbft/diffs/NBFT-static-ipv4`

 * *Files 5% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 subsystem_ns_list[0]->nid=df669a88bd6f4dd68a505f97eb55c835
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.org.nvmexpress.boot.poc:bremer.vagrant-nvmet.subsys02
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=38
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-static-ipv4-discovery` & `libnvme-1.9/test/nbft/diffs/NBFT-static-ipv4-discovery`

 * *Files 5% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 subsystem_ns_list[0]->nid=df669a88bd6f4dd68a505f97eb55c835
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.org.nvmexpress.boot.poc:bremer.vagrant-nvmet.subsys02
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=13
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=1
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/diffs/NBFT-static-ipv6` & `libnvme-1.9/test/nbft/diffs/NBFT-static-ipv6`

 * *Files 5% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 subsystem_ns_list[0]->nid=aab2c3c8444c47c599f23632e6364528
 subsystem_ns_list[0]->subsys_nqn=nqn.2022-12.de.suse.mwilck:zeus.vagrant-nvmet.subsys04
 subsystem_ns_list[0]->pdu_header_digest_required=0
 subsystem_ns_list[0]->data_digest_required=0
 subsystem_ns_list[0]->controller_id=9
 subsystem_ns_list[0]->asqsz=0
 subsystem_ns_list[0]->dhcp_root_path_string=(null)
+subsystem_ns_list[0]->discovered=0
+subsystem_ns_list[0]->unavailable=0
```

### Comparing `libnvme-1.8/test/nbft/meson.build` & `libnvme-1.9/test/nbft/meson.build`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     'NBFT-auto-ipv6',
     'NBFT-dhcp-ipv6',
     'NBFT-rhpoc',
     'NBFT-static-ipv4',
     'NBFT-static-ipv4-discovery',
     'NBFT-static-ipv6',
     'NBFT-Dell.PowerEdge.R760',
-    'NBFT-Dell.PowerEdge.R660-fw1.5.5-single'
+    'NBFT-Dell.PowerEdge.R660-fw1.5.5-single',
+    'NBFT-Dell.PowerEdge.R660-fw1.5.5-mpath+discovery',
+    'NBFT-mpath+disc-ipv4+6_half'
 ]
 
 tables_bad = [
     'NBFT-bad-oldspec',
     'NBFT-random-noise',
 ]
```

### Comparing `libnvme-1.8/test/nbft/nbft-dump.c` & `libnvme-1.9/test/nbft/nbft-dump.c`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 		printf("\n");
 		printf("subsystem_ns_list[%u]->subsys_nqn=%s\n", i, (*ssns)->subsys_nqn);
 		printf("subsystem_ns_list[%u]->pdu_header_digest_required=%d\n", i, (*ssns)->pdu_header_digest_required);
 		printf("subsystem_ns_list[%u]->data_digest_required=%d\n", i, (*ssns)->data_digest_required);
 		printf("subsystem_ns_list[%u]->controller_id=%d\n", i, (*ssns)->controller_id);
 		printf("subsystem_ns_list[%u]->asqsz=%d\n", i, (*ssns)->asqsz);
 		printf("subsystem_ns_list[%u]->dhcp_root_path_string=%s\n", i, (*ssns)->dhcp_root_path_string);
+		printf("subsystem_ns_list[%u]->discovered=%d\n", i, (*ssns)->discovered);
+		printf("subsystem_ns_list[%u]->unavailable=%d\n", i, (*ssns)->unavailable);
 	}
 }
 
 int main(int argc, char **argv)
 {
 	struct nbft_info *table = NULL;
```

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-Dell.PowerEdge.R660-fw1.5.5-single` & `libnvme-1.9/test/nbft/tables/NBFT-Dell.PowerEdge.R660-fw1.5.5-single`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-auto-ipv6` & `libnvme-1.9/test/nbft/tables/NBFT-auto-ipv6`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-dhcp-ipv4` & `libnvme-1.9/test/nbft/tables/NBFT-dhcp-ipv4`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-dhcp-ipv6` & `libnvme-1.9/test/nbft/tables/NBFT-dhcp-ipv6`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-rhpoc` & `libnvme-1.9/test/nbft/tables/NBFT-rhpoc`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-static-ipv4` & `libnvme-1.9/test/nbft/tables/NBFT-static-ipv4`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-static-ipv4-discovery` & `libnvme-1.9/test/nbft/tables/NBFT-static-ipv4-discovery`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables/NBFT-static-ipv6` & `libnvme-1.9/test/nbft/tables/NBFT-static-ipv6`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables_bad/NBFT-bad-oldspec` & `libnvme-1.9/test/nbft/tables_bad/NBFT-bad-oldspec`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/nbft/tables_bad/NBFT-random-noise` & `libnvme-1.9/test/nbft/tables_bad/NBFT-random-noise`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/register.c` & `libnvme-1.9/test/register.c`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,21 @@
 	printf("  %-8s : %llx\n", "CQRS", NVME_CAP_CQR(cap));
 	printf("  %-8s : %llx\n", "AMS", NVME_CAP_AMS(cap));
 	printf("  %-8s : %llx\n", "TO", NVME_CAP_TO(cap));
 	printf("  %-8s : %llx\n", "DSTRD", NVME_CAP_DSTRD(cap));
 	printf("  %-8s : %llx\n", "NSSRC", NVME_CAP_NSSRC(cap));
 	printf("  %-8s : %llx\n", "CSS", NVME_CAP_CSS(cap));
 	printf("  %-8s : %llx\n", "BPS", NVME_CAP_BPS(cap));
+	printf("  %-8s : %llx\n", "CPS", NVME_CAP_CPS(cap));
 	printf("  %-8s : %llx\n", "MPSMIN", NVME_CAP_MPSMIN(cap));
 	printf("  %-8s : %llx\n", "MPSMAX", NVME_CAP_MPSMAX(cap));
-	printf("  %-8s : %llx\n", "CMBS", NVME_CAP_CMBS(cap));
 	printf("  %-8s : %llx\n", "PMRS", NVME_CAP_PMRS(cap));
+	printf("  %-8s : %llx\n", "CMBS", NVME_CAP_CMBS(cap));
+	printf("  %-8s : %llx\n", "NSSS", NVME_CAP_NSSS(cap));
+	printf("  %-8s : %llx\n", "CRMS", NVME_CAP_CRMS(cap));
 
 	printf("%-10s : %x\n", "VS", vs);
 	printf("  %-8s : %x\n", "MJR", NVME_VS_TER(vs));
 	printf("  %-8s : %x\n", "MNR", NVME_VS_MNR(vs));
 	printf("  %-8s : %x\n", "TER", NVME_VS_MJR(vs));
 
 	printf("%-10s : %x\n", "INTMS", intms);
@@ -103,14 +106,15 @@
 
 	printf("%-10s : %x\n", "CSTS", csts);
 	printf("  %-8s : %x\n", "RDY", NVME_CSTS_RDY(csts));
 	printf("  %-8s : %x\n", "CFS", NVME_CSTS_CFS(csts));
 	printf("  %-8s : %x\n", "SHST", NVME_CSTS_SHST(csts));
 	printf("  %-8s : %x\n", "NSSRO", NVME_CSTS_NSSRO(csts));
 	printf("  %-8s : %x\n", "PP", NVME_CSTS_PP(csts));
+	printf("  %-8s : %x\n", "ST", NVME_CSTS_ST(csts));
 
 	printf("%-10s : %x\n", "NSSR", nssr);
 
 	printf("%-10s : %x\n", "AQA", aqa);
 	printf("  %-8s : %x\n", "ASQS", NVME_AQA_ASQS(aqa));
 	printf("  %-8s : %x\n", "ACQS", NVME_AQA_ACQS(aqa));
 
@@ -158,15 +162,15 @@
 	printf("  %-8s : %x\n", "CBAI", NVME_CMBSTS_CBAI(cmbsts));
 
 	printf("%-10s : %x\n", "PMRCAP", pmrcap);
 	printf("  %-8s : %x\n", "RDS", NVME_PMRCAP_RDS(pmrcap));
 	printf("  %-8s : %x\n", "WDS", NVME_PMRCAP_WDS(pmrcap));
 	printf("  %-8s : %x\n", "BIR", NVME_PMRCAP_BIR(pmrcap));
 	printf("  %-8s : %x\n", "PMRTU", NVME_PMRCAP_PMRTU(pmrcap));
-	printf("  %-8s : %x\n", "PMRWMB", NVME_PMRCAP_PMRWMB(pmrcap));
+	printf("  %-8s : %x\n", "PMRWBM", NVME_PMRCAP_PMRWBM(pmrcap));
 	printf("  %-8s : %x\n", "PMRTO", NVME_PMRCAP_PMRTO(pmrcap));
 	printf("  %-8s : %x\n", "CMSS", NVME_PMRCAP_CMSS(pmrcap));
 
 	printf("%-10s : %x\n", "PMRCTL", pmrctl);
 	printf("  %-8s : %x\n", "EN", NVME_PMRCTL_EN(pmrctl));
 
 	printf("%-10s : %x\n", "PMRSTS", pmrsts);
```

### Comparing `libnvme-1.8/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.out` & `libnvme-1.9/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.out`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.tar.xz` & `libnvme-1.9/test/sysfs/data/nvme-sysfs-tw-carbon-6.8.0-rc1+.tar.xz`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/test.c` & `libnvme-1.9/test/test.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/tree.c` & `libnvme-1.9/test/tree.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/utils.c` & `libnvme-1.9/test/utils.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/uuid.c` & `libnvme-1.9/test/uuid.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/test/zns.c` & `libnvme-1.9/test/zns.c`

 * *Files identical despite different names*

### Comparing `libnvme-1.8/PKG-INFO` & `libnvme-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libnvme
-Version: 1.8
+Version: 1.9
 Summary: python bindings for libnvme
 Home-page: https://github.com/linux-nvme/libnvme
 Author: Hannes Reinecke
 Author-email: hare@suse.de
 License: LGPL-2.1-or-later
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
```

