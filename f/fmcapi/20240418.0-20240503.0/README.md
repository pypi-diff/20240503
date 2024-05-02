# Comparing `tmp/fmcapi-20240418.0.tar.gz` & `tmp/fmcapi-20240503.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fmcapi-20240418.0.tar", last modified: Wed Apr 17 20:32:02 2024, max compression
+gzip compressed data, was "dist/fmcapi-20240503.0.tar", last modified: Thu May  2 22:55:38 2024, max compression
```

## Comparing `fmcapi-20240418.0.tar` & `fmcapi-20240503.0.tar`

### file list

```diff
@@ -1,264 +1,264 @@
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:02.000000 fmcapi-20240418.0/
--rw-r--r--   0 marksullivan   (501) staff       (20)     1504 2020-02-10 11:18:14.000000 fmcapi-20240418.0/LICENSE.md
--rw-r--r--   0 marksullivan   (501) staff       (20)     1644 2024-04-17 20:32:02.000000 fmcapi-20240418.0/PKG-INFO
--rw-r--r--   0 marksullivan   (501) staff       (20)     3624 2022-08-06 10:51:39.000000 fmcapi-20240418.0/README.md
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/
--rw-r--r--   0 marksullivan   (501) staff       (20)      782 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/__init__.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/
--rw-r--r--   0 marksullivan   (501) staff       (20)     8447 2024-04-17 20:28:04.000000 fmcapi-20240418.0/fmcapi/api_objects/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    19199 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/apiclasstemplate.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/audit_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      172 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/audit_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2863 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/audit_services/audit_records.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/backup_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      155 2023-09-19 10:03:52.000000 fmcapi-20240418.0/fmcapi/api_objects/backup_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2558 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/backup_services/backup.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/deployment_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      269 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/deployment_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2167 2023-09-19 09:45:43.000000 fmcapi-20240418.0/fmcapi/api_objects/deployment_services/deployabledevices.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2687 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/deployment_services/deploymentrequests.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/device_clusters/
--rw-r--r--   0 marksullivan   (501) staff       (20)      184 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_clusters/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1582 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_clusters/ftddevicecluster.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/device_group_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      209 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_group_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4593 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_group_services/devicegrouprecords.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      413 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4571 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/failoverinterfacemacaddressconfigs.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4776 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/ftddevicehapairs.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2687 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/monitoredinterfaces.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      778 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6008 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/bridgegroupinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/copyconfigrequests.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    10265 2024-03-27 22:42:09.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/devicerecords.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     8265 2021-12-14 09:40:31.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/etherchannelinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/fpinterfacestatistics.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/fplogicalinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/fpphysicalinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/inlinesets.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       47 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/interfaceevents.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     7606 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/ipv4staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6888 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/ipv6staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6039 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/physicalinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6793 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/redundantinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2132 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6887 2021-12-14 09:40:31.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/subinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/virtualswitches.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      100 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/device_services/vlaninterfaces.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/health/
--rw-r--r--   0 marksullivan   (501) staff       (20)      169 2024-01-16 00:41:10.000000 fmcapi-20240418.0/fmcapi/api_objects/health/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1610 2024-01-16 00:41:10.000000 fmcapi-20240418.0/fmcapi/api_objects/health/terminateravpnsessions.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     5042 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/helper_functions.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      117 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/cloudeventsconfigs.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       50 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/cloudregions.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/externallookups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/integration_services/packetanalyzerdevices.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      118 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/collections.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/discoveryinfo.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/element.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/incident.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/indicator.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/observable.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/settings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/intelligence_services/source.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)     3490 2024-04-17 20:28:04.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1508 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/anyprotocolportobjects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1385 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationcategories.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1456 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationfilters.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1460 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationproductivities.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1330 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationrisks.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1420 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applications.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1322 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationtags.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1280 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationtypes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1266 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/certenrollments.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1352 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/continents.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1340 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/countries.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2479 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/dnsservergroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     9669 2024-01-16 00:41:10.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/dynamicobjectmappings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      993 2023-12-11 03:04:13.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/dynamicobjects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1425 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/endpointdevicetypes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3504 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/extendedaccesslist.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2717 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/fqdns.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1340 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/geolocation.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1326 2024-03-27 22:42:09.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/grouppolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1891 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/hosts.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1151 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/icmpv4objects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1128 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/icmpv6objects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1172 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev1ipsecproposals.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2228 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev1policies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4979 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev2ipsecproposals.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     7404 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev2policies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3794 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/interfacegroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1015 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/interfaceobjects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1372 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/isesecuritygrouptags.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/keychain.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1502 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/networkaddresses.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     7210 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/networkgroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1860 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/networks.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3479 2023-11-30 09:39:58.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/portobjectgroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1265 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ports.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      951 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/protocolportobjects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1848 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/ranges.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1157 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/realms.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1339 2022-08-06 10:51:39.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/realmusergroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1228 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/realmusers.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1326 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/securitygrouptags.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1284 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/securityzones.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1351 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/siurlfeeds.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1235 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/siurllists.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2131 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/slamonitors.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      900 2024-04-17 20:30:46.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/timeranges.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1234 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/tunneltags.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1300 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/urlcategories.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     5048 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/urlgroups.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      840 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/urls.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      877 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/usage.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1245 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/variablesets.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     5610 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/vlangrouptags.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1413 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/object_services/vlantags.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_assignment_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      211 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_assignment_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4403 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_assignment_services/policyassignments.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)     1416 2024-03-27 22:37:20.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2282 2023-09-19 09:45:43.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/accesspolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    69801 2024-01-29 21:05:24.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/accessrules.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1750 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/advancedsettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     9740 2023-12-11 03:04:13.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/autonatrules.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3860 2023-09-19 09:45:43.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/categories.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1648 2024-03-27 22:42:09.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/connectionprofiles.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4192 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/defaultactions.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4159 2024-03-27 22:42:09.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/dynamicaccesspolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     7934 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/endpoints.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1231 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/filepolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      884 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/ftdnatpolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1141 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/ftds2svpns.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    11558 2022-09-14 07:10:21.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/hitcounts.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4268 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/ikesettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4743 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/inheritancesettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1344 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/intrusionpolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     5187 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/ipsecsettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4989 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/loggingsettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    16631 2023-11-13 05:46:03.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/manualnatrules.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2754 2022-09-14 07:10:21.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/natrules.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2362 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/prefilterpolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    25207 2024-04-16 20:35:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/prefilterrules.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1754 2024-03-27 22:42:09.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/ravpns.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       27 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/policy_services/snmpalerts.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/search/
--rw-r--r--   0 marksullivan   (501) staff       (20)      253 2022-09-14 07:10:21.000000 fmcapi-20240418.0/fmcapi/api_objects/search/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      863 2022-09-14 07:10:21.000000 fmcapi-20240418.0/fmcapi/api_objects/search/globalsearch.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      945 2022-09-14 07:16:40.000000 fmcapi-20240418.0/fmcapi/api_objects/search/object.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      852 2022-09-14 07:10:21.000000 fmcapi-20240418.0/fmcapi/api_objects/search/policy.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/status_services/
--rw-r--r--   0 marksullivan   (501) staff       (20)      173 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/status_services/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1308 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/status_services/taskstatuses.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/system_information/
--rw-r--r--   0 marksullivan   (501) staff       (20)      182 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/system_information/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)       47 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/system_information/domain.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2115 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/system_information/serverversion.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi/api_objects/update_packages/
--rw-r--r--   0 marksullivan   (501) staff       (20)      328 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/update_packages/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2510 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/update_packages/listapplicabledevices.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3516 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/update_packages/upgradepackage.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1268 2021-12-14 09:40:27.000000 fmcapi-20240418.0/fmcapi/api_objects/update_packages/upgradepackages.py
--rw-r--r--   0 marksullivan   (501) staff       (20)    18251 2024-01-09 23:42:54.000000 fmcapi-20240418.0/fmcapi/fmc.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:01.000000 fmcapi-20240418.0/fmcapi.egg-info/
--rw-r--r--   0 marksullivan   (501) staff       (20)     1644 2024-04-17 20:32:00.000000 fmcapi-20240418.0/fmcapi.egg-info/PKG-INFO
--rw-r--r--   0 marksullivan   (501) staff       (20)    10285 2024-04-17 20:32:00.000000 fmcapi-20240418.0/fmcapi.egg-info/SOURCES.txt
--rw-r--r--   0 marksullivan   (501) staff       (20)        1 2024-04-17 20:32:00.000000 fmcapi-20240418.0/fmcapi.egg-info/dependency_links.txt
--rw-r--r--   0 marksullivan   (501) staff       (20)       38 2024-04-17 20:32:00.000000 fmcapi-20240418.0/fmcapi.egg-info/requires.txt
--rw-r--r--   0 marksullivan   (501) staff       (20)       18 2024-04-17 20:32:00.000000 fmcapi-20240418.0/fmcapi.egg-info/top_level.txt
--rw-r--r--   0 marksullivan   (501) staff       (20)       99 2023-09-19 09:45:43.000000 fmcapi-20240418.0/pyproject.toml
--rw-r--r--   0 marksullivan   (501) staff       (20)       91 2024-04-17 20:32:02.000000 fmcapi-20240418.0/setup.cfg
--rw-r--r--   0 marksullivan   (501) staff       (20)     1960 2024-04-17 20:30:46.000000 fmcapi-20240418.0/setup.py
-drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-04-17 20:32:02.000000 fmcapi-20240418.0/unit_tests/
--rw-r--r--   0 marksullivan   (501) staff       (20)     5946 2024-04-17 20:28:04.000000 fmcapi-20240418.0/unit_tests/__init__.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      950 2023-11-13 05:40:27.000000 fmcapi-20240418.0/unit_tests/acls_extended.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      555 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/acp.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     4809 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/acprule.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      530 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      597 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_category.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      507 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_filter.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      601 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_productivity.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      521 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_risk.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      525 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_tag.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      517 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/application_type.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      235 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/audit_records.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     3546 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/autonat.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      509 2023-09-19 10:03:52.000000 fmcapi-20240418.0/unit_tests/backup.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      405 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/certificate_enrollment.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1131 2024-03-27 22:37:20.000000 fmcapi-20240418.0/unit_tests/connectionprofiles.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      527 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/continent.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      467 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/country.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      256 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/deployable_devices.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      260 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/deployment_requests.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2032 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/device_with_task.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      899 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/devicegrouprecords.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1379 2024-03-27 22:37:20.000000 fmcapi-20240418.0/unit_tests/devicerecords.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      624 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/dns_servers_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      460 2024-01-16 00:36:24.000000 fmcapi-20240418.0/unit_tests/dynamic_object_mappings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      546 2023-12-11 03:01:22.000000 fmcapi-20240418.0/unit_tests/dynamic_objects.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2024 2024-03-27 22:37:20.000000 fmcapi-20240418.0/unit_tests/dynamicaccesspolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      958 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/failoverinterfacemacaddressconfigs.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      367 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/file_policies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      505 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/fqdns.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2746 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ftddevicehapairs.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      519 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/geolocations.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1160 2024-03-27 22:37:20.000000 fmcapi-20240418.0/unit_tests/grouppolicies.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      207 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/helper_functions.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1887 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/hit_counts.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      484 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/icmpv4.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      484 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/icmpv6.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1008 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ikev1.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2703 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ikev2.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1488 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interface_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1150 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interfaces_bridge_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1296 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interfaces_etherchannel.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1820 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interfaces_physical.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1244 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interfaces_redundant.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1122 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/interfaces_subinterfaces.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      364 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/intrusion_policy.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      325 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ip_addresses.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      529 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ip_host.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      551 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ip_network.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      549 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ip_range.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1368 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ipv4staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1373 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ipv6staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1794 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/loggingsettings.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     5794 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/manualnat.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      586 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/monitored_interface.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1538 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/network_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2455 2023-11-13 05:40:27.000000 fmcapi-20240418.0/unit_tests/objects_get_query_filters.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1589 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/port_object_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      313 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/ports.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      552 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/prefilter.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     6617 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/prefilter_rule.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      589 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/protocol_port.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1062 2024-03-27 22:37:20.000000 fmcapi-20240418.0/unit_tests/ravpn.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     2761 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/s2s_vpn.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      307 2022-09-14 07:10:21.000000 fmcapi-20240418.0/unit_tests/search_globalsearch.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      283 2022-09-14 07:10:21.000000 fmcapi-20240418.0/unit_tests/search_object.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      283 2022-09-14 07:10:21.000000 fmcapi-20240418.0/unit_tests/search_policy.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      571 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/security_zone.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      317 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/server_version.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1174 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/sla_monitor.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      439 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/staticroutes.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1192 2024-01-09 23:42:50.000000 fmcapi-20240418.0/unit_tests/terminateravpnsessions.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      640 2024-04-17 20:28:04.000000 fmcapi-20240418.0/unit_tests/timeranges.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1330 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/upgrades.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      512 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/url.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      495 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/url_category.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1475 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/url_group.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      509 2023-11-13 05:40:27.000000 fmcapi-20240418.0/unit_tests/usage.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      325 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/variable_set.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1753 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/vlan_group_tag.py
--rw-r--r--   0 marksullivan   (501) staff       (20)      583 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/vlan_tag.py
--rw-r--r--   0 marksullivan   (501) staff       (20)     1985 2021-12-14 09:40:27.000000 fmcapi-20240418.0/unit_tests/wait_for_task.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:38.000000 fmcapi-20240503.0/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1504 2020-02-10 11:18:14.000000 fmcapi-20240503.0/LICENSE.md
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1644 2024-05-02 22:55:38.000000 fmcapi-20240503.0/PKG-INFO
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3624 2024-04-28 04:40:54.000000 fmcapi-20240503.0/README.md
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      782 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/__init__.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     8447 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    19199 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/apiclasstemplate.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/audit_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      172 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/audit_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2863 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/audit_services/audit_records.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/backup_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      155 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/backup_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2558 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/backup_services/backup.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/deployment_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      269 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/deployment_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2167 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/deployment_services/deployabledevices.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2673 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/deployment_services/deploymentrequests.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/device_clusters/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      184 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_clusters/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1582 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_clusters/ftddevicecluster.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/device_group_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      209 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_group_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4593 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_group_services/devicegrouprecords.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      413 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4571 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/failoverinterfacemacaddressconfigs.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4776 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/ftddevicehapairs.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2687 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/monitoredinterfaces.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      778 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     6008 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/bridgegroupinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/copyconfigrequests.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    10265 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/devicerecords.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     8265 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/etherchannelinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/fpinterfacestatistics.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/fplogicalinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/fpphysicalinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/inlinesets.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       47 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/interfaceevents.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     8149 2024-05-02 22:51:34.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/ipv4staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     7431 2024-05-02 22:54:24.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/ipv6staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     6039 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/physicalinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     6793 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/redundantinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2132 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     6887 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/subinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/virtualswitches.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      100 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/device_services/vlaninterfaces.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/health/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      169 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/health/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1610 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/health/terminateravpnsessions.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5042 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/helper_functions.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      117 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/cloudeventsconfigs.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       50 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/cloudregions.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/externallookups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/integration_services/packetanalyzerdevices.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      118 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/collections.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/discoveryinfo.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/element.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/incident.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/indicator.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/observable.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/settings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/intelligence_services/source.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3490 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1508 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/anyprotocolportobjects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1385 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationcategories.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1456 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationfilters.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1460 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationproductivities.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1330 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationrisks.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1420 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applications.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1322 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationtags.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1280 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationtypes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1266 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/certenrollments.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1352 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/continents.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1340 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/countries.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2479 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/dnsservergroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     9669 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/dynamicobjectmappings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      993 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/dynamicobjects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1425 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/endpointdevicetypes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3504 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/extendedaccesslist.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2717 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/fqdns.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1340 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/geolocation.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1326 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/grouppolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1891 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/hosts.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1151 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/icmpv4objects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1128 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/icmpv6objects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1172 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev1ipsecproposals.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2228 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev1policies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4979 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev2ipsecproposals.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     7404 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev2policies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3794 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/interfacegroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1015 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/interfaceobjects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1372 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/isesecuritygrouptags.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/keychain.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1502 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/networkaddresses.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     7210 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/networkgroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1860 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/networks.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3479 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/portobjectgroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1265 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ports.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      951 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/protocolportobjects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1848 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/ranges.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1157 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/realms.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1339 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/realmusergroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1228 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/realmusers.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1326 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/securitygrouptags.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1284 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/securityzones.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1351 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/siurlfeeds.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1235 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/siurllists.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2131 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/slamonitors.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      900 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/timeranges.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1234 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/tunneltags.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1300 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/urlcategories.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5048 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/urlgroups.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      840 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/urls.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      877 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/usage.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1245 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/variablesets.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5610 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/vlangrouptags.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1413 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/object_services/vlantags.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_assignment_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      211 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_assignment_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4403 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_assignment_services/policyassignments.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1416 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2282 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/accesspolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    69801 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/accessrules.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1750 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/advancedsettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     9740 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/autonatrules.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3860 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/categories.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1648 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/connectionprofiles.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4192 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/defaultactions.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4159 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/dynamicaccesspolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     7934 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/endpoints.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1231 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/filepolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      884 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/ftdnatpolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1141 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/ftds2svpns.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    11558 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/hitcounts.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4268 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/ikesettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4743 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/inheritancesettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1344 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/intrusionpolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5187 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/ipsecsettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4989 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/loggingsettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    16631 2024-04-28 05:00:25.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/manualnatrules.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2754 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/natrules.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2362 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/prefilterpolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    25207 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/prefilterrules.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1754 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/ravpns.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       27 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/policy_services/snmpalerts.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/search/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      253 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/search/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      863 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/search/globalsearch.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      945 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/search/object.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      852 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/search/policy.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/status_services/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      173 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/status_services/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1308 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/status_services/taskstatuses.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/system_information/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      182 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/system_information/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)       47 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/system_information/domain.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2115 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/system_information/serverversion.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:37.000000 fmcapi-20240503.0/fmcapi/api_objects/update_packages/
+-rw-r--r--   0 marksullivan   (501) staff       (20)      328 2024-04-28 04:40:54.000000 fmcapi-20240503.0/fmcapi/api_objects/update_packages/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2510 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/update_packages/listapplicabledevices.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3660 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/api_objects/update_packages/upgradepackage.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1268 2021-12-14 09:40:27.000000 fmcapi-20240503.0/fmcapi/api_objects/update_packages/upgradepackages.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)    18251 2024-04-28 05:09:35.000000 fmcapi-20240503.0/fmcapi/fmc.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi.egg-info/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1644 2024-05-02 22:55:35.000000 fmcapi-20240503.0/fmcapi.egg-info/PKG-INFO
+-rw-r--r--   0 marksullivan   (501) staff       (20)    10285 2024-05-02 22:55:36.000000 fmcapi-20240503.0/fmcapi.egg-info/SOURCES.txt
+-rw-r--r--   0 marksullivan   (501) staff       (20)        1 2024-05-02 22:55:35.000000 fmcapi-20240503.0/fmcapi.egg-info/dependency_links.txt
+-rw-r--r--   0 marksullivan   (501) staff       (20)       38 2024-05-02 22:55:35.000000 fmcapi-20240503.0/fmcapi.egg-info/requires.txt
+-rw-r--r--   0 marksullivan   (501) staff       (20)       18 2024-05-02 22:55:35.000000 fmcapi-20240503.0/fmcapi.egg-info/top_level.txt
+-rw-r--r--   0 marksullivan   (501) staff       (20)       99 2024-04-28 05:00:25.000000 fmcapi-20240503.0/pyproject.toml
+-rw-r--r--   0 marksullivan   (501) staff       (20)       91 2024-05-02 22:55:38.000000 fmcapi-20240503.0/setup.cfg
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1960 2024-05-02 22:54:24.000000 fmcapi-20240503.0/setup.py
+drwxr-xr-x   0 marksullivan   (501) staff       (20)        0 2024-05-02 22:55:38.000000 fmcapi-20240503.0/unit_tests/
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5946 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/__init__.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      950 2024-04-28 05:00:25.000000 fmcapi-20240503.0/unit_tests/acls_extended.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      555 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/acp.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     4809 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/acprule.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      530 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      597 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_category.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      507 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_filter.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      601 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_productivity.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      521 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_risk.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      525 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_tag.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      517 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/application_type.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      235 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/audit_records.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     3546 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/autonat.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      509 2024-04-28 05:00:25.000000 fmcapi-20240503.0/unit_tests/backup.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      405 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/certificate_enrollment.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1131 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/connectionprofiles.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      527 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/continent.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      467 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/country.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      256 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/deployable_devices.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      260 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/deployment_requests.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2032 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/device_with_task.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      899 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/devicegrouprecords.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1379 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/devicerecords.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      624 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/dns_servers_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      460 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/dynamic_object_mappings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      546 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/dynamic_objects.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2024 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/dynamicaccesspolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      958 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/failoverinterfacemacaddressconfigs.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      367 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/file_policies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      505 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/fqdns.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2746 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ftddevicehapairs.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      519 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/geolocations.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1160 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/grouppolicies.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      207 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/helper_functions.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1887 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/hit_counts.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      484 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/icmpv4.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      484 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/icmpv6.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1008 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ikev1.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2703 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ikev2.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1488 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interface_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1150 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interfaces_bridge_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1296 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interfaces_etherchannel.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1820 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interfaces_physical.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1244 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interfaces_redundant.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1122 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/interfaces_subinterfaces.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      364 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/intrusion_policy.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      325 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ip_addresses.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      529 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ip_host.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      551 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ip_network.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      549 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ip_range.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1437 2024-05-02 22:51:34.000000 fmcapi-20240503.0/unit_tests/ipv4staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1442 2024-05-02 22:51:34.000000 fmcapi-20240503.0/unit_tests/ipv6staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1794 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/loggingsettings.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     5794 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/manualnat.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      586 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/monitored_interface.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1538 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/network_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2455 2024-04-28 05:00:25.000000 fmcapi-20240503.0/unit_tests/objects_get_query_filters.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1589 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/port_object_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      313 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/ports.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      552 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/prefilter.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     6617 2024-04-28 04:40:54.000000 fmcapi-20240503.0/unit_tests/prefilter_rule.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      589 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/protocol_port.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1062 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/ravpn.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2761 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/s2s_vpn.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      307 2024-04-28 04:40:54.000000 fmcapi-20240503.0/unit_tests/search_globalsearch.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      283 2024-04-28 04:40:54.000000 fmcapi-20240503.0/unit_tests/search_object.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      283 2024-04-28 04:40:54.000000 fmcapi-20240503.0/unit_tests/search_policy.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      571 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/security_zone.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      317 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/server_version.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1174 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/sla_monitor.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      439 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/staticroutes.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1192 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/terminateravpnsessions.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      640 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/timeranges.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     2899 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/upgrades.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      512 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/url.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      495 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/url_category.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1475 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/url_group.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      509 2024-04-28 05:00:25.000000 fmcapi-20240503.0/unit_tests/usage.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      325 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/variable_set.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1753 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/vlan_group_tag.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)      583 2021-12-14 09:40:27.000000 fmcapi-20240503.0/unit_tests/vlan_tag.py
+-rw-r--r--   0 marksullivan   (501) staff       (20)     1997 2024-04-28 05:09:35.000000 fmcapi-20240503.0/unit_tests/wait_for_task.py
```

### Comparing `fmcapi-20240418.0/LICENSE.md` & `fmcapi-20240503.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/PKG-INFO` & `fmcapi-20240503.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fmcapi
-Version: 20240418.0
+Version: 20240503.0
 Summary: Easier interface to Cisco's FMC API than writing your own way.
 Home-page: https://github.com/daxm/fmcapi
 Author: Dax Mickelson
 Author-email: dmickels@cisco.com
 License: BSD
 Description: With the removal to configure a Cisco NGFW via the command line your only option is to
              do so via a manager.  Some things are better when automated so using the manager's API gives us that power.
