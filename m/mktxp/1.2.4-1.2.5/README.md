# Comparing `tmp/mktxp-1.2.4.tar.gz` & `tmp/mktxp-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktxp-1.2.4.tar", last modified: Tue Apr 30 06:06:33 2024, max compression
+gzip compressed data, was "mktxp-1.2.5.tar", last modified: Fri May  3 18:08:46 2024, max compression
```

## Comparing `mktxp-1.2.4.tar` & `mktxp-1.2.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.946256 mktxp-1.2.4/
--rw-r--r--   0 akpower    (501) staff       (20)      543 2024-01-10 19:35:46.000000 mktxp-1.2.4/LICENSE
--rw-r--r--   0 akpower    (501) staff       (20)    23185 2024-04-30 06:06:33.945996 mktxp-1.2.4/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)    21861 2024-04-23 08:51:14.000000 mktxp-1.2.4/README.md
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.924987 mktxp-1.2.4/mktxp/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.926734 mktxp-1.2.4/mktxp/cli/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.927159 mktxp-1.2.4/mktxp/cli/checks/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/checks/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2024-03-09 15:42:11.000000 mktxp-1.2.4/mktxp/cli/checks/chk_pv.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.928130 mktxp-1.2.4/mktxp/cli/config/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/config/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     1681 2024-03-30 06:02:31.000000 mktxp-1.2.4/mktxp/cli/config/_mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)    22620 2024-04-23 06:58:43.000000 mktxp-1.2.4/mktxp/cli/config/config.py
--rw-r--r--   0 akpower    (501) staff       (20)     3294 2024-04-23 08:50:01.000000 mktxp-1.2.4/mktxp/cli/config/mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/dispatch.py
--rwxr-xr-x   0 akpower    (501) staff       (20)    11096 2024-03-17 12:50:04.000000 mktxp-1.2.4/mktxp/cli/options.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.929119 mktxp-1.2.4/mktxp/cli/output/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2583 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/capsman_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2011 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/conn_stats_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2547 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/dhcp_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2908 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/cli/output/wifi_out.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.935779 mktxp-1.2.4/mktxp/collector/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     3096 2024-03-17 08:13:42.000000 mktxp-1.2.4/mktxp/collector/bandwidth_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2804 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/base_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3241 2024-04-01 13:52:18.000000 mktxp-1.2.4/mktxp/collector/bgp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4931 2024-03-02 17:02:01.000000 mktxp-1.2.4/mktxp/collector/capsman_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2039 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/connection_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3134 2024-03-31 06:18:54.000000 mktxp-1.2.4/mktxp/collector/dhcp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4122 2024-04-02 05:59:40.000000 mktxp-1.2.4/mktxp/collector/firewall_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3741 2024-01-22 16:34:51.000000 mktxp-1.2.4/mktxp/collector/health_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1194 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/identity_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3554 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/interface_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1348 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/ipv6_neighbor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3130 2024-04-13 14:04:55.000000 mktxp-1.2.4/mktxp/collector/kid_control_device_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1144 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/mktxp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3528 2024-04-01 15:58:46.000000 mktxp-1.2.4/mktxp/collector/monitor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     5308 2024-04-14 15:37:01.000000 mktxp-1.2.4/mktxp/collector/netwatch_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1272 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/package_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1310 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/poe_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2326 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/pool_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1448 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/public_ip_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4067 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/queue_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4090 2024-04-02 05:43:49.000000 mktxp-1.2.4/mktxp/collector/resource_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2888 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/route_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1216 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/user_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4734 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/collector/wlan_collector.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.942610 mktxp-1.2.4/mktxp/datasource/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2109 2024-04-01 18:08:30.000000 mktxp-1.2.4/mktxp/datasource/base_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1373 2024-04-01 13:40:34.000000 mktxp-1.2.4/mktxp/datasource/bgp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     4754 2024-03-31 15:33:27.000000 mktxp-1.2.4/mktxp/datasource/capsman_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3863 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/connection_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2639 2024-03-31 06:18:54.000000 mktxp-1.2.4/mktxp/datasource/dhcp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3508 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/firewall_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1880 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/health_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1321 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/identity_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3868 2024-04-01 15:55:46.000000 mktxp-1.2.4/mktxp/datasource/interface_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)      962 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/ipv6_neighbor_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1579 2024-04-13 14:02:36.000000 mktxp-1.2.4/mktxp/datasource/kid_control_device_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1169 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/mktxp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1873 2024-04-14 15:36:43.000000 mktxp-1.2.4/mktxp/datasource/netwatch_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1980 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/package_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3150 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/poe_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1987 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/pool_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1211 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/public_ip_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2120 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/queue_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1306 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/route_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2462 2024-01-22 16:34:51.000000 mktxp-1.2.4/mktxp/datasource/routerboard_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2271 2024-04-02 05:45:09.000000 mktxp-1.2.4/mktxp/datasource/system_resource_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1330 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/user_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2457 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/datasource/wireless_ds.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.944219 mktxp-1.2.4/mktxp/flow/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     6046 2024-03-17 08:13:29.000000 mktxp-1.2.4/mktxp/flow/collector_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     4497 2024-03-02 17:07:07.000000 mktxp-1.2.4/mktxp/flow/collector_registry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.944987 mktxp-1.2.4/mktxp/flow/processor/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/processor/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2519 2024-03-17 08:14:01.000000 mktxp-1.2.4/mktxp/flow/processor/base_proc.py
--rw-r--r--   0 akpower    (501) staff       (20)     8303 2024-04-14 09:33:28.000000 mktxp-1.2.4/mktxp/flow/processor/output.py
--rw-r--r--   0 akpower    (501) staff       (20)     5550 2024-04-23 07:00:42.000000 mktxp-1.2.4/mktxp/flow/router_connection.py
--rw-r--r--   0 akpower    (501) staff       (20)     2392 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/flow/router_entries_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     6359 2024-03-02 17:07:56.000000 mktxp-1.2.4/mktxp/flow/router_entry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.945404 mktxp-1.2.4/mktxp/utils/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.4/mktxp/utils/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)    12368 2024-03-28 14:56:49.000000 mktxp-1.2.4/mktxp/utils/utils.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-04-30 06:06:33.926108 mktxp-1.2.4/mktxp.egg-info/
--rw-r--r--   0 akpower    (501) staff       (20)    23185 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)     2630 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/SOURCES.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/dependency_links.txt
--rw-r--r--   0 akpower    (501) staff       (20)       50 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/entry_points.txt
--rw-r--r--   0 akpower    (501) staff       (20)      149 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/requires.txt
--rw-r--r--   0 akpower    (501) staff       (20)        6 2024-04-30 06:06:33.000000 mktxp-1.2.4/mktxp.egg-info/top_level.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2024-02-18 09:03:50.000000 mktxp-1.2.4/mktxp.egg-info/zip-safe
--rw-r--r--   0 akpower    (501) staff       (20)       38 2024-04-30 06:06:33.946330 mktxp-1.2.4/setup.cfg
--rwxr-xr-x   0 akpower    (501) staff       (20)     2623 2024-03-18 14:33:03.000000 mktxp-1.2.4/setup.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.583529 mktxp-1.2.5/
+-rw-r--r--   0 akpower    (501) staff       (20)      543 2024-01-10 19:35:46.000000 mktxp-1.2.5/LICENSE
+-rw-r--r--   0 akpower    (501) staff       (20)    23431 2024-05-03 18:08:46.583217 mktxp-1.2.5/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)    22057 2024-05-03 13:54:22.000000 mktxp-1.2.5/README.md
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.559254 mktxp-1.2.5/mktxp/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.560775 mktxp-1.2.5/mktxp/cli/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.561246 mktxp-1.2.5/mktxp/cli/checks/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/checks/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2024-03-09 15:42:11.000000 mktxp-1.2.5/mktxp/cli/checks/chk_pv.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.562954 mktxp-1.2.5/mktxp/cli/config/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/config/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1681 2024-03-30 06:02:31.000000 mktxp-1.2.5/mktxp/cli/config/_mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)    23046 2024-05-01 12:26:18.000000 mktxp-1.2.5/mktxp/cli/config/config.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3486 2024-05-03 09:42:58.000000 mktxp-1.2.5/mktxp/cli/config/mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/dispatch.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    11096 2024-03-17 12:50:04.000000 mktxp-1.2.5/mktxp/cli/options.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.568015 mktxp-1.2.5/mktxp/cli/output/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/output/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2583 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/output/capsman_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2011 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/output/conn_stats_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2547 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/output/dhcp_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2908 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/cli/output/wifi_out.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.575657 mktxp-1.2.5/mktxp/collector/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3096 2024-03-17 08:13:42.000000 mktxp-1.2.5/mktxp/collector/bandwidth_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2804 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/base_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3236 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/collector/bgp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4931 2024-03-02 17:02:01.000000 mktxp-1.2.5/mktxp/collector/capsman_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2039 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/connection_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3134 2024-03-31 06:18:54.000000 mktxp-1.2.5/mktxp/collector/dhcp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6471 2024-05-01 07:31:54.000000 mktxp-1.2.5/mktxp/collector/firewall_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3741 2024-01-22 16:34:51.000000 mktxp-1.2.5/mktxp/collector/health_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1194 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/identity_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3554 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/interface_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3130 2024-04-13 14:04:55.000000 mktxp-1.2.5/mktxp/collector/kid_control_device_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1144 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/mktxp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4184 2024-04-30 13:52:35.000000 mktxp-1.2.5/mktxp/collector/monitor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1575 2024-05-01 12:47:30.000000 mktxp-1.2.5/mktxp/collector/neighbor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5308 2024-04-14 15:37:01.000000 mktxp-1.2.5/mktxp/collector/netwatch_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1272 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/package_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1310 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/poe_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2781 2024-05-03 13:52:00.000000 mktxp-1.2.5/mktxp/collector/pool_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1448 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/public_ip_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4067 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/queue_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4090 2024-04-02 05:43:49.000000 mktxp-1.2.5/mktxp/collector/resource_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5221 2024-05-02 07:37:34.000000 mktxp-1.2.5/mktxp/collector/route_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1216 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/user_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4734 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/collector/wlan_collector.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.580357 mktxp-1.2.5/mktxp/datasource/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/datasource/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2109 2024-04-01 18:08:30.000000 mktxp-1.2.5/mktxp/datasource/base_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1374 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/bgp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4757 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/capsman_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3865 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/connection_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2640 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/dhcp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3051 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/firewall_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1881 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/health_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1322 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/identity_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3870 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/interface_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1580 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/kid_control_device_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1169 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/datasource/mktxp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1206 2024-05-01 12:46:35.000000 mktxp-1.2.5/mktxp/datasource/neighbor_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1874 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/netwatch_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1982 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/package_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3151 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/poe_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2181 2024-05-03 13:45:03.000000 mktxp-1.2.5/mktxp/datasource/pool_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1212 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/public_ip_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2121 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/queue_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2175 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/route_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2465 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/routerboard_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2273 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/system_resource_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1331 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/user_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2458 2024-05-02 15:39:02.000000 mktxp-1.2.5/mktxp/datasource/wireless_ds.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.581623 mktxp-1.2.5/mktxp/flow/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/flow/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6046 2024-03-17 08:13:29.000000 mktxp-1.2.5/mktxp/flow/collector_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4479 2024-05-01 12:05:22.000000 mktxp-1.2.5/mktxp/flow/collector_registry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.582238 mktxp-1.2.5/mktxp/flow/processor/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/flow/processor/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2519 2024-03-17 08:14:01.000000 mktxp-1.2.5/mktxp/flow/processor/base_proc.py
+-rw-r--r--   0 akpower    (501) staff       (20)     8303 2024-04-14 09:33:28.000000 mktxp-1.2.5/mktxp/flow/processor/output.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5550 2024-04-23 07:00:42.000000 mktxp-1.2.5/mktxp/flow/router_connection.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2392 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/flow/router_entries_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6354 2024-05-01 12:03:42.000000 mktxp-1.2.5/mktxp/flow/router_entry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.582638 mktxp-1.2.5/mktxp/utils/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2024-01-10 19:35:46.000000 mktxp-1.2.5/mktxp/utils/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    12741 2024-05-02 11:02:06.000000 mktxp-1.2.5/mktxp/utils/utils.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2024-05-03 18:08:46.560155 mktxp-1.2.5/mktxp.egg-info/
+-rw-r--r--   0 akpower    (501) staff       (20)    23431 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)     2620 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/SOURCES.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/dependency_links.txt
+-rw-r--r--   0 akpower    (501) staff       (20)       50 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/entry_points.txt
+-rw-r--r--   0 akpower    (501) staff       (20)      149 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/requires.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        6 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/top_level.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2024-05-03 18:08:46.000000 mktxp-1.2.5/mktxp.egg-info/zip-safe
+-rw-r--r--   0 akpower    (501) staff       (20)       38 2024-05-03 18:08:46.583576 mktxp-1.2.5/setup.cfg
+-rwxr-xr-x   0 akpower    (501) staff       (20)     2671 2024-05-01 13:10:06.000000 mktxp-1.2.5/setup.py
```

### Comparing `mktxp-1.2.4/LICENSE` & `mktxp-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/PKG-INFO` & `mktxp-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2.4
+Version: 1.2.5
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Customer Service
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: prometheus-client>=0.9.0
-Requires-Dist: RouterOS-api>=0.17.0
+Requires-Dist: RouterOS-api>=0.18.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: humanize>=3.2.0
 Requires-Dist: texttable>=1.6.3
 Requires-Dist: speedtest-cli>=2.1.2
 Requires-Dist: waitress>=3.0.0
 Requires-Dist: packaging>=24.0
 
