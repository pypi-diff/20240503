# Comparing `tmp/mkdocs-typedoc-1.0.2.tar.gz` & `tmp/mkdocs_typedoc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-typedoc-1.0.2.tar", last modified: Thu Dec 21 14:13:42 2023, max compression
+gzip compressed data, was "mkdocs_typedoc-1.0.3.tar", last modified: Fri May  3 15:38:58 2024, max compression
```

## Comparing `mkdocs-typedoc-1.0.2.tar` & `mkdocs_typedoc-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-12-21 14:13:42.780980 mkdocs-typedoc-1.0.2/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-02 15:55:15.000000 mkdocs-typedoc-1.0.2/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     4795 2023-12-21 14:13:42.780849 mkdocs-typedoc-1.0.2/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     3466 2023-12-21 14:12:14.000000 mkdocs-typedoc-1.0.2/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-12-21 14:13:42.779644 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     4795 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      304 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       56 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/entry_points.txt
--rw-r--r--   0 kuba       (501) staff       (20)      112 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)        8 2023-12-21 14:13:42.000000 mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)     1236 2023-12-21 14:13:42.781360 mkdocs-typedoc-1.0.2/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)      192 2023-07-02 21:14:13.000000 mkdocs-typedoc-1.0.2/setup.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-12-21 14:13:42.779890 mkdocs-typedoc-1.0.2/typedoc/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs-typedoc-1.0.2/typedoc/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     4451 2023-12-21 14:12:14.000000 mkdocs-typedoc-1.0.2/typedoc/plugin.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 15:38:58.620669 mkdocs_typedoc-1.0.3/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-07-02 15:55:15.000000 mkdocs_typedoc-1.0.3/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     4925 2024-05-03 15:38:58.620533 mkdocs_typedoc-1.0.3/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     3596 2024-05-03 15:31:17.000000 mkdocs_typedoc-1.0.3/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 15:38:58.619799 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     4925 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)      304 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       56 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      112 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        8 2024-05-03 15:38:58.000000 mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     1236 2024-05-03 15:38:58.621078 mkdocs_typedoc-1.0.3/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)      210 2024-05-03 15:38:19.000000 mkdocs_typedoc-1.0.3/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-03 15:38:58.619417 mkdocs_typedoc-1.0.3/typedoc/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-03-26 20:51:00.000000 mkdocs_typedoc-1.0.3/typedoc/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4879 2024-05-03 15:31:28.000000 mkdocs_typedoc-1.0.3/typedoc/plugin.py
```

### Comparing `mkdocs-typedoc-1.0.2/LICENSE` & `mkdocs_typedoc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-typedoc-1.0.2/PKG-INFO` & `mkdocs_typedoc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-typedoc
-Version: 1.0.2
+Version: 1.0.3
 Summary: MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-typedoc
 Project-URL: Documentation, https://typedoc.kubaandrysek.cz/
@@ -69,30 +69,32 @@
   - typedoc:
       source: './ts-examples/@types/*.d.ts'
       output_dir: 'typedocApi'
       tsconfig: './ts-examples/tsconfig.json'
       options: 'typedoc.json'
       name: 'API Doc'
       disable_system_check: False
