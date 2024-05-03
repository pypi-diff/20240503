# Comparing `tmp/lobbyview-0.0.2.tar.gz` & `tmp/lobbyview-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lobbyview-0.0.2.tar", last modified: Mon Apr  1 00:11:29 2024, max compression
+gzip compressed data, was "lobbyview-0.0.3.tar", last modified: Fri May  3 01:58:31 2024, max compression
```

## Comparing `lobbyview-0.0.2.tar` & `lobbyview-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-04-01 00:11:29.056914 lobbyview-0.0.2/
--rw-r--r--   0 nicholasliu   (501) staff       (20)        0 2024-02-27 03:44:13.000000 lobbyview-0.0.2/LICENSE
--rw-r--r--   0 nicholasliu   (501) staff       (20)     8977 2024-04-01 00:11:29.056620 lobbyview-0.0.2/PKG-INFO
--rw-r--r--   0 nicholasliu   (501) staff       (20)     8629 2024-04-01 00:07:57.000000 lobbyview-0.0.2/README.md
--rw-r--r--   0 nicholasliu   (501) staff       (20)      506 2024-04-01 00:11:06.000000 lobbyview-0.0.2/pyproject.toml
--rw-r--r--   0 nicholasliu   (501) staff       (20)       38 2024-04-01 00:11:29.056972 lobbyview-0.0.2/setup.cfg
-drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-04-01 00:11:29.053416 lobbyview-0.0.2/src/
-drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-04-01 00:11:29.054992 lobbyview-0.0.2/src/lobbyview/
--rw-r--r--   0 nicholasliu   (501) staff       (20)    24469 2024-04-01 00:06:02.000000 lobbyview-0.0.2/src/lobbyview/LobbyView.py
--rw-r--r--   0 nicholasliu   (501) staff       (20)        0 2024-02-27 04:13:16.000000 lobbyview-0.0.2/src/lobbyview/__init__.py
-drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-04-01 00:11:29.056365 lobbyview-0.0.2/src/lobbyview.egg-info/
--rw-r--r--   0 nicholasliu   (501) staff       (20)     8977 2024-04-01 00:11:29.000000 lobbyview-0.0.2/src/lobbyview.egg-info/PKG-INFO
--rw-r--r--   0 nicholasliu   (501) staff       (20)      291 2024-04-01 00:11:29.000000 lobbyview-0.0.2/src/lobbyview.egg-info/SOURCES.txt
--rw-r--r--   0 nicholasliu   (501) staff       (20)        1 2024-04-01 00:11:29.000000 lobbyview-0.0.2/src/lobbyview.egg-info/dependency_links.txt
--rw-r--r--   0 nicholasliu   (501) staff       (20)       21 2024-04-01 00:11:29.000000 lobbyview-0.0.2/src/lobbyview.egg-info/requires.txt
--rw-r--r--   0 nicholasliu   (501) staff       (20)       10 2024-04-01 00:11:29.000000 lobbyview-0.0.2/src/lobbyview.egg-info/top_level.txt
-drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-04-01 00:11:29.056042 lobbyview-0.0.2/tests/
--rw-r--r--   0 nicholasliu   (501) staff       (20)     3414 2024-03-31 02:44:30.000000 lobbyview-0.0.2/tests/test_wrapper.py
+drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-05-03 01:58:31.922677 lobbyview-0.0.3/
+-rw-r--r--   0 nicholasliu   (501) staff       (20)        0 2024-02-27 03:44:13.000000 lobbyview-0.0.3/LICENSE
+-rw-r--r--   0 nicholasliu   (501) staff       (20)    17819 2024-05-03 01:58:31.922325 lobbyview-0.0.3/PKG-INFO
+-rw-r--r--   0 nicholasliu   (501) staff       (20)    17471 2024-05-02 04:52:34.000000 lobbyview-0.0.3/README.md
+-rw-r--r--   0 nicholasliu   (501) staff       (20)      506 2024-05-03 01:58:15.000000 lobbyview-0.0.3/pyproject.toml
+-rw-r--r--   0 nicholasliu   (501) staff       (20)       38 2024-05-03 01:58:31.922743 lobbyview-0.0.3/setup.cfg
+drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-05-03 01:58:31.918611 lobbyview-0.0.3/src/
+drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-05-03 01:58:31.920572 lobbyview-0.0.3/src/lobbyview/
+-rw-r--r--   0 nicholasliu   (501) staff       (20)    44381 2024-05-03 01:42:04.000000 lobbyview-0.0.3/src/lobbyview/LobbyView.py
+-rw-r--r--   0 nicholasliu   (501) staff       (20)        0 2024-02-27 04:13:16.000000 lobbyview-0.0.3/src/lobbyview/__init__.py
+-rw-r--r--   0 nicholasliu   (501) staff       (20)     2303 2024-05-03 01:42:04.000000 lobbyview-0.0.3/src/lobbyview/exceptions.py
+drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-05-03 01:58:31.922057 lobbyview-0.0.3/src/lobbyview.egg-info/
+-rw-r--r--   0 nicholasliu   (501) staff       (20)    17819 2024-05-03 01:58:31.000000 lobbyview-0.0.3/src/lobbyview.egg-info/PKG-INFO
+-rw-r--r--   0 nicholasliu   (501) staff       (20)      321 2024-05-03 01:58:31.000000 lobbyview-0.0.3/src/lobbyview.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholasliu   (501) staff       (20)        1 2024-05-03 01:58:31.000000 lobbyview-0.0.3/src/lobbyview.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholasliu   (501) staff       (20)       21 2024-05-03 01:58:31.000000 lobbyview-0.0.3/src/lobbyview.egg-info/requires.txt
+-rw-r--r--   0 nicholasliu   (501) staff       (20)       10 2024-05-03 01:58:31.000000 lobbyview-0.0.3/src/lobbyview.egg-info/top_level.txt
+drwxr-xr-x   0 nicholasliu   (501) staff       (20)        0 2024-05-03 01:58:31.921747 lobbyview-0.0.3/tests/
+-rw-r--r--   0 nicholasliu   (501) staff       (20)     3617 2024-05-03 01:53:57.000000 lobbyview-0.0.3/tests/test_lobbyview.py
```

### Comparing `lobbyview-0.0.2/tests/test_wrapper.py` & `lobbyview-0.0.3/tests/test_lobbyview.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import time
 
 import sys
 sys.path.append('./src/lobbyview/')
 sys.path.append('../src/lobbyview/')
 from LobbyView import LobbyView
 