@@ -90,16 +91,16 @@
 
 [Sample-Router-2]
     # for specific configuration on the router level, overload the defaults here
     hostname = 192.168.88.2
 
 [default]
     # this affects configuration of all routers, unless overloaded on their specific levels
+    
     enabled = True          # turns metrics collection for this RouterOS device on / off
-
     hostname = localhost    # RouterOS IP address
     port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
@@ -110,26 +111,30 @@
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
 
-    pool = True                     # Pool metrics
     interface = True                # Interfaces traffic metrics
     
+    route = True                    # IPv4 Routes metrics
+    pool = True                     # IPv4 Pool metrics
     firewall = True                 # IPv4 Firewall rules traffic metrics
+    neighbor = True                 # IPv4 Reachable Neighbors
+
+    ipv6_route = False              # IPv6 Routes metrics    
+    ipv6_pool = False               # IPv6 Pool metrics
     ipv6_firewall = False           # IPv6 Firewall rules traffic metrics
-    ipv6_neighbor = False           # Reachable IPv6 Neighbors
+    ipv6_neighbor = False           # IPv6 Reachable Neighbors
 
     poe = True                      # POE metrics
     monitor = True                  # Interface monitor metrics
     netwatch = True                 # Netwatch metrics
     public_ip = True                # Public IP metrics
-    route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
     kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
     kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
```

### Comparing `mktxp-1.2.4/README.md` & `mktxp-1.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 [Sample-Router-2]
     # for specific configuration on the router level, overload the defaults here
     hostname = 192.168.88.2
 
 [default]
     # this affects configuration of all routers, unless overloaded on their specific levels
+    
     enabled = True          # turns metrics collection for this RouterOS device on / off
-
     hostname = localhost    # RouterOS IP address
     port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
@@ -76,26 +76,30 @@
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
 
-    pool = True                     # Pool metrics
     interface = True                # Interfaces traffic metrics
     
+    route = True                    # IPv4 Routes metrics
+    pool = True                     # IPv4 Pool metrics
     firewall = True                 # IPv4 Firewall rules traffic metrics
+    neighbor = True                 # IPv4 Reachable Neighbors
+
+    ipv6_route = False              # IPv6 Routes metrics    
+    ipv6_pool = False               # IPv6 Pool metrics
     ipv6_firewall = False           # IPv6 Firewall rules traffic metrics
-    ipv6_neighbor = False           # Reachable IPv6 Neighbors
+    ipv6_neighbor = False           # IPv6 Reachable Neighbors
 
     poe = True                      # POE metrics
     monitor = True                  # Interface monitor metrics
     netwatch = True                 # Netwatch metrics
     public_ip = True                # Public IP metrics
-    route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
     kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
     kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