+      tile_link: "/" # optional, default: '/'
 ```
 
 - `source` (required): The path to your TypeScript source code.
 - `output_dir` (optional): The directory where you want to output your docs. Default is "typedoc".
 - `tsconfig` (required): The path to the tsconfig file for your project.
 - `options` (optional): The path to the typedoc.json options file with more options.
 - `name` (optional): The name for the generated documentation. Default is "TypeDoc API".
 - `disable_system_check` (optional): Disable the TypeScript system check. Default is False.
+- `tile_link` (optional): The link from TypeDoc back to the main page. Default is "/".
 
 The plugin will generate TypeDoc documentation into the output directory specified.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Do You Enjoy My Work?
-Then definitely consider:
+Then you can consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.2 Summary: MkDocs
+Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.3 Summary: MkDocs
 plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc Author: Jakub
 AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Project-URL: Source,
 https://github.com/JakubAndrysek/mkdocs-typedoc Project-URL: Documentation,
 https://typedoc.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/
 JakubAndrysek/mkdocs-typedoc/issues Project-URL: Funding, https://github.com/
 sponsors/jakubandrysek Keywords: mkdocs plugin Classifier: License :: OSI
@@ -32,22 +32,24 @@
 (https://pypi.org/project/mkdocs-typedoc/): ```bash pip install mkdocs-typedoc
 ``` Ensure that you have [Node.js](https://nodejs.org/en/) installed in your
 system. If not, you can download it from the official website. Also, install
 [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/): ```bash
 npm install typedoc typescript --save-dev ``` ## Usage Add the following lines
 to your mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/
 *.d.ts' output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json'
-options: 'typedoc.json' name: 'API Doc' disable_system_check: False ``` -
-`source` (required): The path to your TypeScript source code. - `output_dir`
-(optional): The directory where you want to output your docs. Default is
-"typedoc". - `tsconfig` (required): The path to the tsconfig file for your
-project. - `options` (optional): The path to the typedoc.json options file with
-more options. - `name` (optional): The name for the generated documentation.
-Default is "TypeDoc API". - `disable_system_check` (optional): Disable the
-TypeScript system check. Default is False. The plugin will generate TypeDoc
-documentation into the output directory specified. ## Contributing Pull
-requests are welcome. For major changes, please open an issue first to discuss
-what you would like to change. ## Do You Enjoy My Work? Then definitely
-consider: - supporting me on GitHub Sponsors: [![](https://img.shields.io/
-static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https:/
-/github.com/sponsors/jakubandrysek) ## License [MIT](https://
-choosealicense.com/licenses/mit/)
+options: 'typedoc.json' name: 'API Doc' disable_system_check: False tile_link:
+"/" # optional, default: '/' ``` - `source` (required): The path to your
+TypeScript source code. - `output_dir` (optional): The directory where you want
+to output your docs. Default is "typedoc". - `tsconfig` (required): The path to
+the tsconfig file for your project. - `options` (optional): The path to the
+typedoc.json options file with more options. - `name` (optional): The name for
+the generated documentation. Default is "TypeDoc API". - `disable_system_check`
+(optional): Disable the TypeScript system check. Default is False. -
+`tile_link` (optional): The link from TypeDoc back to the main page. Default is
+"/". The plugin will generate TypeDoc documentation into the output directory
+specified. ## Contributing Pull requests are welcome. For major changes, please
+open an issue first to discuss what you would like to change. ## Do You Enjoy
+My Work? Then you can consider: - supporting me on GitHub Sponsors: [![](https:
+//img.shields.io/static/
+v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
+github.com/sponsors/jakubandrysek) ## License [MIT](https://choosealicense.com/
+licenses/mit/)
```

### Comparing `mkdocs-typedoc-1.0.2/README.md` & `mkdocs_typedoc-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -38,30 +38,32 @@
   - typedoc:
       source: './ts-examples/@types/*.d.ts'
       output_dir: 'typedocApi'
       tsconfig: './ts-examples/tsconfig.json'
       options: 'typedoc.json'
       name: 'API Doc'
       disable_system_check: False
