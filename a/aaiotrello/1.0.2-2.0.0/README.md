# Comparing `tmp/aaiotrello-1.0.2.tar.gz` & `tmp/aaiotrello-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaiotrello-1.0.2.tar", last modified: Fri Feb 16 06:58:18 2024, max compression
+gzip compressed data, was "aaiotrello-2.0.0.tar", last modified: Fri May  3 14:10:41 2024, max compression
```

## Comparing `aaiotrello-1.0.2.tar` & `aaiotrello-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 06:58:18.068221 aaiotrello-1.0.2/
--rw-rw-rw-   0        0        0     1088 2024-02-08 12:36:58.000000 aaiotrello-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1032 2024-02-16 06:58:18.066229 aaiotrello-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      643 2024-02-08 12:34:35.000000 aaiotrello-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 06:58:18.043087 aaiotrello-1.0.2/aaiotrello/
--rw-rw-rw-   0        0        0     1779 2024-02-08 12:33:28.000000 aaiotrello-1.0.2/aaiotrello/__init__.py
--rw-rw-rw-   0        0        0     3880 2024-02-13 07:07:38.000000 aaiotrello-1.0.2/aaiotrello/actions.py
--rw-rw-rw-   0        0        0     7993 2024-02-13 07:07:40.000000 aaiotrello-1.0.2/aaiotrello/boards.py
--rw-rw-rw-   0        0        0     8178 2024-02-13 07:07:41.000000 aaiotrello-1.0.2/aaiotrello/cards.py
--rw-rw-rw-   0        0        0     3675 2024-02-13 07:07:43.000000 aaiotrello-1.0.2/aaiotrello/checklists.py
--rw-rw-rw-   0        0        0     3810 2024-02-16 06:53:44.000000 aaiotrello-1.0.2/aaiotrello/lists.py
--rw-rw-rw-   0        0        0     7014 2024-02-13 07:07:47.000000 aaiotrello-1.0.2/aaiotrello/members.py
--rw-rw-rw-   0        0        0     4409 2024-02-13 07:07:49.000000 aaiotrello-1.0.2/aaiotrello/notifications.py
--rw-rw-rw-   0        0        0     4482 2024-02-13 07:07:51.000000 aaiotrello-1.0.2/aaiotrello/organizations.py
--rw-rw-rw-   0        0        0     1116 2024-02-13 07:07:52.000000 aaiotrello-1.0.2/aaiotrello/tokens.py
--rw-rw-rw-   0        0        0      393 2024-02-13 07:07:53.000000 aaiotrello-1.0.2/aaiotrello/types.py
--rw-rw-rw-   0        0        0     1218 2019-01-24 14:47:17.000000 aaiotrello-1.0.2/aaiotrello/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-16 06:58:18.065228 aaiotrello-1.0.2/aaiotrello.egg-info/
--rw-rw-rw-   0        0        0     1032 2024-02-16 06:58:17.000000 aaiotrello-1.0.2/aaiotrello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-02-16 06:58:17.000000 aaiotrello-1.0.2/aaiotrello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 06:58:17.000000 aaiotrello-1.0.2/aaiotrello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-16 06:58:17.000000 aaiotrello-1.0.2/aaiotrello.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-16 06:58:17.000000 aaiotrello-1.0.2/aaiotrello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-16 06:58:18.068221 aaiotrello-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1279 2024-02-16 06:56:40.000000 aaiotrello-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:10:41.155300 aaiotrello-2.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-02-08 12:36:58.000000 aaiotrello-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1680 2024-05-03 14:10:41.152788 aaiotrello-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      694 2024-05-03 14:10:34.000000 aaiotrello-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 14:10:41.103100 aaiotrello-2.0.0/aaiotrello/
+-rw-rw-rw-   0        0        0     1898 2024-05-03 13:59:30.000000 aaiotrello-2.0.0/aaiotrello/__init__.py
+-rw-rw-rw-   0        0        0     3880 2024-05-03 13:56:32.000000 aaiotrello-2.0.0/aaiotrello/actions.py
+-rw-rw-rw-   0        0        0     7993 2024-02-13 07:07:40.000000 aaiotrello-2.0.0/aaiotrello/boards.py
+-rw-rw-rw-   0        0        0     8178 2024-02-13 07:07:41.000000 aaiotrello-2.0.0/aaiotrello/cards.py
+-rw-rw-rw-   0        0        0     3675 2024-02-13 07:07:43.000000 aaiotrello-2.0.0/aaiotrello/checklists.py
+-rw-rw-rw-   0        0        0     3810 2024-02-16 06:53:44.000000 aaiotrello-2.0.0/aaiotrello/lists.py
+-rw-rw-rw-   0        0        0     7014 2024-02-13 07:07:47.000000 aaiotrello-2.0.0/aaiotrello/members.py
+-rw-rw-rw-   0        0        0     4409 2024-02-13 07:07:49.000000 aaiotrello-2.0.0/aaiotrello/notifications.py
+-rw-rw-rw-   0        0        0     4482 2024-02-13 07:07:51.000000 aaiotrello-2.0.0/aaiotrello/organizations.py
+-rw-rw-rw-   0        0        0     1116 2024-02-13 07:07:52.000000 aaiotrello-2.0.0/aaiotrello/tokens.py
+-rw-rw-rw-   0        0        0      393 2024-02-13 07:07:53.000000 aaiotrello-2.0.0/aaiotrello/types.py
+-rw-rw-rw-   0        0        0     1218 2019-01-24 14:47:17.000000 aaiotrello-2.0.0/aaiotrello/utils.py
+-rw-rw-rw-   0        0        0      944 2024-05-03 14:05:50.000000 aaiotrello-2.0.0/aaiotrello/webhooks.py
+drwxrwxrwx   0        0        0        0 2024-05-03 14:10:41.150792 aaiotrello-2.0.0/aaiotrello.egg-info/
+-rw-rw-rw-   0        0        0     1680 2024-05-03 14:10:40.000000 aaiotrello-2.0.0/aaiotrello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2024-05-03 14:10:40.000000 aaiotrello-2.0.0/aaiotrello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 14:10:40.000000 aaiotrello-2.0.0/aaiotrello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 14:10:40.000000 aaiotrello-2.0.0/aaiotrello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-03 14:10:40.000000 aaiotrello-2.0.0/aaiotrello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 14:10:41.156310 aaiotrello-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2024-05-03 14:09:41.000000 aaiotrello-2.0.0/setup.py
```

### Comparing `aaiotrello-1.0.2/LICENSE` & `aaiotrello-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/README.md` & `aaiotrello-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# aaiotrello
-Async Trello API Client
-
-Python 3.6+
-
-## Install
-
-```bash
-pip install aaiotrello
-```
-
-## Auth
-
-#### TRELLO_APP_KEY: https://trello.com/app-key/
-#### TRELLO_APP_TOKEN:
-
-First you need gen auth url:
-```python
-from aaiotrello import TrelloApi
-
-trello = TrelloApi(config.TRELLO_KEY)
-trello.set_token(config.TRELLO_TOKEN)
-```
-Than you need copy value of token_url and auth your trello account in webbrowser
-After that you will get token
-
-#### Apply token in your app:
-```python
-trello_app.set_token(TRELLO_APP_TOKEN)
-```
-
-#### Sample usage
-
-Get board info:
-```python
-board = await trello_app.boards.get("5c49c07e48557d4e29414936")
-```
+## English
+
+# aaiotrello
+Async Trello API Client
+
+Python 3.7+
+
+## Install
+
+```bash
+pip install aaiotrello
+```
+
+## Auth
+
+#### TRELLO_APP_KEY: https://trello.com/app-key/
+#### TRELLO_APP_TOKEN:
+
+First you need gen auth url:
+```python
+from aaiotrello import TrelloApi
+
+trello = TrelloApi(config.TRELLO_KEY)
+trello.set_token(config.TRELLO_TOKEN)
+```
+Than you need copy value of token_url and auth your trello account in webbrowser
+After that you will get token
+
+#### Apply token in your app:
+```python
+trello_app.set_token(TRELLO_APP_TOKEN)
+```
+
+#### Sample usage
+
+Get board info:
+```python
+board = await trello_app.boards.get("5c49c07e48557d4e29414936")
+```
```

### Comparing `aaiotrello-1.0.2/aaiotrello/__init__.py` & `aaiotrello-2.0.0/aaiotrello/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .checklists import Checklists
 from .lists import Lists
 from .members import Members
 from .notifications import Notifications
 from .organizations import Organizations
 from .tokens import Tokens
 from .types import Types
