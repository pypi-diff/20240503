# Comparing `tmp/crocodeel-1.0.0.tar.gz` & `tmp/crocodeel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crocodeel-1.0.0.tar", max compression
+gzip compressed data, was "crocodeel-1.0.1.tar", max compression
```

## Comparing `crocodeel-1.0.0.tar` & `crocodeel-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,17 @@
--rw-r--r--   0        0        0    35147 2024-04-24 15:38:44.141401 crocodeel-1.0.0/COPYING
--rw-r--r--   0        0        0     4255 2024-04-30 19:52:39.023352 crocodeel-1.0.0/README.md
--rw-r--r--   0        0        0       85 2024-05-02 09:14:00.563668 crocodeel-1.0.0/crocodeel/__init__.py
--rw-r--r--   0        0        0     1649 2024-05-02 09:04:14.502783 crocodeel-1.0.0/crocodeel/ab_table_utils.py
--rw-r--r--   0        0        0     2101 2024-04-24 15:38:44.141401 crocodeel-1.0.0/crocodeel/backup/filter_contamination_results_by_plate.py
--rw-r--r--   0        0        0     2232 2024-04-24 15:38:44.141401 crocodeel-1.0.0/crocodeel/backup/filter_contamination_results_if_longitudinal_samples.py
--rw-r--r--   0        0        0     1220 2024-04-24 15:38:44.141401 crocodeel-1.0.0/crocodeel/backup/write_parameters_file.py
--rw-r--r--   0        0        0     2135 2024-04-24 15:38:44.141401 crocodeel-1.0.0/crocodeel/backup/write_summary_report.py
--rw-r--r--   0        0        0     1788 2024-04-24 19:54:08.425740 crocodeel-1.0.0/crocodeel/conta_event.py
--rw-r--r--   0        0        0     6465 2024-05-02 09:13:06.407228 crocodeel-1.0.0/crocodeel/crocodeel.py
--rw-r--r--   0        0        0      670 2024-05-02 09:29:56.107269 crocodeel-1.0.0/crocodeel/easy_wf.py
--rw-r--r--   0        0        0   623880 2024-04-30 19:52:39.027352 crocodeel-1.0.0/crocodeel/models/crocodeel_rf_Mar2023.joblib
--rw-r--r--   0        0        0     6268 2024-05-02 09:31:56.752219 crocodeel-1.0.0/crocodeel/plot_conta.py
--rw-r--r--   0        0        0      453 2024-05-02 09:32:58.708706 crocodeel-1.0.0/crocodeel/rf_model.py
--rw-r--r--   0        0        0    16530 2024-05-02 09:35:31.769909 crocodeel-1.0.0/crocodeel/search_conta.py
--rw-r--r--   0        0        0   119253 2024-04-30 19:52:39.027352 crocodeel-1.0.0/crocodeel/test_data/mgs_profiles_test.tsv
--rw-r--r--   0        0        0    49550 2024-04-30 19:52:39.027352 crocodeel-1.0.0/crocodeel/test_data/results/contamination_events.pdf
--rw-r--r--   0        0        0     2051 2024-04-30 19:52:39.031353 crocodeel-1.0.0/crocodeel/test_data/results/contamination_events.tsv
--rw-r--r--   0        0        0     1879 2024-05-02 09:38:57.159504 crocodeel-1.0.0/crocodeel/test_install.py
--rw-r--r--   0        0        0     1379 2024-05-02 09:02:50.498048 crocodeel-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 crocodeel-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-04-24 15:38:44.141401 crocodeel-1.0.1/COPYING
+-rw-r--r--   0        0        0     4006 2024-05-02 14:45:55.722689 crocodeel-1.0.1/README.md
+-rw-r--r--   0        0        0       85 2024-05-02 09:14:00.563668 crocodeel-1.0.1/crocodeel/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-02 09:04:14.502783 crocodeel-1.0.1/crocodeel/ab_table_utils.py
+-rw-r--r--   0        0        0     1788 2024-04-24 19:54:08.425740 crocodeel-1.0.1/crocodeel/conta_event.py
+-rw-r--r--   0        0        0     6465 2024-05-02 09:13:06.407228 crocodeel-1.0.1/crocodeel/crocodeel.py
+-rw-r--r--   0        0        0      670 2024-05-02 09:29:56.107269 crocodeel-1.0.1/crocodeel/easy_wf.py
+-rw-r--r--   0        0        0   623880 2024-04-30 19:52:39.027352 crocodeel-1.0.1/crocodeel/models/crocodeel_rf_Mar2023.joblib
+-rw-r--r--   0        0        0     6268 2024-05-02 09:31:56.752219 crocodeel-1.0.1/crocodeel/plot_conta.py
+-rw-r--r--   0        0        0      453 2024-05-02 09:32:58.708706 crocodeel-1.0.1/crocodeel/rf_model.py
+-rw-r--r--   0        0        0    16530 2024-05-02 09:35:31.769909 crocodeel-1.0.1/crocodeel/search_conta.py
+-rw-r--r--   0        0        0   119253 2024-04-30 19:52:39.027352 crocodeel-1.0.1/crocodeel/test_data/mgs_profiles_test.tsv
+-rw-r--r--   0        0        0    49550 2024-04-30 19:52:39.027352 crocodeel-1.0.1/crocodeel/test_data/results/contamination_events.pdf
+-rw-r--r--   0        0        0     2051 2024-04-30 19:52:39.031353 crocodeel-1.0.1/crocodeel/test_data/results/contamination_events.tsv
+-rw-r--r--   0        0        0     1879 2024-05-02 09:38:57.159504 crocodeel-1.0.1/crocodeel/test_install.py
+-rw-r--r--   0        0        0     1379 2024-05-02 14:47:13.691194 crocodeel-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5105 1970-01-01 00:00:00.000000 crocodeel-1.0.1/PKG-INFO
```

### Comparing `crocodeel-1.0.0/COPYING` & `crocodeel-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/README.md` & `crocodeel-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-# CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels
+#  CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels 🐊
 
 ## Introduction
 
 CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data.\
 It accurately identifies contaminated samples but also pinpoints contamination sources and estimates contamination rates.\
 CroCoDeEL relies only on species abundance tables and does not need negative controls.
 
 ## Installation
 
