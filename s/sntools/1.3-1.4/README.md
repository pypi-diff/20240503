# Comparing `tmp/sntools-1.3.tar.gz` & `tmp/sntools-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sntools-1.3.tar", last modified: Sat Aug 12 20:57:00 2023, max compression
+gzip compressed data, was "sntools-1.4.tar", last modified: Fri May  3 15:52:14 2024, max compression
```

## Comparing `sntools-1.3.tar` & `sntools-1.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.532838 sntools-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-12 20:56:44.000000 sntools-1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-12 20:57:00.532838 sntools-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-12 20:56:44.000000 sntools-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-12 20:56:44.000000 sntools-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-12 20:57:00.532838 sntools-1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.524838 sntools-1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.528838 sntools-1.3/src/sntools/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.528838 sntools-1.3/src/sntools/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/nakazato.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/princeton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/totani.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/formats/warren2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/genevts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.532838 sntools-1.3/src/sntools/interaction_channels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/c12e.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/c12eb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/c12nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/es.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/ibd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/o16e.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/o16eb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/interaction_channels/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-08-12 20:56:44.000000 sntools-1.3/src/sntools/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.528838 sntools-1.3/src/sntools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-12 20:57:00.000000 sntools-1.3/src/sntools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 20:57:00.532838 sntools-1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_c12e.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_c12eb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_c12nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_detectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_ibd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_ibd_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_nakazato.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_o16e.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_o16eb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-12 20:56:44.000000 sntools-1.3/tests/test_ps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.073554 sntools-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-03 15:52:05.000000 sntools-1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-03 15:52:14.073554 sntools-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-05-03 15:52:05.000000 sntools-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-03 15:52:05.000000 sntools-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:52:14.073554 sntools-1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.065554 sntools-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.065554 sntools-1.4/src/sntools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.069553 sntools-1.4/src/sntools/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/nakazato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/princeton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/totani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/formats/warren2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/genevts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.069553 sntools-1.4/src/sntools/interaction_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/c12e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/c12eb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/c12nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/ibd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/o16e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/o16eb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/interaction_channels/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-03 15:52:05.000000 sntools-1.4/src/sntools/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.069553 sntools-1.4/src/sntools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 15:52:14.000000 sntools-1.4/src/sntools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:52:14.069553 sntools-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_c12e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_c12eb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_c12nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_ibd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_ibd_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_nakazato.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_o16e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_o16eb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-03 15:52:05.000000 sntools-1.4/tests/test_ps.py
```

### Comparing `sntools-1.3/LICENSE.md` & `sntools-1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sntools-1.3/PKG-INFO` & `sntools-1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sntools
-Version: 1.3
+Version: 1.4
 Summary: Event generator for supernova burst neutrinos
 Author: Jost Migenda, sntools Contributors
-Project-URL: Homepage, https://github.com/JostMigenda/sntools
-Project-URL: Bug Tracker, https://github.com/JostMigenda/sntools/issues
+Project-URL: Homepage, https://github.com/SNEWS2/sntools
+Project-URL: Bug Tracker, https://github.com/SNEWS2/sntools/issues
 Keywords: astrophysics,supernova,neutrino,event generator
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -16,27 +16,33 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: h5py>=2.10
+Requires-Dist: snewpy~=1.5.0
+Requires-Dist: uproot
 
 # sntools
 sntools is a Monte Carlo event generator for supernova neutrino interactions.
 
 It is a command line application that uses detailed time- and energy-dependent neutrino fluxes (provided by various supernova models) to generate interactions within the detector volume and write them to event files that can be used as an input for a full detector simulation.
 sntools was originally developed for Hyper-Kamiokande and later extended to support different detectors and detector materials.
 
 Additionally, sntools can be used as a Python library that implements neutrino cross sections.
 