```

### Comparing `mktxp-1.2.4/mktxp/cli/checks/chk_pv.py` & `mktxp-1.2.5/mktxp/cli/checks/chk_pv.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/config/_mktxp.conf` & `mktxp-1.2.5/mktxp/cli/config/_mktxp.conf`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/config/config.py` & `mktxp-1.2.5/mktxp/cli/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 '''
 
 class CollectorKeys:
     IDENTITY_COLLECTOR = 'IdentityCollector'
     SYSTEM_RESOURCE_COLLECTOR = 'SystemResourceCollector'
     HEALTH_COLLECTOR = 'HealthCollector'
     PUBLIC_IP_ADDRESS_COLLECTOR = 'PublicIPAddressCollector'
-    IPV6_NEIGHBOR_COLLECTOR = 'IPv6NeighborCollector'
+    NEIGHBOR_COLLECTOR = 'NeighborCollector'
     PACKAGE_COLLECTOR = 'PackageCollector'
     DHCP_COLLECTOR = 'DHCPCollector'
     POOL_COLLECTOR = 'PoolCollector'
     IP_CONNECTION_COLLECTOR = 'IPConnectionCollector'
     INTERFACE_COLLECTOR = 'InterfaceCollector'
     FIREWALL_COLLECTOR = 'FirewallCollector'
     MONITOR_COLLECTOR = 'MonitorCollector'
@@ -65,25 +65,29 @@
     NO_SSL_CERTIFICATE = 'no_ssl_certificate'
     SSL_CERTIFICATE_VERIFY = 'ssl_certificate_verify'
     PLAINTEXT_LOGIN_KEY = 'plaintext_login'
 
     FE_PACKAGE_KEY = 'installed_packages'
     FE_DHCP_KEY = 'dhcp'
     FE_DHCP_LEASE_KEY = 'dhcp_lease'
-    FE_DHCP_POOL_KEY = 'pool'
     FE_IP_CONNECTIONS_KEY = 'connections'
     FE_CONNECTION_STATS_KEY = 'connection_stats'
     FE_INTERFACE_KEY = 'interface'
+
+    FE_ROUTE_KEY = 'route'
+    FE_DHCP_POOL_KEY = 'pool'
     FE_FIREWALL_KEY = 'firewall'
+    FE_NEIGHBOR_KEY = 'neighbor'
 
+    FE_IPV6_ROUTE_KEY = 'ipv6_route'
+    FE_IPV6_DHCP_POOL_KEY = 'ipv6_pool'
     FE_IPV6_FIREWALL_KEY = 'ipv6_firewall'
     FE_IPV6_NEIGHBOR_KEY = 'ipv6_neighbor'
 
     FE_MONITOR_KEY = 'monitor'
-    FE_ROUTE_KEY = 'route'
     FE_WIRELESS_KEY = 'wireless'
     FE_WIRELESS_CLIENTS_KEY = 'wireless_clients'
     FE_CAPSMAN_KEY = 'capsman'
     FE_CAPSMAN_CLIENTS_KEY = 'capsman_clients'
     FE_POE_KEY = 'poe'
     FE_PUBLIC_IP_KEY = 'public_ip'
     FE_NETWATCH_KEY = 'netwatch'
@@ -139,19 +143,19 @@
     DEFAULT_MKTXP_MIN_COLLECT_INTERVAL = 5
     DEFAULT_MKTXP_MAX_WORKER_THREADS = 5
     DEFAULT_MKTXP_MAX_SCRAPE_DURATION = 10
     DEFAULT_MKTXP_TOTAL_MAX_SCRAPE_DURATION = 30
 
 
     BOOLEAN_KEYS_NO = {ENABLED_KEY, SSL_KEY, NO_SSL_CERTIFICATE, FE_CHECK_FOR_UPDATES, FE_KID_CONTROL_DEVICE, FE_KID_CONTROL_DYNAMIC,
-                       SSL_CERTIFICATE_VERIFY, FE_IPV6_FIREWALL_KEY, FE_IPV6_NEIGHBOR_KEY, FE_CONNECTION_STATS_KEY, FE_BGP_KEY}
+                       SSL_CERTIFICATE_VERIFY, FE_IPV6_ROUTE_KEY, FE_IPV6_DHCP_POOL_KEY, FE_IPV6_FIREWALL_KEY, FE_IPV6_NEIGHBOR_KEY, FE_CONNECTION_STATS_KEY, FE_BGP_KEY}
 
     # Feature keys enabled by default
-    BOOLEAN_KEYS_YES = {PLAINTEXT_LOGIN_KEY, FE_DHCP_KEY, FE_PACKAGE_KEY, FE_DHCP_LEASE_KEY, FE_DHCP_POOL_KEY, FE_IP_CONNECTIONS_KEY, FE_INTERFACE_KEY, 
-                        FE_FIREWALL_KEY, FE_MONITOR_KEY, FE_ROUTE_KEY, MKTXP_USE_COMMENTS_OVER_NAMES,
+    BOOLEAN_KEYS_YES = {PLAINTEXT_LOGIN_KEY, FE_DHCP_KEY, FE_PACKAGE_KEY, FE_DHCP_LEASE_KEY, FE_IP_CONNECTIONS_KEY, FE_INTERFACE_KEY, 
+                        FE_ROUTE_KEY, FE_DHCP_POOL_KEY, FE_FIREWALL_KEY, FE_NEIGHBOR_KEY, FE_MONITOR_KEY, MKTXP_USE_COMMENTS_OVER_NAMES,
                         FE_WIRELESS_KEY, FE_WIRELESS_CLIENTS_KEY, FE_CAPSMAN_KEY, FE_CAPSMAN_CLIENTS_KEY, FE_POE_KEY,
                         FE_NETWATCH_KEY, FE_PUBLIC_IP_KEY, FE_USER_KEY, FE_QUEUE_KEY}
 
     SYSTEM_BOOLEAN_KEYS_YES = set()
     SYSTEM_BOOLEAN_KEYS_NO = {MKTXP_BANDWIDTH_KEY, MKTXP_VERBOSE_MODE, MKTXP_FETCH_IN_PARALLEL, MKTXP_COMPACT_CONFIG}
 
     STR_KEYS = (HOST_KEY, USER_KEY, PASSWD_KEY, FE_REMOTE_DHCP_ENTRY)
@@ -165,18 +169,20 @@
     MKTXP_CONFIG_ENTRY_NAME = 'MKTXP'
 
 
 class ConfigEntry:
     MKTXPConfigEntry = namedtuple('MKTXPConfigEntry', [MKTXPConfigKeys.ENABLED_KEY, MKTXPConfigKeys.HOST_KEY, MKTXPConfigKeys.PORT_KEY,
                                                        MKTXPConfigKeys.USER_KEY, MKTXPConfigKeys.PASSWD_KEY,
                                                        MKTXPConfigKeys.SSL_KEY, MKTXPConfigKeys.NO_SSL_CERTIFICATE, MKTXPConfigKeys.SSL_CERTIFICATE_VERIFY, MKTXPConfigKeys.PLAINTEXT_LOGIN_KEY,
-                                                       MKTXPConfigKeys.FE_DHCP_KEY, MKTXPConfigKeys.FE_PACKAGE_KEY, MKTXPConfigKeys.FE_DHCP_LEASE_KEY, MKTXPConfigKeys.FE_DHCP_POOL_KEY, MKTXPConfigKeys.FE_INTERFACE_KEY,
-                                                       MKTXPConfigKeys.FE_FIREWALL_KEY, MKTXPConfigKeys.FE_MONITOR_KEY, MKTXPConfigKeys.FE_ROUTE_KEY, MKTXPConfigKeys.FE_WIRELESS_KEY, MKTXPConfigKeys.FE_WIRELESS_CLIENTS_KEY,
+                                                       MKTXPConfigKeys.FE_DHCP_KEY, MKTXPConfigKeys.FE_PACKAGE_KEY, MKTXPConfigKeys.FE_DHCP_LEASE_KEY, MKTXPConfigKeys.FE_INTERFACE_KEY,
+                                                       MKTXPConfigKeys.FE_MONITOR_KEY, MKTXPConfigKeys.FE_WIRELESS_KEY, MKTXPConfigKeys.FE_WIRELESS_CLIENTS_KEY,
                                                        MKTXPConfigKeys.FE_IP_CONNECTIONS_KEY, MKTXPConfigKeys.FE_CONNECTION_STATS_KEY, MKTXPConfigKeys.FE_CAPSMAN_KEY, MKTXPConfigKeys.FE_CAPSMAN_CLIENTS_KEY, MKTXPConfigKeys.FE_POE_KEY, 
-                                                       MKTXPConfigKeys.FE_NETWATCH_KEY, MKTXPConfigKeys.MKTXP_USE_COMMENTS_OVER_NAMES, MKTXPConfigKeys.FE_PUBLIC_IP_KEY, MKTXPConfigKeys.FE_IPV6_FIREWALL_KEY, MKTXPConfigKeys.FE_IPV6_NEIGHBOR_KEY,
+                                                       MKTXPConfigKeys.FE_NETWATCH_KEY, MKTXPConfigKeys.MKTXP_USE_COMMENTS_OVER_NAMES, MKTXPConfigKeys.FE_PUBLIC_IP_KEY, 
+                                                       MKTXPConfigKeys.FE_ROUTE_KEY, MKTXPConfigKeys.FE_DHCP_POOL_KEY, MKTXPConfigKeys.FE_FIREWALL_KEY, MKTXPConfigKeys.FE_NEIGHBOR_KEY,
+                                                       MKTXPConfigKeys.FE_IPV6_ROUTE_KEY, MKTXPConfigKeys.FE_IPV6_DHCP_POOL_KEY, MKTXPConfigKeys.FE_IPV6_FIREWALL_KEY, MKTXPConfigKeys.FE_IPV6_NEIGHBOR_KEY,                                               
                                                        MKTXPConfigKeys.FE_USER_KEY, MKTXPConfigKeys.FE_QUEUE_KEY, MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY, MKTXPConfigKeys.FE_CHECK_FOR_UPDATES, MKTXPConfigKeys.FE_BGP_KEY,
                                                        MKTXPConfigKeys.FE_KID_CONTROL_DEVICE, MKTXPConfigKeys.FE_KID_CONTROL_DYNAMIC
                                                        ])
     MKTXPSystemEntry = namedtuple('MKTXPSystemEntry', [MKTXPConfigKeys.PORT_KEY, MKTXPConfigKeys.LISTEN_KEY, MKTXPConfigKeys.MKTXP_SOCKET_TIMEOUT,
                                                        MKTXPConfigKeys.MKTXP_INITIAL_DELAY, MKTXPConfigKeys.MKTXP_MAX_DELAY,
                                                        MKTXPConfigKeys.MKTXP_INC_DIV, MKTXPConfigKeys.MKTXP_BANDWIDTH_KEY,
                                                        MKTXPConfigKeys.MKTXP_VERBOSE_MODE, MKTXPConfigKeys.MKTXP_BANDWIDTH_TEST_INTERVAL,
```

