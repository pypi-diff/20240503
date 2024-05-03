# Comparing `tmp/usempl-plots-0.0.4.tar.gz` & `tmp/usempl-plots-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usempl-plots-0.0.4.tar", last modified: Fri May  3 07:28:08 2024, max compression
+gzip compressed data, was "usempl-plots-0.0.5.tar", last modified: Fri May  3 15:17:23 2024, max compression
```

## Comparing `usempl-plots-0.0.4.tar` & `usempl-plots-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots/data/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/recession_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01_streaks.csv
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_annual_1919-1938.csv
--rw-r--r--   0 runner    (1001) docker     (127)   105196 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/data/usempl_pk_2024-03-01.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/get_payems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/tseries_payems.py
--rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_industry.py
--rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_npp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-03 07:28:06.000000 usempl-plots-0.0.4/usempl_plots/usempl_streaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 07:28:08.724812 usempl-plots-0.0.4/usempl_plots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 07:28:08.000000 usempl-plots-0.0.4/usempl_plots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/usempl_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/usempl_plots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/data/recession_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18211 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/data/usempl_2024-04-01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/data/usempl_annual_1919-1938.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   105232 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/data/usempl_pk_2024-04-01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/get_payems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/tseries_payems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/usempl_industry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26162 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/usempl_npp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-05-03 15:17:21.000000 usempl-plots-0.0.5/usempl_plots/usempl_streaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:17:23.890716 usempl-plots-0.0.5/usempl_plots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15156 2024-05-03 15:17:23.000000 usempl-plots-0.0.5/usempl_plots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 15:17:23.000000 usempl-plots-0.0.5/usempl_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:17:23.000000 usempl-plots-0.0.5/usempl_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 15:17:23.000000 usempl-plots-0.0.5/usempl_plots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 15:17:23.000000 usempl-plots-0.0.5/usempl_plots.egg-info/top_level.txt
```

### Comparing `usempl-plots-0.0.4/LICENSE` & `usempl-plots-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/PKG-INFO` & `usempl-plots-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usempl-plots
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for creating plots of US employment and unemployment
 Home-page: https://github.com/OpenSourceEcon/usempl-plots
 Download-URL: https://github.com/OpenSourceEcon/usempl-plots
 Author: Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/OpenSourceEcon/usempl-plots/issues
 Keywords: Data analysis visualization tools US employment unemployment
```

### Comparing `usempl-plots-0.0.4/README.md` & `usempl-plots-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/setup.py` & `usempl-plots-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="usempl-plots",
-    version="0.0.4",
+    version="0.0.5",
     author="Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="Package for creating plots of US employment and unemployment",
     long_description=readme,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `usempl-plots-0.0.4/usempl_plots/data/recession_data.csv` & `usempl-plots-0.0.5/usempl_plots/data/recession_data.csv`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/usempl_plots/data/usempl_2024-03-01.csv` & `usempl-plots-0.0.5/usempl_plots/data/usempl_2024-04-01.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1036,9 +1036,10 @@
 2023-07-01,156211
 2023-08-01,156421
 2023-09-01,156667
 2023-10-01,156832
 2023-11-01,157014
 2023-12-01,157304
 2024-01-01,157560