+from .webhooks import Webhooks
 
 
 class TrelloApi(object):
     def __init__(self, apikey, token=None):
         self._apikey = apikey
         self._token = token
         self.actions = Actions(apikey, token)
@@ -24,23 +25,25 @@
         self.checklists = Checklists(apikey, token)
         self.lists = Lists(apikey, token)
         self.members = Members(apikey, token)
         self.notifications = Notifications(apikey, token)
         self.organizations = Organizations(apikey, token)
         self.tokens = Tokens(apikey, token)
         self.types = Types(apikey, token)
+        self.webhooks = Webhooks(apikey, token)
 
     def set_token(self, token):
         self._token = token
         self.actions._token = token
         self.boards._token = token
         self.cards._token = token
         self.checklists._token = token
         self.lists._token = token
         self.members._token = token
         self.notifications._token = token
         self.organizations._token = token
         self.tokens._token = token
         self.types._token = token
+        self.webhooks._token = token
 
     def get_token_url(self, app_name, expires='never', write_access=True):
         return 'https://trello.com/1/authorize?key=%s&name=%s&expiration=%s&response_type=token&scope=%s' % (self._apikey, quote_plus(app_name), expires, 'read,write' if write_access else 'read')
```

### Comparing `aaiotrello-1.0.2/aaiotrello/actions.py` & `aaiotrello-2.0.0/aaiotrello/actions.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/boards.py` & `aaiotrello-2.0.0/aaiotrello/boards.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/cards.py` & `aaiotrello-2.0.0/aaiotrello/cards.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/checklists.py` & `aaiotrello-2.0.0/aaiotrello/checklists.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/lists.py` & `aaiotrello-2.0.0/aaiotrello/lists.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/members.py` & `aaiotrello-2.0.0/aaiotrello/members.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/notifications.py` & `aaiotrello-2.0.0/aaiotrello/notifications.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/organizations.py` & `aaiotrello-2.0.0/aaiotrello/organizations.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/tokens.py` & `aaiotrello-2.0.0/aaiotrello/tokens.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/aaiotrello/utils.py` & `aaiotrello-2.0.0/aaiotrello/utils.py`

 * *Files identical despite different names*

### Comparing `aaiotrello-1.0.2/setup.py` & `aaiotrello-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 from setuptools import setup
 from textwrap import dedent
 
