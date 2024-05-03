# Comparing `tmp/nerpii-0.2.1.tar.gz` & `tmp/nerpii-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerpii-0.2.1.tar", max compression
+gzip compressed data, was "nerpii-0.2.3.tar", max compression
```

## Comparing `nerpii-0.2.1.tar` & `nerpii-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3106 2024-05-02 08:40:04.243945 nerpii-0.2.1/README.md
--rw-r--r--   0        0        0      209 2024-05-02 08:40:04.247945 nerpii-0.2.1/nerpii/__init__.py
--rw-r--r--   0        0        0    22243 2024-05-02 08:40:04.247945 nerpii-0.2.1/nerpii/faker_generator.py
--rw-r--r--   0        0        0    18421 2024-05-02 08:40:04.247945 nerpii-0.2.1/nerpii/named_entity_recognizer.py
--rw-r--r--   0        0        0      841 2024-05-02 08:40:04.247945 nerpii-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 nerpii-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3336 2024-05-03 10:23:15.578353 nerpii-0.2.3/README.md
+-rw-r--r--   0        0        0      209 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/__init__.py
+-rw-r--r--   0        0        0    22243 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/faker_generator.py
+-rw-r--r--   0        0        0    18421 2024-05-03 10:23:15.578353 nerpii-0.2.3/nerpii/named_entity_recognizer.py
+-rw-r--r--   0        0        0      843 2024-05-03 10:23:15.582353 nerpii-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 nerpii-0.2.3/PKG-INFO
```

### Comparing `nerpii-0.2.1/README.md` & `nerpii-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 You can import the NamedEntityRecognizer using
 ```python
 from nerpii.named_entity_recognizer import NamedEntityRecognizer
 ```
 You can create a recognizer passing as parameter a path to a csv file or a Pandas Dataframe
 
 ```python
-recognizer = NamedEntityRecognizer('./csv_path.csv')
+recognizer = NamedEntityRecognizer('./csv_path.csv', lang)
 ```
+The <strong>lang</strong> parameter is used to define the language of the dataset. The deafult value is <strong>en</strong> (english), but it can be also selelcted <strong>it</strong> (italian).
+
 Please note that if there are columns in the dataset containing names of people consisting of first and last names (e.g. John Smith), before creating a recognizer, it is necessary to split the name into two different columns called <strong>first_name</strong> and <strong>last_name</strong> using the function `split_name()`.
 
 ```python
 from nerpii.named_entity_recognizer import split_name
 
 df = split_name('./csv_path.csv', name_of_column_to_split)
 ```
@@ -71,15 +73,15 @@
 ```
 
 You can create a generator using
 
 ```python
 generator = FakerGenerator(dataset, recognizer.dict_global_entities)
 ```
-If you want to generate Italian PII, add ```lang = "it"``` as parameter to the previous object.
+If you want to generate Italian PII, add ```lang = "it"``` as parameter to the previous object (default: ```lang = "en"```)
 
 To generate new PII you can run
 
 ```python
 generator.get_faker_generation()
 ```
 The method above can generate the following PII:
```

### Comparing `nerpii-0.2.1/nerpii/faker_generator.py` & `nerpii-0.2.3/nerpii/faker_generator.py`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.1/nerpii/named_entity_recognizer.py` & `nerpii-0.2.3/nerpii/named_entity_recognizer.py`

 * *Files identical despite different names*

### Comparing `nerpii-0.2.1/pyproject.toml` & `nerpii-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nerpii"
-version = "0.2.1"
+version = "0.2.3"
 description = "A python library to perform NER on structured data and generate PII with Faker"
 authors = ["Clearbox AI <info@clearbox.ai>"]
 license = "GPL"
 readme = "README.md"
 homepage = "https://github.com/Clearbox-AI/nerpii"
 repository = "https://github.com/Clearbox-AI/nerpii"
 packages = [{include = "nerpii"}]
@@ -13,15 +13,15 @@
 python = "^3.9"
 pandas = "^1.5.3"
 presidio-analyzer = "^2.2.32"
 transformers = "^4.26.1"
 faker = "^17.3.0"
 gender-guesser = "^0.4.0"
 simple-colors = "^0.1.5"
-spacy = "3.5.0"
+spacy = ">=3.5.0"
 torch = ">=1.13.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.1"
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
```

### Comparing `nerpii-0.2.1/PKG-INFO` & `nerpii-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerpii
-Version: 0.2.1
+Version: 0.2.3
 Summary: A python library to perform NER on structured data and generate PII with Faker
 Home-page: https://github.com/Clearbox-AI/nerpii
 License: GPL
 Author: Clearbox AI
 Author-email: info@clearbox.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=17.3.0,<18.0.0)
 Requires-Dist: gender-guesser (>=0.4.0,<0.5.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: presidio-analyzer (>=2.2.32,<3.0.0)
 Requires-Dist: simple-colors (>=0.1.5,<0.2.0)
-Requires-Dist: spacy (==3.5.0)
+Requires-Dist: spacy (>=3.5.0)
 Requires-Dist: torch (>=1.13.1)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Project-URL: Repository, https://github.com/Clearbox-AI/nerpii
 Description-Content-Type: text/markdown
 
 # Nerpii 
 Nerpii is a Python library developed to perform Named Entity Recognition (NER) on structured datasets and synthesize Personal Identifiable Information (PII).
@@ -39,16 +39,18 @@
 You can import the NamedEntityRecognizer using
 ```python
 from nerpii.named_entity_recognizer import NamedEntityRecognizer
 ```
 You can create a recognizer passing as parameter a path to a csv file or a Pandas Dataframe
 
 ```python
-recognizer = NamedEntityRecognizer('./csv_path.csv')
+recognizer = NamedEntityRecognizer('./csv_path.csv', lang)
 ```
+The <strong>lang</strong> parameter is used to define the language of the dataset. The deafult value is <strong>en</strong> (english), but it can be also selelcted <strong>it</strong> (italian).
+
 Please note that if there are columns in the dataset containing names of people consisting of first and last names (e.g. John Smith), before creating a recognizer, it is necessary to split the name into two different columns called <strong>first_name</strong> and <strong>last_name</strong> using the function `split_name()`.
 
 ```python
 from nerpii.named_entity_recognizer import split_name
 
 df = split_name('./csv_path.csv', name_of_column_to_split)
 ```
@@ -96,15 +98,15 @@
 ```
 
 You can create a generator using
 
 ```python
 generator = FakerGenerator(dataset, recognizer.dict_global_entities)
 ```
-If you want to generate Italian PII, add ```lang = "it"``` as parameter to the previous object.
+If you want to generate Italian PII, add ```lang = "it"``` as parameter to the previous object (default: ```lang = "en"```)
 
 To generate new PII you can run
 
 ```python
 generator.get_faker_generation()
 ```
 The method above can generate the following PII:
```

