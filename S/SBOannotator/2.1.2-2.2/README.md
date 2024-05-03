# Comparing `tmp/SBOannotator-2.1.2.tar.gz` & `tmp/SBOannotator-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SBOannotator-2.1.2.tar", last modified: Thu Jul  6 11:24:56 2023, max compression
+gzip compressed data, was "dist/SBOannotator-2.2.tar", last modified: Fri May  3 15:29:01 2024, max compression
```

## Comparing `SBOannotator-2.1.2.tar` & `SBOannotator-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-07-06 11:24:56.923191 SBOannotator-2.1.2/
--rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.1.2/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     4147 2023-07-06 11:24:56.922770 SBOannotator-2.1.2/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)     3375 2023-05-02 20:20:24.000000 SBOannotator-2.1.2/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-07-06 11:24:56.922273 SBOannotator-2.1.2/SBOannotator.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     4147 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      259 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       52 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       18 2023-07-06 11:24:56.000000 SBOannotator-2.1.2/SBOannotator.egg-info/top_level.txt
--rw-r--r--   0 leonidou   (501) staff       (20)    21544 2023-05-23 14:06:51.000000 SBOannotator-2.1.2/SBOannotator.py
--rw-r--r--   0 leonidou   (501) staff       (20)    13264 2023-01-23 22:12:54.000000 SBOannotator-2.1.2/create_dbs.sql
--rw-r--r--   0 leonidou   (501) staff       (20)     1261 2023-05-08 09:07:21.000000 SBOannotator-2.1.2/main.py
--rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.1.2/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-07-06 11:24:56.923323 SBOannotator-2.1.2/setup.cfg
--rw-r--r--   0 leonidou   (501) staff       (20)     1315 2023-07-06 11:20:45.000000 SBOannotator-2.1.2/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2024-05-03 15:29:01.779506 SBOannotator-2.2/
+-rw-r--r--   0 leonidou   (501) staff       (20)    35149 2023-01-23 22:12:54.000000 SBOannotator-2.2/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     4503 2024-05-03 15:29:01.779199 SBOannotator-2.2/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)     3734 2024-05-02 12:07:59.000000 SBOannotator-2.2/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2024-05-03 15:29:01.778745 SBOannotator-2.2/SBOannotator.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     4503 2024-05-03 15:29:01.000000 SBOannotator-2.2/SBOannotator.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)      259 2024-05-03 15:29:01.000000 SBOannotator-2.2/SBOannotator.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2024-05-03 15:29:01.000000 SBOannotator-2.2/SBOannotator.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       52 2024-05-03 15:29:01.000000 SBOannotator-2.2/SBOannotator.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       18 2024-05-03 15:29:01.000000 SBOannotator-2.2/SBOannotator.egg-info/top_level.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)    21384 2024-05-02 14:37:35.000000 SBOannotator-2.2/SBOannotator.py
+-rw-r--r--   0 leonidou   (501) staff       (20)    13264 2023-01-23 22:12:54.000000 SBOannotator-2.2/create_dbs.sql
+-rw-r--r--   0 leonidou   (501) staff       (20)     1225 2023-12-06 13:40:04.000000 SBOannotator-2.2/main.py
+-rw-r--r--   0 leonidou   (501) staff       (20)      104 2023-01-30 09:25:48.000000 SBOannotator-2.2/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2024-05-03 15:29:01.779599 SBOannotator-2.2/setup.cfg
+-rw-r--r--   0 leonidou   (501) staff       (20)     1312 2024-05-03 15:28:50.000000 SBOannotator-2.2/setup.py
```

### Comparing `SBOannotator-2.1.2/LICENSE` & `SBOannotator-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SBOannotator-2.1.2/PKG-INFO` & `SBOannotator-2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SBOannotator
-Version: 2.1.2
+Version: 2.2
 Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
 Home-page: https://github.com/draeger-lab/SBOannotator
 Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
 Author-email: nantia.leonidou@uni-tuebingen.de