-This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/JostMigenda/sntools/releases).
+This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/SNEWS2/sntools/releases).
 
 ## Getting Started
 ### Installation Instructions
 First, make sure you have Python 3.8 or higher installed on your computer.
 Then, in a terminal, run
 ```
 pip install sntools
@@ -103,12 +109,12 @@
 Water-based liquid scintillator, a mixture of the two materials, is also supported.
 
 
 ## Output
 A text file in the NUANCE format (used by the `/mygen/vecfile` options in WCSim) or the RATPAC format.
 
 ## Support and Contributing
-To report problems or ask for help, [open an issue on GitHub](https://github.com/JostMigenda/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
+To report problems or ask for help, [open an issue on GitHub](https://github.com/SNEWS2/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
 
-Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/JostMigenda/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
+Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/SNEWS2/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
 
 Please note that this project is released with a Contributor Code of Conduct (see `CODE_OF_CONDUCT.md`). By participating in this project you agree to abide by its terms.
```

### Comparing `sntools-1.3/README.md` & `sntools-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sntools is a Monte Carlo event generator for supernova neutrino interactions.
 
 It is a command line application that uses detailed time- and energy-dependent neutrino fluxes (provided by various supernova models) to generate interactions within the detector volume and write them to event files that can be used as an input for a full detector simulation.
 sntools was originally developed for Hyper-Kamiokande and later extended to support different detectors and detector materials.
 
 Additionally, sntools can be used as a Python library that implements neutrino cross sections.
 
-This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/JostMigenda/sntools/releases).
+This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/SNEWS2/sntools/releases).
 
 ## Getting Started
 ### Installation Instructions
 First, make sure you have Python 3.8 or higher installed on your computer.
 Then, in a terminal, run
 ```
 pip install sntools
@@ -77,12 +77,12 @@
 Water-based liquid scintillator, a mixture of the two materials, is also supported.
 
 
 ## Output
 A text file in the NUANCE format (used by the `/mygen/vecfile` options in WCSim) or the RATPAC format.
 
 ## Support and Contributing
-To report problems or ask for help, [open an issue on GitHub](https://github.com/JostMigenda/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
+To report problems or ask for help, [open an issue on GitHub](https://github.com/SNEWS2/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
 
-Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/JostMigenda/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
+Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/SNEWS2/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
 
 Please note that this project is released with a Contributor Code of Conduct (see `CODE_OF_CONDUCT.md`). By participating in this project you agree to abide by its terms.
```