-CroCoDeEL can be easily installed with conda.
-
-First, clone the git repository in a local directory:
-```
-git clone https://github.com/metagenopolis/crocodeel.git
-cd crocodeel
-```
-
-Then, create a specific conda environment with all requirements:
+CroCoDeEL can be easily installed with conda:
 ```
-conda env create -n crocodeel_env --file conda_env/environment.yml
+conda create --name crocodeel_env -c conda-forge -c fplazaonate crocodeel
+conda activate crocodeel_env
 ```
 
-Next, activate the conda environment: 
-
+Alternatively, you can use pip:
 ```
-conda activate crocodeel_env
+pip install crocodeel
 ```
 
 Finally, you can test that CroCoDeEL is correctly installed with the following command:
 ```
-python3 crocodeel/crocodeel.py test_install
+crocodeel test_install
 ```
 
-_CroCoDeEL will be released on bioconda soon._
-
 ## Quick start
 ### Input
 CroCoDeEL takes as input a species abundance table in TSV format.\
 The first column should correspond to species names. The other columns correspond to the abundance of species in each sample.
 
 |   species_name  | sample1 | sample2 | sample3 |    ...   | 
 |:----------------|:-------:|:-------:|:-------:|:--------:| 
@@ -45,39 +35,39 @@
 | species 2       |   0.1   |  0.01   |   0     |    ...   | 
 |       ...       |   ...   |   ...   |   ...   |    ...   | 
 
 CroCoDeEL works with relative abundances.
 The table will automatically be normalized so the abundance of each column equals 1.
 
 **Important**: CroCoDeEL requires the abundance of subdominant species to be accurately estimated.\