-License:  GPL-3.0
+License: GPL-3.0
 Keywords: SBOannotator,SBO Terms,automated tool
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Operating System :: MacOS
@@ -21,34 +21,38 @@
 <img align="right" src="SBOannotator_logo.png" alt="drawing" width="200"/>
 
 **SBOannotator: a Python tool for the automated assignment of Systems Biology Ontology terms**
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
 [![Latest version](https://img.shields.io/badge/Latest_version-0.9-brightgreen.svg?style=plastic)](https://github.com/draeger-lab/SBOannotator/releases/)
 ![Code Size](https://img.shields.io/github/languages/code-size/draeger-lab/SBOannotator.svg?style=plastic)
-![Downloads of all releases](https://img.shields.io/github/downloads/draeger-lab/SBOannotator/total.svg?style=plastic)
-[![DOI](https://img.shields.io/badge/DOI-10.20944%2Fpreprints202012.0296.v1-blue.svg?style=plastic)](https://www.preprints.org/manuscript/202302.0317/v1)
+[![PyPI version](https://badge.fury.io/py/SBOannotator.svg)](https://badge.fury.io/py/SBOannotator)
+![PyPI - Format](https://img.shields.io/pypi/format/SBOannotator)
+[![PyPI downloads](https://img.shields.io/pypi/dm/SBOannotator.svg)](https://pypistats.org/packages/SBOannotator)
+[![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad437-blue.svg?style=plastic)](https://doi.org/10.1093/bioinformatics/btad437)
 
-*Authors* : Elisabeth Fritze & [Nantia Leonidou](https://github.com/NantiaL)
+*Developers* : [Nantia Leonidou](https://github.com/NantiaL) & Elisabeth Fritze
 ___________________________________________________________________________________________________________
 
 ### How to cite the SBOannotator?
 
-The online version of the SBOannotator is described in this article: https://www.preprints.org/manuscript/202302.0317/v1
+The SBOannotator is described in this article: https://doi.org/10.1093/bioinformatics/btad437
 
 ### Overview
-The SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
+SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
 The main focus lies on the reactions, as the correct assignment of precise SBO annotations requires their extensive classification. 
 Our implementation does not consider only top-level terms but examines the functionality of the underlying enzymes to 
 allocate precise and highly specific ontology terms to biochemical reactions. 
 Transport reactions are examined separately and are classified based on the mechanism of molecule transport. 
 Pseudo-reactions that serve modeling purposes are given reasonable terms to distinguish between biomass production and the 
 import or export of metabolites. Finally, other model entities, such as metabolites and genes, are annotated with appropriate terms. 
 Including SBO annotations in the models will enhance the reproducibility, usability, and analysis of biochemical networks.
 
+### Web Application
+Web application hosted at [TueVis](https://tuevis.cs.uni-tuebingen.de/sboannotator/) is accessible and ready to use at [sbo-annotator-tuevis.cs.uni-tuebingen.de/](https://sbo-annotator-tuevis.cs.uni-tuebingen.de/)
 
 ### Installation
 ```
 pip install SBOannotator
 ```
 
 ### Prerequisites
@@ -77,27 +81,25 @@
 - constraint-based
 - logical
 - continuous
 - discrete
 - hybrid
 - logical
 
-
 ### Outputs
-+ `model_libsbml`: Annotated libsbml model
-  
++ `model_libsbml`: Annotated libSBML model
 
 ### Usage
 To run SBOannotator use the `main.py` script and modify the parameters in the `readSBML` and `sbo_annotator` 
 functions as wished.
 
 If ERROR occurs, check the current version of Python: 
 
 - `python --version'`
-- `conda install python=3.8.5`
+- `conda install python>=3.8.5`
 
 ### Exemplary models and Results
 The folder `models/BiGG_Models` contains all the tested models as they were downloaded from
 the BiGG database. 
 The annotated models after using the SBOannotator are listed in the folder named `models/Annotated_Models`.
```

### Comparing `SBOannotator-2.1.2/README.md` & `SBOannotator-2.2/SBOannotator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,58 @@
+Metadata-Version: 2.1
+Name: SBOannotator
+Version: 2.2
+Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
+Home-page: https://github.com/draeger-lab/SBOannotator
+Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
+Author-email: nantia.leonidou@uni-tuebingen.de
+License: GPL-3.0
+Keywords: SBOannotator,SBO Terms,automated tool
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SBOannotator
 <img align="right" src="SBOannotator_logo.png" alt="drawing" width="200"/>
 
 **SBOannotator: a Python tool for the automated assignment of Systems Biology Ontology terms**
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
 [![Latest version](https://img.shields.io/badge/Latest_version-0.9-brightgreen.svg?style=plastic)](https://github.com/draeger-lab/SBOannotator/releases/)
 ![Code Size](https://img.shields.io/github/languages/code-size/draeger-lab/SBOannotator.svg?style=plastic)
-![Downloads of all releases](https://img.shields.io/github/downloads/draeger-lab/SBOannotator/total.svg?style=plastic)
-[![DOI](https://img.shields.io/badge/DOI-10.20944%2Fpreprints202012.0296.v1-blue.svg?style=plastic)](https://www.preprints.org/manuscript/202302.0317/v1)
+[![PyPI version](https://badge.fury.io/py/SBOannotator.svg)](https://badge.fury.io/py/SBOannotator)
+![PyPI - Format](https://img.shields.io/pypi/format/SBOannotator)
+[![PyPI downloads](https://img.shields.io/pypi/dm/SBOannotator.svg)](https://pypistats.org/packages/SBOannotator)
+[![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad437-blue.svg?style=plastic)](https://doi.org/10.1093/bioinformatics/btad437)
 
-*Authors* : Elisabeth Fritze & [Nantia Leonidou](https://github.com/NantiaL)
+*Developers* : [Nantia Leonidou](https://github.com/NantiaL) & Elisabeth Fritze
 ___________________________________________________________________________________________________________
 
 ### How to cite the SBOannotator?
 
-The online version of the SBOannotator is described in this article: https://www.preprints.org/manuscript/202302.0317/v1
+The SBOannotator is described in this article: https://doi.org/10.1093/bioinformatics/btad437
 
 ### Overview
-The SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
+SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
 The main focus lies on the reactions, as the correct assignment of precise SBO annotations requires their extensive classification. 
 Our implementation does not consider only top-level terms but examines the functionality of the underlying enzymes to 
 allocate precise and highly specific ontology terms to biochemical reactions. 
 Transport reactions are examined separately and are classified based on the mechanism of molecule transport. 
 Pseudo-reactions that serve modeling purposes are given reasonable terms to distinguish between biomass production and the 
 import or export of metabolites. Finally, other model entities, such as metabolites and genes, are annotated with appropriate terms. 
 Including SBO annotations in the models will enhance the reproducibility, usability, and analysis of biochemical networks.
 
+### Web Application
+Web application hosted at [TueVis](https://tuevis.cs.uni-tuebingen.de/sboannotator/) is accessible and ready to use at [sbo-annotator-tuevis.cs.uni-tuebingen.de/](https://sbo-annotator-tuevis.cs.uni-tuebingen.de/)
 
 ### Installation
 ```
 pip install SBOannotator
 ```
 
 ### Prerequisites
@@ -58,25 +81,25 @@
 - constraint-based
 - logical
 - continuous
 - discrete
 - hybrid
 - logical
 
-
 ### Outputs
-+ `model_libsbml`: Annotated libsbml model
-  
++ `model_libsbml`: Annotated libSBML model
 
 ### Usage
 To run SBOannotator use the `main.py` script and modify the parameters in the `readSBML` and `sbo_annotator` 
 functions as wished.
 
 If ERROR occurs, check the current version of Python: 
 
 - `python --version'`
-- `conda install python=3.8.5`
+- `conda install python>=3.8.5`
 
 ### Exemplary models and Results
 The folder `models/BiGG_Models` contains all the tested models as they were downloaded from
 the BiGG database. 
 The annotated models after using the SBOannotator are listed in the folder named `models/Annotated_Models`.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SBOannotator-2.1.2/SBOannotator.egg-info/PKG-INFO` & `SBOannotator-2.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,39 @@
-Metadata-Version: 2.1
-Name: SBOannotator
-Version: 2.1.2
-Summary: SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms
-Home-page: https://github.com/draeger-lab/SBOannotator
-Author: Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger
-Author-email: nantia.leonidou@uni-tuebingen.de
-License:  GPL-3.0
-Keywords: SBOannotator,SBO Terms,automated tool
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SBOannotator
 <img align="right" src="SBOannotator_logo.png" alt="drawing" width="200"/>
 
 **SBOannotator: a Python tool for the automated assignment of Systems Biology Ontology terms**
 
 [![License (LGPL version 3)](https://img.shields.io/badge/license-LGPLv3.0-blue.svg?style=plastic)](http://opensource.org/licenses/LGPL-3.0)
 [![Latest version](https://img.shields.io/badge/Latest_version-0.9-brightgreen.svg?style=plastic)](https://github.com/draeger-lab/SBOannotator/releases/)
 ![Code Size](https://img.shields.io/github/languages/code-size/draeger-lab/SBOannotator.svg?style=plastic)
-![Downloads of all releases](https://img.shields.io/github/downloads/draeger-lab/SBOannotator/total.svg?style=plastic)
-[![DOI](https://img.shields.io/badge/DOI-10.20944%2Fpreprints202012.0296.v1-blue.svg?style=plastic)](https://www.preprints.org/manuscript/202302.0317/v1)
+[![PyPI version](https://badge.fury.io/py/SBOannotator.svg)](https://badge.fury.io/py/SBOannotator)
+![PyPI - Format](https://img.shields.io/pypi/format/SBOannotator)
+[![PyPI downloads](https://img.shields.io/pypi/dm/SBOannotator.svg)](https://pypistats.org/packages/SBOannotator)
+[![DOI](https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtad437-blue.svg?style=plastic)](https://doi.org/10.1093/bioinformatics/btad437)
 
-*Authors* : Elisabeth Fritze & [Nantia Leonidou](https://github.com/NantiaL)
+*Developers* : [Nantia Leonidou](https://github.com/NantiaL) & Elisabeth Fritze
 ___________________________________________________________________________________________________________
 
 ### How to cite the SBOannotator?
 
-The online version of the SBOannotator is described in this article: https://www.preprints.org/manuscript/202302.0317/v1
+The SBOannotator is described in this article: https://doi.org/10.1093/bioinformatics/btad437
 
 ### Overview
-The SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
+SBOannotator is the first standalone tool that automatically assigns SBO terms to multiple entities of a given SBML model, 
 The main focus lies on the reactions, as the correct assignment of precise SBO annotations requires their extensive classification. 
 Our implementation does not consider only top-level terms but examines the functionality of the underlying enzymes to 
 allocate precise and highly specific ontology terms to biochemical reactions. 
 Transport reactions are examined separately and are classified based on the mechanism of molecule transport. 
 Pseudo-reactions that serve modeling purposes are given reasonable terms to distinguish between biomass production and the 
 import or export of metabolites. Finally, other model entities, such as metabolites and genes, are annotated with appropriate terms. 
 Including SBO annotations in the models will enhance the reproducibility, usability, and analysis of biochemical networks.
 
+### Web Application
+Web application hosted at [TueVis](https://tuevis.cs.uni-tuebingen.de/sboannotator/) is accessible and ready to use at [sbo-annotator-tuevis.cs.uni-tuebingen.de/](https://sbo-annotator-tuevis.cs.uni-tuebingen.de/)
 
 ### Installation
 ```
 pip install SBOannotator
 ```
 
 ### Prerequisites
@@ -77,27 +62,23 @@
 - constraint-based
 - logical
 - continuous
 - discrete
 - hybrid
 - logical
 
-
 ### Outputs
-+ `model_libsbml`: Annotated libsbml model
-  
++ `model_libsbml`: Annotated libSBML model
 
 ### Usage
 To run SBOannotator use the `main.py` script and modify the parameters in the `readSBML` and `sbo_annotator` 
 functions as wished.
 
 If ERROR occurs, check the current version of Python: 
 
 - `python --version'`
-- `conda install python=3.8.5`
+- `conda install python>=3.8.5`
 
 ### Exemplary models and Results
 The folder `models/BiGG_Models` contains all the tested models as they were downloaded from
 the BiGG database. 
 The annotated models after using the SBOannotator are listed in the folder named `models/Annotated_Models`.
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SBOannotator-2.1.2/SBOannotator.py` & `SBOannotator-2.2/SBOannotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__author__ = 'Elisabeth Fritze & Nantia Leonidou'
+__author__ = 'Nantia Leonidou & Elisabeth Fritze'
 
 """ SBOannotator: a Python tool for the automated assignment of Systems Biology Ontology terms """
 
 import sqlite3
 from libsbml import writeSBMLToFile
 from collections import Counter
 import requests
@@ -407,14 +407,15 @@
 #         if getECNums(react)[0].startswith('3'):
 #             react.setSBOTerm('SBO:0000376')
 #     else:
 #         handleMultipleOrNoECs(react, getECNums(react))
 
 
 def addSBOviaEC(react, cur):
+    # cur.execute(): case insensitive
     if len(getECNums(react)) == 1:
         ECnum = getECNums(react)[0]
         splittedEC = ECnum.split('.')
         if len(splittedEC) == 4:
             ECpos1 = splittedEC[0]
             ECpos1to2 = ECpos1 + '.' + splittedEC[1]
             ECpos1to3 = ECpos1to2 + '.' + splittedEC[2]
@@ -492,16 +493,14 @@
         doc.setSBOTerm('SBO:0000234')
     elif modelType == 'continuous':
         doc.setSBOTerm('SBO:0000062')
     elif modelType == 'discrete':
         doc.setSBOTerm('SBO:0000063')
     elif modelType == 'hybrid':
         doc.setSBOTerm('SBO:0000681')
-    elif modelType == 'logical':
-        doc.setSBOTerm('SBO:0000234')
     else:
         doc.setSBOTerm('SBO_0000004')
 
 
 def addSBOforGroups(model):
     mplugin = model.getPlugin('groups')
     # if groups are in model defined
@@ -644,19 +643,13 @@
     return model_libsbml
 
 
 def printCounts(model_sbml):
     model_fbc = model_sbml.getPlugin('fbc')
 
     # count assigned SBO
-    SBO_rxns, SBO_genes, SBO_mets, SBO_comps = [], [], [], []
-    for r in model_sbml.reactions:
-        SBO_rxns.append(r.getSBOTermID())
-    for m in model_sbml.species:
-        SBO_mets.append(m.getSBOTermID())
-    if model_fbc is not None:
-        for g in model_fbc.getListOfGeneProducts():
-            SBO_genes.append(g.getSBOTermID())
-    for c in model_sbml.compartments:
-        SBO_comps.append(c.getSBOTermID())
+    SBO_rxns = [r.getSBOTermID() for r in model_sbml.reactions]
+    SBO_mets = [m.getSBOTermID() for m in model_sbml.species]
+    SBO_genes = [g.getSBOTermID() for g in model_fbc.getListOfGeneProducts() if model_fbc is not None]
+    SBO_comps = [c.getSBOTermID() for c in model_sbml.compartments]
 
     return Counter(SBO_rxns), Counter(SBO_mets), Counter(SBO_genes), Counter(SBO_comps)
```

### Comparing `SBOannotator-2.1.2/create_dbs.sql` & `SBOannotator-2.2/create_dbs.sql`

 * *Files identical despite different names*

### Comparing `SBOannotator-2.1.2/main.py` & `SBOannotator-2.2/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+__author__ = 'Nantia Leonidou'
+
 from SBOannotator import *
 from libsbml import *
 import time
 
 start = time.time()
 
-#doc = readSBML('models/BiGG_Models/RECON1.xml')
-doc = readSBML('/Users/leonidou/Downloads/BIOMD0000000497_url.xml')
+doc = readSBML('models/BiGG_Models/RECON1.xml')
 model = doc.getModel()
 
 print('-----------------------------')
 print('SBO before: ')
 print('-----------------------------')
 print(f'Reactions: {printCounts(model)[0]}')
 print(f'\nMetabolites: {printCounts(model)[1]}')
@@ -32,8 +33,8 @@
 for r in model.reactions:
     if r.isSetSBOTerm() is False:
         print('\n*********************')
         print(f'No SBO set for reactions: {r.getId()}')
         print('\n*********************')
 
 end = time.time()
-print(f'SBOannotator done after:  {end - start}s')
+print(f'SBOannotator done after:  {end - start}s')
```

### Comparing `SBOannotator-2.1.2/setup.py` & `SBOannotator-2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SBOannotator',
-    version='2.1.2',
+    version='2.2',
     description='SBOannotator: A Python tool for the automated assignment of Systems Biology Ontology terms',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/SBOannotator',
     author='Nantia Leonidou, Elisabeth Fritze, Alina Renz, Andreas Dräger',
     author_email='nantia.leonidou@uni-tuebingen.de',
-    license=' GPL-3.0',
+    license='GPL-3.0',
     keywords=['SBOannotator', 'SBO Terms', 'automated tool'],
     install_requires=['python-libsbml',
                       'python-collection',
                       'requests',
                       'pypi-json'],
     #packages=find_packages(include=['models']),
     py_modules=['SBOannotator', 'main'],
```

