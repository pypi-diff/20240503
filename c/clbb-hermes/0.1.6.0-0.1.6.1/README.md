# Comparing `tmp/clbb_hermes-0.1.6.0.tar.gz` & `tmp/clbb_hermes-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clbb_hermes-0.1.6.0.tar", last modified: Thu May  2 13:50:15 2024, max compression
+gzip compressed data, was "clbb_hermes-0.1.6.1.tar", last modified: Thu May  2 21:54:31 2024, max compression
```

## Comparing `clbb_hermes-0.1.6.0.tar` & `clbb_hermes-0.1.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.315558 clbb_hermes-0.1.6.0/
--rw-rw-rw-   0        0        0      321 2024-05-02 13:50:15.314831 clbb_hermes-0.1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-03-07 13:43:35.000000 clbb_hermes-0.1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.313752 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/
--rw-rw-rw-   0        0        0      321 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-02 13:50:15.000000 clbb_hermes-0.1.6.0/clbb_hermes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 13:50:15.312473 clbb_hermes-0.1.6.0/hermes/
--rw-rw-rw-   0        0        0       48 2024-03-08 14:31:46.000000 clbb_hermes-0.1.6.0/hermes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-03-06 20:27:32.000000 clbb_hermes-0.1.6.0/hermes/functions.py
--rw-rw-rw-   0        0        0     5486 2024-04-30 21:07:15.000000 clbb_hermes-0.1.6.0/hermes/handler.py
--rw-rw-rw-   0        0        0       42 2024-05-02 13:50:15.316578 clbb_hermes-0.1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      384 2024-04-30 21:21:54.000000 clbb_hermes-0.1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:54:31.573852 clbb_hermes-0.1.6.1/
+-rw-rw-rw-   0        0        0      321 2024-05-02 21:54:31.572795 clbb_hermes-0.1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-03-07 13:43:35.000000 clbb_hermes-0.1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 21:54:31.570987 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/
+-rw-rw-rw-   0        0        0      321 2024-05-02 21:54:31.000000 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-02 21:54:31.000000 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:54:31.000000 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-02 21:54:31.000000 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-02 21:54:31.000000 clbb_hermes-0.1.6.1/clbb_hermes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 21:54:31.569991 clbb_hermes-0.1.6.1/hermes/
+-rw-rw-rw-   0        0        0       48 2024-03-08 14:31:46.000000 clbb_hermes-0.1.6.1/hermes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 20:27:32.000000 clbb_hermes-0.1.6.1/hermes/functions.py
+-rw-rw-rw-   0        0        0     5536 2024-05-02 21:54:13.000000 clbb_hermes-0.1.6.1/hermes/handler.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:54:31.573852 clbb_hermes-0.1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      384 2024-05-02 21:54:19.000000 clbb_hermes-0.1.6.1/setup.py
```

### Comparing `clbb_hermes-0.1.6.0/hermes/handler.py` & `clbb_hermes-0.1.6.1/hermes/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,18 @@
 
     def load_amenities(self):
         amenities = None
         endpoint = f'{self.server_address}/interactive/project/{self.project_id}/get-data/amenities/'
         response = requests.get(endpoint)
         data_json = response.json()
         amenities = self.geojson_to_geodataframe(data_json=data_json)
-        amenities.drop(columns=['tags'], inplace=True)
+        try:
+            amenities.drop(columns=['tags'], inplace=True)
+        except:
+            pass
         return amenities
 
     def load_area_of_interest(self, id=1):
         area_of_interest = None
         endpoint = f'{self.server_address}/interactive/project/{self.project_id}/area-of-interest/'
         response = requests.get(endpoint)
         data = response.json()
```