+      tile_link: "/" # optional, default: '/'
 ```
 
 - `source` (required): The path to your TypeScript source code.
 - `output_dir` (optional): The directory where you want to output your docs. Default is "typedoc".
 - `tsconfig` (required): The path to the tsconfig file for your project.
 - `options` (optional): The path to the typedoc.json options file with more options.
 - `name` (optional): The name for the generated documentation. Default is "TypeDoc API".
 - `disable_system_check` (optional): Disable the TypeScript system check. Default is False.
+- `tile_link` (optional): The link from TypeDoc back to the main page. Default is "/".
 
 The plugin will generate TypeDoc documentation into the output directory specified.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Do You Enjoy My Work?
-Then definitely consider:
+Then you can consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -15,22 +15,24 @@
 (https://pypi.org/project/mkdocs-typedoc/): ```bash pip install mkdocs-typedoc
 ``` Ensure that you have [Node.js](https://nodejs.org/en/) installed in your
 system. If not, you can download it from the official website. Also, install
 [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/): ```bash
 npm install typedoc typescript --save-dev ``` ## Usage Add the following lines
 to your mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/
 *.d.ts' output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json'
-options: 'typedoc.json' name: 'API Doc' disable_system_check: False ``` -
-`source` (required): The path to your TypeScript source code. - `output_dir`
-(optional): The directory where you want to output your docs. Default is
-"typedoc". - `tsconfig` (required): The path to the tsconfig file for your
-project. - `options` (optional): The path to the typedoc.json options file with
-more options. - `name` (optional): The name for the generated documentation.
-Default is "TypeDoc API". - `disable_system_check` (optional): Disable the
-TypeScript system check. Default is False. The plugin will generate TypeDoc
-documentation into the output directory specified. ## Contributing Pull
-requests are welcome. For major changes, please open an issue first to discuss
-what you would like to change. ## Do You Enjoy My Work? Then definitely
-consider: - supporting me on GitHub Sponsors: [![](https://img.shields.io/
-static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https:/
-/github.com/sponsors/jakubandrysek) ## License [MIT](https://
-choosealicense.com/licenses/mit/)
+options: 'typedoc.json' name: 'API Doc' disable_system_check: False tile_link:
+"/" # optional, default: '/' ``` - `source` (required): The path to your
+TypeScript source code. - `output_dir` (optional): The directory where you want
+to output your docs. Default is "typedoc". - `tsconfig` (required): The path to
+the tsconfig file for your project. - `options` (optional): The path to the
+typedoc.json options file with more options. - `name` (optional): The name for
+the generated documentation. Default is "TypeDoc API". - `disable_system_check`
+(optional): Disable the TypeScript system check. Default is False. -
+`tile_link` (optional): The link from TypeDoc back to the main page. Default is
+"/". The plugin will generate TypeDoc documentation into the output directory
+specified. ## Contributing Pull requests are welcome. For major changes, please
+open an issue first to discuss what you would like to change. ## Do You Enjoy
+My Work? Then you can consider: - supporting me on GitHub Sponsors: [![](https:
+//img.shields.io/static/
+v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
+github.com/sponsors/jakubandrysek) ## License [MIT](https://choosealicense.com/
+licenses/mit/)
```

### Comparing `mkdocs-typedoc-1.0.2/mkdocs_typedoc.egg-info/PKG-INFO` & `mkdocs_typedoc-1.0.3/mkdocs_typedoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-typedoc
-Version: 1.0.2
+Version: 1.0.3
 Summary: MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/mkdocs-typedoc
 Project-URL: Documentation, https://typedoc.kubaandrysek.cz/
@@ -69,30 +69,32 @@
   - typedoc:
       source: './ts-examples/@types/*.d.ts'
       output_dir: 'typedocApi'
       tsconfig: './ts-examples/tsconfig.json'
       options: 'typedoc.json'
       name: 'API Doc'
       disable_system_check: False
+      tile_link: "/" # optional, default: '/'
 ```
 
 - `source` (required): The path to your TypeScript source code.
 - `output_dir` (optional): The directory where you want to output your docs. Default is "typedoc".
 - `tsconfig` (required): The path to the tsconfig file for your project.
 - `options` (optional): The path to the typedoc.json options file with more options.
 - `name` (optional): The name for the generated documentation. Default is "TypeDoc API".
 - `disable_system_check` (optional): Disable the TypeScript system check. Default is False.
+- `tile_link` (optional): The link from TypeDoc back to the main page. Default is "/".
 
 The plugin will generate TypeDoc documentation into the output directory specified.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Do You Enjoy My Work?
-Then definitely consider:
+Then you can consider:
 
 - supporting me on GitHub Sponsors: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/jakubandrysek)
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.2 Summary: MkDocs
+Metadata-Version: 2.1 Name: mkdocs-typedoc Version: 1.0.3 Summary: MkDocs
 plugin to generate documentation from TypeScript source code using TypeDoc.
 Home-page: https://github.com/JakubAndrysek/mkdocs-typedoc Author: Jakub
 AndrÃ½sek Author-email: email@kubaandrysek.cz License: MIT Project-URL: Source,
 https://github.com/JakubAndrysek/mkdocs-typedoc Project-URL: Documentation,
 https://typedoc.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/
 JakubAndrysek/mkdocs-typedoc/issues Project-URL: Funding, https://github.com/
 sponsors/jakubandrysek Keywords: mkdocs plugin Classifier: License :: OSI
@@ -32,22 +32,24 @@
 (https://pypi.org/project/mkdocs-typedoc/): ```bash pip install mkdocs-typedoc
 ``` Ensure that you have [Node.js](https://nodejs.org/en/) installed in your
 system. If not, you can download it from the official website. Also, install
 [TypeDoc](https://typedoc.org/) using [NPM](https://www.npmjs.com/): ```bash
 npm install typedoc typescript --save-dev ``` ## Usage Add the following lines
 to your mkdocs.yml: ```yaml plugins: - typedoc: source: './ts-examples/@types/
 *.d.ts' output_dir: 'typedocApi' tsconfig: './ts-examples/tsconfig.json'