```

### Comparing `fmcapi-20240418.0/README.md` & `fmcapi-20240503.0/README.md`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/__init__.py` & `fmcapi-20240503.0/fmcapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/__init__.py` & `fmcapi-20240503.0/fmcapi/api_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/apiclasstemplate.py` & `fmcapi-20240503.0/fmcapi/api_objects/apiclasstemplate.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/audit_services/audit_records.py` & `fmcapi-20240503.0/fmcapi/api_objects/audit_services/audit_records.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/backup_services/backup.py` & `fmcapi-20240503.0/fmcapi/api_objects/backup_services/backup.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/deployment_services/deployabledevices.py` & `fmcapi-20240503.0/fmcapi/api_objects/deployment_services/deployabledevices.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/deployment_services/deploymentrequests.py` & `fmcapi-20240503.0/fmcapi/api_objects/deployment_services/deploymentrequests.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             if int(json_data["version"]) > int(device["version"]):
                 logging.info(f"Updating version to {device['version']}")
                 json_data["version"] = device["version"]
         logging.info("Deploying changes to devices.")
         response = self.fmc.send_to_api(
             method="post", url=self.URL, json_data=json_data
         )
-        return response["deviceList"]
+        return response
 
     def put(self):
         """PUT method for API for DeploymentRequests not supported."""
         logging.info("PUT method for API for DeploymentRequests not supported.")
         pass
 
     def delete(self):
```

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_clusters/ftddevicecluster.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_clusters/ftddevicecluster.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_group_services/devicegrouprecords.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_group_services/devicegrouprecords.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/failoverinterfacemacaddressconfigs.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/failoverinterfacemacaddressconfigs.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/ftddevicehapairs.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/ftddevicehapairs.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_ha_pair_services/monitoredinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_ha_pair_services/monitoredinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/__init__.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/bridgegroupinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/bridgegroupinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/devicerecords.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/devicerecords.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/etherchannelinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/etherchannelinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/ipv4staticroutes.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/ipv4staticroutes.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,7 +192,20 @@
                 "id": ipsla1.id,
                 "name": ipsla1.name,
             }
         else:
             logging.warning(
                 f"Object {name} not found.  Cannot set up device for IPv4StaticRoute."
             )
