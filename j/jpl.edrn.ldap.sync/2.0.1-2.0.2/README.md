# Comparing `tmp/jpl.edrn.ldap.sync-2.0.1.tar.gz` & `tmp/jpl_edrn_ldap_sync-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpl.edrn.ldap.sync-2.0.1.tar", last modified: Wed Oct 19 20:23:30 2022, max compression
+gzip compressed data, was "jpl_edrn_ldap_sync-2.0.2.tar", last modified: Thu May  2 22:16:08 2024, max compression
```

## Comparing `jpl.edrn.ldap.sync-2.0.1.tar` & `jpl_edrn_ldap_sync-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.233932 jpl.edrn.ldap.sync-2.0.1/
--rw-r--r--   0 kelly      (501) staff       (20)    10496 2021-08-24 22:06:27.000000 jpl.edrn.ldap.sync-2.0.1/LICENSE.md
--rw-r--r--   0 kelly      (501) staff       (20)       28 2022-10-19 19:00:46.000000 jpl.edrn.ldap.sync-2.0.1/MANIFEST.in
--rw-r--r--   0 kelly      (501) staff       (20)     2765 2022-10-19 20:23:30.234059 jpl.edrn.ldap.sync-2.0.1/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)     1984 2022-10-19 18:57:20.000000 jpl.edrn.ldap.sync-2.0.1/README.md
--rw-r--r--   0 kelly      (501) staff       (20)       90 2021-08-24 22:06:51.000000 jpl.edrn.ldap.sync-2.0.1/pyproject.toml
--rw-r--r--   0 kelly      (501) staff       (20)     1221 2022-10-19 20:23:30.234631 jpl.edrn.ldap.sync-2.0.1/setup.cfg
--rw-r--r--   0 kelly      (501) staff       (20)       57 2021-08-24 22:14:37.000000 jpl.edrn.ldap.sync-2.0.1/setup.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.223389 jpl.edrn.ldap.sync-2.0.1/src/
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.226242 jpl.edrn.ldap.sync-2.0.1/src/jpl/
--rw-r--r--   0 kelly      (501) staff       (20)      125 2022-10-19 18:53:23.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/__init__.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.228790 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/
--rw-r--r--   0 kelly      (501) staff       (20)      132 2021-08-24 22:24:37.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/__init__.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.229083 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/
--rw-r--r--   0 kelly      (501) staff       (20)      146 2021-08-24 22:24:56.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/__init__.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.233290 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/
--rw-r--r--   0 kelly      (501) staff       (20)        6 2022-10-19 20:23:21.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/VERSION.txt
--rw-r--r--   0 kelly      (501) staff       (20)      199 2022-10-19 13:54:27.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/__init__.py
--rw-r--r--   0 kelly      (501) staff       (20)     2769 2022-10-19 20:22:59.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/allgroup.py
--rw-r--r--   0 kelly      (501) staff       (20)     1038 2022-10-19 18:08:49.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/constants.py
--rw-r--r--   0 kelly      (501) staff       (20)     2870 2022-10-19 18:46:23.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/groupsync.py
--rw-r--r--   0 kelly      (501) staff       (20)     7903 2022-10-19 18:51:59.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/rdf.py
--rw-r--r--   0 kelly      (501) staff       (20)     3986 2022-10-19 18:46:13.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/usersync.py
--rw-r--r--   0 kelly      (501) staff       (20)     1844 2022-10-19 14:21:38.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/utils.py
-drwxr-xr-x   0 kelly      (501) staff       (20)        0 2022-10-19 20:23:30.228226 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/
--rw-r--r--   0 kelly      (501) staff       (20)     2765 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/PKG-INFO
--rw-r--r--   0 kelly      (501) staff       (20)      789 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/SOURCES.txt
--rw-r--r--   0 kelly      (501) staff       (20)        1 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/dependency_links.txt
--rw-r--r--   0 kelly      (501) staff       (20)      157 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/entry_points.txt
--rw-r--r--   0 kelly      (501) staff       (20)       27 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/namespace_packages.txt
--rw-r--r--   0 kelly      (501) staff       (20)       33 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/requires.txt
--rw-r--r--   0 kelly      (501) staff       (20)        4 2022-10-19 20:23:30.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/top_level.txt
--rw-r--r--   0 kelly      (501) staff       (20)        1 2021-08-24 22:26:25.000000 jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/zip-safe
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.157011 jpl_edrn_ldap_sync-2.0.2/
+-rw-r--r--   0 kelly      (501) staff       (20)    10496 2021-08-24 22:06:27.000000 jpl_edrn_ldap_sync-2.0.2/LICENSE.md
+-rw-r--r--   0 kelly      (501) staff       (20)       28 2022-10-19 19:00:46.000000 jpl_edrn_ldap_sync-2.0.2/MANIFEST.in
+-rw-r--r--   0 kelly      (501) staff       (20)     2828 2024-05-02 22:16:08.156939 jpl_edrn_ldap_sync-2.0.2/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)     1984 2022-10-19 18:57:20.000000 jpl_edrn_ldap_sync-2.0.2/README.md
+-rw-r--r--   0 kelly      (501) staff       (20)       90 2021-08-24 22:06:51.000000 jpl_edrn_ldap_sync-2.0.2/pyproject.toml
+-rw-r--r--   0 kelly      (501) staff       (20)     1269 2024-05-02 22:16:08.157273 jpl_edrn_ldap_sync-2.0.2/setup.cfg
+-rw-r--r--   0 kelly      (501) staff       (20)       57 2021-08-24 22:14:37.000000 jpl_edrn_ldap_sync-2.0.2/setup.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.152686 jpl_edrn_ldap_sync-2.0.2/src/
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.153841 jpl_edrn_ldap_sync-2.0.2/src/jpl/
+-rw-r--r--   0 kelly      (501) staff       (20)      125 2022-10-19 18:53:23.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/__init__.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.155112 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/
+-rw-r--r--   0 kelly      (501) staff       (20)      132 2021-08-24 22:24:37.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/__init__.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.155232 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/
+-rw-r--r--   0 kelly      (501) staff       (20)      146 2021-08-24 22:24:56.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/__init__.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.156472 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/
+-rw-r--r--   0 kelly      (501) staff       (20)        6 2024-05-02 22:15:50.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/VERSION.txt
+-rw-r--r--   0 kelly      (501) staff       (20)      199 2022-10-19 13:54:27.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/__init__.py
+-rw-r--r--   0 kelly      (501) staff       (20)     2769 2022-10-19 20:22:59.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/allgroup.py
+-rw-r--r--   0 kelly      (501) staff       (20)     1038 2022-10-19 18:08:49.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/constants.py
+-rw-r--r--   0 kelly      (501) staff       (20)     1608 2022-12-09 15:08:17.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/crypt.py
+-rw-r--r--   0 kelly      (501) staff       (20)     3284 2024-05-02 21:56:54.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/groupsync.py
+-rw-r--r--   0 kelly      (501) staff       (20)     8539 2024-05-02 21:49:18.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/rdf.py
+-rw-r--r--   0 kelly      (501) staff       (20)     3986 2022-10-19 18:46:13.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/usersync.py
+-rw-r--r--   0 kelly      (501) staff       (20)     1844 2022-10-19 14:21:38.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/utils.py
+drwxr-xr-x   0 kelly      (501) staff       (20)        0 2024-05-02 22:16:08.156680 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/
+-rw-r--r--   0 kelly      (501) staff       (20)     2828 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/PKG-INFO
+-rw-r--r--   0 kelly      (501) staff       (20)      821 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/SOURCES.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        1 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/dependency_links.txt
+-rw-r--r--   0 kelly      (501) staff       (20)      204 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/entry_points.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       27 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/namespace_packages.txt
+-rw-r--r--   0 kelly      (501) staff       (20)       33 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/requires.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        4 2024-05-02 22:16:08.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/top_level.txt
+-rw-r--r--   0 kelly      (501) staff       (20)        1 2021-08-24 22:26:25.000000 jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/zip-safe
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/LICENSE.md` & `jpl_edrn_ldap_sync-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/PKG-INFO` & `jpl_edrn_ldap_sync-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpl.edrn.ldap.sync
-Version: 2.0.1
+Version: 2.0.2
 Summary: LDAP utilities for the Early Detection Research Network Directory
 Home-page: https://github.com/EDRN/jpl.edrn.ldap.sync
 Author: Sean Kelly
 Author-email: kelly@seankelly.biz
 License: apache-2.0
 Keywords: ldap directory cancer
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: python-ldap~=3.3.1
+Requires-Dist: rdflib~=6.2.0
 
 # ☎️ EDRN LDAP Sync
 
 This package contains utilities for the dirctory service of the [EDRN](https://edrn.nci.nih.gov/). There are three console scripts provided:
 
 -   `usersync` — adds and removes users from the EDRN RDF feed for registered people
 -   `groupsync` — adds and updates funded sites and collaborative groups from the EDRN RDF feeds for sites and committees
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/README.md` & `jpl_edrn_ldap_sync-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/setup.cfg` & `jpl_edrn_ldap_sync-2.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -38,12 +38,13 @@
 where = src
 
 [options.entry_points]
 console_scripts = 
 	all-edrn-sync = jpl.edrn.ldap.sync.allgroup:main
 	usersync = jpl.edrn.ldap.sync.usersync:main
 	groupsync = jpl.edrn.ldap.sync.groupsync:main
+	cryptpasswords = jpl.edrn.ldap.sync.crypt:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/allgroup.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/allgroup.py`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/constants.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/constants.py`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/groupsync.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/groupsync.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 '''☎️ EDRN LDAP Sync: group sync with data from the DMCC.'''
 
 from . import VERSION
 from .constants import USER_RDF_URL, SITE_RDF_URL, COMMITTEE_RDF_URL, GROUP_BASE, GROUP_OBJECT_CLASSES, USER_BASE
 from .rdf import get_rdf_people, get_rdf_sites, get_rdf_collab_groups, Group
 from .utils import add_logging_arguments, add_ldap_arguments, get_manager_password
-import sys, ldap, ldap.modlist, logging, argparse
+import sys, ldap, ldap.modlist, ldap.filter, logging, argparse
 
 __version__ = VERSION
 _logger = logging.getLogger(__name__)
 _prog_desc = 'Synchronizes EDRN groups from the DMCC SOAP (RDF) feed into the EDRN LDAP'
 
 
 def _add_to_ldap(connection: ldap.ldapobject.LDAPObject, group: Group):
@@ -54,13 +54,22 @@
     rdf_collab_groups = get_rdf_collab_groups(rdf_people, args.committee_rdf_url)
     _logger.info('Collab Groups found in DMCC RDF: %d', len(rdf_collab_groups))
 
     connection = ldap.initialize(args.url)
     password = get_manager_password(args)
     connection.simple_bind_s(args.manager_dn, password)
 
+    # Find obsolete groups?
+    # breakpoint()
+    # group_names = set(rdf_sites.keys())
+    # group_names |= set(rdf_collab_groups.keys())
+    # for group_name in list(group_names):
+    #     query = '(cn=' + ldap.filter.escape_filter_chars(group_name) + ')'
+    #     if connection.search_s('dc=edrn,dc=jpl,dc=nasa,dc=gov', ldap.SCOPE_ONELEVEL, query):
+    #         group_names.remove(group_name)
+
     for group in rdf_sites.values():
         _add_to_ldap(connection, group)
     for group in rdf_collab_groups.values():
         _add_to_ldap(connection, group)
 
     sys.exit(0)
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/rdf.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/rdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # encoding: utf-8
 
 '''☎️ EDRN LDAP Sync: Resource Description Format classes and functions.'''
 
 
-import rdflib, logging, enum
 from dataclasses import dataclass
+import rdflib, logging, enum
+from urllib.parse import urlparse
 
 _logger = logging.getLogger(__name__)
 
 
 # RDF Predicates
 # --------------
 
 _account_pred_uri  = rdflib.term.URIRef('http://xmlns.com/foaf/0.1/accountName')
 _chair_pred_uri    = rdflib.term.URIRef('http://edrn.nci.nih.gov/xml/rdf/edrn.rdf#chair')
 _cochair_pred_uri  = rdflib.term.URIRef('http://edrn.nci.nih.gov/xml/rdf/edrn.rdf#coChair')
 _com_type_pred_uri = rdflib.term.URIRef('http://edrn.nci.nih.gov/xml/rdf/edrn.rdf#committeeType')
 _email_pred_uri    = rdflib.term.URIRef('http://xmlns.com/foaf/0.1/mbox')
 _gn_pred_uri       = rdflib.term.URIRef('http://xmlns.com/foaf/0.1/givenname')
 _member_pred_uri   = rdflib.term.URIRef('http://edrn.nci.nih.gov/xml/rdf/edrn.rdf#member')
+_officer_uri       = rdflib.term.URIRef('urn:edrn:rdf:predicates:program_officer')
 _phone_pred_uri    = rdflib.term.URIRef('http://xmlns.com/foaf/0.1/phone')
 _pi_pred_uri       = rdflib.term.URIRef('http://edrn.nci.nih.gov/rdf/schema.rdf#pi')
+_scientist_uri     = rdflib.term.URIRef('urn:edrn:rdf:predicates:project_scientist')
 _sn_pred_uri       = rdflib.term.URIRef('http://xmlns.com/foaf/0.1/surname')
 _staff_pred_uri    = rdflib.term.URIRef('http://edrn.nci.nih.gov/rdf/schema.rdf#staff')
 _status_pred_uri   = rdflib.term.URIRef('http://edrn.nci.nih.gov/rdf/schema.rdf#employmentActive')
 
 
 # RDF object types
 # ----------------
@@ -112,17 +115,18 @@
 
 def get_rdf_people(url: str) -> dict:
     '''Return all people currently in RDF as a mapping from user ID to ``Person`` objects. Skip anyone who is
     without an account name.
     '''
     statements, people = parse(url), {}
     for subject_uri, predicates in statements.items():
+        person_id = urlparse(subject_uri).path.split('/')[-1]
         uid = sv(_account_pred_uri, predicates)
-        if not uid: continue
-        uid = str(uid).lower()
+        if uid:
+            uid = str(uid).lower()
 
         status = sv(_status_pred_uri, predicates)
         if not status:
             status = Status.UNKNOWN
         elif str(status) == 'Former employee':
             status = Status.INACTIVE
         else:
@@ -136,29 +140,34 @@
         email = sv(_email_pred_uri, predicates)
         if not email:
             email = 'UNKNOWN@UNKNOWN.COM'
         else:
             # Strip the 'mailto:'
             email = str(email[7:])
 
+        if status == status.INACTIVE and uid:
+            _logger.warning('Former person %s (%s, %s) has a user ID "%s"', person_id, sn, gn, uid)
+        elif status == status.ACTIVE and not uid:
+            _logger.warning('Current person %s (%s, %s) has no user ID', person_id, sn, gn)
+
         p = Person(str(uid), str(sn), str(gn), email, str(sv(_phone_pred_uri, predicates)), status, subject_uri)
         people[uid] = p
 
     return people
 
 
 def get_rdf_sites(rdf_people: dict, url: str) -> dict:
     '''Return all sites currently in RDF as a mapping from site name (which is the bizarre convention of
     the principal investigator's last name plus the name of the institution) to ``Site`` objects. We skip
     any site for which we cannot determine a PI. This takes as input the ``rdf_people`` output from
     ``get_rdf_people`` and the ``url`` to the site RDF data source.
     '''
     people = {i.subject_uri: i for i in rdf_people.values()}
     statements, sites = parse(url), {}
-    for predicates in statements.values():
+    for subject_uri, predicates in statements.items():
         if get_rdf_type(predicates) != _site_type: continue     # Not a Site? Skip it
         title = sv(rdflib.DCTERMS.title, predicates)            # Grab thte name of the site
         title = str(title).strip().replace(',', '')             # DMCC data is always weirdly padded; see [1]
         if not title: continue                                  # Unnamed? Skipt it
         pi = people.get(sv(_pi_pred_uri, predicates))           # Find the PI
         if not pi: continue                                     # No principal investigator? Skip it
         site_name = f'{pi.sn} {title}'                          # Figure out weird site name we use in EDRN
@@ -185,17 +194,18 @@
         if not title: continue
         title = title[0:title.rindex(' Cancers Research Group')]
         members = set()
         chair = people.get(sv(_chair_pred_uri, predicates))
         if chair: members.add(chair)
         cochair = people.get(sv(_cochair_pred_uri, predicates))
         if cochair: members.add(cochair)
-        for person_uri in predicates.get(_member_pred_uri, []):
-            member = people.get(person_uri)
-            if member: members.add(member)
+        for predicate in (_member_pred_uri, _scientist_uri, _officer_uri):
+            for person_uri in predicates.get(predicate, []):
+                member = people.get(person_uri)
+                if member: members.add(member)
         group = Committee(title, members)
         groups[title] = group
     return groups
 
 
 # [1] While the common name for some sites may indeed be "Boutros The University of California, Los Angeles",
 # the best practices for LDAP (see https://cutt.ly/aBNFeUE) suggest avoiding any special characaters in
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/usersync.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/usersync.py`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl/edrn/ldap/sync/utils.py` & `jpl_edrn_ldap_sync-2.0.2/src/jpl/edrn/ldap/sync/utils.py`

 * *Files identical despite different names*

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/PKG-INFO` & `jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpl.edrn.ldap.sync
-Version: 2.0.1
+Version: 2.0.2
 Summary: LDAP utilities for the Early Detection Research Network Directory
 Home-page: https://github.com/EDRN/jpl.edrn.ldap.sync
 Author: Sean Kelly
 Author-email: kelly@seankelly.biz
 License: apache-2.0
 Keywords: ldap directory cancer
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: python-ldap~=3.3.1
+Requires-Dist: rdflib~=6.2.0
 
 # ☎️ EDRN LDAP Sync
 
 This package contains utilities for the dirctory service of the [EDRN](https://edrn.nci.nih.gov/). There are three console scripts provided:
 
 -   `usersync` — adds and removes users from the EDRN RDF feed for registered people
 -   `groupsync` — adds and updates funded sites and collaborative groups from the EDRN RDF feeds for sites and committees
```

### Comparing `jpl.edrn.ldap.sync-2.0.1/src/jpl.edrn.ldap.sync.egg-info/SOURCES.txt` & `jpl_edrn_ldap_sync-2.0.2/src/jpl.edrn.ldap.sync.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 src/jpl.edrn.ldap.sync.egg-info/zip-safe
 src/jpl/edrn/__init__.py
 src/jpl/edrn/ldap/__init__.py
 src/jpl/edrn/ldap/sync/VERSION.txt
 src/jpl/edrn/ldap/sync/__init__.py
 src/jpl/edrn/ldap/sync/allgroup.py
 src/jpl/edrn/ldap/sync/constants.py
+src/jpl/edrn/ldap/sync/crypt.py
 src/jpl/edrn/ldap/sync/groupsync.py
 src/jpl/edrn/ldap/sync/rdf.py
 src/jpl/edrn/ldap/sync/usersync.py
 src/jpl/edrn/ldap/sync/utils.py
```

