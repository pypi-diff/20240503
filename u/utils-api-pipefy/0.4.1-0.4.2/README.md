# Comparing `tmp/utils_api_pipefy-0.4.1.tar.gz` & `tmp/utils_api_pipefy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_api_pipefy-0.4.1.tar", max compression
+gzip compressed data, was "utils_api_pipefy-0.4.2.tar", max compression
```

## Comparing `utils_api_pipefy-0.4.1.tar` & `utils_api_pipefy-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1091 2023-01-12 23:43:28.565576 utils_api_pipefy-0.4.1/LICENSE
--rw-r--r--   0        0        0      787 2023-03-08 11:20:53.533175 utils_api_pipefy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1554 2023-01-26 00:48:24.297085 utils_api_pipefy-0.4.1/README.md
--rw-r--r--   0        0        0      161 2023-01-26 00:48:24.297085 utils_api_pipefy-0.4.1/utils_api_pipefy/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 23:43:28.569970 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/__init__.py
--rw-r--r--   0        0        0    14823 2023-03-08 11:18:16.860379 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/engine.py
--rw-r--r--   0        0        0     1027 2023-01-25 23:48:43.105797 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/excepts.py
--rw-r--r--   0        0        0     1888 2023-01-29 15:07:17.738810 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/log.py
--rw-r--r--   0        0        0    66622 2023-03-06 11:49:30.328826 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/pipefy.py
--rw-r--r--   0        0        0    22508 2023-01-29 21:23:16.544420 utils_api_pipefy-0.4.1/utils_api_pipefy/libs/utilits_pipe.py
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 utils_api_pipefy-0.4.1/setup.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 utils_api_pipefy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-03 12:14:26.696723 utils_api_pipefy-0.4.2/LICENSE
+-rw-r--r--   0        0        0      784 2024-05-03 12:27:29.914299 utils_api_pipefy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1590 2024-05-03 12:14:26.696723 utils_api_pipefy-0.4.2/README.md
+-rw-r--r--   0        0        0      161 2024-05-03 12:14:26.696723 utils_api_pipefy-0.4.2/utils_api_pipefy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:14:26.712430 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/__init__.py
+-rw-r--r--   0        0        0    14823 2024-05-03 12:22:19.516797 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/engine.py
+-rw-r--r--   0        0        0     1027 2024-05-03 12:22:19.527975 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/excepts.py
+-rw-r--r--   0        0        0     2064 2024-05-03 12:24:31.137671 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/log.py
+-rw-r--r--   0        0        0    66652 2024-05-03 12:22:19.562079 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/pipefy.py
+-rw-r--r--   0        0        0    22509 2024-05-03 12:22:19.580184 utils_api_pipefy-0.4.2/utils_api_pipefy/libs/utilits_pipe.py
+-rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 utils_api_pipefy-0.4.2/PKG-INFO
```

### Comparing `utils_api_pipefy-0.4.1/LICENSE` & `utils_api_pipefy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_api_pipefy-0.4.1/pyproject.toml` & `utils_api_pipefy-0.4.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "utils-api-pipefy"
-version = "0.4.1"
+version = "0.4.2"
 description = "Ferramentas para otimizar o consumo paralelizado de api do pipefy, trantando os retornos."
 readme = "README.md"
 repository = "https://github.com/YuriMotoshima/utils-api-pipefy"
 homepage = "https://github.com/YuriMotoshima/utils-api-pipefy"
 authors = ["Yuri Motoshima <yurimotoshima@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.27.1"
 python-dotenv = "^0.19.2"
 
 [tool.poetry.dev-dependencies]
-requests = "^2.27.1"
 pylint = "^2.12.2"
-autopep8 = "^1.6.0"
-pandas = "^1.3.5"
+
+[tool.poetry.group.dev.dependencies]
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "GitHub" = "https://github.com/YuriMotoshima/utils-api-pipefy"
```

### Comparing `utils_api_pipefy-0.4.1/README.md` & `utils_api_pipefy-0.4.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 Biblioteca que possui um kit de ferramentas úteis para ações usualmente rotineiras de quem trabalha com Pipefy, desde consulta de cards a criação de Pipes, Tables e atualizações em geral.
 
 Utilizamos como apoio as collection requests e python-dotenv.
 
 ## Instalação
 
-```
+```sh
 pip install utils-api-pipefy
 ```
 
 ## .env
-HOST_PIPE=app or seu_host_pipefy<br>
-PIPE= seu_numero_pipe<br>
-NONPHASES= [numeros_fases_ignoradas]<br>
-TOKEN= seu_token<br>
-LOGENV = DEV or PROD [ PROD remove urlib3 logs ]<br>
-LOGNAME = nome_arquivo_logs<br>
-DISABLELOG = True or False [True desabilita a criação de pasta e arquivo de logs, temos essa opção para utilização em plataformas como Google Cloud Platform, neste caso o logging apenas imprime da tela, sem salvar o log.]<br>
+>> HOST_PIPE=app or seu_host_pipefy<br>
+>> PIPE= seu_numero_pipe<br>
+>> NONPHASES= [id das fases que devem ser ignoradas]<br>
+>> TOKEN= seu_token<br>
+>> LOGENV = DEV or PROD [ PROD remove urlib3 logs ]<br>
+>> LOGNAME = nome_arquivo_logs<br>
+>> DISABLELOG = True or False [True desabilita a criação de pasta e arquivo de logs, temos essa opção para utilização em plataformas como Google Cloud Platform, neste caso o logging apenas imprime da tela, sem salvar o log.]<br>
 
 ## Exemplo de uso
 
 ```py
 import os
 import json
 import time
```

### Comparing `utils_api_pipefy-0.4.1/utils_api_pipefy/libs/engine.py` & `utils_api_pipefy-0.4.2/utils_api_pipefy/libs/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import re
 import logging
-from typing import NoReturn
-from datetime import datetime
-from os import (environ, getcwd)
+import re
 from concurrent.futures import ProcessPoolExecutor, as_completed
+from datetime import datetime
+from os import environ, getcwd
+from typing import NoReturn
 
 import requests
 from requests.adapters import HTTPAdapter
-
 from urllib3.util.retry import Retry
+
 from utils_api_pipefy.libs.excepts import exceptions
 from utils_api_pipefy.libs.utilits_pipe import Pipe
 
+
 class Engine(Pipe):
     def __init__(self, TOKEN=None, HOST=None, PIPE=None, NONPHASES=None):
         self.TOKEN = TOKEN or environ.get('TOKEN')
         self.HOST = HOST or environ.get('HOST_PIPE')
         self.PIPE = PIPE or environ.get('PIPE')
         self.NONPHASES = NONPHASES or environ.get('NONPHASES')
```

### Comparing `utils_api_pipefy-0.4.1/utils_api_pipefy/libs/excepts.py` & `utils_api_pipefy-0.4.2/utils_api_pipefy/libs/excepts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
-import sys
 import logging
-from traceback import (StackSummary, TracebackException, walk_tb)
+import sys
+from traceback import StackSummary, TracebackException, walk_tb
+
 
 class exceptions(Exception):
 
     def __init__(self, *args: object) -> None:
         self.args = args
         self.stack_summary = StackSummary()
         self.exc_info = sys.exc_info()
```

### Comparing `utils_api_pipefy-0.4.1/utils_api_pipefy/libs/log.py` & `utils_api_pipefy-0.4.2/utils_api_pipefy/libs/log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-from os import (path, environ, getcwd, makedirs)
-from sys import stdout
+import pathlib
+import re
+from logging import StreamHandler, basicConfig, FileHandler
 from datetime import datetime
-import logging
-from logging import (FileHandler, StreamHandler, basicConfig)
-from dotenv import load_dotenv
+import os
+import dotenv
+from sys import stdout
 from urllib3.connectionpool import log as urllib_log
 
-load_dotenv(dotenv_path=fr"{getcwd()}\.env")
+dotenv.load_dotenv(dotenv_path=fr"{os.getcwd()}\.env")
 
 formatter = '[%(levelname)s]: [%(filename)s line - %(lineno)d] | Date_Time: %(asctime)s | Function: [%(funcName)s] | Message: ➪ %(message)s'
 stdout_handler = StreamHandler(stdout)
-handlers = [stdout_handler]
-basicConfig(level=10,format=formatter, handlers=handlers, encoding='utf-8')
 
-def loginit(name_file_log:str = "Utils_Api_Pipefy", dev_env:str="DEV", disable_log:str=True):
-    name_file_log = environ.get("LOGNAME") if environ.get("LOGNAME") else name_file_log
-    dev_env = environ.get("LOGENV") if environ.get("LOGENV") else dev_env
-    disable_log = environ.get("DISABLELOG") if environ.get("DISABLELOG") else disable_log
-    valid_variables = list(set([name_file_log, dev_env, disable_log]))
+
+def loginit(name_file_log: str = "GPC", dev_env: str = "DEV", disable_log: str | bool = True):
+    """
+    Inicializa a configuração de log.
+
+    Args:
+        name_file_log (str, opcional): Nome base para o arquivo de log. Padrão "GPC".
+        dev_env (str, opcional): Indicador de ambiente (DEV ou PROD). Padrão "DEV".
+        disable_log (bool, opcional): Se desabilita o log. Padrão True.
+    """
+    basicConfig( level=10, format=formatter, handlers=[stdout_handler], encoding='utf-8')
     
     if (disable_log == True) or (disable_log == "True"):
         urllib_log.disabled = True
         return
-        
+    
+    valid_variables = list(set([name_file_log, dev_env, disable_log]))
+    
     if valid_variables:
-        filename = f'{name_file_log} - {datetime.now().strftime("%d-%m-%Y %H")}.log'
-        filename = f'[DEV] {filename}' if dev_env == 'DEV' else f'[PROD] {filename}'
-        dirname = f'{getcwd()}\\logs'
-        makedirs(dirname, exist_ok=True)
-        dirname = f'{getcwd()}\\logs\\{datetime.now().strftime("%d-%m-%Y")}'
-        makedirs(dirname, exist_ok=True)
-        full_filename = path.join(dirname, filename)
-        file_handler = logging.FileHandler(filename=full_filename, encoding='utf-8')
-        stdout_handler = logging.StreamHandler(stdout)
-        handlers = [file_handler, stdout_handler]
-        basicConfig(level=10,format=formatter, handlers=handlers, encoding='utf-8')
+        
+        filename_regex = re.compile(r"^[a-zA-Z0-9 -]{1,255}$")
+        
+        filename = f"Logs - {datetime.now().strftime('%d-%m-%Y %H')}.log"
+        if filename_regex.match(name_file_log):
+            filename = f"{name_file_log} - {datetime.now().strftime('%d-%m-%Y %H')}.log"
+            
+        new_filename = f'[DEV] {filename}' if dev_env == 'DEV' else f'[PROD] {filename}'
+        dirname = f"{os.getcwd()}/logs"
+        os.makedirs(dirname, exist_ok=True)
+        dirname = f"{dirname}/{datetime.now().strftime('%d-%m-%Y')}"
+        os.makedirs(dirname, exist_ok=True)
+        full_filename = pathlib.Path(dirname) / new_filename
+        
+        file_handler = FileHandler(filename=full_filename, encoding='utf-8')
+        basicConfig(level=10, format=formatter, handlers=[file_handler, stdout_handler], encoding='utf-8')
```

### Comparing `utils_api_pipefy-0.4.1/utils_api_pipefy/libs/pipefy.py` & `utils_api_pipefy-0.4.2/utils_api_pipefy/libs/pipefy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 import json
-import time
 import re
+import time
 
 import requests
-from requests.adapters import HTTPAdapter
-
 import urllib3
+from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from utils_api_pipefy.libs.excepts import exceptions
+
 urllib3.disable_warnings()
 
 
 class Pipefy(object):
     """ Integration class with Pipefy rest api. """
 
     def __init__(self, token, host="app"):
@@ -226,15 +226,15 @@
         except Exception as err:
           raise exceptions(err)
 
     def phase(self, id, after = None, response_fields=None, headers={}):
         """ Show phase: Get a phase by its identifier. """
         try:
           if after:
-            response_fields = response_fields or 'pageInfo { endCursor hasNextPage } edges { node { id title finished_at updated_at createdBy { id name } assignees { id name email } comments { text } comments_count current_phase { name } done due_date fields { name value datetime_value field { id } array_value  } labels { name } createdAt phases_history { phase { name id } created_at duration firstTimeIn lastTimeOut } url } }'
+            response_fields = response_fields or 'pageInfo { endCursor hasNextPage } edges { node { id title createdAt finished_at updated_at createdBy { id name } assignees { id name email } comments { text } comments_count current_phase { name } done due_date fields { name value datetime_value field { id } array_value  } labels { name } createdAt phases_history { phase { name id } created_at duration firstTimeIn lastTimeOut } url } }'
             query = '{ phase(id: %(id)s){ cards_count cards(after:%(after)s) {%(response_fields)s } } }' % {
                 'id': json.dumps(id),
                 'after':json.dumps(after),
                 'response_fields': response_fields,
             }
             return self.request(query, headers).get('data', {}).get('phase')
           else:
@@ -503,15 +503,15 @@
         except Exception as err:
           raise exceptions(err)
 
     def cards(self, pipe_id, count=10, search={}, response_fields=None, headers={}):
         """ List cards: Get cards by pipe identifier. """
         try:
           
-          response_fields = response_fields or 'edges { node { id title assignees { id }' \
+          response_fields = response_fields or 'edges { node { id title createdAt assignees { id }' \
                   ' comments { text } comments_count current_phase { name } done due_date ' \
                   'fields { field { id uuid } name value } labels { name } phases_history { phase { name } firstTimeIn lastTimeOut } url } }'
                   
           query = '{ cards(pipe_id: %(pipe_id)s, first: %(count)s, search: %(search)s) { %(response_fields)s } }' % {
               'pipe_id': json.dumps(pipe_id),
               'count': json.dumps(count),
               'search': self.__prepare_json_dict(search),
@@ -599,15 +599,15 @@
           raise exceptions(err)  
             
 
     def card(self, id, response_fields=None, headers={}):
         """ Show card: Get a card by its identifier. """
         try:
           
-          response_fields = response_fields or 'title assignees { id } comments { id } comments_count' \
+          response_fields = response_fields or 'title createdAt assignees { id } comments { id } comments_count' \
                   ' current_phase { name } done due_date fields { field { id uuid } name value } labels { name } phases_history ' \
                   '{ phase { name } firstTimeIn lastTimeOut } url '
           query = '{ card(id: %(id)s) { %(response_fields)s } }' % {
               'id': json.dumps(id),
               'response_fields': response_fields,
           }
           return self.request(query, headers).get('data', {}).get('card', [])
```

### Comparing `utils_api_pipefy-0.4.1/utils_api_pipefy/libs/utilits_pipe.py` & `utils_api_pipefy-0.4.2/utils_api_pipefy/libs/utilits_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import time
-from utils_api_pipefy.libs.pipefy import Pipefy
+
 from utils_api_pipefy.libs.excepts import exceptions
+from utils_api_pipefy.libs.pipefy import Pipefy
+
 
 class Pipe(Pipefy):
     def __init__(self, token, host, pipe, nonphases):
         """
             `Classe criada para`:
                 - Consumo das API's do Pipefy.
                 - Organização dos retornos das API's
@@ -78,19 +80,19 @@
                     else:
                         self.phases_id = [n.get("id") for n in campos_pipefy["phases"]]
                     
                     self.fields = {"fields":[{"id": d.get("id"), "nameField":d.get("label"), "editable":d.get("editable"), "uuid":d.get("uuid") , "required":d.get("required")} for n in campos_pipefy['phases'] for d in n['fields']] + [{"id": n.get("id"), "nameField": n.get("label"), "editable":n.get("editable"), "uuid":n.get("uuid"), "required":n.get("required")} for n in campos_pipefy['start_form_fields']]}
 
                     self.phases = {"phases" : [{ "id": d.get("id"), "nameFase": d.get("name"), "informacoes": [ "firstTimeIn", "lastTimeOut"] } for d in campos_pipefy['phases']]}
                 else:
-                    logging.info(f"Verificar se o token está habilitado ao pipefy.")
-                    raise exceptions(f"Verificar se o token está habilitado ao pipefy.")
+                    logging.info("Verificar se o token está habilitado ao pipefy.")
+                    raise exceptions("Verificar se o token está habilitado ao pipefy.")
 
             else:
-                logging.info(f"Por falta de informação do PIPE, não foi gerado as variávels : [self.phases_id, self.fields, self.phases]")
+                logging.info("Por falta de informação do PIPE, não foi gerado as variávels : [self.phases_id, self.fields, self.phases]")
                 
         except Exception as error:
             logging.info(error)
             raise exceptions(error)
     
     
     def __extract_basics(self, card : dict) -> list:
```

### Comparing `utils_api_pipefy-0.4.1/PKG-INFO` & `utils_api_pipefy-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: utils-api-pipefy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Ferramentas para otimizar o consumo paralelizado de api do pipefy, trantando os retornos.
 Home-page: https://github.com/YuriMotoshima/utils-api-pipefy
 License: MIT
 Author: Yuri Motoshima
 Author-email: yurimotoshima@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: GitHub, https://github.com/YuriMotoshima/utils-api-pipefy
 Project-URL: Repository, https://github.com/YuriMotoshima/utils-api-pipefy
 Description-Content-Type: text/markdown
 
 # utils-api-pipefy
 
 Biblioteca que possui um kit de ferramentas úteis para ações usualmente rotineiras de quem trabalha com Pipefy, desde consulta de cards a criação de Pipes, Tables e atualizações em geral.
 
 Utilizamos como apoio as collection requests e python-dotenv.
 
 ## Instalação
 
-```
+```sh
 pip install utils-api-pipefy
 ```
 
 ## .env
-HOST_PIPE=app or seu_host_pipefy<br>
-PIPE= seu_numero_pipe<br>
-NONPHASES= [numeros_fases_ignoradas]<br>
-TOKEN= seu_token<br>
-LOGENV = DEV or PROD [ PROD remove urlib3 logs ]<br>
-LOGNAME = nome_arquivo_logs<br>
-DISABLELOG = True or False [True desabilita a criação de pasta e arquivo de logs, temos essa opção para utilização em plataformas como Google Cloud Platform, neste caso o logging apenas imprime da tela, sem salvar o log.]<br>
+>> HOST_PIPE=app or seu_host_pipefy<br>
+>> PIPE= seu_numero_pipe<br>
+>> NONPHASES= [id das fases que devem ser ignoradas]<br>
+>> TOKEN= seu_token<br>
+>> LOGENV = DEV or PROD [ PROD remove urlib3 logs ]<br>
+>> LOGNAME = nome_arquivo_logs<br>
+>> DISABLELOG = True or False [True desabilita a criação de pasta e arquivo de logs, temos essa opção para utilização em plataformas como Google Cloud Platform, neste caso o logging apenas imprime da tela, sem salvar o log.]<br>
 
 ## Exemplo de uso
 
 ```py
 import os
 import json
 import time
```

