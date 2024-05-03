# Comparing `tmp/animaire-1.1.5.tar.gz` & `tmp/animaire-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animaire-1.1.5.tar", last modified: Mon Apr 22 10:42:41 2024, max compression
+gzip compressed data, was "animaire-1.1.6.tar", last modified: Fri May  3 11:36:15 2024, max compression
```

## Comparing `animaire-1.1.5.tar` & `animaire-1.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.109123 animaire-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/AniMAIRE/
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/AniMAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/dose_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-22 10:42:32.000000 animaire-1.1.5/AniMAIRE/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/AniMAIRE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-04-22 10:42:41.000000 animaire-1.1.5/AniMAIRE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-22 10:42:41.000000 animaire-1.1.5/AniMAIRE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 10:42:41.000000 animaire-1.1.5/AniMAIRE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-22 10:42:41.000000 animaire-1.1.5/AniMAIRE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 10:42:41.000000 animaire-1.1.5/AniMAIRE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-22 10:42:32.000000 animaire-1.1.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 10:42:32.000000 animaire-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-04-22 10:42:41.109123 animaire-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-04-22 10:42:32.000000 animaire-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:41.105123 animaire-1.1.5/pytests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 10:42:35.000000 animaire-1.1.5/pytests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-22 10:42:35.000000 animaire-1.1.5/pytests/test_anisotropic_MAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 10:42:41.109123 animaire-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-22 10:42:35.000000 animaire-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.689767 animaire-1.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.685767 animaire-1.1.6/AniMAIRE/
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/AniMAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.685767 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.689767 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.689767 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/dose_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-03 11:36:06.000000 animaire-1.1.6/AniMAIRE/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.689767 animaire-1.1.6/AniMAIRE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-05-03 11:36:15.000000 animaire-1.1.6/AniMAIRE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 11:36:15.000000 animaire-1.1.6/AniMAIRE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:36:15.000000 animaire-1.1.6/AniMAIRE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 11:36:15.000000 animaire-1.1.6/AniMAIRE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 11:36:15.000000 animaire-1.1.6/AniMAIRE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-03 11:36:06.000000 animaire-1.1.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 11:36:06.000000 animaire-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-05-03 11:36:15.689767 animaire-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-03 11:36:06.000000 animaire-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:15.689767 animaire-1.1.6/pytests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:36:10.000000 animaire-1.1.6/pytests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-03 11:36:10.000000 animaire-1.1.6/pytests/test_anisotropic_MAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:36:15.689767 animaire-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-03 11:36:10.000000 animaire-1.1.6/setup.py
```

### Comparing `animaire-1.1.5/AniMAIRE/AniMAIRE.py` & `animaire-1.1.6/AniMAIRE/AniMAIRE.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py` & `animaire-1.1.6/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/dose_plotting.py` & `animaire-1.1.6/AniMAIRE/dose_plotting.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE/utils.py` & `animaire-1.1.6/AniMAIRE/utils.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/AniMAIRE.egg-info/PKG-INFO` & `animaire-1.1.6/AniMAIRE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
```

### Comparing `animaire-1.1.5/AniMAIRE.egg-info/SOURCES.txt` & `animaire-1.1.6/AniMAIRE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/LICENCE` & `animaire-1.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/PKG-INFO` & `animaire-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
```

### Comparing `animaire-1.1.5/README.md` & `animaire-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/pytests/test_anisotropic_MAIRE.py` & `animaire-1.1.6/pytests/test_anisotropic_MAIRE.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.5/setup.py` & `animaire-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='AniMAIRE',
     packages=find_packages(exclude='pytests'),
     package_data={"AniMAIRE":[
                                 "anisotropic_MAIRE_engine/data/*.csv"
                                          ]},
-    version='1.1.5',
+    version='1.1.6',
     description='Python library for running the anisotropic version of MAIRE+',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     license='GNU General Public License v3.0',
     url='https://github.com/ssc-maire/AniMAIRE-public',
```