-2024-02-01,157830
-2024-03-01,158133
+2024-02-01,157796
+2024-03-01,158111
+2024-04-01,158286
```

### Comparing `usempl-plots-0.0.4/usempl_plots/data/usempl_pk_2024-03-01.csv` & `usempl-plots-0.0.5/usempl_plots/data/usempl_pk_2024-04-01.csv`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 41,1932-12-01,23207.143428015497,0.7408741995918624,1940-12-01,34174.0,1.1019960659120958,1948-07-01,45160.0,1.0778814712270568,1952-02-01,48522.0,1.0712677175784873,1956-12-01,52929.0,1.0473523824600286,1961-01-01,53683.0,1.0104464689052854,1963-09-01,57078.0,1.0413223140495869,1973-08-01,77168.0,1.0800128759569496,1977-12-01,84410.0,1.0734269291418688,1983-08-01,90129.0,0.990493878717278,1984-12-01,96107.0,1.0491916027117607,1993-11-01,111990.0,1.0194161500860208,2004-07-01,131850.0,0.9929510641182052,2011-06-01,131936.0,0.9533154620403621,2023-07-01,156211.0,1.0256189719583215
 42,1933-01-01,23206.61173048141,0.7408572254655028,1941-01-01,34481.0,1.1118957789171584,1948-08-01,45178.0,1.0783110962598754,1952-03-01,48504.0,1.0708703139488673,1957-01-01,52887.0,1.046521291752414,1961-02-01,53557.0,1.008074838126788,1963-10-01,57283.0,1.0450623027384014,1973-09-01,77276.0,1.08152440133798,1978-01-01,84594.0,1.0757668243552572,1983-09-01,91247.0,1.0027804031035012,1985-01-01,96372.0,1.0520845842294297,1993-12-01,112324.0,1.022456466133246,2004-08-01,131936.0,0.9935987227569172,2011-07-01,131992.0,0.9537200950887664,2023-08-01,156421.0,1.0269977479991332
 43,1933-02-01,23231.101603476127,0.7416390500407396,1941-02-01,34843.0,1.1235690561413691,1948-09-01,45294.0,1.0810797909158174,1952-04-01,48620.0,1.0734313595619729,1957-02-01,53097.0,1.050676745290486,1961-03-01,53659.0,1.0099947297093812,1963-11-01,57255.0,1.044551475015051,1973-10-01,77607.0,1.0861569467187304,1978-02-01,84948.0,1.080268579276667,1983-10-01,91520.0,1.005780600918742,1985-02-01,96503.0,1.0535146996211833,1994-01-01,112598.0,1.0249506176210892,2004-09-01,132083.0,0.9947057671742503,2011-08-01,132123.0,0.9546666473984262,2023-09-01,156667.0,1.0286128856469414
 44,1933-03-01,23279.759489103035,0.7431924239912857,1941-03-01,35092.0,1.1315984650607849,1948-10-01,45245.0,1.0799102561042557,1952-05-01,48642.0,1.073917075109286,1957-03-01,53156.0,1.0518442298559443,1961-04-01,53627.0,1.0093924107815089,1963-12-01,57361.0,1.0464853228248774,1973-11-01,77920.0,1.0905375712026424,1978-03-01,85460.0,1.0867795920443564,1983-11-01,91875.0,1.0096819570521134,1985-03-01,96842.0,1.057215532581522,1994-02-01,112779.0,1.0265982140418908,2004-10-01,132435.0,0.997356649044327,2011-09-01,132346.0,0.9562779540018931,2023-10-01,156832.0,1.0296962096790079
 45,1933-04-01,23351.731829465505,0.7454900979908539,1941-04-01,35468.0,1.1437231949953242,1948-11-01,45192.0,1.0786452490631788,1952-06-01,48282.0,1.0659690025168898,1957-04-01,53238.0,1.0534668355231913,1961-05-01,53786.0,1.0123851829543744,1964-01-01,57487.0,1.0487840475799537,1973-12-01,78031.0,1.0920910833998125,1978-04-01,86162.0,1.095706800956305,1983-12-01,92230.0,1.0135833131854848,1985-04-01,97038.0,1.0593552472134584,1994-03-01,113240.0,1.0307945784064738,2004-11-01,132509.0,0.9979139367101953,2011-10-01,132557.0,0.957802553523559,2023-11-01,157014.0,1.030891148914378
 46,1933-05-01,23446.165066666897,0.748504822713156,1941-05-01,36182.0,1.1667472832220824,1948-12-01,45032.0,1.0748263598825691,1952-07-01,48143.0,1.0629001633770476,1957-05-01,53150.0,1.0517255026119994,1961-06-01,53977.0,1.0159802740551123,1964-02-01,57753.0,1.0536369109517816,1974-01-01,78100.0,1.0930567801710263,1978-05-01,86509.0,1.1001195381250317,1984-01-01,92673.0,1.0184517660505088,1985-05-01,97312.0,1.0623464809336143,1994-04-01,113587.0,1.0339532301082317,2004-12-01,132633.0,0.998847770096245,2011-11-01,132701.0,0.9588430385051699,2023-12-01,157304.0,1.0327951729707372
 47,1933-06-01,23562.205642810604,0.7522093488319054,1941-06-01,36650.0,1.181838702395924,1949-01-01,44668.0,1.0661383869966823,1952-08-01,48924.0,1.080143065306663,1957-06-01,53067.0,1.0500831090707614,1961-07-01,54123.0,1.0187283541635297,1964-03-01,57897.0,1.056264024957583,1974-02-01,78254.0,1.0952121033995326,1978-06-01,86950.0,1.1057276565440766,1984-02-01,93157.0,1.0237707980745983,1985-06-01,97459.0,1.0639512669075666,1994-05-01,113923.0,1.0370117516407693,2005-01-01,132779.0,0.9999472835991746,2011-12-01,132902.0,0.960295382125335,2024-01-01,157560.0,1.0344759666204886
-48,1933-07-01,23699.0,0.7565764270208147,1941-07-01,37137.0,1.1975428073909258,1949-02-01,44497.0,1.062056949184906,1952-09-01,49320.0,1.088885945158299,1957-07-01,53123.0,1.0511912300142472,1961-08-01,54298.0,1.0220222858003312,1964-04-01,57922.0,1.056720121139146,1974-03-01,78296.0,1.0957999188254888,1978-07-01,87204.0,1.1089577292842974,1984-03-01,93429.0,1.026760006154252,1985-07-01,97648.0,1.0660145631597908,1994-06-01,114237.0,1.0398700128348672,2005-02-01,133033.0,1.0018601358576957,2012-01-01,133243.0,0.9627593083665108,2024-02-01,157830.0,1.036248678672961
-49,1933-08-01,23855.284492298244,0.7615657161377296,1941-08-01,37544.0,1.2106671826126214,1949-03-01,44240.0,1.0559228584385516,1952-10-01,49597.0,1.0950015454585595,1957-08-01,53128.0,1.0512901693842014,1961-09-01,54388.0,1.0237163077849722,1964-05-01,58089.0,1.0597668436319851,1974-04-01,78382.0,1.097003540888161,1978-08-01,87483.0,1.1125057225698154,1984-04-01,93792.0,1.030749280172319,1985-08-01,97840.0,1.0681106101461775,1994-07-01,114607.0,1.043238027617721,2005-03-01,133154.0,1.0027713765005346,2012-02-01,133521.0,0.9647680224282318,2024-03-01,158133.0,1.0382380555318464
-50,1933-09-01,24028.15512160773,0.7670845077770314,1941-09-01,37835.0,1.2200509496630227,1949-04-01,44236.0,1.0558273862090364,1952-11-01,49816.0,1.0998366229522674,1957-09-01,52934.0,1.0474513218299826,1961-10-01,54522.0,1.0262385182954374,1964-06-01,58219.0,1.0621385437761115,1974-05-01,78549.0,1.0993408069866062,1978-09-01,87621.0,1.1142606439798566,1984-05-01,94098.0,1.0341121392619295,1985-09-01,98045.0,1.0703485769806007,1994-08-01,114899.0,1.045896028473379,2005-04-01,133515.0,1.005490036600244,2012-03-01,133745.0,0.9663865546218487,,,
+48,1933-07-01,23699.0,0.7565764270208147,1941-07-01,37137.0,1.1975428073909258,1949-02-01,44497.0,1.062056949184906,1952-09-01,49320.0,1.088885945158299,1957-07-01,53123.0,1.0511912300142472,1961-08-01,54298.0,1.0220222858003312,1964-04-01,57922.0,1.056720121139146,1974-03-01,78296.0,1.0957999188254888,1978-07-01,87204.0,1.1089577292842974,1984-03-01,93429.0,1.026760006154252,1985-07-01,97648.0,1.0660145631597908,1994-06-01,114237.0,1.0398700128348672,2005-02-01,133033.0,1.0018601358576957,2012-01-01,133243.0,0.9627593083665108,2024-02-01,157796.0,1.0360254482663533
+49,1933-08-01,23855.284492298244,0.7615657161377296,1941-08-01,37544.0,1.2106671826126214,1949-03-01,44240.0,1.0559228584385516,1952-10-01,49597.0,1.0950015454585595,1957-08-01,53128.0,1.0512901693842014,1961-09-01,54388.0,1.0237163077849722,1964-05-01,58089.0,1.0597668436319851,1974-04-01,78382.0,1.097003540888161,1978-08-01,87483.0,1.1125057225698154,1984-04-01,93792.0,1.030749280172319,1985-08-01,97840.0,1.0681106101461775,1994-07-01,114607.0,1.043238027617721,2005-03-01,133154.0,1.0027713765005346,2012-02-01,133521.0,0.9647680224282318,2024-03-01,158111.0,1.038093612327571
+50,1933-09-01,24028.15512160773,0.7670845077770314,1941-09-01,37835.0,1.2200509496630227,1949-04-01,44236.0,1.0558273862090364,1952-11-01,49816.0,1.0998366229522674,1957-09-01,52934.0,1.0474513218299826,1961-10-01,54522.0,1.0262385182954374,1964-06-01,58219.0,1.0621385437761115,1974-05-01,78549.0,1.0993408069866062,1978-09-01,87621.0,1.1142606439798566,1984-05-01,94098.0,1.0341121392619295,1985-09-01,98045.0,1.0703485769806007,1994-08-01,114899.0,1.045896028473379,2005-04-01,133515.0,1.005490036600244,2012-03-01,133745.0,0.9663865546218487,2024-04-01,158286.0,1.0392425923615807
 51,1933-10-01,24214.29780179063,0.7730270017172338,1941-10-01,37949.0,1.2237270645899843,1949-05-01,43984.0,1.0498126357495763,1952-12-01,50166.0,1.1075639157504304,1957-10-01,52763.0,1.0440675953775527,1961-11-01,54742.0,1.0303794609245596,1964-07-01,58412.0,1.0656596062977761,1974-06-01,78604.0,1.1001105652825014,1978-10-01,87956.0,1.1185207792868406,1984-06-01,94479.0,1.038299228520562,1985-10-01,98233.0,1.0724009563214376,1994-09-01,115253.0,1.0491183993737314,2005-05-01,133687.0,1.0067853538776679,2012-04-01,133828.0,0.966986278604305,,,
 52,1933-11-01,24410.398446709125,0.7792873977368512,1941-11-01,38024.0,1.2261455612524588,1949-06-01,43739.0,1.043964961691768,1953-01-01,50144.0,1.1070782002031174,1957-11-01,52558.0,1.0400110812094348,1961-12-01,54872.0,1.0328263815690408,1964-08-01,58619.0,1.0694360826811158,1974-07-01,78636.0,1.1005584246546585,1978-11-01,88391.0,1.124052596775014,1984-07-01,94789.0,1.0417060465525199,1985-11-01,98443.0,1.074693507712798,1994-10-01,115458.0,1.0509844616182855,2005-06-01,133939.0,1.0086831443073818,2012-05-01,133935.0,0.967759416750363,,,
 53,1933-12-01,24613.14297022539,0.7857598956143976,1941-12-01,38104.0,1.228725291025765,1949-07-01,43531.0,1.0390004057569755,1953-02-01,50339.0,1.1113834061906653,1957-12-01,52384.0,1.0365679911350325,1962-01-01,54891.0,1.033184008432465,1964-09-01,58903.0,1.0746173353036688,1974-08-01,78619.0,1.1003204993631999,1978-12-01,88671.0,1.127613306882344,1984-08-01,95032.0,1.0443765523001516,1985-12-01,98609.0,1.0765057150031114,1994-11-01,115873.0,1.054762099820676,2005-07-01,134297.0,1.0113792116638802,2012-06-01,134008.0,0.9682868848313186,,,
 54,1934-01-01,24819.217286201616,0.7923386951283877,1942-01-01,38347.0,1.2365612202121827,1949-08-01,43624.0,1.0412201350932047,1953-03-01,50473.0,1.1143418554333908,1958-01-01,52076.0,1.0304733259458603,1962-02-01,55188.0,1.03877428098178,1964-10-01,58793.0,1.0726105121047926,1974-09-01,78610.0,1.1001945389147807,1979-01-01,88808.0,1.1293555114705733,1984-09-01,95344.0,1.0478053498032838,1986-01-01,98732.0,1.0778484951037652,1994-12-01,116176.0,1.0575202308455538,2005-08-01,134495.0,1.0128703327157984,2012-07-01,134153.0,0.9693345954030795,,,
 55,1934-02-01,25025.307308499967,0.7989179960573352,1942-02-01,38512.0,1.241881912869627,1949-09-01,43780.0,1.0449435520442991,1953-04-01,50435.0,1.1135028922153045,1958-02-01,51576.0,1.020579388950451,1962-03-01,55275.0,1.0404118355669327,1964-11-01,59218.0,1.0803641471913596,1974-10-01,78630.0,1.100474451022379,1979-02-01,89055.0,1.1324965664581108,1984-10-01,95629.0,1.0509374244455678,1986-02-01,98847.0,1.0791039399133198,1995-01-01,116504.0,1.0605059304368407,2005-09-01,134552.0,1.013299594836805,2012-08-01,134329.0,0.9706062992694928,,,
 56,1934-03-01,25228.098950982636,0.8053919981797547,1942-03-01,38935.0,1.2555222340459837,1949-10-01,42942.0,1.0249421199608564,1953-05-01,50490.0,1.1147171810835872,1958-03-01,51299.0,1.0150981478549945,1962-04-01,55602.0,1.0465667821111277,1964-12-01,59421.0,1.0840676481856495,1974-11-01,78265.0,1.0953660550587117,1979-03-01,89479.0,1.1378884989063534,1984-11-01,95982.0,1.0548168011077654,1986-03-01,98934.0,1.0800537112040263,1995-02-01,116693.0,1.0622263487988932,2005-10-01,134646.0,1.014007500790746,2012-09-01,134512.0,0.9719285822669567,,,
 57,1934-04-01,25424.278127511796,0.8116549012741603,1942-04-01,39352.0,1.2689690754893426,1949-11-01,43242.0,1.0321025371744994,1953-06-01,50519.0,1.1153574424868635,1958-04-01,51027.0,1.009715846129492,1962-05-01,55628.0,1.0470561662400242,1965-01-01,59582.0,1.0870049075949135,1974-12-01,77652.0,1.0867867489608263,1979-04-01,89417.0,1.1371000559540159,1984-12-01,96107.0,1.0561905180561355,1986-04-01,99121.0,1.0820951736334756,1995-03-01,116907.0,1.0641743357273548,2005-11-01,135001.0,1.0166809754040336,2012-10-01,134672.0,0.9730846766909688,,,
```