-load_dotenv("./.env")
-load_dotenv("./tests/.env")
+env_paths = ["tests/.env", "../../tests/.env"]
+for env_path in env_paths:
+    load_dotenv(env_path)
+    
 LOBBYVIEW_TOKEN = os.environ.get('LOBBYVIEW_TOKEN', "NO TOKEN FOUND")
 
 lobbyview = LobbyView(LOBBYVIEW_TOKEN)
 
 def test_legislators():
     output = lobbyview.legislators(legislator_first_name="John", legislator_last_name="McCain")
     assert output.data[0]['legislator_id'] == 'M000303'
@@ -49,16 +51,16 @@
     assert len(output.data) > 0
 
 def test_issues():
     output = lobbyview.issues(issue_code="TRD")
     assert len(output.data) > 0
 
 def test_networks():
-    output = lobbyview.networks(client_uuid="44563806-56d2-5e99-84a1-95d22a7a69b3", legislator_id="M000303")
-    assert output.data[0]['report_year'] == 2017
+    output = lobbyview.networks(client_uuid="44563806-56d2-5e99-84a1-95d22a7a69b3", legislator_id="M000303", min_report_year=2017, max_report_year=2017)
+    assert output.data[0]['n_bills_sponsored'] == 1
 
 def test_networks_ranges():
     output = lobbyview.networks(min_report_year=2015, max_report_year=2020, min_bills_sponsored=1)
     assert len(output.data) > 0
 
 def test_texts():
     output = lobbyview.texts(issue_code="HCR", issue_text="covid")
@@ -69,14 +71,15 @@
     assert output.data[0]['n_bills_sponsored'] == 1
 
 def test_quarter_level_networks_ranges():
     output = lobbyview.quarter_level_networks(min_bills_sponsored=1, max_bills_sponsored=5)
     assert len(output.data) > 0
 
 def test_bill_client_networks():
+    print(f"LOBBYVIEW_TOKEN is {'present' if LOBBYVIEW_TOKEN != 'NO TOKEN FOUND' else 'not found'}")
     output = lobbyview.bill_client_networks(congress_number=114, bill_chamber="H", bill_number=1174, client_uuid="44563806-56d2-5e99-84a1-95d22a7a69b3")
     assert output.data[0]['issue_ordi'] == 2
 
 if __name__ == "__main__":
     test_legislators()
     test_legislators_ranges()
     test_bills()
```