+
+    def post(self, **kwargs):
+        """
+        Modified post method for ipv4staticroutes
+        """
+        logging.debug("In post() for IPv4StaticRoute class.")
+        # Handle Null0 routes not needing a gateway
+        if self.interfaceName:
+            if self.interfaceName == "Null0" or self.interfaceName == "null0":
+                # Remove gateway from REQUIRED_FOR_POST global const
+                self.REQUIRED_FOR_POST = ["interfaceName", "selectedNetworks"]
+        response = super().post(**kwargs)
+        return response
```

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/ipv6staticroutes.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/ipv6staticroutes.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,7 +170,20 @@
             self.gateway = {
                 "object": {"type": gw1.type, "id": gw1.id, "name": gw1.name}
             }
         else:
             logging.warning(
                 f'Network "{name}" not found.  Cannot set up device for IPv6StaticRoute.'
             )
+
+    def post(self, **kwargs):
+        """
+        Modified post method for ipv6staticroutes
+        """
+        logging.debug("In post() for IPv6StaticRoute class.")
+        # Handle Null0 routes not needing a gateway
+        if self.interfaceName:
+            if self.interfaceName == "Null0" or self.interfaceName == "null0":
+                # Remove gateway from REQUIRED_FOR_POST global const
+                self.REQUIRED_FOR_POST = ["interfaceName", "selectedNetworks"]
+        response = super().post(**kwargs)
+        return response
```

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/physicalinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/physicalinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/redundantinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/redundantinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/staticroutes.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/staticroutes.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/device_services/subinterfaces.py` & `fmcapi-20240503.0/fmcapi/api_objects/device_services/subinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/health/terminateravpnsessions.py` & `fmcapi-20240503.0/fmcapi/api_objects/health/terminateravpnsessions.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/helper_functions.py` & `fmcapi-20240503.0/fmcapi/api_objects/helper_functions.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/__init__.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/anyprotocolportobjects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/anyprotocolportobjects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationcategories.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationcategories.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationfilters.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationfilters.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationproductivities.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationproductivities.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationrisks.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationrisks.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applications.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applications.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationtags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationtags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/applicationtypes.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/applicationtypes.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/certenrollments.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/certenrollments.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/continents.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/continents.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/countries.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/countries.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/dnsservergroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/dnsservergroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/dynamicobjectmappings.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/dynamicobjectmappings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/dynamicobjects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/dynamicobjects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/endpointdevicetypes.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/endpointdevicetypes.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/extendedaccesslist.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/extendedaccesslist.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/fqdns.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/fqdns.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/geolocation.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/geolocation.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/grouppolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/grouppolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/hosts.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/hosts.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/icmpv4objects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/icmpv4objects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/icmpv6objects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/icmpv6objects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev1ipsecproposals.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev1ipsecproposals.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev1policies.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev1policies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev2ipsecproposals.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev2ipsecproposals.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ikev2policies.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ikev2policies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/interfacegroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/interfacegroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/interfaceobjects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/interfaceobjects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/isesecuritygrouptags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/isesecuritygrouptags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/networkaddresses.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/networkaddresses.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/networkgroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/networkgroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/networks.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/networks.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/portobjectgroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/portobjectgroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ports.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ports.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/protocolportobjects.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/protocolportobjects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/ranges.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/ranges.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/realms.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/realms.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/realmusergroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/realmusergroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/realmusers.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/realmusers.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/securitygrouptags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/securitygrouptags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/securityzones.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/securityzones.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/siurlfeeds.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/siurlfeeds.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/siurllists.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/siurllists.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/slamonitors.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/slamonitors.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/timeranges.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/timeranges.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/tunneltags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/tunneltags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/urlcategories.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/urlcategories.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/urlgroups.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/urlgroups.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/urls.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/urls.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/usage.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/usage.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/variablesets.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/variablesets.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/vlangrouptags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/vlangrouptags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/object_services/vlantags.py` & `fmcapi-20240503.0/fmcapi/api_objects/object_services/vlantags.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_assignment_services/policyassignments.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_assignment_services/policyassignments.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/__init__.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/accesspolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/accesspolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/accessrules.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/accessrules.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/advancedsettings.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/advancedsettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/autonatrules.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/autonatrules.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/categories.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/categories.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/connectionprofiles.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/connectionprofiles.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/defaultactions.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/defaultactions.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/dynamicaccesspolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/dynamicaccesspolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/endpoints.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/endpoints.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/filepolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/filepolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/ftdnatpolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/ftdnatpolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/ftds2svpns.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/ftds2svpns.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/hitcounts.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/hitcounts.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/ikesettings.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/ikesettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/inheritancesettings.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/inheritancesettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/intrusionpolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/intrusionpolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/ipsecsettings.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/ipsecsettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/loggingsettings.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/loggingsettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/manualnatrules.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/manualnatrules.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/natrules.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/natrules.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/prefilterpolicies.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/prefilterpolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/prefilterrules.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/prefilterrules.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/policy_services/ravpns.py` & `fmcapi-20240503.0/fmcapi/api_objects/policy_services/ravpns.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/search/globalsearch.py` & `fmcapi-20240503.0/fmcapi/api_objects/search/globalsearch.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/search/object.py` & `fmcapi-20240503.0/fmcapi/api_objects/search/object.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/search/policy.py` & `fmcapi-20240503.0/fmcapi/api_objects/search/policy.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/status_services/taskstatuses.py` & `fmcapi-20240503.0/fmcapi/api_objects/status_services/taskstatuses.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/system_information/serverversion.py` & `fmcapi-20240503.0/fmcapi/api_objects/system_information/serverversion.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/update_packages/listapplicabledevices.py` & `fmcapi-20240503.0/fmcapi/api_objects/update_packages/listapplicabledevices.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/update_packages/upgradepackage.py` & `fmcapi-20240503.0/fmcapi/api_objects/update_packages/upgradepackage.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     VALID_JSON_DATA = [
         "id",
         "name",
         "type",
         "upgradePackage",
         "targets",
         "pushUpgradeFileOnly",
+        "readinessCheckOnly",
+        "enableUpgradeRevert",
+        "autoUpgradeCancel",
     ]