### Comparing `usempl-plots-0.0.4/usempl_plots/get_payems.py` & `usempl-plots-0.0.5/usempl_plots/get_payems.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/usempl_plots/tseries_payems.py` & `usempl-plots-0.0.5/usempl_plots/tseries_payems.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/usempl_plots/usempl_industry.py` & `usempl-plots-0.0.5/usempl_plots/usempl_streaks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,16 @@
 """
-This module plots the change in monthly US seasonally adjusted US nonfarm
-employment (PAYEMS) by industry. The data is either taken from the St. Louis
-Federal Reserve's FRED system(https://fred.stlouisfed.org/) or loads it from
-this directory.
-
-https://www.bls.gov/webapps/legacy/cesbtab1.htm
+This module plots the streaks of consecutive positive employment gains from the
+US nonfarm employment (PAYEMS) seasonally adjusted monthly time series from the
+St. Louis Federal Reserve's FRED system
+(https://fred.stlouisfed.org/series/PAYEMS) or loads it from this directory and
+organizes it into series of consecutive positive monthly gain streaks.
 
 This module defines the following function(s):
-    usempl_ind_chg()
-
-The industries are:
-- Goods Producing:
-  - Mining and Logging
-  - Construction
-  - Manufacturing
-- Private Service Providing:
-  - Wholesale Trade
-  - Retail Trade
-  - Transportation and Warehousing
-  - Utilities
-- Information
-- Financial Activities
-- Professional and Business Services
-- Private Education and Health Services
-  - Private Educational Services
-  - Health Care and Social Assistance
-- Leisure and Hospitality
-- Other Services
-- Government
-  - Federal Government
-  - State Government
-  - Local Government
-
-Use this URL for API access: https://data.bls.gov/cgi-bin/srgate
+    usempl_streaks()
 """
 
 # Import packages
 import numpy as np
 import pandas as pd
 import pandas_datareader as pddr
 import datetime as dt