### Comparing `mktxp-1.2.4/mktxp/cli/config/mktxp.conf` & `mktxp-1.2.5/mktxp/cli/config/mktxp.conf`

 * *Files 12% similar despite different names*

```diff
@@ -33,26 +33,30 @@
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
 
-    pool = True                     # Pool metrics
     interface = True                # Interfaces traffic metrics
     
+    route = True                    # IPv4 Routes metrics
+    pool = True                     # IPv4 Pool metrics
     firewall = True                 # IPv4 Firewall rules traffic metrics
+    neighbor = True                 # IPv4 Reachable Neighbors
+
+    ipv6_route = False              # IPv6 Routes metrics    
+    ipv6_pool = False               # IPv6 Pool metrics
     ipv6_firewall = False           # IPv6 Firewall rules traffic metrics
-    ipv6_neighbor = False           # Reachable IPv6 Neighbors
+    ipv6_neighbor = False           # IPv6 Reachable Neighbors
 
     poe = True                      # POE metrics
     monitor = True                  # Interface monitor metrics
     netwatch = True                 # Netwatch metrics
     public_ip = True                # Public IP metrics
-    route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
     kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
     kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
```

### Comparing `mktxp-1.2.4/mktxp/cli/dispatch.py` & `mktxp-1.2.5/mktxp/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/options.py` & `mktxp-1.2.5/mktxp/cli/options.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/output/capsman_out.py` & `mktxp-1.2.5/mktxp/cli/output/capsman_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/output/conn_stats_out.py` & `mktxp-1.2.5/mktxp/cli/output/conn_stats_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/output/dhcp_out.py` & `mktxp-1.2.5/mktxp/cli/output/dhcp_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/cli/output/wifi_out.py` & `mktxp-1.2.5/mktxp/cli/output/wifi_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/bandwidth_collector.py` & `mktxp-1.2.5/mktxp/collector/bandwidth_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/base_collector.py` & `mktxp-1.2.5/mktxp/collector/base_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/bgp_collector.py` & `mktxp-1.2.5/mktxp/collector/bgp_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 'established': lambda value: '1' if value=='true' else '0',
                 'uptime': lambda value: BaseOutputProcessor.parse_timedelta_milliseconds(value) if value else '0'
                 }
         bgp_records = BGPMetricsDataSource.metric_records(router_entry, metric_labels=bgp_labels, translation_table = translation_table)
         
         if bgp_records:
             session_info_labes = ['name', 'remote_address', 'remote_as', 'local_as', 'remote_afi', 'local_afi']
-            bgp_sessions_metrics = BaseCollector.info_collector('bgp_sessions_info', 'BGP sessions info', bgp_records, session_info_labes)
+            bgp_sessions_metrics = BaseCollector.info_collector('bgp_sessions', 'BGP sessions info', bgp_records, session_info_labes)
             yield bgp_sessions_metrics
 
             session_id_labes = ['name']
             remote_messages_metrics = BaseCollector.counter_collector('bgp_remote_messages', 'Number of remote messages', bgp_records, 'remote_messages', session_id_labes)
             yield remote_messages_metrics
```

### Comparing `mktxp-1.2.4/mktxp/collector/capsman_collector.py` & `mktxp-1.2.5/mktxp/collector/capsman_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/connection_collector.py` & `mktxp-1.2.5/mktxp/collector/connection_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/dhcp_collector.py` & `mktxp-1.2.5/mktxp/collector/dhcp_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/health_collector.py` & `mktxp-1.2.5/mktxp/collector/health_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/identity_collector.py` & `mktxp-1.2.5/mktxp/collector/identity_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/interface_collector.py` & `mktxp-1.2.5/mktxp/collector/interface_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/ipv6_neighbor_collector.py` & `mktxp-1.2.5/mktxp/collector/user_collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 # coding=utf8
-# Copyright (c) 2020 Arseniy Kuznetsov
+## Copyright (c) 2020 Arseniy Kuznetsov
 ##
-# This program is free software; you can redistribute it and/or
-# modify it under the terms of the GNU General Public License
-# as published by the Free Software Foundation; either version 2
-# of the License, or (at your option) any later version.
+## This program is free software; you can redistribute it and/or
+## modify it under the terms of the GNU General Public License
+## as published by the Free Software Foundation; either version 2
+## of the License, or (at your option) any later version.
 ##
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+## This program is distributed in the hope that it will be useful,
+## but WITHOUT ANY WARRANTY; without even the implied warranty of
+## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+## GNU General Public License for more details.
 
 
 from mktxp.collector.base_collector import BaseCollector
-from mktxp.datasource.ipv6_neighbor_ds import IPv6NeighborDataSource
+from mktxp.datasource.user_ds import UserMetricsDataSource
 
 
-class IPv6NeighborCollector(BaseCollector):
-    '''IPv6 Neighbor Collector'''
+class UserCollector(BaseCollector):
+    '''Active Users collector'''
     @staticmethod
     def collect(router_entry):
-        if not router_entry.config_entry.ipv6_neighbor:
+        if not router_entry.config_entry.installed_packages:
             return
-            
-        metric_labels = ['address', 'interface', 'mac_address', 'status']
 
-        records = IPv6NeighborDataSource.metric_records(
-            router_entry,
-            metric_labels=metric_labels
-        )
-
-        metrics = BaseCollector.gauge_collector(
-            'ipv6_neighbor_info',
-            'Reachable IPv6 neighbors',
-            records,
-            'ipv6_neighbor',
-            metric_labels=metric_labels
-        )
-        yield metrics
+        user_labels = ['name', 'when', 'address', 'via', 'group']
+        user_records = UserMetricsDataSource.metric_records(router_entry, metric_labels=user_labels)
+        if user_records:
+            user_metrics = BaseCollector.info_collector('active_users', 'Active Users', user_records, user_labels)
+            yield user_metrics
+
```

### Comparing `mktxp-1.2.4/mktxp/collector/kid_control_device_collector.py` & `mktxp-1.2.5/mktxp/collector/kid_control_device_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/mktxp_collector.py` & `mktxp-1.2.5/mktxp/collector/mktxp_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/monitor_collector.py` & `mktxp-1.2.5/mktxp/collector/monitor_collector.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,21 @@
     ''' Ethernet Interface Monitor Metrics collector
     '''    
     @staticmethod
     def collect(router_entry):
         if not router_entry.config_entry.monitor:
             return
 
