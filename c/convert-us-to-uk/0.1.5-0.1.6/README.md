# Comparing `tmp/convert-us-to-uk-0.1.5.tar.gz` & `tmp/convert-us-to-uk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.5.tar", last modified: Tue Apr 30 10:47:51 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.6.tar", last modified: Fri May  3 15:50:23 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.5.tar` & `convert-us-to-uk-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.171639 convert-us-to-uk-0.1.5/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-04-30 10:47:51.163532 convert-us-to-uk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.002599 convert-us-to-uk-0.1.5/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    40125 2024-04-23 12:59:33.000000 convert-us-to-uk-0.1.5/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.140412 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-30 10:47:50.000000 convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 10:47:51.176559 convert-us-to-uk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-04-30 10:37:08.000000 convert-us-to-uk-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:47:51.146749 convert-us-to-uk-0.1.5/tests/
--rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.5/tests/test_converter.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.130891 convert-us-to-uk-0.1.6/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-03 15:50:23.128745 convert-us-to-uk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.110747 convert-us-to-uk-0.1.6/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1533 2024-04-30 10:34:39.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    39780 2024-05-03 15:49:27.000000 convert-us-to-uk-0.1.6/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.123752 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-05-03 15:50:23.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-03 15:50:22.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 15:50:23.000000 convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:50:23.130891 convert-us-to-uk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-05-03 15:49:59.000000 convert-us-to-uk-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:50:23.125745 convert-us-to-uk-0.1.6/tests/
+-rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.6/tests/test_converter.py
```

### Comparing `convert-us-to-uk-0.1.5/PKG-INFO` & `convert-us-to-uk-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.5/README.md` & `convert-us-to-uk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.5/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.6/convert_us_to_uk/converter.py`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.5/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.6/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 accessorizing,accessorising
 acclimatization,acclimatisation
 acclimatize,acclimatise
 acclimatized,acclimatised
 acclimatizes,acclimatises
 acclimatizing,acclimatising
 accouterments,accoutrements
-eon,aeon
-eons,aeons
 aerogram,aerogramme
 aerograms,aerogrammes
 airplane,aeroplane
 airplanes,aeroplanes
 esthete,aesthete
 esthetes,aesthetes
 esthetic,aesthetic
@@ -327,14 +325,15 @@
 crystallization,crystallisation
 crystallize,crystallise
 crystallized,crystallised
 crystallizes,crystallises
 crystallizing,crystallising
 cudgeled,cudgelled
 cudgeling,cudgelling
+customization,customisation
 customize,customise
 customized,customised
 customizes,customises
 customizing,customising
 cipher,cypher
 ciphers,cyphers
 decentralization,decentralisation
@@ -623,24 +622,14 @@
 funneling,funnelling
 galvanize,galvanise
 galvanized,galvanised
 galvanizes,galvanises
 galvanizing,galvanising
 gamboled,gambolled
 gamboling,gambolling
-jail,gaol
-jailbird,gaolbird
-jailbirds,gaolbirds
-jailbreak,gaolbreak
-jailbreaks,gaolbreaks
-jailed,gaoled
-jailer,gaoler
-jailers,gaolers
-jailing,gaoling
-jails,gaols
 generalization,generalisation
 generalizations,generalisations
 generalize,generalise
 generalized,generalised
 generalizes,generalises
 generalizing,generalising
 ghettoize,ghettoise
@@ -668,16 +657,14 @@
 grayed,greyed
 graying,greying
 grayish,greyish
 grayness,greyness
 grays,greys
 groveled,grovelled
 groveling,grovelling
-groin,groyne
-groins,groynes
 grueling,gruelling
 gruelingly,gruellingly
 griffin,gryphon
 griffins,gryphons
 gynecological,gynaecological
 gynecologist,gynaecologist
 gynecologists,gynaecologists
@@ -785,18 +772,14 @@
 inflections,inflexions
 initialize,initialise
 initialized,initialised
 initializes,initialises
 initializing,initialising
 initialed,initialled
 initialing,initialling
-install,instal
-installment,instalment
-installments,instalments
-installs,instals
 instill,instil
 instills,instils
 institutionalization,institutionalisation
 institutionalize,institutionalise
 institutionalized,institutionalised
 institutionalizes,institutionalises
 institutionalizing,institutionalising
@@ -1168,16 +1151,14 @@
 personalizing,personalising
 pharmacopeia,pharmacopoeia
 pharmacopeias,pharmacopoeias
 philosophize,philosophise
 philosophized,philosophised
 philosophizes,philosophises
 philosophizing,philosophising
-filter,philtre
-filters,philtres
 phony,phoney
 plagiarize,plagiarise
 plagiarized,plagiarised
 plagiarizes,plagiarises
 plagiarizing,plagiarising
 plow,plough
 plowed,ploughed
@@ -1261,15 +1242,14 @@
 pulverized,pulverised
 pulverizes,pulverises
 pulverizing,pulverising
 pummel,pummelled
 pummeled,pummelling
 pajama,pyjama
 pajamas,pyjamas
-pizzazz,pzazz
 quarreled,quarrelled
 quarreling,quarrelling
 radicalize,radicalise
 radicalized,radicalised
 radicalizes,radicalises
 radicalizing,radicalising
 rancor,rancour
@@ -1349,14 +1329,15 @@
 romanticizing,romanticising
 rumor,rumour
 rumored,rumoured
 rumors,rumours
 saber,sabre
 sabers,sabres
 saltpeter,saltpetre
+sanitization,sanitisation
 sanitize,sanitise
 sanitized,sanitised
 sanitizes,sanitises
 sanitizing,sanitising
 satirize,satirise
 satirized,satirised
 satirizes,satirises
@@ -1664,16 +1645,14 @@
 verbalizes,verbalises
 verbalizing,verbalising
 victimization,victimisation
 victimize,victimise
 victimized,victimised
 victimizes,victimises
 victimizing,victimising
-videodisk,videodisc
-videodisks,videodiscs
 vigor,vigour
 visualization,visualisation
 visualizations,visualisations
 visualize,visualise
 visualized,visualised
 visualizes,visualises
 visualizing,visualising
```

### Comparing `convert-us-to-uk-0.1.5/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.6/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `convert-us-to-uk-0.1.5/setup.py` & `convert-us-to-uk-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='convert-us-to-uk',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     include_package_data=True,
     description='A simple utility to convert US spelling to UK spelling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Oliver Blane',
     author_email='oliverblane72@gmail.com',
```