@@ -51,27 +25,26 @@
 from bokeh.palettes import Category20, Plasma256, Viridis8
 
 """
 Define functions
 """
 
 
-def usempl_ind_chg(
-    start_date="2010-10-01",
+def usempl_streaks(
+    start_date="min",
     end_date="max",
     download_from_internet=True,
-    fig_title_strk=(
-        "Change in US employment my industry: October 2010 to March 2024"
-    ),
+    scatter_histogram=True,
+    table_output=True,
     html_show=True,
 ):
     """
     This function creates the HTML and JavaScript code for the dynamic
-    visualization of the US change in monthly seasonally adjusted nonfarm
-    employment (PAYEMS) by industry.
+    visualization of the US positive employment streaks from 1939 (the
+    beginning of US monthly data) to the given end date.
 
     Args:
         start_date (str): start date of PAYEMS time series in 'YYYY-mm-dd'
             format or 'min'
     """
     # Create data and images directory paths
     cur_path = os.path.split(os.path.abspath(__file__))[0]
@@ -155,14 +128,15 @@
         columns=[
             "strk_num",
             "start_date",
             "end_date",
             "months_in_streak",
             "total_emp_gain",
             "avg_monthly_emp_gain",
+            "marker_color",
         ]
     )
     for i in range(usempl_df.shape[0]):
         if usempl_df.loc[i, "diff_monthly"] > 0:
             if strk_mths == 0:
                 j = i
                 strk_num += 1