-        monitor_labels = ['status', 'rate', 'full_duplex', 'name', 'sfp_temperature']
+        monitor_labels = ['status', 'rate', 'full_duplex', 'name', 'sfp_temperature', 'sfp_module_present', 'sfp_wavelength', 'sfp_tx_power', 'sfp_rx_power']
         translation_table = {
                 'status': lambda value: '1' if value=='link-ok' else '0',
                 'rate': lambda value: MonitorCollector._rates(value) if value else '0',
                 'full_duplex': lambda value: '1' if value=='true' else '0',
                 'name': lambda value: value if value else '',
+                'sfp_module_present': lambda value: '1' if value=='true' else '0',
                 'sfp_temperature': lambda value: value if value else '0'
                 }
         monitor_records = InterfaceMonitorMetricsDataSource.metric_records(router_entry, metric_labels = monitor_labels, 
                                                                                         translation_table=translation_table, include_comments = True)   
         if monitor_records:
             monitor_status_metrics = BaseCollector.gauge_collector('interface_status', 'Current interface link status', monitor_records, 'status', ['name'])
             yield monitor_status_metrics
@@ -44,16 +45,21 @@
             monitor_rates_metrics = BaseCollector.gauge_collector('interface_rate', 'Actual interface connection data rate', rate_records, 'rate', ['name'])
             yield monitor_rates_metrics
 
             full_duplex_records = [monitor_record for monitor_record in monitor_records if monitor_record.get('full_duplex', None)]
             monitor_rates_metrics = BaseCollector.gauge_collector('interface_full_duplex', 'Full duplex data transmission', full_duplex_records, 'full_duplex', ['name'])
             yield monitor_rates_metrics
 
-            sfp_temperature_metrics = BaseCollector.gauge_collector('interface_sfp_temperature', 'Current SFP temperature', monitor_records, 'sfp_temperature', ['name'])
-            yield sfp_temperature_metrics
+            sfp_metrics = [record for record in monitor_records if int(record.get("sfp_module_present"))]
+            if sfp_metrics:
+                yield BaseCollector.gauge_collector('interface_sfp_temperature', 'Current SFP Temperature', sfp_metrics, 'sfp_temperature', ['name'])
+                yield BaseCollector.gauge_collector('interface_sfp_wavelength', 'Current SFP Wavelength',sfp_metrics, 'sfp_wavelength', ['name'])
+                yield BaseCollector.gauge_collector('interface_sfp_tx_power', 'Current SFP TX Power', sfp_metrics, 'sfp_tx_power', ['name'])
+                yield BaseCollector.gauge_collector('interface_sfp_rx_power', 'Current SFP RX Power', sfp_metrics, 'sfp_rx_power', ['name'])
+
 
     @staticmethod
     def _rates(rate_option):
         # according mikrotik docs, an interface rate should be one of these
         rate_value =  {
                 '10Mbps': '10',
                 '100Mbps': '100',
```

### Comparing `mktxp-1.2.4/mktxp/collector/netwatch_collector.py` & `mktxp-1.2.5/mktxp/collector/netwatch_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/package_collector.py` & `mktxp-1.2.5/mktxp/collector/package_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/poe_collector.py` & `mktxp-1.2.5/mktxp/collector/poe_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/public_ip_collector.py` & `mktxp-1.2.5/mktxp/collector/public_ip_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/queue_collector.py` & `mktxp-1.2.5/mktxp/collector/queue_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/resource_collector.py` & `mktxp-1.2.5/mktxp/collector/resource_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/collector/user_collector.py` & `mktxp-1.2.5/mktxp/datasource/mktxp_ds.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,24 +8,22 @@
 ##
 ## This program is distributed in the hope that it will be useful,
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
-from mktxp.collector.base_collector import BaseCollector
-from mktxp.datasource.user_ds import UserMetricsDataSource
+from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class UserCollector(BaseCollector):
-    '''Active Users collector'''
+class MKTXPMetricsDataSource:
+    ''' MKTXP Metrics data provider
+    '''             
     @staticmethod
-    def collect(router_entry):
-        if not router_entry.config_entry.installed_packages:
-            return
-
-        user_labels = ['name', 'when', 'address', 'via', 'group']
-        user_records = UserMetricsDataSource.metric_records(router_entry, metric_labels=user_labels)
-        if user_records:
-            user_metrics = BaseCollector.info_collector('active_users', 'Active Users', user_records, user_labels)
-            yield user_metrics
-
+    def metric_records(router_entry):
+        mktxp_records = []
+        for key in router_entry.time_spent.keys():
+            mktxp_records.append({'name': key, 'duration': router_entry.time_spent[key]})           
+
+        # translation rules            
+        translation_table = {'duration': lambda d: d*1000}
+        return BaseDSProcessor.trimmed_records(router_entry, router_records = mktxp_records, translation_table = translation_table)
```

### Comparing `mktxp-1.2.4/mktxp/collector/wlan_collector.py` & `mktxp-1.2.5/mktxp/collector/wlan_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/datasource/base_ds.py` & `mktxp-1.2.5/mktxp/datasource/base_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/datasource/bgp_ds.py` & `mktxp-1.2.5/mktxp/datasource/bgp_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     def metric_records(router_entry, *, metric_labels = None, translation_table = None):
         if metric_labels is None:
             metric_labels = []                
         try:
             bgp_records = router_entry.api_connection.router_api().get_resource('/routing/bgp/session').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = bgp_records, metric_labels = metric_labels, translation_table = translation_table)
         except Exception as exc:
-            print(f'Error getting BGP sessions info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting BGP sessions info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/capsman_ds.py` & `mktxp-1.2.5/mktxp/datasource/capsman_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             metric_labels = []                
         try:
             remote_caps_records = []
             for capsman_path in CapsmanInfo.capsman_paths(router_entry):
                 remote_caps_records.extend(router_entry.api_connection.router_api().get_resource(f'{capsman_path}/remote-cap').get())
             return BaseDSProcessor.trimmed_records(router_entry, router_records = remote_caps_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting CAPsMAN remote caps info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting CAPsMAN remote caps info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 class CapsmanRegistrationsMetricsDataSource:
     ''' Capsman Registrations Metrics data provider
     '''             
     @staticmethod
@@ -71,15 +71,15 @@
             # For backward compatibility, including both variants
             for record in registration_table_records:
                 if 'signal' in record:
                     record['rx-signal'] = record['signal']
 
             return BaseDSProcessor.trimmed_records(router_entry, router_records = registration_table_records, metric_labels = metric_labels, add_router_id = add_router_id)
         except Exception as exc:
-            print(f'Error getting CAPsMAN registration table info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting CAPsMAN registration table info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 class CapsmanInterfacesDatasource:
     ''' Data provider for CAPsMaN interfaces
     '''
     @staticmethod
@@ -88,9 +88,9 @@
             return None            
         if metric_labels is None:
             metric_labels = []                
         try:
             caps_interfaces = router_entry.api_connection.router_api().get_resource('/caps-man/interface').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = caps_interfaces, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting CAPsMAN interfaces info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting CAPsMAN interfaces info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/connection_ds.py` & `mktxp-1.2.5/mktxp/datasource/connection_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             # answer looks and feels like an empty list: [], but it has a special attribute `done_message`
             done_message = answer.done_message
             # `done_msg` is a dict with the return code as a key - which is the count that we are looking for
             cnt = done_message['ret'].decode()
             records = [{'count': cnt}]
             return BaseDSProcessor.trimmed_records(router_entry, router_records = records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting IP connection info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting IP connection info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 class IPConnectionStatsDatasource:
     ''' IP connections stats data provider
     '''             
     @staticmethod
@@ -66,12 +66,12 @@
                 record = {'src_address': key, 'connection_count': entry.count, 'dst_addresses': ', '.join(entry.destinations)}
                 if add_router_id: 
                     for router_key, router_value in router_entry.router_id.items():
                         record[router_key] = router_value
                 records.append(record)
             return records 
         except Exception as exc:
-            print(f'Error getting IP connection stats info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting IP connection stats info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 ConnStatsEntry = namedtuple('ConnStatsEntry', ['count', 'destinations'])
```

### Comparing `mktxp-1.2.4/mktxp/datasource/dhcp_ds.py` & `mktxp-1.2.5/mktxp/datasource/dhcp_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 
             records = BaseDSProcessor.trimmed_records(router_entry, router_records = dhcp_lease_records, metric_labels = metric_labels, add_router_id = add_router_id, translation_table = translation_table)
             if dhcp_cache:
                 router_entry.dhcp_records = records
             return records
 
         except Exception as exc:
-            print(f'Error getting dhcp info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting dhcp info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/health_ds.py` & `mktxp-1.2.5/mktxp/datasource/health_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,9 +32,9 @@
                     # Otherwise it is not possible to get the value by name (e.g. records['voltage'])
                     name = record['name']
                     val = record.get('value', None)
                     record[name] = val
 
             return BaseDSProcessor.trimmed_records(router_entry, router_records = health_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting system health info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system health info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/identity_ds.py` & `mktxp-1.2.5/mktxp/datasource/identity_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
             identity_records = router_entry.api_connection.router_api().get_resource('/system/identity').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = identity_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting system identity info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system identity info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/interface_ds.py` & `mktxp-1.2.5/mktxp/datasource/interface_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
             traffic_records = router_entry.api_connection.router_api().get_resource('/interface').get(running='yes', disabled='no')
             return BaseDSProcessor.trimmed_records(router_entry, router_records = traffic_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting interface traffic info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting interface traffic info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 class InterfaceMonitorMetricsDataSource:
     ''' Interface Monitor Metrics data provider
     '''             
     @staticmethod
@@ -58,10 +58,10 @@
             # With wifiwave2, Mikrotik renamed the field 'registered-clients' to 'registered-peers'
             # For backward compatibility, including both variants
             for interface_monitor_record in interface_monitor_records:
                 if 'registered-peers' in interface_monitor_record:
                     interface_monitor_record['registered-clients'] = interface_monitor_record['registered-peers']
             return BaseDSProcessor.trimmed_records(router_entry, router_records = interface_monitor_records, metric_labels = metric_labels, translation_table=translation_table)
         except Exception as exc:
-            print(f'Error getting {kind} interface monitor info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting {kind} interface monitor info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/ipv6_neighbor_ds.py` & `mktxp-1.2.5/mktxp/datasource/neighbor_ds.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,13 +11,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class IPv6NeighborDataSource:
+class NeighborDataSource:
+    def metric_records(router_entry, metric_labels, ipv6=False):    
+        
+        metric_labels = metric_labels or []                        
+        router_records = []        
+        
+        if ipv6:
+            router_records = router_entry.api_connection.router_api().get_resource(f'/ipv6/neighbor').get(status='reachable')
+        else:
+            router_records = router_entry.api_connection.router_api().get_resource(f'/ip/neighbor').get()
 
-    def metric_records(router_entry, metric_labels):
-        metric_labels = metric_labels or []
-        records = router_entry.api_connection.router_api().get_resource('/ipv6/neighbor').get(status='reachable')
-        return BaseDSProcessor.trimmed_records(router_entry, router_records=records, metric_labels=metric_labels, )
+        return BaseDSProcessor.trimmed_records(router_entry, router_records=router_records, metric_labels=metric_labels)
```

### Comparing `mktxp-1.2.4/mktxp/datasource/kid_control_device_ds.py` & `mktxp-1.2.5/mktxp/datasource/kid_control_device_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,9 @@
             records = router_entry.api_connection.router_api().get_resource('/ip/kid-control/device').get()
             for record in records:
                 if record.get('user') or router_entry.config_entry.kid_control_dynamic:
                     device_records.append(record)
             return BaseDSProcessor.trimmed_records(router_entry, router_records=device_records, metric_labels=metric_labels, translation_table=translation_table)
         except Exception as exc:
             print(
-                f'Error getting Kid-control device info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+                f'Error getting Kid-control device info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/netwatch_ds.py` & `mktxp-1.2.5/mktxp/datasource/netwatch_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,10 +31,10 @@
                     if comment:
                         netwatch_record['name'] = f'{host} ({comment[0:20]})' if not router_entry.config_entry.use_comments_over_names else comment
                     else:
                         netwatch_record['name'] = host
 
             return BaseDSProcessor.trimmed_records(router_entry, router_records = netwatch_records, translation_table = translation_table, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting Netwatch info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting Netwatch info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/package_ds.py` & `mktxp-1.2.5/mktxp/datasource/package_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     def metric_records(router_entry, *, metric_labels = None, add_router_id = True):
         if metric_labels is None:
             metric_labels = []                
         try:
             package_records = router_entry.api_connection.router_api().get_resource('/system/package').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = package_records, metric_labels = metric_labels, add_router_id = add_router_id)
         except Exception as exc:
-            print(f'Error getting installed packages info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting installed packages info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
     @staticmethod
     def is_package_installed (router_entry, package_name = None):
         if package_name:
             try:
                 package_records = router_entry.api_connection.router_api().get_resource('/system/package').get()
                 for package_record in package_records:
                     if package_record['name'] == package_name:
                         return True
             except Exception as exc:
-                print(f'Error getting installed packages info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')        
+                print(f'Error getting installed packages info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')        
         return False
```

### Comparing `mktxp-1.2.4/mktxp/datasource/poe_ds.py` & `mktxp-1.2.5/mktxp/datasource/poe_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
                     comment = [comment_fn(interface) for interface in interfaces if interface['name'] == poe_record['name']][0]       
                     if comment:
                         # combines name with comment
                         poe_record['name'] = comment if router_entry.config_entry.use_comments_over_names else \
                                                                                                     f"{poe_record['name']} ({comment})"                                
             return BaseDSProcessor.trimmed_records(router_entry, router_records = poe_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting PoE info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting PoE info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/pool_ds.py` & `mktxp-1.2.5/mktxp/datasource/pool_ds.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,31 +15,33 @@
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
 class PoolMetricsDataSource:
     ''' Pool Metrics data provider
     '''             
     @staticmethod
-    def metric_records(router_entry, *, metric_labels = None):
+    def metric_records(router_entry, *, metric_labels = None, ipv6 = False):
+        ip_stack = 'ipv6' if ipv6 else 'ip'
         if metric_labels is None:
             metric_labels = []                
         try:
-            pool_records = router_entry.api_connection.router_api().get_resource('/ip/pool').get()
+            pool_records = router_entry.api_connection.router_api().get_resource(f'/{ip_stack}/pool').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = pool_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting pool info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting {"IPv6" if ipv6 else "IPv4"} pool info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
 
 class PoolUsedMetricsDataSource:
     ''' Pool/Used Metrics data provider
     '''             
     @staticmethod
-    def metric_records(router_entry, *, metric_labels = None):
+    def metric_records(router_entry, *, metric_labels = None, ipv6 = False):
+        ip_stack = 'ipv6' if ipv6 else 'ip'
         if metric_labels is None:
             metric_labels = []                
         try:
-            pool_used_records = router_entry.api_connection.router_api().get_resource('/ip/pool/used').get()
+            pool_used_records = router_entry.api_connection.router_api().get_resource(f'/{ip_stack}/pool/used').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = pool_used_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting pool used info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting {"IPv6" if ipv6 else "IPv4"} pool used info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/public_ip_ds.py` & `mktxp-1.2.5/mktxp/datasource/public_ip_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,9 @@
         if metric_labels is None:
             metric_labels = []
 
         try:
             records = router_entry.api_connection.router_api().get_resource('/ip/cloud/').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records=records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error public IP address info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error public IP address info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/queue_ds.py` & `mktxp-1.2.5/mktxp/datasource/queue_ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def metric_records(router_entry, *, metric_labels = None, kind = 'tree'):
         if metric_labels is None:
             metric_labels = []                
         try:
             queue_records = router_entry.api_connection.router_api().get_resource(f'/queue/{kind}/').get()
             queue_records = BaseDSProcessor.trimmed_records(router_entry, router_records = queue_records, metric_labels = metric_labels)            
         except Exception as exc:
-            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system resource info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
         if kind == 'tree':            
             return queue_records
 
         # simple queue records need splitting upload/download values
         splitted_queue_records = []
```

### Comparing `mktxp-1.2.4/mktxp/datasource/route_ds.py` & `mktxp-1.2.5/mktxp/datasource/user_ds.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
 
 
-class RouteMetricsDataSource:
-    ''' Routes Metrics data provider
+class UserMetricsDataSource:
+    ''' Active Users Metrics data provider
     '''             
-    @staticmethod
+    @staticmethod    
     def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
-            route_records = router_entry.api_connection.router_api().get_resource('/ip/route').get(active='yes')
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = route_records, metric_labels = metric_labels)
+            active_users_records = router_entry.api_connection.router_api().get_resource('/user/active/').get()
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = active_users_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting routes info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system resource info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/routerboard_ds.py` & `mktxp-1.2.5/mktxp/datasource/routerboard_ds.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,32 @@
     def metric_records(router_entry, *, metric_labels = None):
         if metric_labels is None:
             metric_labels = []                
         try:
             routerboard_records = router_entry.api_connection.router_api().get_resource('/system/routerboard').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = routerboard_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting system routerboard info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system routerboard info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
     @staticmethod
     def firmware_version(router_entry):
         try:
             version_st = router_entry.api_connection.router_api().get_resource('/system/routerboard').call('print', {'proplist':'current-firmware'})[0]
             if version_st.get('current-firmware'):
                 return version_st['current-firmware']
             return None
         except Exception as exc:
-            print(f'Error getting routerboard current-firmware from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting routerboard current-firmware from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
     @staticmethod
     def firmware_upgrade_version(router_entry):
         try:
             version_st = router_entry.api_connection.router_api().get_resource('/system/routerboard').call('print', {'proplist':'upgrade-firmware'})[0]
             if version_st.get('upgrade-firmware'):
                 return version_st['upgrade-firmware']
             return None
         except Exception as exc:
-            print(f'Error getting routerboard upgrade-firmware from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting routerboard upgrade-firmware from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
```

### Comparing `mktxp-1.2.4/mktxp/datasource/system_resource_ds.py` & `mktxp-1.2.5/mktxp/datasource/system_resource_ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     def metric_records(router_entry, *, metric_labels = None, translation_table=None):
         if metric_labels is None:
             metric_labels = []                
         try:
             system_resource_records = router_entry.api_connection.router_api().get_resource('/system/resource').get()
             return BaseDSProcessor.trimmed_records(router_entry, router_records = system_resource_records, metric_labels = metric_labels, translation_table=translation_table)
         except Exception as exc:
-            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system resource info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
     @staticmethod
     def os_version(router_entry):
         try:
             system_version_records = router_entry.api_connection.router_api().get_resource('/system/resource').call('print', {'proplist':'version'})
             for record in system_version_records:
                 ver = record.get('version', None)
                 if ver:
                     return ver
                     
             return None
         except Exception as exc:
-            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting system resource info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
         return False
     
     @staticmethod
     def has_builtin_wifi_capsman(router_entry):
         ver = SystemResourceMetricsDataSource.os_version(router_entry)
         return builtin_wifi_capsman_version(ver)
```

### Comparing `mktxp-1.2.4/mktxp/datasource/user_ds.py` & `mktxp-1.2.5/mktxp/datasource/route_ds.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,40 @@
 ## This program is distributed in the hope that it will be useful,
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.datasource.base_ds import BaseDSProcessor
+from mktxp.utils.utils import str2bool
 
-
-class UserMetricsDataSource:
-    ''' Active Users Metrics data provider
+class RouteMetricsDataSource:
+    ''' Routes Metrics data provider
     '''             
-    @staticmethod    
-    def metric_records(router_entry, *, metric_labels = None):
+    @staticmethod
+    def metric_records(router_entry, *, metric_labels = None, ipv6 = False):
+        ip_stack = 'ipv6' if ipv6 else 'ip'
         if metric_labels is None:
             metric_labels = []                
         try:
-            active_users_records = router_entry.api_connection.router_api().get_resource('/user/active/').get()
-            return BaseDSProcessor.trimmed_records(router_entry, router_records = active_users_records, metric_labels = metric_labels)
+            #route_records = router_entry.api_connection.router_api().get_resource(f'/{ip_stack}/route').get(active='yes')
+            route_records = router_entry.api_connection.router_api().get_resource(f'/{ip_stack}/route').call('print', {'proplist':'active,connect,dynamic,static,bgp,ospf'})            
+            
+            #active_records = [record for record in route_records if record.get('active')]
+            RouteMetricsDataSource._remove_from_list_of_dict(route_records, 'active')
+
+            return BaseDSProcessor.trimmed_records(router_entry, router_records = route_records, metric_labels = metric_labels)
         except Exception as exc:
-            print(f'Error getting system resource info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting {"IPv6" if ipv6 else "IPv4"} routes info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
+
+    # helpers
+    @staticmethod
+    def _remove_from_list_of_dict(dict_list, key):
+        indexes = []
+        for index, dict in enumerate(dict_list):
+            if not str2bool(dict.get(key)):
+                indexes.append(index)
+        offset = 0
+        for index in indexes:
+            dict_list.pop(index-offset)
+            offset += 1
```

### Comparing `mktxp-1.2.4/mktxp/datasource/wireless_ds.py` & `mktxp-1.2.5/mktxp/datasource/wireless_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             # For backward compatibility, including both variants
             for record in registration_table_records:
                 if 'signal' in record:
                     record['signal-strength'] = record['signal']
 
             return BaseDSProcessor.trimmed_records(router_entry, router_records = registration_table_records, metric_labels = metric_labels, add_router_id = add_router_id,)
         except Exception as exc:
-            print(f'Error getting wireless registration table info from router{router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
+            print(f'Error getting wireless registration table info from router {router_entry.router_name}@{router_entry.config_entry.hostname}: {exc}')
             return None
 
     @staticmethod
     def wireless_package(router_entry):
         if router_entry.wireless_type in (RouterEntryWirelessType.DUAL, RouterEntryWirelessType.WIRELESS):
             return WirelessMetricsDataSource.WIRELESS
         elif router_entry.wireless_type == RouterEntryWirelessType.WIFIWAVE2:
```

### Comparing `mktxp-1.2.4/mktxp/flow/collector_handler.py` & `mktxp-1.2.5/mktxp/flow/collector_handler.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/flow/collector_registry.py` & `mktxp-1.2.5/mktxp/flow/collector_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from mktxp.collector.dhcp_collector import DHCPCollector
 from mktxp.collector.package_collector import PackageCollector
 from mktxp.collector.connection_collector import IPConnectionCollector
 from mktxp.collector.interface_collector import InterfaceCollector
 from mktxp.collector.health_collector import HealthCollector
 from mktxp.collector.identity_collector import IdentityCollector
 from mktxp.collector.public_ip_collector import PublicIPAddressCollector
-from mktxp.collector.ipv6_neighbor_collector import IPv6NeighborCollector
+from mktxp.collector.neighbor_collector import NeighborCollector
 from mktxp.collector.monitor_collector import MonitorCollector
 from mktxp.collector.poe_collector import POECollector
 from mktxp.collector.netwatch_collector import NetwatchCollector
 from mktxp.collector.pool_collector import PoolCollector
 from mktxp.collector.resource_collector import SystemResourceCollector
 from mktxp.collector.route_collector import RouteCollector
 from mktxp.collector.wlan_collector import WLANCollector
@@ -49,15 +49,15 @@
         self.bandwidthCollector = BandwidthCollector()
 
         self.register(CollectorKeys.IDENTITY_COLLECTOR, IdentityCollector.collect)
         self.register(CollectorKeys.SYSTEM_RESOURCE_COLLECTOR, SystemResourceCollector.collect)
         self.register(CollectorKeys.HEALTH_COLLECTOR, HealthCollector.collect)
         self.register(CollectorKeys.PUBLIC_IP_ADDRESS_COLLECTOR, PublicIPAddressCollector.collect)
 
-        self.register(CollectorKeys.IPV6_NEIGHBOR_COLLECTOR, IPv6NeighborCollector.collect)
+        self.register(CollectorKeys.NEIGHBOR_COLLECTOR, NeighborCollector.collect)
 
         self.register(CollectorKeys.PACKAGE_COLLECTOR, PackageCollector.collect)
         self.register(CollectorKeys.DHCP_COLLECTOR, DHCPCollector.collect)
         self.register(CollectorKeys.IP_CONNECTION_COLLECTOR, IPConnectionCollector.collect)
         self.register(CollectorKeys.POOL_COLLECTOR, PoolCollector.collect)
         self.register(CollectorKeys.INTERFACE_COLLECTOR, InterfaceCollector.collect)
```

### Comparing `mktxp-1.2.4/mktxp/flow/processor/base_proc.py` & `mktxp-1.2.5/mktxp/flow/processor/base_proc.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/flow/processor/output.py` & `mktxp-1.2.5/mktxp/flow/processor/output.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/flow/router_connection.py` & `mktxp-1.2.5/mktxp/flow/router_connection.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/flow/router_entries_handler.py` & `mktxp-1.2.5/mktxp/flow/router_entries_handler.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2.4/mktxp/flow/router_entry.py` & `mktxp-1.2.5/mktxp/flow/router_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             MKTXPConfigKeys.ROUTERBOARD_ADDRESS: self.config_entry.hostname
             }
         
         self.time_spent =  { CollectorKeys.IDENTITY_COLLECTOR: 0,
                             CollectorKeys.SYSTEM_RESOURCE_COLLECTOR: 0,
                             CollectorKeys.HEALTH_COLLECTOR: 0,
                             CollectorKeys.PUBLIC_IP_ADDRESS_COLLECTOR: 0,
-                            CollectorKeys.IPV6_NEIGHBOR_COLLECTOR: 0,
+                            CollectorKeys.NEIGHBOR_COLLECTOR: 0,
                             CollectorKeys.PACKAGE_COLLECTOR: 0,
                             CollectorKeys.DHCP_COLLECTOR: 0,
                             CollectorKeys.POOL_COLLECTOR: 0,
                             CollectorKeys.IP_CONNECTION_COLLECTOR: 0,
                             CollectorKeys.INTERFACE_COLLECTOR: 0,
                             CollectorKeys.FIREWALL_COLLECTOR: 0,
                             CollectorKeys.MONITOR_COLLECTOR: 0,
```

### Comparing `mktxp-1.2.4/mktxp/utils/utils.py` & `mktxp-1.2.5/mktxp/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,25 @@
         return -1
 
 def parse_mkt_uptime(time):
     time_dict = re.match(r'((?P<weeks>\d+)w)?((?P<days>\d+)d)?((?P<hours>\d+)h)?((?P<minutes>\d+)m)?((?P<seconds>\d+)s)?', time).groupdict()
     delta = timedelta(**{key: int(value) for key, value in time_dict.items() if value}).total_seconds() 
     return int(delta) if delta else 0
 
+def str2bool(str_value):
+    if not str_value or not type(str_value) is str:
+        return False
+    str_value = str_value.lower()
+    if str_value in ('y', 'yes', 't', 'true', 'on', '1'):
+        return True
+    elif str_value in ('n', 'no', 'f', 'false', 'off', '0'):
+        return False
+    else:
+        raise ValueError(f'Invalid truth value: {str_value}')
+        
 class FSHelper:
     ''' File System ops helper
     '''
     @staticmethod
     def full_path(path, check_parent_path = False):
         ''' Full path
         '''
```

### Comparing `mktxp-1.2.4/mktxp.egg-info/PKG-INFO` & `mktxp-1.2.5/mktxp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2.4
+Version: 1.2.5
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Customer Service
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: prometheus-client>=0.9.0
-Requires-Dist: RouterOS-api>=0.17.0
+Requires-Dist: RouterOS-api>=0.18.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: humanize>=3.2.0
 Requires-Dist: texttable>=1.6.3
 Requires-Dist: speedtest-cli>=2.1.2
 Requires-Dist: waitress>=3.0.0
 Requires-Dist: packaging>=24.0
 
@@ -90,16 +91,16 @@
 
 [Sample-Router-2]
     # for specific configuration on the router level, overload the defaults here
     hostname = 192.168.88.2
 
 [default]
     # this affects configuration of all routers, unless overloaded on their specific levels
+    
     enabled = True          # turns metrics collection for this RouterOS device on / off
-
     hostname = localhost    # RouterOS IP address
     port = 8728             # RouterOS IP Port
     
     username = username     # RouterOS user, needs to have 'read' and 'api' permissions
     password = password
     
     use_ssl = False                 # enables connection via API-SSL servis
@@ -110,26 +111,30 @@
     installed_packages = True       # Installed packages
     dhcp = True                     # DHCP general metrics
     dhcp_lease = True               # DHCP lease metrics
 
     connections = True              # IP connections metrics
     connection_stats = False        # Open IP connections metrics 
 
-    pool = True                     # Pool metrics
     interface = True                # Interfaces traffic metrics
     
+    route = True                    # IPv4 Routes metrics
+    pool = True                     # IPv4 Pool metrics
     firewall = True                 # IPv4 Firewall rules traffic metrics
+    neighbor = True                 # IPv4 Reachable Neighbors
+
+    ipv6_route = False              # IPv6 Routes metrics    
+    ipv6_pool = False               # IPv6 Pool metrics
     ipv6_firewall = False           # IPv6 Firewall rules traffic metrics
-    ipv6_neighbor = False           # Reachable IPv6 Neighbors
+    ipv6_neighbor = False           # IPv6 Reachable Neighbors
 
     poe = True                      # POE metrics
     monitor = True                  # Interface monitor metrics
     netwatch = True                 # Netwatch metrics
     public_ip = True                # Public IP metrics
-    route = True                    # Routes metrics
     wireless = True                 # WLAN general metrics
     wireless_clients = True         # WLAN clients metrics
     capsman = True                  # CAPsMAN general metrics
     capsman_clients = True          # CAPsMAN clients metrics    
 
     kid_control_assigned = False    # Allow Kid Control metrics for connected devices with assigned users
     kid_control_dynamic = False     # Allow Kid Control metrics for all connected devices, including those without assigned user
```

### Comparing `mktxp-1.2.4/mktxp.egg-info/SOURCES.txt` & `mktxp-1.2.5/mktxp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 mktxp/collector/capsman_collector.py
 mktxp/collector/connection_collector.py
 mktxp/collector/dhcp_collector.py
 mktxp/collector/firewall_collector.py
 mktxp/collector/health_collector.py
 mktxp/collector/identity_collector.py
 mktxp/collector/interface_collector.py
-mktxp/collector/ipv6_neighbor_collector.py
 mktxp/collector/kid_control_device_collector.py
 mktxp/collector/mktxp_collector.py
 mktxp/collector/monitor_collector.py
+mktxp/collector/neighbor_collector.py
 mktxp/collector/netwatch_collector.py
 mktxp/collector/package_collector.py
 mktxp/collector/poe_collector.py
 mktxp/collector/pool_collector.py
 mktxp/collector/public_ip_collector.py
 mktxp/collector/queue_collector.py
 mktxp/collector/resource_collector.py
@@ -54,17 +54,17 @@
 mktxp/datasource/capsman_ds.py
 mktxp/datasource/connection_ds.py
 mktxp/datasource/dhcp_ds.py
 mktxp/datasource/firewall_ds.py
 mktxp/datasource/health_ds.py
 mktxp/datasource/identity_ds.py
 mktxp/datasource/interface_ds.py
-mktxp/datasource/ipv6_neighbor_ds.py
 mktxp/datasource/kid_control_device_ds.py
 mktxp/datasource/mktxp_ds.py
+mktxp/datasource/neighbor_ds.py
 mktxp/datasource/netwatch_ds.py
 mktxp/datasource/package_ds.py
 mktxp/datasource/poe_ds.py
 mktxp/datasource/pool_ds.py
 mktxp/datasource/public_ip_ds.py
 mktxp/datasource/queue_ds.py
 mktxp/datasource/route_ds.py
```

### Comparing `mktxp-1.2.4/setup.py` & `mktxp-1.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # read the README.md contents
 pkg_dir = path.abspath(path.dirname(__file__))
 with open(path.join(pkg_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mktxp',
-    version='1.2.4',
+    version='1.2.5',
 
     url='https://github.com/akpw/mktxp',
 
     author='Arseniy Kuznetsov',
     author_email='k.arseniy@gmail.com',
 
     long_description=long_description,
@@ -40,15 +40,15 @@
     package_data = {
         '': ['config/*.conf'],
     },
 
     keywords = 'Mikrotik RouterOS Prometheus Exporter',
 
     install_requires = ['prometheus-client>=0.9.0', 
-                        'RouterOS-api>=0.17.0', 
+                        'RouterOS-api>=0.18.0',
                         'configobj>=5.0.6',
                         'humanize>=3.2.0',
                         'texttable>=1.6.3',
                         'speedtest-cli>=2.1.2',
                         'waitress>=3.0.0',
                         'packaging>=24.0'
                         ],
@@ -66,14 +66,15 @@
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3 :: Only',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Information Technology',
+        'Intended Audience :: Customer Service',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: BSD :: FreeBSD',
         'Operating System :: POSIX :: Linux',
         'Topic :: System',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities'
     ]
```