+with open("README.md", "r", encoding="utf8") as fh:
+    long_description = fh.read()
+
 setup(name='aaiotrello',
-      version='1.0.2',
+      version='2.0.0',
       packages=['aaiotrello'],
       description='Async Python library for interacting with the Trello API',
-      long_description=dedent("""\
-        Python Trello API Wrapper
-        --------------------------
-
-        This Python API is simply a wrapper around the Trello API
-
-        Getting Started:
-        ----------------
-        To use the Trello API, install the package either by downloading the source and running
-
-          $ python setup.py install
-
-        Documentation:
-        --------------
-        You can find documentation for the Python API at:
-
-            http://packages.python.org/trello/
-
-        And documentation for the Trello API at:
-
-            https://trello.com/docs/api/
-
-        """),
+      long_description=long_description,
+      long_description_content_type="text/markdown",
       url='https://trello.com/',
       download_url='https://github.com/developerreva/aaiotrello',
-      install_requires=['requests>=0.9.1'],
-      requires='requests',
+      keywords='python python3 api-client aiohttp api-wrapper trello trello-api trello-async',
+      install_requires=['aiohttp>=3.9.0'],
+      requires='aiohttp',
       license='BSD License',
+      author='Developereva',
+      author_email='developereva@protonmail.com',
+      project_urls={
+        'Source Code': 'https://github.com/developerreva/aaiotrello',
+        'Documentation': 'https://github.com/developerreva/aaiotrello#-getting-started',
+        'Trello REST API Documentation': 'https://developer.atlassian.com/cloud/trello/rest/'
+    },
       classifiers=[
-	    	"Programming Language :: Python :: 3.6",
+	    	"Programming Language :: Python :: 3.7",
 	    	"License :: OSI Approved :: MIT License",
 	    	"Operating System :: OS Independent",
 	    ],
       include_package_data=True,
       )
```

