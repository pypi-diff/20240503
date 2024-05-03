# Comparing `tmp/plex-api-client-0.6.4.tar.gz` & `tmp/plex-api-client-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.6.4.tar", last modified: Mon Apr 22 16:16:22 2024, max compression
+gzip compressed data, was "plex-api-client-0.6.5.tar", last modified: Fri May  3 01:19:23 2024, max compression
```

## Comparing `plex-api-client-0.6.4.tar` & `plex-api-client-0.6.5.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.044982 plex-api-client-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.044982 plex-api-client-0.6.4/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.044982 plex-api-client-0.6.4/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.044982 plex-api-client-0.6.4/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.044982 plex-api-client-0.6.4/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.052982 plex-api-client-0.6.4/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.052982 plex-api-client-0.6.4/src/plex_api/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    33949 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-22 16:16:13.000000 plex-api-client-0.6.4/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:16:22.064982 plex-api-client-0.6.4/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-22 16:16:21.000000 plex-api-client-0.6.4/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-22 16:16:22.000000 plex-api-client-0.6.4/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:16:21.000000 plex-api-client-0.6.4/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-22 16:16:21.000000 plex-api-client-0.6.4/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-22 16:16:21.000000 plex-api-client-0.6.4/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.772498 plex-api-client-0.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.776498 plex-api-client-0.6.5/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.776498 plex-api-client-0.6.5/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.776498 plex-api-client-0.6.5/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.776498 plex-api-client-0.6.5/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.784498 plex-api-client-0.6.5/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.784498 plex-api-client-0.6.5/src/plex_api/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33949 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14315 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-03 01:19:13.000000 plex-api-client-0.6.5/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:19:23.796498 plex-api-client-0.6.5/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-05-03 01:19:23.000000 plex-api-client-0.6.5/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-03 01:19:23.000000 plex-api-client-0.6.5/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:19:23.000000 plex-api-client-0.6.5/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-03 01:19:23.000000 plex-api-client-0.6.5/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 01:19:23.000000 plex-api-client-0.6.5/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.6.4/LICENSE.md` & `plex-api-client-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/PKG-INFO` & `plex-api-client-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -28,15 +28,15 @@
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -168,15 +168,15 @@
         
         ```python
         import plex_api
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
@@ -208,15 +208,15 @@
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -236,15 +236,15 @@
         The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -255,19 +255,19 @@
         ### Override Server URL Per-Operation
         
         The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
+        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -301,15 +301,15 @@
         
         To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -319,15 +319,15 @@
         <!-- End Authentication [security] -->
         
         <!-- Start Global Parameters [global-parameters] -->
         ## Global Parameters
         
         A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
         
-        For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        For example, you can set `X-Plex-Client-Identifier` to `'Postman'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
         
         
         ### Available Globals
         
         The following global parameter is available. The required parameter must be set when you initialize the SDK client.
         
         | Name | Type | Required | Description |