@@ -204,14 +178,15 @@
                 strk_table_df.loc[strk_num - 1] = [
                     strk_num,
                     strk_start_mth_str,
                     strk_end_mth_str,
                     strk_mths,
                     strk_cum,
                     strk_cum / strk_mths,
+                    "",
                 ]
         elif (
             usempl_df.loc[i, "diff_monthly"] <= 0
             and usempl_df.loc[i - 1, "diff_monthly"] > 0
             and i > 0
         ):
             strk_df["strk_mths_tot"] = strk_mths
@@ -231,25 +206,31 @@
             strk_table_df.loc[strk_num - 1] = [
                 strk_num,
                 strk_start_mth_str,
                 strk_end_mth_str,
                 strk_mths,
                 strk_cum,
                 strk_cum / strk_mths,
+                "",
             ]
             strk_mths = 0
             strk_cum = 0
 
     print("Number of streaks:", strk_num)
 
     # Create Bokeh plot of PAYEMS normalized peak plot figure
+    fig_title_lst = [
+        ("US employment streaks: consecutive positive monthly"),
+        ("gains and cumulative employment gains, 1939 to 2024"),
+    ]
+    fig_title_short = "Figure 1. US employment streaks"
     filename_strk = "usempl_streaks_" + end_date_str2 + ".html"
     output_file(
         os.path.join(image_dir, filename_strk),
-        title=fig_title_strk,
+        title=fig_title_short,
         mode="inline",
     )
 
     # Format the tooltip
     tooltips = [
         ("Date", "@Date{%F}"),
         ("Current month in streak", "@strk_mths{0.}"),
@@ -319,26 +300,35 @@
 
     fig_lst_strk = []
     label_items_strk_lst = []
     j = -1
     for i in range(strk_num):
         if max_cum_val_lst[i] > 10_000_000 or max_mth_val_lst[i] > 40:
             j += 1
+            strk_table_df.loc[strk_table_df.index == i, "marker_color"] = (
+                Viridis8[7 - j]
+            )
             li = fig_strk.line(
                 x="strk_mths",
                 y="strk_cum",
                 source=strk_cds_lst[i],
                 color=Viridis8[7 - j],
                 # color=Plasma256[255 - int(i * (256 - 1) / (strk_num - 1))],
                 line_width=4,
                 alpha=0.7,
                 muted_alpha=0.15,
             )
             label_items_strk_lst.append((strk_label_lst[i], [li]))
         else:
+            # replace all values of strk_table_df["marker_color"] with "orange" if streak_table_df["months_in_streak"]<40 and streak_table_df["total_emp_gain"]<10_000_000
+            strk_table_df.loc[
+                (strk_table_df["months_in_streak"] < 40)
+                & (strk_table_df["total_emp_gain"] < 10_000_000),
+                "marker_color",
+            ] = "orange"
             li = fig_strk.line(
                 x="strk_mths",
                 y="strk_cum",
                 source=strk_cds_lst[i],
                 color="orange",
                 line_width=2,
                 alpha=0.7,
@@ -347,24 +337,26 @@
         fig_lst_strk.append(li)
 
     # Add legend
     legend = Legend(items=label_items_strk_lst, location="center")
     fig_strk.add_layout(legend, "right")
     fig_strk.legend.click_policy = "mute"
 
-    # Add title and subtitle to the plot
-    fig_strk.add_layout(
-        Title(
-            text=fig_title_strk,
-            text_font_style="bold",
-            text_font_size="11pt",
-            align="center",
-        ),
-        "above",
-    )
+    # Add title and subtitle to the plot doing reverse loop through items in
+    # fig_title_lst
+    for title_line_str in fig_title_lst[::-1]:
+        fig_strk.add_layout(
+            Title(
+                text=title_line_str,
+                text_font_style="bold",
+                text_font_size="15pt",
+                align="center",
+            ),
+            "above",
+        )
 
     # Add source text below figure
     updated_date_str = (
         download_date.strftime("%B")
         + " "
         + download_date.strftime("%d").lstrip("0")
         + ", "
@@ -401,53 +393,65 @@
         print("")
         print(
             strk_table_df[
                 (
                     (strk_table_df["months_in_streak"] >= 40)
                     | (strk_table_df["total_emp_gain"] >= 10_000_000)
                 )
-            ].sort_values(by="months_in_streak", ascending=False)
+            ][
+                [
+                    "strk_num",
+                    "start_date",
+                    "end_date",
+                    "months_in_streak",
+                    "total_emp_gain",
+                    "avg_monthly_emp_gain",
+                ]
+            ].sort_values(
+                by="months_in_streak", ascending=False
+            )
         )
 
     if html_show:
         show(fig_strk)
 
     fig_lst = [fig_strk]
 
     if scatter_histogram:
-        fig_title_scat = (
-            "US employment streaks: consecutive positive monthly gains and "
-            + "average monthly employment gains, 1939 to 2024"
-        )
+        fig_title_scat_lst = [
+            ("US employment streaks: consecutive positive monthly"),
+            ("gains and average monthly employment gains, 1939 to 2024"),
+        ]
+        fig_title_scat_short = "Figure 2. US employment streaks scatterplot"
         filename_scat = "usempl_streaks_scatter" + end_date_str2 + ".html"
         output_file(
             os.path.join(image_dir, filename_scat),
-            title=fig_title_scat,
+            title=fig_title_scat_short,
             mode="inline",
         )
 
         # Format the tooltip
         tooltips_scat = [
-            ("Start date", "@start_date{%F}"),
-            ("End date", "@end_date{%F}"),
+            ("Start date", "@start_date"),
+            ("End date", "@end_date"),
             ("Months in streak", "@months_in_streak{0.}"),
             ("Total employment gain", "@total_emp_gain{0,0.}"),
             ("Avg. monthly employment gain", "@avg_monthly_emp_gain{0,0.}"),
         ]
 
         min_avg_val = strk_table_df["avg_monthly_emp_gain"].min()
         max_avg_val = strk_table_df["avg_monthly_emp_gain"].max()
 
         strk_table_cds = ColumnDataSource(strk_table_df)
         datarange_avgmth_vals = max_avg_val - min_avg_val
         fig_scat = figure(
             height=500,
             width=700,
             x_axis_label="Streak length (months)",
-            y_axis_label="Avg. monthly employment gains (thousands)",
+            y_axis_label="Avg. monthly employment gains",
             x_minor_ticks=4,
             y_range=(
                 min_avg_val - fig_buffer_pct * datarange_avgmth_vals,
                 max_avg_val + fig_buffer_pct * datarange_avgmth_vals,
             ),
             y_minor_ticks=5,
             x_range=(
@@ -460,15 +464,14 @@
                 "zoom_in",
                 "zoom_out",
                 "box_zoom",
                 "pan",
                 "undo",
                 "redo",
                 "reset",
-                "hover",
                 "help",
             ],
             toolbar_location="left",
         )
         fig_scat.toolbar.logo = None
 
         # Set title font size and axes font sizes
@@ -484,45 +487,83 @@
             1_000_000: "1.0m",
             1_500_000: "1.5m",
             2_000_000: "2.0m",
         }
 
         fig_scat.yaxis.major_label_overrides = y_tick_label_dict_scat
 
-        scat = fig_scat.scatter(
+        # Add scatter points for all streaks with months <40 and
+        # total employment gain < 10 mil
+        strk_table_other_cds = ColumnDataSource(
+            strk_table_df[
+                (strk_table_df["months_in_streak"] < 40)
+                & (strk_table_df["total_emp_gain"] < 10_000_000)
+            ]
+        )
+        strk_table_big_df = strk_table_df[
+            (strk_table_df["months_in_streak"] >= 40)
+            | (strk_table_df["total_emp_gain"] >= 10_000_000)
+        ].sort_values(by="strk_num", ascending=True)
+        strk_table_big_cds = ColumnDataSource(strk_table_big_df)
+
+        for strk in range(strk_table_big_df.shape[0]):
+            strk_table_i_cds = ColumnDataSource(strk_table_big_df.iloc[[strk]])
+            scat_i = fig_scat.scatter(
+                x="months_in_streak",
+                y="avg_monthly_emp_gain",
+                source=strk_table_i_cds,
+                size=8,
+                line_width=1,
+                line_color="black",
+                fill_color="marker_color",
+                alpha=0.6,
+                legend_label=(
+                    strk_table_big_df.iloc[strk]["start_date"]
+                    + " to "
+                    + strk_table_big_df.iloc[strk]["end_date"]
+                ),
+            )
+
+        scat_other = fig_scat.scatter(
             x="months_in_streak",
             y="avg_monthly_emp_gain",
-            source=strk_table_cds,
+            source=strk_table_other_cds,
             size=8,
             line_width=1,
             line_color="black",
-            fill_color="blue",
+            fill_color="marker_color",
             alpha=0.6,
+            legend_label="All other streaks",
         )
-
-        # Add title and subtitle to the plot
-        fig_scat.add_layout(
-            Title(
-                text=fig_title_scat,
-                text_font_style="bold",
-                text_font_size="14pt",
-                align="center",
-            ),
-            "above",
-        )
+        # Add legend
+        fig_scat.legend.location = "top_right"
+        fig_scat.legend.border_line_width = 2
+        fig_scat.legend.border_line_color = "black"
+        fig_scat.legend.border_line_alpha = 1
+        fig_scat.legend.label_text_font_size = "4mm"
+        fig_scat.legend.click_policy = "mute"
+
+        # Add title and subtitle to the plot doing reverse loop through items
+        # in fig_title_scat_lst
+        for title_line_str in fig_title_scat_lst[::-1]:
+            fig_scat.add_layout(
+                Title(
+                    text=title_line_str,
+                    text_font_style="bold",
+                    text_font_size="15pt",
+                    align="center",
+                ),
+                "above",
+            )
 
         # Add the HoverTool to the figure
         fig_scat.add_tools(
             HoverTool(
                 tooltips=tooltips_scat,
                 visible=False,
-                formatters={
-                    "@Start date": "datetime",
-                    "@End date": "datetime",
-                },
             )
         )
 
         # create the horizontal histogram
         hhist, hedges = np.histogram(
             strk_table_df["months_in_streak"], bins=24, range=(0, 120)
         )
@@ -713,10 +754,15 @@
 
         # fig_lst.append(fig_scat)
         fig_lst.append(layout)
 
     return fig_lst, beg_date_str2, end_date_str2
 
 
+# def usempl_streaks_hist():
+
+#     return fig, beg_date_str2, end_date_str2
+
+
 if __name__ == "__main__":
     # execute only if run as a script
     fig_lst, beg_date_str, end_date_str = usempl_streaks()
```

### Comparing `usempl-plots-0.0.4/usempl_plots/usempl_npp.py` & `usempl-plots-0.0.5/usempl_plots/usempl_npp.py`

 * *Files identical despite different names*

### Comparing `usempl-plots-0.0.4/usempl_plots.egg-info/PKG-INFO` & `usempl-plots-0.0.5/usempl_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usempl-plots
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package for creating plots of US employment and unemployment
 Home-page: https://github.com/OpenSourceEcon/usempl-plots
 Download-URL: https://github.com/OpenSourceEcon/usempl-plots
 Author: Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/OpenSourceEcon/usempl-plots/issues
 Keywords: Data analysis visualization tools US employment unemployment
```

### Comparing `usempl-plots-0.0.4/usempl_plots.egg-info/SOURCES.txt` & `usempl-plots-0.0.5/usempl_plots.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,11 +10,10 @@
 usempl_plots/usempl_streaks.py
 usempl_plots.egg-info/PKG-INFO
 usempl_plots.egg-info/SOURCES.txt
 usempl_plots.egg-info/dependency_links.txt
 usempl_plots.egg-info/requires.txt
 usempl_plots.egg-info/top_level.txt
 usempl_plots/data/recession_data.csv
-usempl_plots/data/usempl_2024-03-01.csv
-usempl_plots/data/usempl_2024-03-01_streaks.csv
+usempl_plots/data/usempl_2024-04-01.csv
 usempl_plots/data/usempl_annual_1919-1938.csv
-usempl_plots/data/usempl_pk_2024-03-01.csv
+usempl_plots/data/usempl_pk_2024-04-01.csv
```