+    REQUIRED_FOR_POST = ["upgradePackage", "targets"]
     VALID_FOR_KWARGS = VALID_JSON_DATA + []
     URL_SUFFIX = "/updates/upgrades"
 
     def __init__(self, fmc, **kwargs):
         """
         Initialize Upgrades object.
```

### Comparing `fmcapi-20240418.0/fmcapi/api_objects/update_packages/upgradepackages.py` & `fmcapi-20240503.0/fmcapi/api_objects/update_packages/upgradepackages.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi/fmc.py` & `fmcapi-20240503.0/fmcapi/fmc.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/fmcapi.egg-info/PKG-INFO` & `fmcapi-20240503.0/fmcapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fmcapi
-Version: 20240418.0
+Version: 20240503.0
 Summary: Easier interface to Cisco's FMC API than writing your own way.
 Home-page: https://github.com/daxm/fmcapi
 Author: Dax Mickelson
 Author-email: dmickels@cisco.com
 License: BSD
 Description: With the removal to configure a Cisco NGFW via the command line your only option is to
              do so via a manager.  Some things are better when automated so using the manager's API gives us that power.
```

### Comparing `fmcapi-20240418.0/fmcapi.egg-info/SOURCES.txt` & `fmcapi-20240503.0/fmcapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/setup.py` & `fmcapi-20240503.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __author__ = "Dax Mickelson"
 __author_email = "dmickels@cisco.com"
 __license__ = "BSD"
 
 setup(
     name="fmcapi",
-    version="20240418.0",
+    version="20240503.0",
     description="Easier interface to Cisco's FMC API than writing your own way.",
     long_description="""With the removal to configure a Cisco NGFW via the command line your only option is to
      do so via a manager.  Some things are better when automated so using the manager's API gives us that power. 
      However, the current way to write external scripts and interact with the FMC's API isn't that great.  We created 
      this "wrapper" to give you an easier to use way of communicating with the FMC's API than using the example code 
      provided in the API Explorer.""",
     url="https://github.com/daxm/fmcapi",
```

### Comparing `fmcapi-20240418.0/unit_tests/__init__.py` & `fmcapi-20240503.0/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/acls_extended.py` & `fmcapi-20240503.0/unit_tests/acls_extended.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/acp.py` & `fmcapi-20240503.0/unit_tests/acp.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/acprule.py` & `fmcapi-20240503.0/unit_tests/acprule.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application.py` & `fmcapi-20240503.0/unit_tests/application.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application_category.py` & `fmcapi-20240503.0/unit_tests/application_category.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application_productivity.py` & `fmcapi-20240503.0/unit_tests/application_productivity.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application_risk.py` & `fmcapi-20240503.0/unit_tests/application_risk.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application_tag.py` & `fmcapi-20240503.0/unit_tests/application_tag.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/application_type.py` & `fmcapi-20240503.0/unit_tests/application_type.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/autonat.py` & `fmcapi-20240503.0/unit_tests/autonat.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/connectionprofiles.py` & `fmcapi-20240503.0/unit_tests/connectionprofiles.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/continent.py` & `fmcapi-20240503.0/unit_tests/continent.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/device_with_task.py` & `fmcapi-20240503.0/unit_tests/device_with_task.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/devicegrouprecords.py` & `fmcapi-20240503.0/unit_tests/devicegrouprecords.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/devicerecords.py` & `fmcapi-20240503.0/unit_tests/devicerecords.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/dns_servers_group.py` & `fmcapi-20240503.0/unit_tests/dns_servers_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/dynamic_objects.py` & `fmcapi-20240503.0/unit_tests/dynamic_objects.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/dynamicaccesspolicies.py` & `fmcapi-20240503.0/unit_tests/dynamicaccesspolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/failoverinterfacemacaddressconfigs.py` & `fmcapi-20240503.0/unit_tests/failoverinterfacemacaddressconfigs.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ftddevicehapairs.py` & `fmcapi-20240503.0/unit_tests/ftddevicehapairs.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/geolocations.py` & `fmcapi-20240503.0/unit_tests/geolocations.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/grouppolicies.py` & `fmcapi-20240503.0/unit_tests/grouppolicies.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/hit_counts.py` & `fmcapi-20240503.0/unit_tests/hit_counts.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ikev1.py` & `fmcapi-20240503.0/unit_tests/ikev1.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ikev2.py` & `fmcapi-20240503.0/unit_tests/ikev2.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interface_group.py` & `fmcapi-20240503.0/unit_tests/interface_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interfaces_bridge_group.py` & `fmcapi-20240503.0/unit_tests/interfaces_bridge_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interfaces_etherchannel.py` & `fmcapi-20240503.0/unit_tests/interfaces_etherchannel.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interfaces_physical.py` & `fmcapi-20240503.0/unit_tests/interfaces_physical.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interfaces_redundant.py` & `fmcapi-20240503.0/unit_tests/interfaces_redundant.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/interfaces_subinterfaces.py` & `fmcapi-20240503.0/unit_tests/interfaces_subinterfaces.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ip_host.py` & `fmcapi-20240503.0/unit_tests/ip_host.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ip_network.py` & `fmcapi-20240503.0/unit_tests/ip_network.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ip_range.py` & `fmcapi-20240503.0/unit_tests/ip_range.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ipv4staticroutes.py` & `fmcapi-20240503.0/unit_tests/ipv4staticroutes.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,22 @@
     ipnet2 = fmcapi.Networks(fmc=fmc, name="_ipnet2" + namer, value="192.0.2.128/25")
     ipnet1.post()
     ipnet2.post()
 
     ipv4route1 = fmcapi.IPv4StaticRoutes(fmc=fmc, name="_ipv4route1")
     ipv4route1.device(device_name="ftdv01.ccie.lab")
     ipv4route1.networks(action="add", networks=[ipnet1.name, ipnet2.name])
+    # NO GATEWAY IS EXPECTED WHEN IMPLEMENTING A ROUTE VIA NULL0
     ipv4route1.gw(name=iphost1.name)
     ipv4route1.interfaceName = "ifname"
     ipv4route1.metricValue = 1
     result = ipv4route1.post()
 
     ipv4route2 = fmcapi.IPv4StaticRoutes(fmc=fmc, name="_ipv4route1")
-    ipv4route2.device(device_name="device_name")
+    ipv4route2.device(device_name="ftdv01.ccie.lab")
     ipv4route2.id = result["id"]
     ipv4route2.get()
 
     del ipv4route1
     ipv4route2.networks(action="remove", networks=[ipnet2.name])
     ipv4route2.put()
```

### Comparing `fmcapi-20240418.0/unit_tests/ipv6staticroutes.py` & `fmcapi-20240503.0/unit_tests/ipv6staticroutes.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     iphost1 = fmcapi.Hosts(fmc=fmc, name="_iphost1" + namer, value="2001:db8::1")
     iphost1.post()
     ipnet1 = fmcapi.Networks(fmc=fmc, name="_ipnet1" + namer, value="2001:db8:1::/64")
     ipnet2 = fmcapi.Networks(fmc=fmc, name="_ipnet2" + namer, value="2001:db8:2::/64")
     ipnet1.post()
     ipnet2.post()
 
-    ipv4route1 = fmcapi.IPv6StaticRoutes(fmc=fmc, name="_ipv6route1")
-    ipv4route1.device(device_name="ftdv01.ccie.lab")
-    ipv4route1.networks(action="add", networks=[ipnet1.name, ipnet2.name])
-    ipv4route1.gw(name=iphost1.name)
-    ipv4route1.interfaceName = "ifname"
-    ipv4route1.metricValue = 1
-    result = ipv4route1.post()
+    ipv6route1 = fmcapi.IPv6StaticRoutes(fmc=fmc, name="_ipv6route1")
+    ipv6route1.device(device_name="ftdv01.ccie.lab")
+    ipv6route1.networks(action="add", networks=[ipnet1.name, ipnet2.name])
+    # NO GATEWAY IS EXPECTED WHEN IMPLEMENTING A ROUTE VIA NULL0
+    ipv6route1.gw(name=iphost1.name)
+    ipv6route1.interfaceName = "ifname"
+    ipv6route1.metricValue = 1
+    result = ipv6route1.post()
 
-    ipv4route2 = fmcapi.IPv4StaticRoutes(fmc=fmc, name="_ipv6route1")
-    ipv4route2.device(device_name="device_name")
-    ipv4route2.id = result["id"]
-    ipv4route2.get()
+    ipv6route2 = fmcapi.IPv6StaticRoutes(fmc=fmc, name="_ipv6route1")
+    ipv6route2.device(device_name="ftdv01.ccie.lab")
+    ipv6route2.id = result["id"]
+    ipv6route2.get()
 
-    del ipv4route1
-    ipv4route2.networks(action="remove", networks=[ipnet2.name])
-    ipv4route2.put()
+    del ipv6route1
+    ipv6route2.networks(action="remove", networks=[ipnet2.name])
+    ipv6route2.put()
 
-    ipv4route2.delete()
+    ipv6route2.delete()
     ipnet1.delete()
     ipnet2.delete()
     iphost1.delete()
     logging.info("Testing IPv6StaticRoutes class done.\n")
```

### Comparing `fmcapi-20240418.0/unit_tests/loggingsettings.py` & `fmcapi-20240503.0/unit_tests/loggingsettings.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/manualnat.py` & `fmcapi-20240503.0/unit_tests/manualnat.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/monitored_interface.py` & `fmcapi-20240503.0/unit_tests/monitored_interface.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/network_group.py` & `fmcapi-20240503.0/unit_tests/network_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/objects_get_query_filters.py` & `fmcapi-20240503.0/unit_tests/objects_get_query_filters.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/port_object_group.py` & `fmcapi-20240503.0/unit_tests/port_object_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/prefilter.py` & `fmcapi-20240503.0/unit_tests/prefilter.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/prefilter_rule.py` & `fmcapi-20240503.0/unit_tests/prefilter_rule.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/protocol_port.py` & `fmcapi-20240503.0/unit_tests/protocol_port.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/ravpn.py` & `fmcapi-20240503.0/unit_tests/ravpn.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/s2s_vpn.py` & `fmcapi-20240503.0/unit_tests/s2s_vpn.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/security_zone.py` & `fmcapi-20240503.0/unit_tests/security_zone.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/sla_monitor.py` & `fmcapi-20240503.0/unit_tests/sla_monitor.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/terminateravpnsessions.py` & `fmcapi-20240503.0/unit_tests/terminateravpnsessions.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/timeranges.py` & `fmcapi-20240503.0/unit_tests/timeranges.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/url.py` & `fmcapi-20240503.0/unit_tests/url.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/url_group.py` & `fmcapi-20240503.0/unit_tests/url_group.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/vlan_group_tag.py` & `fmcapi-20240503.0/unit_tests/vlan_group_tag.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/vlan_tag.py` & `fmcapi-20240503.0/unit_tests/vlan_tag.py`

 * *Files identical despite different names*

### Comparing `fmcapi-20240418.0/unit_tests/wait_for_task.py` & `fmcapi-20240503.0/unit_tests/wait_for_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import fmcapi
 import time
 import logging
 
 
 def wait_for_task(fmc, task, wait_time=10):
-    task_completed_states = ["Success", "SUCCESS", "COMPLETED"]
+    task_completed_states = ["Success", "SUCCESS", "COMPLETED", "Deployed"]
     try:
         status = fmcapi.TaskStatuses(fmc=fmc, id=task["id"])
         current_status = status.get()
         """
         Task Status for new device registration behaves differently than other tasks
         On new device registration, a task is sent for the initial registration. After completion 
         the UUID is deleted without any change in task status. So we check to see if the object no longer exists
```