@@ -340,19 +340,19 @@
         
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
-        res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.4 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.5 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+( access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ## Available Resources and Operations ### [server](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/server/README.md) *
 [get_server_capabilities](https://github.com/LukeHagar/plexpy/blob/master/docs/
 sdks/server/README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](https://github.com/LukeHagar/plexpy/blob/master/docs/
 sdks/server/README.md#get_server_preferences) - Get Server Preferences *
@@ -145,79 +145,80 @@
 operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | -------------------------------
 --------- | ---------------------------------------- | ------------------------
 ---------------- | | errors.GetServerCapabilitiesResponseBody | 401 |
 application/json | | errors.SDKError | 4xx-5xx | */* | ### Example ```python
 import plex_api from plex_api.models import errors s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res = None try: res =
+( access_token="", x_plex_client_identifier='Postman', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` #### Variables Some of the server options above contain
-variables. If you want to set the values of those variables, the following
-optional parameters are available when initializing the SDK client instance: *
-`protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
-URL Per-Client The default server can also be overridden globally by passing a
-URL to the `server_url: str` optional parameter when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="",
-x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
-res.object is not None: # handle response pass ``` ### Override Server URL Per-
-Operation The server URL can also be overridden on a per-operation basis,
-provided a server list was specified for the operation. For example: ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
-x_plex_client_identifier='') if res.object is not None: # handle response pass
-``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
-(https://pypi.org/project/requests/) HTTP library. In order to provide a
-convenient way to configure timeouts, cookies, proxies, custom headers, and
-other low-level configuration, you can initialize the SDK client with a custom
-`requests.Session` object. For example, you could specify a header for every
-request that this sdk makes as follows: ```python import plex_api import
-requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
-Authentication ### Per-Client Security Schemes This SDK supports the following
-security scheme globally: | Name | Type | Scheme | | -------------- | ---------
------ | -------------- | | `access_token` | apiKey | API key | To authenticate
-with the API the `access_token` parameter must be set when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+plex_api.PlexAPI( server_idx=0, access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` #### Variables Some of
+the server options above contain variables. If you want to set the values of
+those variables, the following optional parameters are available when
+initializing the SDK client instance: * `protocol: models.ServerProtocol` *
+`ip: str` * `port: str` ### Override Server URL Per-Client The default server
+can also be overridden globally by passing a URL to the `server_url: str`
+optional parameter when initializing the SDK client instance. For example:
+```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
+{port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ## Global Parameters A parameter is configured globally. This
-parameter must be set on the SDK client instance itself during initialization.
-When configured as an option during SDK initialization, This global value will
-be used as the default on the operations that use it. When such operations are
-called, there is a place in each to override the global value, if needed. For
-example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
-and then you do not have to pass the same value on calls to operations like
-`get_pin`. But if you want to do so you may, which will locally override the
-global setting. See the example code below for a demonstration. ### Available
-Globals The following global parameter is available. The required parameter
-must be set when you initialize the SDK client. | Name | Type | Required |
-Description | | ---- | ---- |:--------:| ----------- | |
-x_plex_client_identifier | str | âï¸ | The unique identifier for the client
-application This is used to track the client application and its usage (UUID,
-serial number, or other number unique per device) | ### Example ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
-None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ## Contributions
-While we value open-source contributions to this SDK, this library is generated
+pass ``` ### Override Server URL Per-Operation The server URL can also be
+overridden on a per-operation basis, provided a server list was specified for
+the operation. For example: ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
+//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+res.object is not None: # handle response pass ``` ## Custom HTTP Client The
+Python SDK makes API calls using the [requests](https://pypi.org/project/
+requests/) HTTP library. In order to provide a convenient way to configure
+timeouts, cookies, proxies, custom headers, and other low-level configuration,
+you can initialize the SDK client with a custom `requests.Session` object. For
+example, you could specify a header for every request that this sdk makes as
+follows: ```python import plex_api import requests http_client =
+requests.Session() http_client.headers.update({'x-custom-header': 'someValue'})
+s = plex_api.PlexAPI(client=http_client) ``` ## Authentication ### Per-Client
+Security Schemes This SDK supports the following security scheme globally: |
+Name | Type | Scheme | | -------------- | -------------- | -------------- | |
+`access_token` | apiKey | API key | To authenticate with the API the
+`access_token` parameter must be set when initializing the SDK client instance.
+For example: ```python import plex_api s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` ## Global Parameters A
+parameter is configured globally. This parameter must be set on the SDK client
+instance itself during initialization. When configured as an option during SDK
+initialization, This global value will be used as the default on the operations
+that use it. When such operations are called, there is a place in each to
+override the global value, if needed. For example, you can set `X-Plex-Client-
+Identifier` to `'Postman'` at SDK initialization and then you do not have to
+pass the same value on calls to operations like `get_pin`. But if you want to
+do so you may, which will locally override the global setting. See the example
+code below for a demonstration. ### Available Globals The following global
+parameter is available. The required parameter must be set when you initialize
+the SDK client. | Name | Type | Required | Description | | ---- | ---- |:------
+--:| ----------- | | x_plex_client_identifier | str | âï¸ | The unique
+identifier for the client application This is used to track the client
+application and its usage (UUID, serial number, or other number unique per
+device) | ### Example ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman') if res.object is not None: # handle
+response pass ``` # Development ## Maturity This SDK is in beta, and there may
+be breaking changes between versions without a major version update. Therefore,
+we recommend pinning usage to a specific package version. This way, you can
+install the same version each time without breaking changes unless you are
+intentionally looking for the latest version. ## Contributions While we value
+open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev
```

### Comparing `plex-api-client-0.6.4/README.md` & `plex-api-client-0.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ### Example
 
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -161,15 +161,15 @@
 
 ```python
 import plex_api
 from plex_api.models import errors
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
 res = None
 try:
     res = s.server.get_server_capabilities()
 except errors.GetServerCapabilitiesResponseBody as e:
@@ -201,15 +201,15 @@
 
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     server_idx=0,
     access_token="<YOUR_API_KEY_HERE>",
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -229,15 +229,15 @@
 The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     server_url="{protocol}://{ip}:{port}",
     access_token="<YOUR_API_KEY_HERE>",
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -248,19 +248,19 @@
 ### Override Server URL Per-Operation
 
 The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
-res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
+res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -294,15 +294,15 @@
 
 To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
     access_token="<YOUR_API_KEY_HERE>",
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
 res = s.server.get_server_capabilities()
 
 if res.object is not None:
     # handle response
@@ -312,15 +312,15 @@
 <!-- End Authentication [security] -->
 
 <!-- Start Global Parameters [global-parameters] -->
 ## Global Parameters
 
 A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
 
-For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+For example, you can set `X-Plex-Client-Identifier` to `'Postman'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
 
 
 ### Available Globals
 
 The following global parameter is available. The required parameter must be set when you initialize the SDK client.
 
 | Name | Type | Required | Description |
@@ -333,19 +333,19 @@
 
 ### Example
 
 ```python
 import plex_api
 
 s = plex_api.PlexAPI(
-    x_plex_client_identifier='<value>',
+    x_plex_client_identifier='Postman',
 )
 
 
-res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Global Parameters [global-parameters] -->
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+( access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ## Available Resources and Operations ### [server](docs/sdks/server/
 README.md) * [get_server_capabilities](docs/sdks/server/
 README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](docs/sdks/server/README.md#get_server_preferences) -
 Get Server Preferences * [get_available_clients](docs/sdks/server/
 README.md#get_available_clients) - Get Available Clients * [get_devices](docs/
@@ -96,78 +96,79 @@
 Error objects are specified in your OpenAPI Spec, the SDK will raise the
 appropriate Error type. | Error Object | Status Code | Content Type | | -------
 --------------------------------- | ---------------------------------------- |
 ---------------------------------------- | |
 errors.GetServerCapabilitiesResponseBody | 401 | application/json | |
 errors.SDKError | 4xx-5xx | */* | ### Example ```python import plex_api from
 plex_api.models import errors s = plex_api.PlexAPI( access_token="",
-x_plex_client_identifier='', ) res = None try: res =
+x_plex_client_identifier='Postman', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` #### Variables Some of the server options above contain
-variables. If you want to set the values of those variables, the following
-optional parameters are available when initializing the SDK client instance: *
-`protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
-URL Per-Client The default server can also be overridden globally by passing a
-URL to the `server_url: str` optional parameter when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="",
-x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
-res.object is not None: # handle response pass ``` ### Override Server URL Per-
-Operation The server URL can also be overridden on a per-operation basis,
-provided a server list was specified for the operation. For example: ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
-x_plex_client_identifier='') if res.object is not None: # handle response pass
-``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
-(https://pypi.org/project/requests/) HTTP library. In order to provide a
-convenient way to configure timeouts, cookies, proxies, custom headers, and
-other low-level configuration, you can initialize the SDK client with a custom
-`requests.Session` object. For example, you could specify a header for every
-request that this sdk makes as follows: ```python import plex_api import
-requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
-Authentication ### Per-Client Security Schemes This SDK supports the following
-security scheme globally: | Name | Type | Scheme | | -------------- | ---------
------ | -------------- | | `access_token` | apiKey | API key | To authenticate
-with the API the `access_token` parameter must be set when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+plex_api.PlexAPI( server_idx=0, access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` #### Variables Some of
+the server options above contain variables. If you want to set the values of
+those variables, the following optional parameters are available when
+initializing the SDK client instance: * `protocol: models.ServerProtocol` *
+`ip: str` * `port: str` ### Override Server URL Per-Client The default server
+can also be overridden globally by passing a URL to the `server_url: str`
+optional parameter when initializing the SDK client instance. For example:
+```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
+{port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ## Global Parameters A parameter is configured globally. This
-parameter must be set on the SDK client instance itself during initialization.
-When configured as an option during SDK initialization, This global value will
-be used as the default on the operations that use it. When such operations are
-called, there is a place in each to override the global value, if needed. For
-example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
-and then you do not have to pass the same value on calls to operations like
-`get_pin`. But if you want to do so you may, which will locally override the
-global setting. See the example code below for a demonstration. ### Available
-Globals The following global parameter is available. The required parameter
-must be set when you initialize the SDK client. | Name | Type | Required |
-Description | | ---- | ---- |:--------:| ----------- | |
-x_plex_client_identifier | str | âï¸ | The unique identifier for the client
-application This is used to track the client application and its usage (UUID,
-serial number, or other number unique per device) | ### Example ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
-None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ## Contributions
-While we value open-source contributions to this SDK, this library is generated
+pass ``` ### Override Server URL Per-Operation The server URL can also be
+overridden on a per-operation basis, provided a server list was specified for
+the operation. For example: ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
+//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+res.object is not None: # handle response pass ``` ## Custom HTTP Client The
+Python SDK makes API calls using the [requests](https://pypi.org/project/
+requests/) HTTP library. In order to provide a convenient way to configure
+timeouts, cookies, proxies, custom headers, and other low-level configuration,
+you can initialize the SDK client with a custom `requests.Session` object. For
+example, you could specify a header for every request that this sdk makes as
+follows: ```python import plex_api import requests http_client =
+requests.Session() http_client.headers.update({'x-custom-header': 'someValue'})
+s = plex_api.PlexAPI(client=http_client) ``` ## Authentication ### Per-Client
+Security Schemes This SDK supports the following security scheme globally: |
+Name | Type | Scheme | | -------------- | -------------- | -------------- | |
+`access_token` | apiKey | API key | To authenticate with the API the
+`access_token` parameter must be set when initializing the SDK client instance.
+For example: ```python import plex_api s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` ## Global Parameters A
+parameter is configured globally. This parameter must be set on the SDK client
+instance itself during initialization. When configured as an option during SDK
+initialization, This global value will be used as the default on the operations
+that use it. When such operations are called, there is a place in each to
+override the global value, if needed. For example, you can set `X-Plex-Client-
+Identifier` to `'Postman'` at SDK initialization and then you do not have to
+pass the same value on calls to operations like `get_pin`. But if you want to
+do so you may, which will locally override the global setting. See the example
+code below for a demonstration. ### Available Globals The following global
+parameter is available. The required parameter must be set when you initialize
+the SDK client. | Name | Type | Required | Description | | ---- | ---- |:------
+--:| ----------- | | x_plex_client_identifier | str | âï¸ | The unique
+identifier for the client application This is used to track the client
+application and its usage (UUID, serial number, or other number unique per
+device) | ### Example ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman') if res.object is not None: # handle
+response pass ``` # Development ## Maturity This SDK is in beta, and there may
+be breaking changes between versions without a major version update. Therefore,
+we recommend pinning usage to a specific package version. This way, you can
+install the same version each time without breaking changes unless you are
+intentionally looking for the latest version. ## Contributions While we value
+open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks)
```

### Comparing `plex-api-client-0.6.4/setup.py` & `plex-api-client-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='plex-api-client',
-    version='0.6.4',
+    version='0.6.5',
     author='LukeHagar',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/LukeHagar/plexpy.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `plex-api-client-0.6.4/src/plex_api/_hooks/registration.py` & `plex-api-client-0.6.5/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.6.5/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/_hooks/types.py` & `plex-api-client-0.6.5/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/activities.py` & `plex-api-client-0.6.5/src/plex_api/activities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/authentication.py` & `plex-api-client-0.6.5/src/plex_api/authentication.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/butler.py` & `plex-api-client-0.6.5/src/plex_api/butler.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/hubs.py` & `plex-api-client-0.6.5/src/plex_api/hubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/library.py` & `plex-api-client-0.6.5/src/plex_api/library.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/log.py` & `plex-api-client-0.6.5/src/plex_api/log.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/media.py` & `plex-api-client-0.6.5/src/plex_api/media.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/logline.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/internal/globals.py` & `plex-api-client-0.6.5/src/plex_api/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getlibraryitems.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/logline.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/searchlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.6.5/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/playlists.py` & `plex-api-client-0.6.5/src/plex_api/playlists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/plex.py` & `plex-api-client-0.6.5/src/plex_api/plex.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/sdk.py` & `plex-api-client-0.6.5/src/plex_api/sdk.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.6.5/src/plex_api/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.6.4'
-    gen_version: str = '2.311.1'
-    user_agent: str = 'speakeasy-sdk/python 0.6.4 2.311.1 0.0.3 plex-api-client'
+    sdk_version: str = '0.6.5'
+    gen_version: str = '2.312.1'
+    user_agent: str = 'speakeasy-sdk/python 0.6.5 2.312.1 0.0.3 plex-api-client'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `plex-api-client-0.6.4/src/plex_api/search.py` & `plex-api-client-0.6.5/src/plex_api/search.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/server.py` & `plex-api-client-0.6.5/src/plex_api/server.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/sessions.py` & `plex-api-client-0.6.5/src/plex_api/sessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/statistics.py` & `plex-api-client-0.6.5/src/plex_api/statistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/updater.py` & `plex-api-client-0.6.5/src/plex_api/updater.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/utils/retries.py` & `plex-api-client-0.6.5/src/plex_api/utils/retries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/utils/utils.py` & `plex-api-client-0.6.5/src/plex_api/utils/utils.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api/video.py` & `plex-api-client-0.6.5/src/plex_api/video.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.4/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.6.5/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
@@ -28,15 +28,15 @@
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -168,15 +168,15 @@
         
         ```python
         import plex_api
         from plex_api.models import errors
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = None
         try:
             res = s.server.get_server_capabilities()
         except errors.GetServerCapabilitiesResponseBody as e:
@@ -208,15 +208,15 @@
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_idx=0,
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -236,15 +236,15 @@
         The default server can also be overridden globally by passing a URL to the `server_url: str` optional parameter when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             server_url="{protocol}://{ip}:{port}",
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -255,19 +255,19 @@
         ### Override Server URL Per-Operation
         
         The server URL can also be overridden on a per-operation basis, provided a server list was specified for the operation. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
-        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='<value>')
+        res = s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -301,15 +301,15 @@
         
         To authenticate with the API the `access_token` parameter must be set when initializing the SDK client instance. For example:
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
             access_token="<YOUR_API_KEY_HERE>",
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
         res = s.server.get_server_capabilities()
         
         if res.object is not None:
             # handle response
@@ -319,15 +319,15 @@
         <!-- End Authentication [security] -->
         
         <!-- Start Global Parameters [global-parameters] -->
         ## Global Parameters
         
         A parameter is configured globally. This parameter must be set on the SDK client instance itself during initialization. When configured as an option during SDK initialization, This global value will be used as the default on the operations that use it. When such operations are called, there is a place in each to override the global value, if needed.
         
-        For example, you can set `X-Plex-Client-Identifier` to `'<value>'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
+        For example, you can set `X-Plex-Client-Identifier` to `'Postman'` at SDK initialization and then you do not have to pass the same value on calls to operations like `get_pin`. But if you want to do so you may, which will locally override the global setting. See the example code below for a demonstration.
         
         
         ### Available Globals
         
         The following global parameter is available. The required parameter must be set when you initialize the SDK client.
         
         | Name | Type | Required | Description |
@@ -340,19 +340,19 @@
         
         ### Example
         
         ```python
         import plex_api
         
         s = plex_api.PlexAPI(
-            x_plex_client_identifier='<value>',
+            x_plex_client_identifier='Postman',
         )
         
         
-        res = s.plex.get_pin(strong=False, x_plex_client_identifier='<value>')
+        res = s.plex.get_pin(strong=False, x_plex_client_identifier='Postman')
         
         if res.object is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.4 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.5 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+( access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
 pass ``` ## Available Resources and Operations ### [server](https://github.com/
 LukeHagar/plexpy/blob/master/docs/sdks/server/README.md) *
 [get_server_capabilities](https://github.com/LukeHagar/plexpy/blob/master/docs/
 sdks/server/README.md#get_server_capabilities) - Server Capabilities *
 [get_server_preferences](https://github.com/LukeHagar/plexpy/blob/master/docs/
 sdks/server/README.md#get_server_preferences) - Get Server Preferences *
@@ -145,79 +145,80 @@
 operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | -------------------------------
 --------- | ---------------------------------------- | ------------------------
 ---------------- | | errors.GetServerCapabilitiesResponseBody | 401 |
 application/json | | errors.SDKError | 4xx-5xx | */* | ### Example ```python
 import plex_api from plex_api.models import errors s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res = None try: res =
+( access_token="", x_plex_client_identifier='Postman', ) res = None try: res =
 s.server.get_server_capabilities() except
 errors.GetServerCapabilitiesResponseBody as e: # handle exception raise(e)
 except errors.SDKError as e: # handle exception raise(e) if res.object is not
 None: # handle response pass ``` ## Server Selection ### Select Server by Index
 You can override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `{protocol}://{ip}:
 {port}` | `protocol` (default is `http`), `ip` (default is `10.10.10.47`),
 `port` (default is `32400`) | #### Example ```python import plex_api s =
-plex_api.PlexAPI( server_idx=0, access_token="", x_plex_client_identifier='', )
-res = s.server.get_server_capabilities() if res.object is not None: # handle
-response pass ``` #### Variables Some of the server options above contain
-variables. If you want to set the values of those variables, the following
-optional parameters are available when initializing the SDK client instance: *
-`protocol: models.ServerProtocol` * `ip: str` * `port: str` ### Override Server
-URL Per-Client The default server can also be overridden globally by passing a
-URL to the `server_url: str` optional parameter when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( server_url="{protocol}://{ip}:{port}", access_token="",
-x_plex_client_identifier='', ) res = s.server.get_server_capabilities() if
-res.object is not None: # handle response pass ``` ### Override Server URL Per-
-Operation The server URL can also be overridden on a per-operation basis,
-provided a server list was specified for the operation. For example: ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(server_url="https://plex.tv/api/v2", strong=False,
-x_plex_client_identifier='') if res.object is not None: # handle response pass
-``` ## Custom HTTP Client The Python SDK makes API calls using the [requests]
-(https://pypi.org/project/requests/) HTTP library. In order to provide a
-convenient way to configure timeouts, cookies, proxies, custom headers, and
-other low-level configuration, you can initialize the SDK client with a custom
-`requests.Session` object. For example, you could specify a header for every
-request that this sdk makes as follows: ```python import plex_api import
-requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = plex_api.PlexAPI(client=http_client) ``` ##
-Authentication ### Per-Client Security Schemes This SDK supports the following
-security scheme globally: | Name | Type | Scheme | | -------------- | ---------
------ | -------------- | | `access_token` | apiKey | API key | To authenticate
-with the API the `access_token` parameter must be set when initializing the SDK
-client instance. For example: ```python import plex_api s = plex_api.PlexAPI
-( access_token="", x_plex_client_identifier='', ) res =
+plex_api.PlexAPI( server_idx=0, access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` #### Variables Some of
+the server options above contain variables. If you want to set the values of
+those variables, the following optional parameters are available when
+initializing the SDK client instance: * `protocol: models.ServerProtocol` *
+`ip: str` * `port: str` ### Override Server URL Per-Client The default server
+can also be overridden globally by passing a URL to the `server_url: str`
+optional parameter when initializing the SDK client instance. For example:
+```python import plex_api s = plex_api.PlexAPI( server_url="{protocol}://{ip}:
+{port}", access_token="", x_plex_client_identifier='Postman', ) res =
 s.server.get_server_capabilities() if res.object is not None: # handle response
-pass ``` ## Global Parameters A parameter is configured globally. This
-parameter must be set on the SDK client instance itself during initialization.
-When configured as an option during SDK initialization, This global value will
-be used as the default on the operations that use it. When such operations are
-called, there is a place in each to override the global value, if needed. For
-example, you can set `X-Plex-Client-Identifier` to `''` at SDK initialization
-and then you do not have to pass the same value on calls to operations like
-`get_pin`. But if you want to do so you may, which will locally override the
-global setting. See the example code below for a demonstration. ### Available
-Globals The following global parameter is available. The required parameter
-must be set when you initialize the SDK client. | Name | Type | Required |
-Description | | ---- | ---- |:--------:| ----------- | |
-x_plex_client_identifier | str | âï¸ | The unique identifier for the client
-application This is used to track the client application and its usage (UUID,
-serial number, or other number unique per device) | ### Example ```python
-import plex_api s = plex_api.PlexAPI( x_plex_client_identifier='', ) res =
-s.plex.get_pin(strong=False, x_plex_client_identifier='') if res.object is not
-None: # handle response pass ``` # Development ## Maturity This SDK is in beta,
-and there may be breaking changes between versions without a major version
-update. Therefore, we recommend pinning usage to a specific package version.
-This way, you can install the same version each time without breaking changes
-unless you are intentionally looking for the latest version. ## Contributions
-While we value open-source contributions to this SDK, this library is generated
+pass ``` ### Override Server URL Per-Operation The server URL can also be
+overridden on a per-operation basis, provided a server list was specified for
+the operation. For example: ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(server_url="https:
+//plex.tv/api/v2", strong=False, x_plex_client_identifier='Postman') if
+res.object is not None: # handle response pass ``` ## Custom HTTP Client The
+Python SDK makes API calls using the [requests](https://pypi.org/project/
+requests/) HTTP library. In order to provide a convenient way to configure
+timeouts, cookies, proxies, custom headers, and other low-level configuration,
+you can initialize the SDK client with a custom `requests.Session` object. For
+example, you could specify a header for every request that this sdk makes as
+follows: ```python import plex_api import requests http_client =
+requests.Session() http_client.headers.update({'x-custom-header': 'someValue'})
+s = plex_api.PlexAPI(client=http_client) ``` ## Authentication ### Per-Client
+Security Schemes This SDK supports the following security scheme globally: |
+Name | Type | Scheme | | -------------- | -------------- | -------------- | |
+`access_token` | apiKey | API key | To authenticate with the API the
+`access_token` parameter must be set when initializing the SDK client instance.
+For example: ```python import plex_api s = plex_api.PlexAPI( access_token="",
+x_plex_client_identifier='Postman', ) res = s.server.get_server_capabilities()
+if res.object is not None: # handle response pass ``` ## Global Parameters A
+parameter is configured globally. This parameter must be set on the SDK client
+instance itself during initialization. When configured as an option during SDK
+initialization, This global value will be used as the default on the operations
+that use it. When such operations are called, there is a place in each to
+override the global value, if needed. For example, you can set `X-Plex-Client-
+Identifier` to `'Postman'` at SDK initialization and then you do not have to
+pass the same value on calls to operations like `get_pin`. But if you want to
+do so you may, which will locally override the global setting. See the example
+code below for a demonstration. ### Available Globals The following global
+parameter is available. The required parameter must be set when you initialize
+the SDK client. | Name | Type | Required | Description | | ---- | ---- |:------
+--:| ----------- | | x_plex_client_identifier | str | âï¸ | The unique
+identifier for the client application This is used to track the client
+application and its usage (UUID, serial number, or other number unique per
+device) | ### Example ```python import plex_api s = plex_api.PlexAPI
+( x_plex_client_identifier='Postman', ) res = s.plex.get_pin(strong=False,
+x_plex_client_identifier='Postman') if res.object is not None: # handle
+response pass ``` # Development ## Maturity This SDK is in beta, and there may
+be breaking changes between versions without a major version update. Therefore,
+we recommend pinning usage to a specific package version. This way, you can
+install the same version each time without breaking changes unless you are
+intentionally looking for the latest version. ## Contributions While we value
+open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
 Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
 client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev
```

### Comparing `plex-api-client-0.6.4/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.6.5/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