-options: 'typedoc.json' name: 'API Doc' disable_system_check: False ``` -
-`source` (required): The path to your TypeScript source code. - `output_dir`
-(optional): The directory where you want to output your docs. Default is
-"typedoc". - `tsconfig` (required): The path to the tsconfig file for your
-project. - `options` (optional): The path to the typedoc.json options file with
-more options. - `name` (optional): The name for the generated documentation.
-Default is "TypeDoc API". - `disable_system_check` (optional): Disable the
-TypeScript system check. Default is False. The plugin will generate TypeDoc
-documentation into the output directory specified. ## Contributing Pull
-requests are welcome. For major changes, please open an issue first to discuss
-what you would like to change. ## Do You Enjoy My Work? Then definitely
-consider: - supporting me on GitHub Sponsors: [![](https://img.shields.io/
-static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https:/
-/github.com/sponsors/jakubandrysek) ## License [MIT](https://
-choosealicense.com/licenses/mit/)
+options: 'typedoc.json' name: 'API Doc' disable_system_check: False tile_link:
+"/" # optional, default: '/' ``` - `source` (required): The path to your
+TypeScript source code. - `output_dir` (optional): The directory where you want
+to output your docs. Default is "typedoc". - `tsconfig` (required): The path to
+the tsconfig file for your project. - `options` (optional): The path to the
+typedoc.json options file with more options. - `name` (optional): The name for
+the generated documentation. Default is "TypeDoc API". - `disable_system_check`
+(optional): Disable the TypeScript system check. Default is False. -
+`tile_link` (optional): The link from TypeDoc back to the main page. Default is
+"/". The plugin will generate TypeDoc documentation into the output directory
+specified. ## Contributing Pull requests are welcome. For major changes, please
+open an issue first to discuss what you would like to change. ## Do You Enjoy
+My Work? Then you can consider: - supporting me on GitHub Sponsors: [![](https:
+//img.shields.io/static/
+v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://
+github.com/sponsors/jakubandrysek) ## License [MIT](https://choosealicense.com/
+licenses/mit/)
```

### Comparing `mkdocs-typedoc-1.0.2/setup.cfg` & `mkdocs_typedoc-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-typedoc
-version = 1.0.2
+version = 1.0.3
 description = MkDocs plugin to generate documentation from TypeScript source code using TypeDoc.
 keywords = mkdocs plugin
 url = https://github.com/JakubAndrysek/mkdocs-typedoc
 author = Jakub Andrýsek
 author_email = email@kubaandrysek.cz
 project_urls = 
 	Source = https://github.com/JakubAndrysek/mkdocs-typedoc
```

### Comparing `mkdocs-typedoc-1.0.2/typedoc/plugin.py` & `mkdocs_typedoc-1.0.3/typedoc/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,63 +15,70 @@
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class TypeDocPlugin(BasePlugin):
 
     config_scheme = (
-        ('source', config_options.Type(str, required=True)),
-        ('output_dir', config_options.Type(str, required=False, default="typedoc")),
-        ('tsconfig', config_options.Type(str, required=True)),
-        ('options', config_options.Type(str, required=False)),
-        ('name', config_options.Type(str, required=False, default="TypeDoc API")),
+        ("source", config_options.Type(str, required=True)),
+        ("output_dir", config_options.Type(str, required=False, default="typedoc")),
+        ("tsconfig", config_options.Type(str, required=True)),
+        ("options", config_options.Type(str, required=False)),
+        ("name", config_options.Type(str, required=False, default="TypeDoc API")),
+        ("tile_link", config_options.Type(str, required=False, default="/")),
     )
 
     def on_files(self, files, config):
         # Path to your TypeScript source code