-We strongly recommend using [the Meteor software suite](https://github.com/metagenopolis/meteor) to generate the species abundance table. 
-Otherwise, you can use [sylph](https://github.com/bluenote-1577/sylph).\
+We strongly recommend using [the Meteor software suite](https://github.com/metagenopolis/meteor) to generate the species abundance table.\
+Alternatively, you can use [sylph](https://github.com/bluenote-1577/sylph) although low-level contaminations may go unnoticed.\
 We advise against the use of other taxonomic profilers (e.g. MetaPhlan4 or mOTUs) that do not meet this requirement according to our benchmarks.
 
 ### Search contamination
 Run the following command to search for cross-sample contamination:
 ```
-python3 crocodeel/crocodeel.py search_conta -s species_abundance.tsv -c contamination_events.tsv
+crocodeel search_conta -s species_abundance.tsv -c contamination_events.tsv
 ```
 CroCoDeEL will report all detected contamination events in the _contamination_events.tsv_ output file.\
 This TSV file reports for each event the contamination source, the contaminated sample (target) and the estimated contamination rate.\
 The score (probability) computed by the Random Forest model as well as species specifically introduced by contamination in the target are also given.
 
 ### Visualization of the results
 Contaminations events can be visually inspected by generating a PDF file consisting in scatterplots.
 ```
-python3 crocodeel/crocodeel.py plot_conta -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
+crocodeel plot_conta -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
 ```
 Each scatterplot compares in a log-scale the species abundance profiles of a contaminated sample (x-axis) and its contamination source (y-axis).\
 The contamination line (in red) highlights species specifically introduced by contamination.
 
 ### Easy workflow
 Alternatively, you can search for cross-sample contamination and create the PDF report in one command.
 ```
-python3 crocodeel/crocodeel.py easy_wf -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
+crocodeel easy_wf -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
 ```
 
 ### Results interpretation
 CroCoDeEL will probably report false contamination events for samples with similar species abundances profiles (e.g. longitudinal data, animals raised together).\
 For non-related samples, CroCoDeEL may occasionally generate false positives that can be filtered out by a human-expert.\
 Thus, we strongly recommend inspecting scatterplots of each contamination event to discard potential false positives.\
 _We will explain how to do it soon._
```

### Comparing `crocodeel-1.0.0/crocodeel/ab_table_utils.py` & `crocodeel-1.0.1/crocodeel/ab_table_utils.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/conta_event.py` & `crocodeel-1.0.1/crocodeel/conta_event.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/crocodeel.py` & `crocodeel-1.0.1/crocodeel/crocodeel.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/easy_wf.py` & `crocodeel-1.0.1/crocodeel/easy_wf.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/models/crocodeel_rf_Mar2023.joblib` & `crocodeel-1.0.1/crocodeel/models/crocodeel_rf_Mar2023.joblib`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/plot_conta.py` & `crocodeel-1.0.1/crocodeel/plot_conta.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/search_conta.py` & `crocodeel-1.0.1/crocodeel/search_conta.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/test_data/mgs_profiles_test.tsv` & `crocodeel-1.0.1/crocodeel/test_data/mgs_profiles_test.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/test_data/results/contamination_events.pdf` & `crocodeel-1.0.1/crocodeel/test_data/results/contamination_events.pdf`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/test_data/results/contamination_events.tsv` & `crocodeel-1.0.1/crocodeel/test_data/results/contamination_events.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/crocodeel/test_install.py` & `crocodeel-1.0.1/crocodeel/test_install.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.0/pyproject.toml` & `crocodeel-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crocodeel"
-version = "1.0.0"
+version = "1.0.1"
 description = "CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data"
 authors = [
     "Lindsay Goulet <lindsay.goulet@inrae.fr>",
     "Florian Plaza Oñate <florian.plaza-onate@inrae.fr>",
     "Edi Prifti <edi.prifti@ird.fr>",
     "Eugeni Belda <eugeni.belda@ird.fr>",
     "Emmanuelle Le Chatelier <emmanuelle.le-chatelier@inrae.fr>",
```

### Comparing `crocodeel-1.0.0/PKG-INFO` & `crocodeel-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crocodeel
-Version: 1.0.0
+Version: 1.0.1
 Summary: CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data
 Home-page: https://github.com/metagenopolis/CroCoDeEL
 License: GPL-3.0-or-later
 Keywords: Metagenomics
 Author: Lindsay Goulet
 Author-email: lindsay.goulet@inrae.fr
 Requires-Python: >=3.12
@@ -21,50 +21,40 @@
 Requires-Dist: pandas (>=2.2,<3.0)
 Requires-Dist: scikit-learn (==1.3.0)
 Requires-Dist: scipy (>=1.13,<2.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Project-URL: Repository, https://github.com/metagenopolis/CroCoDeEL
 Description-Content-Type: text/markdown
 
-# CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels
+#  CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels 🐊
 
 ## Introduction
 
 CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data.\
 It accurately identifies contaminated samples but also pinpoints contamination sources and estimates contamination rates.\
 CroCoDeEL relies only on species abundance tables and does not need negative controls.
 
 ## Installation
 
-CroCoDeEL can be easily installed with conda.
-
-First, clone the git repository in a local directory:
-```
-git clone https://github.com/metagenopolis/crocodeel.git
-cd crocodeel
-```
-
-Then, create a specific conda environment with all requirements:
+CroCoDeEL can be easily installed with conda:
 ```
-conda env create -n crocodeel_env --file conda_env/environment.yml
+conda create --name crocodeel_env -c conda-forge -c fplazaonate crocodeel
+conda activate crocodeel_env
 ```
 
-Next, activate the conda environment: 
-
+Alternatively, you can use pip:
 ```
-conda activate crocodeel_env
+pip install crocodeel
 ```
 
 Finally, you can test that CroCoDeEL is correctly installed with the following command:
 ```
-python3 crocodeel/crocodeel.py test_install
+crocodeel test_install
 ```
 
-_CroCoDeEL will be released on bioconda soon._
-
 ## Quick start
 ### Input
 CroCoDeEL takes as input a species abundance table in TSV format.\
 The first column should correspond to species names. The other columns correspond to the abundance of species in each sample.
 
 |   species_name  | sample1 | sample2 | sample3 |    ...   | 
 |:----------------|:-------:|:-------:|:-------:|:--------:| 
@@ -72,39 +62,39 @@
 | species 2       |   0.1   |  0.01   |   0     |    ...   | 
 |       ...       |   ...   |   ...   |   ...   |    ...   | 
 
 CroCoDeEL works with relative abundances.
 The table will automatically be normalized so the abundance of each column equals 1.
 
 **Important**: CroCoDeEL requires the abundance of subdominant species to be accurately estimated.\
-We strongly recommend using [the Meteor software suite](https://github.com/metagenopolis/meteor) to generate the species abundance table. 
-Otherwise, you can use [sylph](https://github.com/bluenote-1577/sylph).\
+We strongly recommend using [the Meteor software suite](https://github.com/metagenopolis/meteor) to generate the species abundance table.\
+Alternatively, you can use [sylph](https://github.com/bluenote-1577/sylph) although low-level contaminations may go unnoticed.\
 We advise against the use of other taxonomic profilers (e.g. MetaPhlan4 or mOTUs) that do not meet this requirement according to our benchmarks.
 
 ### Search contamination
 Run the following command to search for cross-sample contamination:
 ```
-python3 crocodeel/crocodeel.py search_conta -s species_abundance.tsv -c contamination_events.tsv
+crocodeel search_conta -s species_abundance.tsv -c contamination_events.tsv
 ```
 CroCoDeEL will report all detected contamination events in the _contamination_events.tsv_ output file.\
 This TSV file reports for each event the contamination source, the contaminated sample (target) and the estimated contamination rate.\
 The score (probability) computed by the Random Forest model as well as species specifically introduced by contamination in the target are also given.
 
 ### Visualization of the results
 Contaminations events can be visually inspected by generating a PDF file consisting in scatterplots.
 ```
-python3 crocodeel/crocodeel.py plot_conta -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
+crocodeel plot_conta -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
 ```
 Each scatterplot compares in a log-scale the species abundance profiles of a contaminated sample (x-axis) and its contamination source (y-axis).\
 The contamination line (in red) highlights species specifically introduced by contamination.
 
 ### Easy workflow
 Alternatively, you can search for cross-sample contamination and create the PDF report in one command.
 ```
-python3 crocodeel/crocodeel.py easy_wf -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
+crocodeel easy_wf -s species_abundance.tsv -c contamination_events.tsv -r contamination_events.pdf
 ```
 
 ### Results interpretation
 CroCoDeEL will probably report false contamination events for samples with similar species abundances profiles (e.g. longitudinal data, animals raised together).\
 For non-related samples, CroCoDeEL may occasionally generate false positives that can be filtered out by a human-expert.\
 Thus, we strongly recommend inspecting scatterplots of each contamination event to discard potential false positives.\
 _We will explain how to do it soon._
```