### Comparing `sntools-1.3/pyproject.toml` & `sntools-1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 license = {file = "LICENSE"}
 
 requires-python = ">=3.8"  # TODO: Also update classifiers below!
 dependencies = [
     "numpy",
     "scipy",
     "h5py >= 2.10",
-    "snewpy ~=1.4b1",
+    "snewpy ~=1.5.0",
     "uproot"
 ]
 
 keywords = ["astrophysics", "supernova", "neutrino", "event generator"]
 classifiers = [
     'License :: OSI Approved :: BSD License',
     'Development Status :: 5 - Production/Stable',
@@ -35,24 +35,25 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 
 
 [project.scripts]
 sntools = "sntools.genevts:main"
 
 
 [project.urls]
-"Homepage" = "https://github.com/JostMigenda/sntools"
-"Bug Tracker" = "https://github.com/JostMigenda/sntools/issues"
+"Homepage" = "https://github.com/SNEWS2/sntools"
+"Bug Tracker" = "https://github.com/SNEWS2/sntools/issues"
 
 
 [tool.setuptools.dynamic]
 version = {attr = "sntools.__version__"}
 
 
 [tool.setuptools.packages.find]
```

### Comparing `sntools-1.3/src/sntools/__init__.py` & `sntools-1.4/src/sntools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 and writes them to event files that can be used as an input for a full detector
 simulation.
 sntools was originally developed for Hyper-Kamiokande and later extended to
 support different detectors and detector materials.
 
 For usage information, run `sntools -h` or `python sntools/genevts.py -h`.
 For more extensive documentation, to report issues or to contribute code,
-see https://github.com/JostMigenda/sntools.
+see https://github.com/SNEWS2/sntools.
 """
-__version__ = '1.3'
+__version__ = '1.4'
 
 
 def setup():
     """
     Downloads sample flux file from GitHub if necessary and performs integration test.
     """
     tryprint(u"\u2705", "[SUCCESS]")
@@ -24,15 +24,15 @@
     import hashlib
     import os
     import sys
     from . import genevts
 
     flux_dir = 'fluxes/'
     flux_file = flux_dir + 'intp2001.data'
-    flux_url = 'https://raw.githubusercontent.com/JostMigenda/sntools/main/fluxes/intp2001.data'
+    flux_url = 'https://raw.githubusercontent.com/SNEWS2/sntools/main/fluxes/intp2001.data'
     if os.path.exists(flux_file):
         tryprint(u"\u2705", "[SUCCESS]")
         print("Using sample flux file at " + flux_file)
     else:
         tryprint(u"\U0001f6e0")
         print("Downloading sample flux file from " + flux_url)
         if not os.path.isdir(flux_dir):
@@ -64,15 +64,15 @@
         print("Everything seems to work fine. Enjoy using sntools!")
     else:
         tryprint(u"\u274c", "[ERROR]")
         print("Test did not generate the expected events.")
         tryprint(u"\u274c", "[ERROR]")
         print("Please ensure you have installed the most recent version of sntools and all dependencies.")
         tryprint(u"\u274c", "[ERROR]")
-        print("If this persists, please go to https://github.com/JostMigenda/sntools and open a new issue.")
+        print("If this persists, please go to https://github.com/SNEWS2/sntools and open a new issue.")
 
 
 def tryprint(default, alternative=''):
     try:
         print(default, end=' ')
     except UnicodeEncodeError:
         print(alternative, end=' ')
```

### Comparing `sntools-1.3/src/sntools/channel.py` & `sntools-1.4/src/sntools/channel.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/detectors.py` & `sntools-1.4/src/sntools/detectors.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/event.py` & `sntools-1.4/src/sntools/event.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/formats/__init__.py` & `sntools-1.4/src/sntools/formats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     def from_file(cls, file, format, starttime=None, endtime=None):
         """Create a SNEWPYCompositeFlux from an input file."""
         self = SNEWPYCompositeFlux()
         self._repr = f"SNEWPYCompositeFlux.from_file('{file}', format='{format}', starttime={starttime}, endtime={endtime})"
 
         # snewpy.models.loaders classes treat relative file paths as relative to the snewpy cache directory,
         # so we’ll turn it into an absolute path first.
-        sn_model = getattr(import_module('snewpy.models.loaders'), format)(abspath(file))
+        sn_model = getattr(import_module('snewpy.models.ccsn_loaders'), format)(abspath(file))
 
         for flv in ('e', 'eb', 'x', 'xb'):
             f = SNEWPYFlux(sn_model, flv, starttime, endtime)
             self.components[flv] = [f]
 
         return self
```

### Comparing `sntools-1.3/src/sntools/formats/gamma.py` & `sntools-1.4/src/sntools/formats/gamma.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/formats/nakazato.py` & `sntools-1.4/src/sntools/formats/nakazato.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/formats/princeton.py` & `sntools-1.4/src/sntools/formats/princeton.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/formats/totani.py` & `sntools-1.4/src/sntools/formats/totani.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/formats/warren2020.py` & `sntools-1.4/src/sntools/formats/warren2020.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/genevts.py` & `sntools-1.4/src/sntools/genevts.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,44 +44,47 @@
 
     events = []
     for result in as_completed(results):
         events.extend(result.result())
 
     # Sort events by time and write them to an output file
     events.sort(key=lambda evt: evt.time)
-    with open(args.output, "w") as outfile:
-        if args.verbose:  # write parameters to file as a comment
-            outfile.write(f"# Generated on {datetime.now()} with the options:\n")
-            outfile.write(f"# {args}\n")
-        if args.mcformat == 'NUANCE':
-            for (i, evt) in enumerate(events):
-                evt.vertex = args.detector.generate_random_vertex()
-                outfile.write(evt.nuance_string(i))
-            outfile.write("$ stop\n")
-        if args.mcformat == 'RATPAC':
-            for (i, evt) in enumerate(events):
-                evt.vertex = args.detector.generate_random_vertex()
-                outfile.write(evt.ratpac_string(i, events))
-        if args.mcformat == 'ROOT_JUNO':
-            fname =	args.output+".root"
-            root_outfile = uproot.recreate(fname)
-            root_outfile.mktree("SNEvents",{"nparticles": "uint64", "origPDGID":"int32", "nuE":"double", "pdgid": ("int32",(2,)),"t": ("float64",(2,)),
-                                            "px": ("float64",(2,)),"py":("float64",(2,)),"pz":("float64",(2,)),"m":("float64",(2,)), "channel": "int64"})
-            for (i, evt) in enumerate(events):
-                evt.vertex = args.detector.generate_random_vertex()
-                evt.juno_string(i, root_outfile)
+    for evt in events:
+        evt.vertex = args.detector.generate_random_vertex()
+
+    if args.mcformat in ('NUANCE', 'RATPAC'):
+        with open(args.output, "w") as outfile:
+            if args.verbose:  # write parameters to file as a comment
+                outfile.write(f"# Generated on {datetime.now()} with the options:\n")
+                outfile.write(f"# {args}\n")
+            if args.mcformat == 'NUANCE':
+                for (i, evt) in enumerate(events):
+                    outfile.write(evt.nuance_string(i))
+                outfile.write("$ stop\n")
+            if args.mcformat == 'RATPAC':
+                for (i, evt) in enumerate(events):
+                    outfile.write(evt.ratpac_string(i, events))
+    if args.mcformat == 'ROOT_JUNO':
+        fname =	args.output+".root"
+        root_outfile = uproot.recreate(fname)
+        root_outfile.mktree("SNEvents",{"nparticles": "uint64", "origPDGID":"int32", "nuE":"double", "pdgid": ("int32",(2,)),"t": ("float64",(2,)),
+                                        "px": ("float64",(2,)),"py":("float64",(2,)),"pz":("float64",(2,)),"m":("float64",(2,)), "channel": "int64"})
+        for (i, evt) in enumerate(events):
+            evt.juno_string(i, root_outfile)
 
 def parse_command_line_options():
     """Define and parse command line options."""
     parser = argparse.ArgumentParser()
 
     parser.add_argument("input_file", help="Name or common prefix of the input file(s). Required.")
 
     choices = ("gamma", "nakazato", "princeton", "totani", "warren2020",
-               "SNEWPY-Bollig_2016", "SNEWPY-Fornax_2021", "SNEWPY-Kuroda_2020", "SNEWPY-Nakazato_2013", "SNEWPY-OConnor_2015", "SNEWPY-Sukhbold_2015", "SNEWPY-Tamborra_2014", "SNEWPY-Walk_2018", "SNEWPY-Walk_2019", "SNEWPY-Zha_2021")
+               "SNEWPY-Bollig_2016", "SNEWPY-Fornax_2021", "SNEWPY-Fornax_2022", "SNEWPY-Kuroda_2020",
+               "SNEWPY-Mori_2023", "SNEWPY-Nakazato_2013", "SNEWPY-OConnor_2015", "SNEWPY-Sukhbold_2015",
+               "SNEWPY-Tamborra_2014", "SNEWPY-Walk_2018", "SNEWPY-Walk_2019", "SNEWPY-Zha_2021")
     parser.add_argument("-f", "--format", metavar="FORMAT", choices=choices, default=choices[1],
                         help="Format of input file(s). Choices: %(choices)s. Default: %(default)s.")
 
     parser.add_argument("-o", "--output", metavar="FILE", default="outfile.kin", help="Name of the output file. Default: %(default)s.")
 
     choices = ("NUANCE", "RATPAC","ROOT_JUNO")
     parser.add_argument("-m", "--mcformat", metavar="MCFORMAT", choices=choices, default=choices[0],
```

### Comparing `sntools-1.3/src/sntools/interaction_channels/__init__.py` & `sntools-1.4/src/sntools/interaction_channels/__init__.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/c12e.py` & `sntools-1.4/src/sntools/interaction_channels/c12e.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/c12eb.py` & `sntools-1.4/src/sntools/interaction_channels/c12eb.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/c12nc.py` & `sntools-1.4/src/sntools/interaction_channels/c12nc.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/es.py` & `sntools-1.4/src/sntools/interaction_channels/es.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/ibd.py` & `sntools-1.4/src/sntools/interaction_channels/ibd.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/o16e.py` & `sntools-1.4/src/sntools/interaction_channels/o16e.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/o16eb.py` & `sntools-1.4/src/sntools/interaction_channels/o16eb.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/interaction_channels/ps.py` & `sntools-1.4/src/sntools/interaction_channels/ps.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools/transformation.py` & `sntools-1.4/src/sntools/transformation.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/src/sntools.egg-info/PKG-INFO` & `sntools-1.4/src/sntools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sntools
-Version: 1.3
+Version: 1.4
 Summary: Event generator for supernova burst neutrinos
 Author: Jost Migenda, sntools Contributors
-Project-URL: Homepage, https://github.com/JostMigenda/sntools
-Project-URL: Bug Tracker, https://github.com/JostMigenda/sntools/issues
+Project-URL: Homepage, https://github.com/SNEWS2/sntools
+Project-URL: Bug Tracker, https://github.com/SNEWS2/sntools/issues
 Keywords: astrophysics,supernova,neutrino,event generator
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -16,27 +16,33 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: h5py>=2.10
+Requires-Dist: snewpy~=1.5.0
+Requires-Dist: uproot
 
 # sntools
 sntools is a Monte Carlo event generator for supernova neutrino interactions.
 
 It is a command line application that uses detailed time- and energy-dependent neutrino fluxes (provided by various supernova models) to generate interactions within the detector volume and write them to event files that can be used as an input for a full detector simulation.
 sntools was originally developed for Hyper-Kamiokande and later extended to support different detectors and detector materials.
 
 Additionally, sntools can be used as a Python library that implements neutrino cross sections.
 
-This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/JostMigenda/sntools/releases).
+This README file should give a brief overview over sntools and help you get started. For more information, see the [full documentation for each release on GitHub](https://github.com/SNEWS2/sntools/releases).
 
 ## Getting Started
 ### Installation Instructions
 First, make sure you have Python 3.8 or higher installed on your computer.
 Then, in a terminal, run
 ```
 pip install sntools
@@ -103,12 +109,12 @@
 Water-based liquid scintillator, a mixture of the two materials, is also supported.
 
 
 ## Output
 A text file in the NUANCE format (used by the `/mygen/vecfile` options in WCSim) or the RATPAC format.
 
 ## Support and Contributing
-To report problems or ask for help, [open an issue on GitHub](https://github.com/JostMigenda/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
+To report problems or ask for help, [open an issue on GitHub](https://github.com/SNEWS2/sntools/issues) or email the [lead developer](https://github.com/JostMigenda/).
 
-Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/JostMigenda/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
+Contributions to sntools are welcome! See instructions in the [full documentation](https://github.com/SNEWS2/sntools/releases) for help on common ways to extend sntools (e. g. by adding a new detector, input format or interaction channel) and please submit a pull request with your contributions!
 
 Please note that this project is released with a Contributor Code of Conduct (see `CODE_OF_CONDUCT.md`). By participating in this project you agree to abide by its terms.
```

### Comparing `sntools-1.3/src/sntools.egg-info/SOURCES.txt` & `sntools-1.4/src/sntools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_c12e.py` & `sntools-1.4/tests/test_c12e.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_c12eb.py` & `sntools-1.4/tests/test_c12eb.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_c12nc.py` & `sntools-1.4/tests/test_c12nc.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_detectors.py` & `sntools-1.4/tests/test_detectors.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_es.py` & `sntools-1.4/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_formats.py` & `sntools-1.4/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_gamma.py` & `sntools-1.4/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_ibd.py` & `sntools-1.4/tests/test_ibd.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_ibd_extended.py` & `sntools-1.4/tests/test_ibd_extended.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_nakazato.py` & `sntools-1.4/tests/test_nakazato.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_o16e.py` & `sntools-1.4/tests/test_o16e.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_o16eb.py` & `sntools-1.4/tests/test_o16eb.py`

 * *Files identical despite different names*

### Comparing `sntools-1.3/tests/test_ps.py` & `sntools-1.4/tests/test_ps.py`

 * *Files identical despite different names*