-        src_path = self.config['source']
+        src_path = self.config["source"]
 
         # Path to the typedoc.json options file
-        typedoc_options = self.config.get('options')
+        typedoc_options = self.config.get("options")
 
-        output_dir = self.config['output_dir']
+        output_dir = self.config["output_dir"]
 
         # Path to the generated documentation
         doc_path = os.path.join(config["site_dir"], output_dir)
 
         if not os.path.exists(doc_path):
             os.makedirs(doc_path)
 
         # Name for the generated documentation
-        typedoc_name = self.config['name']
+        typedoc_name = self.config["name"]
 
         # Path to the tsconfig file
-        tsconfig_path = self.config['tsconfig']
+        tsconfig_path = self.config["tsconfig"]
 
         if not os.path.exists(tsconfig_path):
-            log.error("tsconfig.json file does not exist. Please create it or change the path in mkdocs.yml.")
+            log.error(
+                "tsconfig.json file does not exist. Please create it or change the path in mkdocs.yml."
+            )
             return files
 
         # Check if Node.js is installed
         if not self.is_node_installed():
-            log.error("Node.js is not installed. Please install it from https://nodejs.org/en/download/.")
+            log.error(
+                "Node.js is not installed. Please install it from https://nodejs.org/en/download/."
+            )
             return files
 
         # Check if TypeDoc is installed
         if not self.is_typedoc_installed():
-            log.error("TypeDoc is not installed. Please install it with `npm install typedoc --save-dev`. See https://typedoc.kubaandrysek.cz for more information.")
+            log.error(
+                "TypeDoc is not installed. Please install it with `npm install typedoc --save-dev`. See https://typedoc.kubaandrysek.cz for more information."
+            )
             return files
 
         # Build TypeDoc documentation
         try:
             typedoc_config = [
                 ("--out", doc_path),
                 ("--name", typedoc_name),
                 ("--tsconfig", tsconfig_path),
-                ("--titleLink", "/"),
+                ("--titleLink", self.config.get("tile_link", "/")),
             ]
 
             if typedoc_options:
                 typedoc_config.insert(2, ("--options", typedoc_options))
 
             # Flattening the list of pairs to pass into subprocess.run
             flattened_config = [item for pair in typedoc_config for item in pair]
@@ -86,34 +93,47 @@
             return files
 
         # Add generated TypeDoc documentation to MkDocs
         for dirpath, dirnames, filenames in os.walk(doc_path):
             for filename in filenames:
                 abs_src_path = os.path.join(dirpath, filename)
                 doc_rel_path = os.path.relpath(abs_src_path, config["site_dir"])
-                files.append(File(doc_rel_path, config["site_dir"], config["site_dir"], config["use_directory_urls"]))
+                files.append(
+                    File(
+                        doc_rel_path,
+                        config["site_dir"],
+                        config["site_dir"],
+                        config["use_directory_urls"],
+                    )
+                )
 
         return files
 
     def get_npx_filename(self):
         return "npx.cmd" if os.name == "nt" else "npx"
 
     def is_node_installed(self):
         try:
-            result = subprocess.run(["node", "--version"], check=True, capture_output=True, text=True)
+            result = subprocess.run(
+                ["node", "--version"], check=True, capture_output=True, text=True
+            )
             return result.returncode == 0
         except subprocess.CalledProcessError:
             return False
         except Exception as e:
             log.error(f"TypeDoc: Node.js failed with error: {e}")
             return False
 
     def is_typedoc_installed(self):
         try:
-            result = subprocess.run([self.get_npx_filename(), "typedoc", "--version"], check=True,
-                                    capture_output=True, text=True)
+            result = subprocess.run(
+                [self.get_npx_filename(), "typedoc", "--version"],
+                check=True,
+                capture_output=True,
+                text=True,
+            )
             return result.returncode == 0
         except subprocess.CalledProcessError:
             return False
         except Exception as e:
             log.error(f"TypeDoc: TypeDoc failed with error: {e}")
             return False
```

