# Comparing `tmp/knowsmore-0.1.37.tar.gz` & `tmp/knowsmore-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowsmore-0.1.37.tar", last modified: Fri Aug 25 02:52:53 2023, max compression
+gzip compressed data, was "knowsmore-0.1.38.tar", last modified: Fri May  3 11:55:59 2024, max compression
```

## Comparing `knowsmore-0.1.37.tar` & `knowsmore-0.1.38.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.176055 knowsmore-0.1.37/
--rw-r--r--   0 runner    (1001) docker     (999)    35121 2023-08-25 02:51:59.000000 knowsmore-0.1.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     9800 2023-08-25 02:52:53.176055 knowsmore-0.1.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     8456 2023-08-25 02:51:59.000000 knowsmore-0.1.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.172055 knowsmore-0.1.37/knowsmore/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      115 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4097 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/args.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.172055 knowsmore-0.1.37/knowsmore/cmd/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    68560 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/bloodhound.py
--rw-r--r--   0 runner    (1001) docker     (999)     2375 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/createdb.py
--rw-r--r--   0 runner    (1001) docker     (999)     6852 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/find.py
--rw-r--r--   0 runner    (1001) docker     (999)    20281 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/hashes.py
--rw-r--r--   0 runner    (1001) docker     (999)     6240 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/precomputed.py
--rw-r--r--   0 runner    (1001) docker     (999)    31611 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/secretsdump.py
--rw-r--r--   0 runner    (1001) docker     (999)     6532 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/splunk.py
--rw-r--r--   0 runner    (1001) docker     (999)    11551 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/stats.py
--rw-r--r--   0 runner    (1001) docker     (999)     4511 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/userpass.py
--rw-r--r--   0 runner    (1001) docker     (999)     4334 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/wipe.py
--rw-r--r--   0 runner    (1001) docker     (999)    14773 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmd/wordlist.py
--rw-r--r--   0 runner    (1001) docker     (999)     4247 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/cmdbase.py
--rw-r--r--   0 runner    (1001) docker     (999)     4185 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     3674 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/knowsmore.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.172055 knowsmore-0.1.37/knowsmore/libs/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2438 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/libs/bloodhoundsync.py
--rw-r--r--   0 runner    (1001) docker     (999)     4780 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/libs/exporterbase.py
--rw-r--r--   0 runner    (1001) docker     (999)     1007 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/libs/ntdsuseraccount.py
--rw-r--r--   0 runner    (1001) docker     (999)   135758 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/libs/secretsdump.py
--rw-r--r--   0 runner    (1001) docker     (999)      417 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/module.py
--rw-r--r--   0 runner    (1001) docker     (999)     8461 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/password.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.176055 knowsmore-0.1.37/knowsmore/util/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3775 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/color.py
--rw-r--r--   0 runner    (1001) docker     (999)    18179 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/database.py
--rw-r--r--   0 runner    (1001) docker     (999)    10504 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/knowsmoredb.py
--rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     6413 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/process.py
--rw-r--r--   0 runner    (1001) docker     (999)     5726 2023-08-25 02:51:59.000000 knowsmore-0.1.37/knowsmore/util/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 02:52:53.172055 knowsmore-0.1.37/knowsmore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     9800 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      237 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-25 02:52:53.000000 knowsmore-0.1.37/knowsmore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      322 2023-08-25 02:51:59.000000 knowsmore-0.1.37/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-25 02:52:53.176055 knowsmore-0.1.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3004 2023-08-25 02:51:59.000000 knowsmore-0.1.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.824613 knowsmore-0.1.38/
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-03 11:55:26.000000 knowsmore-0.1.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-05-03 11:55:59.824613 knowsmore-0.1.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-03 11:55:26.000000 knowsmore-0.1.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.816613 knowsmore-0.1.38/knowsmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.820613 knowsmore-0.1.38/knowsmore/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68560 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/bloodhound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/createdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20281 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/precomputed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31611 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/secretsdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/splunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/userpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/wipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15650 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmd/wordlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/cmdbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/knowsmore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.820613 knowsmore-0.1.38/knowsmore/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/libs/bloodhoundsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/libs/exporterbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/libs/ntdsuseraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135758 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/libs/secretsdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.824613 knowsmore-0.1.38/knowsmore/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17582 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/knowsmoredb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-03 11:55:26.000000 knowsmore-0.1.38/knowsmore/util/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:55:59.820613 knowsmore-0.1.38/knowsmore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 11:55:59.000000 knowsmore-0.1.38/knowsmore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-03 11:55:26.000000 knowsmore-0.1.38/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:55:59.824613 knowsmore-0.1.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-03 11:55:26.000000 knowsmore-0.1.38/setup.py
```

### Comparing `knowsmore-0.1.37/LICENSE` & `knowsmore-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/PKG-INFO` & `knowsmore-0.1.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: knowsmore
-Version: 0.1.37
+Version: 0.1.38
 Summary: KnowsMore is a swiss army knife tool for pentesting Microsoft Active Directory (NTLM Hashes, BloodHound, NTDS and DCSync).
 Home-page: https://github.com/helviojunior/knowsmore
 Author: Helvio Junior  (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/knowsmore
 Project-URL: Source, https://github.com/helviojunior/knowsmore
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -208,20 +207,27 @@
 knowsmore --word-list -o "~/Desktop/Wordlist/my_custom_wordlist.txt" --batch --name company_name
 ```
 
 ## Importing cracked hashes
 
 ### Cracking hashes
 
-In order to crack the hashes, I usually use `hashcat` with the command bellow
+First extract all hashes to a txt file
 
 ```bash
-# Extract NTLM hashes from file
+# Extract NTLM hashes to file
+nowsmore --ntlm-hash --export-hashes "~/Desktop/ntlm_hash.txt"
+
+# Or, extract NTLM hashes from NTDS file
 cat ~/Desktop/client_name.ntds | cut -d ':' -f4 > ntlm_hashes.txt
+```
 
+In order to crack the hashes, I usually use `hashcat` with the command bellow
+
+```bash
 # Wordlist attack
 hashcat -m 1000 -a 0 -O -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" "~/Desktop/Wordlist/*"
 
 # Mask attack
 hashcat -m 1000 -a 3 -O --increment --increment-min 4 -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" ?a?a?a?a?a?a?a?a
 ```
 
@@ -269,8 +275,7 @@
 ```
 server.bolt.listen_address=0.0.0.0:7687
 ```
 
 # To do
 
 [Check the TODO file](TODO.md)
-
```

### Comparing `knowsmore-0.1.37/README.md` & `knowsmore-0.1.38/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,20 +173,27 @@
 knowsmore --word-list -o "~/Desktop/Wordlist/my_custom_wordlist.txt" --batch --name company_name
 ```
 
 ## Importing cracked hashes
 
 ### Cracking hashes
 
-In order to crack the hashes, I usually use `hashcat` with the command bellow
+First extract all hashes to a txt file
 
 ```bash
-# Extract NTLM hashes from file
+# Extract NTLM hashes to file
+nowsmore --ntlm-hash --export-hashes "~/Desktop/ntlm_hash.txt"
+
+# Or, extract NTLM hashes from NTDS file
 cat ~/Desktop/client_name.ntds | cut -d ':' -f4 > ntlm_hashes.txt
+```
 
+In order to crack the hashes, I usually use `hashcat` with the command bellow
+
+```bash
 # Wordlist attack
 hashcat -m 1000 -a 0 -O -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" "~/Desktop/Wordlist/*"
 
 # Mask attack
 hashcat -m 1000 -a 3 -O --increment --increment-min 4 -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" ?a?a?a?a?a?a?a?a
 ```
```

### Comparing `knowsmore-0.1.37/knowsmore/args.py` & `knowsmore-0.1.38/knowsmore/args.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/bloodhound.py` & `knowsmore-0.1.38/knowsmore/cmd/bloodhound.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/createdb.py` & `knowsmore-0.1.38/knowsmore/cmd/createdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,12 +59,12 @@
         if os.path.isfile(self.db_name) and self.force:
             Color.pl(
                 '{!} {W}Database exists (you have 10 seconds to abort...) to prevent overwriting.')
             time.sleep(10)
 
             os.remove(self.db_name)
 
-        Database(auto_create=True,
-                 db_name=self.db_name)
+        KnowsMoreDB(auto_create=True,
+                    db_name=self.db_name)
 
         Logger.pl('{+} {C}Database created {O}%s{W}' % self.db_name)
```

### Comparing `knowsmore-0.1.37/knowsmore/cmd/find.py` & `knowsmore-0.1.38/knowsmore/cmd/find.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/hashes.py` & `knowsmore-0.1.38/knowsmore/cmd/hashes.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/precomputed.py` & `knowsmore-0.1.38/knowsmore/cmd/precomputed.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/secretsdump.py` & `knowsmore-0.1.38/knowsmore/cmd/secretsdump.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/splunk.py` & `knowsmore-0.1.38/knowsmore/cmd/splunk.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/stats.py` & `knowsmore-0.1.38/knowsmore/cmd/stats.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/userpass.py` & `knowsmore-0.1.38/knowsmore/cmd/userpass.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/wipe.py` & `knowsmore-0.1.38/knowsmore/cmd/wipe.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/cmd/wordlist.py` & `knowsmore-0.1.38/knowsmore/cmd/wordlist.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     max_size = 32
     level = 3
     padding = False
     no_leets = False
     small = False
     unique_chars = []
     unique_ch_b = 0
-    char_space = LEETS1
+    char_space = None
     filename = None
     batch = False
     check_database = False
     append_file = False
 
     def __init__(self):
         super().__init__('word-list', 'Generates a wordlist based on one word (generally, company name)')
@@ -115,16 +115,14 @@
             else:
                 Logger.pl('{!} {R}error: could not open NTLM hashes file {W}\r\n')
                 Tools.exit_gracefully(1)
 
         # Database not yet needed
         #self.db = self.open_db(args)
 
-        self.setup()
-
         return True
 
     def setup(self):
 
         if self.level < 1:
             self.level = 1
 
@@ -134,19 +132,31 @@
         if self.min_size < 1:
             self.min_size = 1
 
         if self.no_leets:
             self.char_space = LEETS2
         elif self.small or self.level == 2:
             self.char_space = LEETS3
+        else:
+            self.char_space = LEETS1
+
+        # Add non listed chars (and used by name) in char_space
+        self.char_space = {
+            **self.char_space,
+            **{
+                c: c for c in self.name
+                if self.char_space.get(c, None) is None
+            }
+        }
 
         self.unique_chars = set([v for l1 in [list(value) for value in self.char_space.values()] for v in l1])
         self.unique_ch_b = int(np.sum([len(v.encode("UTF-8")) for v in self.unique_chars]))
 
     def run(self):
+        self.setup()
 
         estimated_size = self.calculate()
         Logger.pl(
             '{+} {W}KnowsMore will generate +- the following amount of data: {O}%s{W}.' % Tools.sizeof_fmt(
                 estimated_size, start_unit="K")
         )
         stat = shutil.disk_usage(Path(self.filename).parent)
@@ -205,14 +215,27 @@
                 Logger.pl('{!} {R}error: could not open NTLM hashes file {W}\r\n')
                 Tools.exit_gracefully(1)
         finally:
             file_stats = os.stat(self.filename).st_size
             Logger.pl('{+} {W}Generate {O}%d{W} lines ({O}%s{W}) to {G}%s{W}' % (lines, Tools.sizeof_fmt(file_stats), self.filename))
 
     def calculate(self) -> int:
+
+        if self.name is None:
+            return 0
+
+        if not isinstance(self.name, str):
+            raise Exception("Invalid type received: %s" % type(self.name))
+
+        if self.name.strip() == 0:
+            return 0
+
+        if self.char_space is None:
+            self.setup()
+
         s = len(self.name)
         leet_lines = np.prod([len([chars for chars in self.char_space.get(c)]) for c in self.name])
         padding_space = 0
         if len(self.name) < self.min_size and self.padding:
             s1 = self.min_size - len(self.name)
             if s1 > 0:
                 pl = math.pow(len(self.unique_chars), s1)
@@ -229,14 +252,25 @@
             float(padding_space)/1024.0
         )
         if r < 0:
             r = 0
         return r
 
     def generate(self, word, index) -> list:
+
+        if index <= 1:
+            if self.name is None:
+                return []
+
+            if not isinstance(self.name, str):
+                raise Exception("Invalid type received: %s" % type(self.name))
+
+            if self.name.strip() == 0:
+                return []
+
         c = word[index:index + 1]
         if c in self.char_space:
             for i, s in enumerate(self.char_space.get(c)):
                 if index == len(word) - 1:
                     p = "%s%s" % (word[0:index], s)
                     if len(p) < self.min_size and self.padding:
                         yield from self.add_padding(p)
```

### Comparing `knowsmore-0.1.37/knowsmore/cmdbase.py` & `knowsmore-0.1.38/knowsmore/cmdbase.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/config.py` & `knowsmore-0.1.38/knowsmore/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
         a1[0] = 'knowsmore'
         for a in a1:
             Configuration.cmd_line += "%s " % a
 
         module = args.get_module()
 
         if module is None:
-            Color.pl('{!} {R}error: missing a mandatory option, use -h help{W}\r\n')
-            exit(1)
+            Configuration.mandatory()
 
         Configuration.verbose = args.args.v
 
         Color.pl('{+} {W}Startup parameters')
         Logger.pl('     {C}command line:{O} %s{W}' % Configuration.cmd_line)
 
         if Configuration.verbose > 0:
@@ -78,15 +77,15 @@
         Logger.pl('     {C}module:{O} %s{W}' % module.name)
 
         if args.args.company is not None and args.args.company.strip(' .,'):
             Configuration.company = [] + Tools.clear_string(args.args.company).split(',')
 
         if len(Configuration.company) > 0:
             for c in Configuration.company:
-                if len(c.strip()) >= 7:
+                if len(c.strip()) >= 8:
                     Color.pl('{!} {R}error: company name {O}%s{R} reached maximum name length. {G}The name must have up to 7 digits.{W}\r\n' % c)
                     exit(1)
 
         if len(Configuration.company) > 0:
             Logger.pl('     {C}company name:{O} %s{W}' % ', '.join(Configuration.company))
 
         if not module.load_from_arguments(args.args):
@@ -99,14 +98,19 @@
 
         db_name = os.path.abspath(args.args.dbfile.strip())
         Logger.pl('     {C}database file:{O} %s{W}' % db_name)
 
         print('  ')
 
     @staticmethod
+    def mandatory():
+        Logger.pl('{!} {R}error: missing a mandatory option, use -h help{W}\r\n')
+        exit(1)
+
+    @staticmethod
     def get_banner():
             Configuration.version = str(__version__)
 
             return '''\
 
 {G}KnowsMore {D}v%s{W}{G} by Helvio Junior{W}
 {W}{D}Active Directory, BloodHound, NTDS hashes and Password Cracks correlation tool{W}
```

### Comparing `knowsmore-0.1.37/knowsmore/knowsmore.py` & `knowsmore-0.1.38/knowsmore/knowsmore.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/libs/bloodhoundsync.py` & `knowsmore-0.1.38/knowsmore/libs/bloodhoundsync.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/libs/exporterbase.py` & `knowsmore-0.1.38/knowsmore/libs/exporterbase.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/libs/ntdsuseraccount.py` & `knowsmore-0.1.38/knowsmore/libs/ntdsuseraccount.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/libs/secretsdump.py` & `knowsmore-0.1.38/knowsmore/libs/secretsdump.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/password.py` & `knowsmore-0.1.38/knowsmore/password.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/util/color.py` & `knowsmore-0.1.38/knowsmore/util/color.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/util/database.py` & `knowsmore-0.1.38/knowsmore/util/knowsmoredb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,325 +1,298 @@
 #!/usr/bin/python3
 # -*- coding: UTF-8 -*-
-import math
-import shutil
+import datetime
 import sys, os.path
 import sqlite3
 import string, base64
-from functools import reduce
+import json
+import hashlib
 from sqlite3 import Connection, OperationalError, IntegrityError, ProgrammingError
 
+from .color import Color
+from .database import Database
+from ..password import Password
 
-# TODO: use this decorator to wrap commit/rollback in a try/except block ?
-# see http://www.kylev.com/2009/05/22/python-decorators-and-database-idioms/
-def connect(func):
-    """Decorator to (re)open a sqlite database connection when needed.
 
-    A database connection must be open when we want to perform a database query
-    but we are in one of the following situations:
-    1) there is no connection
-    2) the connection is closed
-
-    Parameters
-    ----------
-    func : function
-        function which performs the database query
-
-    Returns
-    -------
-    inner func : function
-    """
-
-    def inner_func(self, *args, **kwargs):
-        if f'{func.__module__}.{func.__qualname__}' != f'{Database.__module__}.{Database.__qualname__}.{func.__name__}':
-            raise Exception('The connect decorator cannot be used outside of Database class')
-
-        if not isinstance(self, Database):
-            raise Exception('The connect decorator cannot be used outside of Database class')
-
-        conn = kwargs.get('conn', None) if kwargs is not None else None
-        if conn is None:
-            conn = self.connect_to_db()
-
-        return func(self, conn, *args, **kwargs)
-
-    return inner_func
-
-
-class Database(object):
-    db_name = ""
-
-    # Static value
-    db_connection = None
-    constraints = []
+class KnowsMoreDB(Database):
+    dbName = ""
 
     def __init__(self, auto_create=True, db_name=None):
 
-        self.db_name = db_name
-
-        if not os.path.isfile(self.db_name):
-            if auto_create:
-                self.create_db()
-            else:
-                raise Exception("Database not found")
-        else:
-            self.connect_to_db()
-
-    @connect
-    def insert_one(self, conn, table_name, **kwargs):
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-        sql = "INSERT INTO {} ({}) VALUES ({})" \
-            .format(table_name, ','.join(columns), ', '.join(['?'] * len(columns)))
-        conn.execute(sql, values)
-        conn.commit()
-
-    @connect
-    def insert_ignore_one(self, conn, table_name, **kwargs):
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-        sql = "INSERT OR IGNORE INTO {} ({}) VALUES ({})" \
-            .format(table_name, ','.join(columns), ', '.join(['?'] * len(columns)))
-        conn.execute(sql, values)
-        conn.commit()
-
-    @connect
-    def insert_replace_one(self, conn, table_name, **kwargs):
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-        sql = "INSERT OR REPLACE INTO {} ({}) VALUES ({})" \
-            .format(table_name, ','.join(columns), ', '.join(['?'] * len(columns)))
-        conn.execute(sql, values)
-        conn.commit()
-
-    @connect
-    def insert_update_one(self, conn: str, table_name: str, **kwargs):
-        self.insert_update_one_exclude(table_name, [], **kwargs)
-
-    @connect
-    def insert_update_one_exclude(self, conn: str, table_name: str, exclude_on_update: list = [], **kwargs):
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-        sql = "INSERT OR IGNORE INTO {} ({}) VALUES ({})" \
-            .format(table_name, ','.join(columns), ', '.join(['?'] * len(columns)))
-        c = conn.execute(sql, values)
-
-        # No inserted, need to update
-        if c.rowcount == 0:
-            table_name = self.scrub(table_name)
-            f_columns = self.constraints[table_name]
-            f_values = tuple([kwargs.get(c, None) for c in f_columns],)
-            args = {k: v for k, v in kwargs.items() if k not in exclude_on_update}
-            (u_columns, u_values) = self.parse_args(args)
-
-            sql = f"UPDATE {table_name} SET "
-            sql += "{}".format(', '.join([f'{col} = ?' for col in u_columns]))
-            if len(f_columns) > 0:
-                sql += " WHERE {}".format(f' and '.join([f'{col} = ?' for col in f_columns]))
-            conn.execute(sql, tuple(u_values + f_values, ))
-            conn.commit()
-
-        conn.commit()
-
-
-    @connect
-    def select(self, conn, table_name, **kwargs):
+        if db_name is None:
+            db_name = "knowsmore.db"
 
-        operator = self.scrub(kwargs.get('__operator', 'and'))
+        super().__init__(
+            auto_create=auto_create,
+            db_name=db_name
+        )
+        self.fill_data()
+
+    def has_data(self) -> bool:
+        return self.select_count('passwords') > 0
+
+    def check_open(self) -> bool:
+        return self.select_count('passwords') >= 0
+
+    def insert_group(self, domain: int, object_identifier: str, name: str, dn: str = '', members: str = '',
+                     membership: str = '') -> int:
+
+        if domain == -1:
+            raise Exception('Invalid domain')
+
+        if object_identifier is None or object_identifier.strip() == '':
+            raise Exception('object_identifier cannot be empty')
+
+        #grp = self.select('groups',
+        #                  object_identifier=object_identifier
+        #                  )
+
+        #if len(grp) == 0:
+        #    self.insert_one('groups',
+        self.insert_update_one('groups',
+                               domain_id=domain,
+                               name=name,
+                               object_identifier=object_identifier,
+                               dn=dn,
+                               members=members,
+                               membership=membership
+                               )
+
+    def update_password(self, password: Password, **kwargs):
+
+        filter_data = {
+            'ntlm_hash': password.ntlm_hash,
+        }
+
+        pwd = {
+            'password': password.clear_text,
+            'length': password.length,
+            'entropy': password.entropy,
+            'strength': password.strength,
+            'upper': password.upper,
+            'lower': password.lower,
+            'digit': password.digit,
+            'special': password.special,
+            'latin': password.latin,
+            'md5_hash': password.md5_hash,
+            'sha1_hash': password.sha1_hash,
+            'sha256_hash': password.sha256_hash,
+            'sha512_hash': password.sha512_hash,
+        }
+
+        pwd.update(kwargs)
+
+        self.update('passwords', filter_data, **pwd)
+
+        # Get all credentials (user/computer) using this password
+        credentials = self.select_raw(
+            sql='select distinct c.credential_id, c.name, c.full_name, c.user_data_similarity from credentials as c '
+                'inner join passwords as p on c.password_id = p.password_id '
+                'where c.type = "U" '
+                'and c.full_name != "" '
+                'and p.ntlm_hash = ?',
+            args=[password.ntlm_hash]
+        )
+        for c in credentials:
+            names = [
+                n.lower() for n in c['full_name'].split(' ')
+                if len(n) > 3
+            ]
+            score = sorted(
+                [password.calc_ratio(n) for n in names]
+            )[-1]
+            if int(c['user_data_similarity']) != int(score):
+                self.update('credentials',
+                            filter_data={'credential_id': c['credential_id']},
+                            user_data_similarity=score
+                            )
+
+    def insert_password_manually(self, password: Password, **kwargs):
+
+        self.insert_ignore_one('pre_computed',
+                               ntlm_hash=password.ntlm_hash,
+                               password=password.clear_text if password.length > 0 else ''
+                               )
+
+        self.update_password(password, **kwargs)
+
+        self.insert_update_one('pre_computed',
+                               ntlm_hash=password.ntlm_hash,
+                               md5_hash=password.md5_hash,
+                               sha1_hash=password.sha1_hash,
+                               sha256_hash=password.sha256_hash,
+                               sha512_hash=password.sha512_hash,
+                               password=password.clear_text,
+                               )
+
+    def insert_or_update_bloodhound_object(self, label: str, object_id: str, filter_type: str = 'objectid',  **props):
+
+        object_id = object_id.upper()
+
+        name = props.get('name', '')
+        domain = props.get('domain', '').upper()
+        name = name.replace(f'@{domain}', '').replace(f'.{domain}', '')
+
+        rid = ''
+        if object_id[0:2] == "S-" and \
+                (label.lower() == 'group' or label.lower() == 'user' or label.lower() == 'machine'):
+            rid = object_id.split('-')[-1]
+
+        self.insert_update_one(
+            'bloodhound_objects',
+            object_id=object_id,
+            filter_type=filter_type,
+            object_label=label,
+            name=name,
+            r_id=rid,
+            props=json.dumps(props)
+        )
+
+    def insert_or_update_bloodhound_edge(self, source: str, target: str, source_label: str, target_label: str,
+                                         edge_type: str, edge_props: str, filter_type: str = 'objectid',
+                                         props: dict = {}):
+
+        txt_props = json.dumps(props)
+        checksum = hashlib.md5(
+            f'{source_label}:{target_label}:{edge_type}:{source}:{target}:{txt_props}'.encode("UTF-8")
+        ).hexdigest().lower()
+
+        data = dict(
+            edge_id=checksum,
+            source_id=source,
+            destination_id=target,
+            edge_props=edge_props,
+            source_label=source_label,
+            target_label=target_label,
+            edge_type=edge_type,
+            source_filter_type=filter_type,
+            updated_date=datetime.datetime.utcnow(),
+            props=txt_props
+        )
+
+        self.insert_update_one('bloodhound_edge', **data)
+
+        from ..config import Configuration
+        from .tools import Tools
+        if Configuration.verbose >= 4:
+            Color.pl('{*} {O}insert_or_update_bloodhound_edge: {G}%s{W}{D}{W}' % (
+                json.dumps(data, default=Tools.json_serial)))
+
+    def insert_or_update_credential(self, domain: int, username: str, ntlm_hash: str,
+                                    dn: str = '', groups: str = '', object_identifier: str = '',
+                                    type: str = 'U', full_name: str = '', enabled: bool = True,
+                                    pwd_last_set: datetime.datetime = datetime.datetime(1970, 1, 1, 0, 0, 0, 0)):
+        try:
+
+            # Hard-coded empty password
+            update_password = True
+            if ntlm_hash is None or ntlm_hash.strip == '':
+                update_password = False
+                ntlm_hash = '31d6cfe0d16ae931b73c59d7e0c089c0'
+
+            passwd = self.select_first('passwords', ntlm_hash=ntlm_hash)
+            password_id = -1 if passwd is None else passwd['password_id']
+
+            if password_id == -1:
+                self.insert_one('passwords', domain_id=domain, ntlm_hash=ntlm_hash)
+
+                passwd = self.select_first('passwords', ntlm_hash=ntlm_hash)
+                password_id = -1 if passwd is None else passwd['password_id']
+
+            if password_id == -1:
+                raise Exception('Password not found at database')
+
+            data = {
+                'domain_id': domain,
+                'name': username,
+                'type': type,
+                'enabled': enabled,
+                'password_id': password_id
+            }
+            if full_name is not None:
+                data['full_name'] = full_name
+            if dn is not None:
+                data['dn'] = dn
+            if groups is not None:
+                data['groups'] = groups
+            if object_identifier is not None:
+                data['object_identifier'] = object_identifier
+            if pwd_last_set is not None and pwd_last_set.year > 1970:
+                data['pwd_last_set'] = pwd_last_set
+
+            self.insert_update_one_exclude('credentials',
+                                           exclude_on_update=['password_id'] if not update_password else [],
+                                           **data)
+
+        except Exception as e:
+            Color.pl('{!} {R}Error inserting credential data:{O} %s{W}' % str(e))
+        pass
+
+    def insert_or_get_domain(self, domain: str, dn: str = '', object_identifier: str = '') -> int:
+
+        if domain is None or domain.strip() == '':
+            raise Exception('Domain cannot be empty')
+
+        domain = domain.lower()
+        dn = '' if dn is None else dn.lower()
+        object_identifier = '' if object_identifier is None else object_identifier.strip()
+
+        f = {
+            '__operator': 'or',
+            'name': domain.lower()
+        }
+        if dn is not None and dn != '':
+            f['dn'] = dn
+
+        if f is None and object_identifier is not None and object_identifier != '':
+            f['object_identifier'] = object_identifier
+
+        domain_id = self.get_domain(**f)
+
+        if domain_id == -1:
+            data = {
+                'name': domain.lower()
+            }
+
+            if dn is not None and dn != '':
+                data['dn'] = dn
 
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
+            if object_identifier is not None and object_identifier != '':
+                data['object_identifier'] = object_identifier
 
-        sql = f"SELECT * FROM {table_name}"
-        if len(columns) > 0:
-            sql += " WHERE {}".format(f' {operator} '.join([f'{col} = ?' for col in columns]))
+            self.insert_ignore_one('domains', **data)
 
-        cursor = conn.execute(sql, values)
-        if cursor.rowcount == 0:
-            return []
+            domain_id = self.get_domain(**f)
 
-        columns = cursor.description
-        return [{columns[index][0]: column for index, column in enumerate(value)} for value in cursor.fetchall()]
-
-    def select_first(self, table_name, **kwargs):
-        data = self.select(table_name, **kwargs)
-        if len(data) == 0:
-            return None
-        return data[0]
-
-    @connect
-    def select_raw(self, conn, sql: str, args: any):
-        cursor = conn.execute(sql, tuple(args,))
-        if cursor.rowcount == 0:
-            return []
-        columns = cursor.description
-        return [{columns[index][0]: column for index, column in enumerate(value)} for value in cursor.fetchall()]
-
-    @connect
-    def select_count(self, conn, table_name, **kwargs) -> int:
-
-        operator = self.scrub(kwargs.get('__operator', 'and'))
-
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-
-        sql = f"SELECT count(*) FROM {table_name}"
-        if len(columns) > 0:
-            sql += " WHERE {}".format(f' {operator} '.join([f'{col} = ?' for col in columns]))
-        cursor = conn.execute(sql, values)
-        if cursor.rowcount == 0:
-            return 0
-        data = cursor.fetchone()
-
-        return int(data[0])
-
-    @connect
-    def delete(self, conn, table_name, **kwargs) -> None:
-
-        operator = self.scrub(kwargs.get('__operator', 'and'))
-
-        table_name = self.scrub(table_name)
-        (columns, values) = self.parse_args(kwargs)
-
-        sql = f"DELETE FROM {table_name}"
-        if len(columns) > 0:
-            sql += " WHERE {}".format(f' {operator} '.join([f'{col} = ?' for col in columns]))
-        conn.execute(sql, values)
-        conn.commit()
-
-    @connect
-    def update(self, conn, table_name, filter_data, **kwargs):
-
-        operator = self.scrub(kwargs.get('__operator', 'and'))
-
-        table_name = self.scrub(table_name)
-        (f_columns, f_values) = self.parse_args(filter_data)
-        (u_columns, u_values) = self.parse_args(kwargs)
-
-        sql = f"UPDATE {table_name} SET "
-        sql += "{}".format(', '.join([f'{col} = ?' for col in u_columns]))
-        if len(f_columns) > 0:
-            sql += " WHERE {}".format(f' {operator} '.join([f'{col} = ?' for col in f_columns]))
-        conn.execute(sql, tuple(u_values + f_values, ))
-        conn.commit()
-
-    def get_contraints(self) -> dict:
-        sql = ('SELECT '
-               '  m.tbl_name AS table_name, '
-               '  il.name AS key_name, '
-               '  ii.name AS column_name '
-               'FROM  '
-               '  sqlite_master AS m,  '
-               '  pragma_index_list(m.name) AS il,  '
-               '  pragma_index_info(il.name) AS ii  '
-               'WHERE  '
-               '  m.type = "table" AND  '
-               '  il.origin = "u"  '
-               'ORDER BY table_name, key_name, ii.seqno')
-
-        cursor = Database.db_connection.execute(sql)
-        columns = cursor.description
-        db_scheme = [{columns[index][0]: column for index, column in enumerate(value)} for value in cursor.fetchall()]
-
-        if len(db_scheme) > 0:
-            self.constraints = reduce(lambda a, b: {**a, **b},
-                                      [{table: [
-                                            v['column_name'] for idx, v in enumerate(db_scheme)
-                                            if v['table_name'] == table
-                                        ]} for table in set([t['table_name'] for t in db_scheme])])
         else:
-            self.constraints = {}
-
-        return self.constraints
-
-    def parse_args(self, source_dict) -> tuple:
-        if source_dict is None:
-            return [], tuple([])
-
-        if not isinstance(source_dict, dict):
-            raise Exception('kwargs is not a dictionary')
-
-        columns = []
-        values = []
-
-        for key, value in source_dict.items():
-            try:
-                if key[0:2] != '__':
-                    columns.append(f"[{self.scrub(key)}]")
-                    values.append(value)
-            except Exception as e:
-                raise Exception(f'Error parsing {key}: {value}', e)
-
-        return columns, tuple(values, )
-
-    def connect_to_db(self, check: bool = True) -> Connection:
-        """Connect to a sqlite DB. Create the database if there isn't one yet.
-
-        Open a connection to a SQLite DB (either a DB file or an in-memory DB).
-        When a database is accessed by multiple connections, and one of the
-        processes modifies the database, the SQLite database is locked until that
-        transaction is committed.
-
-        Returns
-        -------
-        connection : sqlite3.Connection
-            connection object
-        """
-
-        if Database.db_connection is not None:
-            return Database.db_connection
-
-        conn = sqlite3.connect(self.db_name, detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES)
-        conn.create_function('log', 2, math.log)
-
-        if check:
-            try:
-                # I don't know if this is the simplest and fastest query to try
-                conn.execute(
-                    'SELECT name FROM sqlite_temp_master WHERE type="table";')
-                pass
-            except (AttributeError, ProgrammingError) as e:
-                raise Exception(f'Fail connecting to SQLite file: {self.db_name}', e)
-
-        shutil.copy(self.db_name, f'{self.db_name}.bkp')
-
-        cursor = conn.cursor()
-        # www.sqlite.org/pragma.html
-        # https://blog.devart.com/increasing-sqlite-performance.html
-        cursor.execute("PRAGMA temp_store = MEMORY")
-        # cursor.execute("PRAGMA page_size = 4096")
-        # cursor.execute("PRAGMA cache_size = 10000")
-        cursor.execute("PRAGMA locking_mode=EXCLUSIVE")
-        cursor.execute("PRAGMA synchronous=OFF")
-        cursor.execute("PRAGMA journal_mode=MEMORY")
-        # cursor.execute("PRAGMA foreign_keys=ON")
-
-        Database.db_connection = conn
-
-        # get database constraints
-        self.get_contraints()
-
-        return Database.db_connection
-
-    def scrub(self, input_string):
-        return Database.scrub(input_string)
-
-    @staticmethod
-    def scrub(input_string):
-        """Clean an input string (to prevent SQL injection).
-
-        Parameters
-        ----------
-        input_string : str
-
-        Returns
-        -------
-        str
-        """
-        return ''.join(k for k in input_string if k.isalnum() or k in '_-')
+            data = {
+                'name': domain.lower()
+            }
+
+            if dn is not None and dn != '':
+                data['dn'] = dn
+
+            if object_identifier is not None and object_identifier != '':
+                data['object_identifier'] = object_identifier
+
+            self.update('domains', {'domain_id': domain_id}, **data)
+
+        return domain_id
+
+    def get_domain(self, **kwargs) -> int:
+        dom = self.select_first('domains', **kwargs)
+        return dom.get('domain_id', None) if dom is not None else -1
+
+    def fill_data(self):
+        if not self.has_data():
+            # Create default empty password hash
+            self.insert_ignore_one('passwords',
+                                   ntlm_hash='31d6cfe0d16ae931b73c59d7e0c089c0',
+                                   password='(empty)'
+                                   )
 
     def create_db(self):
 
         conn = self.connect_to_db(check=False)
 
         # definindo um cursor
         cursor = conn.cursor()
@@ -488,7 +461,10 @@
         conn.commit()
 
         cursor.execute("""
             INSERT INTO [domains](name) values('default');
         """)
 
         conn.commit()
+
+        #Must get the constraints
+        self.get_constraints()
```

### Comparing `knowsmore-0.1.37/knowsmore/util/logger.py` & `knowsmore-0.1.38/knowsmore/util/logger.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/util/process.py` & `knowsmore-0.1.38/knowsmore/util/process.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore/util/tools.py` & `knowsmore-0.1.38/knowsmore/util/tools.py`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/knowsmore.egg-info/PKG-INFO` & `knowsmore-0.1.38/knowsmore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: knowsmore
-Version: 0.1.37
+Version: 0.1.38
 Summary: KnowsMore is a swiss army knife tool for pentesting Microsoft Active Directory (NTLM Hashes, BloodHound, NTDS and DCSync).
 Home-page: https://github.com/helviojunior/knowsmore
 Author: Helvio Junior  (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/knowsmore
 Project-URL: Source, https://github.com/helviojunior/knowsmore
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -208,20 +207,27 @@
 knowsmore --word-list -o "~/Desktop/Wordlist/my_custom_wordlist.txt" --batch --name company_name
 ```
 
 ## Importing cracked hashes
 
 ### Cracking hashes
 
-In order to crack the hashes, I usually use `hashcat` with the command bellow
+First extract all hashes to a txt file
 
 ```bash
-# Extract NTLM hashes from file
+# Extract NTLM hashes to file
+nowsmore --ntlm-hash --export-hashes "~/Desktop/ntlm_hash.txt"
+
+# Or, extract NTLM hashes from NTDS file
 cat ~/Desktop/client_name.ntds | cut -d ':' -f4 > ntlm_hashes.txt
+```
 
+In order to crack the hashes, I usually use `hashcat` with the command bellow
+
+```bash
 # Wordlist attack
 hashcat -m 1000 -a 0 -O -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" "~/Desktop/Wordlist/*"
 
 # Mask attack
 hashcat -m 1000 -a 3 -O --increment --increment-min 4 -o "~/Desktop/cracked.txt" --remove "~/Desktop/ntlm_hash.txt" ?a?a?a?a?a?a?a?a
 ```
 
@@ -269,8 +275,7 @@
 ```
 server.bolt.listen_address=0.0.0.0:7687
 ```
 
 # To do
 
 [Check the TODO file](TODO.md)
-
```

### Comparing `knowsmore-0.1.37/knowsmore.egg-info/SOURCES.txt` & `knowsmore-0.1.38/knowsmore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knowsmore-0.1.37/setup.py` & `knowsmore-0.1.38/setup.py`

 * *Files identical despite different names*

