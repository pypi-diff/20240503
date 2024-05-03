# Comparing `tmp/skillsnetwork_jupyter_extension-2.2.1rc0.tar.gz` & `tmp/skillsnetwork_jupyter_extension-2.3.0rc0.tar.gz`

## Comparing `skillsnetwork_jupyter_extension-2.2.1rc0.tar` & `skillsnetwork_jupyter_extension-2.3.0rc0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.copier-answers.yml
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.prettierignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.tool-versions
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.yarnrc.yml
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/CHANGELOG.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/CODEOWNERS
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/install.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/setup.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/tsconfig.json
--rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/yarn.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/schema/toolbar.json
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
--rw-r--r--   0        0        0    21518 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/496.fe9a7d2284d4fc77abac.js
--rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.add80f4969ddadebc0ba.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/config.ts
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/dialog.ts
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/handler.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/index.ts
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/sn-file-library.ts
--rw-r--r--   0        0        0    23267 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/tools.ts
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/menu/index.ts
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/theme/index.ts
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/src/toolbar/index.ts
--rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/static/extension_demo.gif
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/LICENSE
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/README.md
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/pyproject.toml
--rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.copier-answers.yml
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.prettierignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.tool-versions
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.whitesource
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.yarnrc.yml
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/CODEOWNERS
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/install.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/setup.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/tsconfig.json
+-rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/yarn.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/schema/toolbar.json
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
+-rw-r--r--   0        0        0    21429 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/496.9f74bf3e410d1c115cd7.js
+-rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.deab4c15018528576b5d.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/config.ts
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/dialog.ts
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/handler.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/index.ts
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/sn-file-library.ts
+-rw-r--r--   0        0        0    22974 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/tools.ts
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/menu/index.ts
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/theme/index.ts
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/src/toolbar/index.ts
+-rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/static/extension_demo.gif
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/style/index.js
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/LICENSE
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc0/PKG-INFO
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/.copier-answers.yml` & `skillsnetwork_jupyter_extension-2.3.0rc0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/CHANGELOG.md` & `skillsnetwork_jupyter_extension-2.3.0rc0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 2.2.1rc0
+## 2.3.0rc0
 
 No merged PRs
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
 ## 2.2.0
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/CODEOWNERS` & `skillsnetwork_jupyter_extension-2.3.0rc0/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/RELEASE.md` & `skillsnetwork_jupyter_extension-2.3.0rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc0'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc0"
+    "version": "2.3.0-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/tsconfig.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/yarn.lock` & `skillsnetwork_jupyter_extension-2.3.0rc0/yarn.lock`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/schema/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/schema/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/__init__.py` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/handlers.py` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.deab4c15018528576b5d.js'}}",*

 * * "'version'": "'2.3.0-rc0'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.add80f4969ddadebc0ba.js",
+            "load": "static/remoteEntry.deab4c15018528576b5d.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "skillsnetwork_jupyter_extension"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc0"
+    "version": "2.3.0-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc0'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.2.1-rc0"
+    "version": "2.3.0-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/496.fe9a7d2284d4fc77abac.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/496.9f74bf3e410d1c115cd7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,29 +2,29 @@
 (self.webpackChunkskillsnetwork_jupyter_extension = self.webpackChunkskillsnetwork_jupyter_extension || []).push([
     [496], {
         904: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         AP: () => m,
-                        CS: () => h,
+                        CS: () => g,
                         CY: () => u,
-                        Gq: () => E,
+                        Gq: () => k,
                         Mh: () => s,
                         Ut: () => l,
                         a: () => i,
-                        aQ: () => f,
+                        aQ: () => y,
                         mW: () => a,
-                        o7: () => g,
+                        o7: () => p,
                         qK: () => b,
                         sd: () => _,
-                        wr: () => y,
-                        xy: () => p
+                        wr: () => f,
+                        xy: () => h
                     });
-                    var a, i, r = o(348);
+                    var a, i, r = o(420);
                     ! function(e) {
                         e.JUPYTERLAB = "jupyterlab", e.JUPYTERLITE = "jupyterlite", e.LOCAL = "local"
                     }(a || (a = {})),
                     function(e) {
                         e.LEARN = "learn", e.AUTHOR = "author"
                     }(i || (i = {}));
                     const e = e => {
@@ -56,30 +56,30 @@
                                 if (l === a.JUPYTERLITE) return console.log(`${e} not found in URL parameters, leaving empty due to env_type...`), "";
                                 if (s === i.LEARN) return console.log(`${e} not found in URL parameters, leaving empty due to mode...`), "";
                                 console.log(`${e} not found in URL parameters, making server request...`);
                                 const o = await c();
                                 return console.log(`${t} from server: ${o[t]}`), o[t]
                             }
                             return decodeURIComponent(n)
-                        }, u = await d("atlas_base_url", "ATLAS_BASE_URL"), p = await d("awb_base_url", "AWB_BASE_URL"), h = await d("sn_file_library_url", "SN_V2_FILE_LIBRARY_URL"), g = await d("sn_file_library_url", "SN_FILE_LIBRARY_URL"), w = (e, t, o) => {
+                        }, u = await d("atlas_base_url", "ATLAS_BASE_URL"), h = await d("awb_base_url", "AWB_BASE_URL"), g = await d("sn_file_library_url", "SN_V2_FILE_LIBRARY_URL"), p = await d("sn_file_library_url", "SN_FILE_LIBRARY_URL"), w = (e, t, o) => {
                             const n = window.location.href,
                                 a = new URL(n).searchParams.get(e);
                             return null !== a ? t ? decodeURIComponent(a) : a : o
-                        }, b = w("atlas_token", !1, "NO_TOKEN"), m = w("awb_token", !1, "NO_TOKEN"), y = w("notebook_url", !0, null), f = w("file_path", !0, null), _ = async () => {
+                        }, b = w("atlas_token", !1, "NO_TOKEN"), m = w("awb_token", !1, "NO_TOKEN"), f = w("notebook_url", !0, null), y = w("file_path", !0, null), _ = async () => {
                             const e = l;
-                            return e === a.JUPYTERLAB || e === a.LOCAL ? (E.PY_KERNEL_NAME = await v(), E.DEFAULT_LAB_NAME = "lab.ipynb") : e === a.JUPYTERLITE && (E.PY_KERNEL_NAME = "python", E.DEFAULT_LAB_NAME = "lab.jupyterlite.ipynb"), e
+                            return e === a.JUPYTERLAB || e === a.LOCAL ? (k.PY_KERNEL_NAME = await v(), k.DEFAULT_LAB_NAME = "lab.ipynb") : e === a.JUPYTERLITE && (k.PY_KERNEL_NAME = "python", k.DEFAULT_LAB_NAME = "lab.jupyterlite.ipynb"), e
                         }, v = async () => {
                             const e = await (await r.KernelSpecAPI.getSpecs()).kernelspecs,
                                 t = Object.keys(e).filter((function(e) {
                                     return e.includes("python")
                                 })).sort();
                             return t[t.length - 1]
                         };
-                    class E {}
-                    E.TOKENS = new Map, E.SHOW_PUBLISH_BUTTON_FOR = void 0, E.PREV_PUB_HASH = "prev_pub_hash", E.BACKUP_EXT = ".backup", n()
+                    class k {}
+                    k.TOKENS = new Map, k.SHOW_PUBLISH_BUTTON_FOR = void 0, k.PREV_PUB_HASH = "prev_pub_hash", k.BACKUP_EXT = ".backup", n()
                 } catch (e) {
                     n(e)
                 }
             }), 1)
         },
         780: (e, t, o) => {
             o.d(t, {
@@ -87,15 +87,15 @@
                 KQ: () => d,
                 Sc: () => l,
                 WA: () => s,
                 Zm: () => u,
                 g3: () => c
             });
             var n = o(760),
-                a = o(352);
+                a = o(300);
             class i extends n.Widget {
                 constructor() {
                     const e = document.createElement("div"),
                         t = new a.Spinner;
                     e.appendChild(t.node), e.style.padding = "15px", super({
                         node: e
                     })
@@ -155,97 +155,90 @@
                 }
         },
         480: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         CU: () => b,
-                        E$: () => v,
                         GK: () => w,
-                        I7: () => y,
-                        Oc: () => _,
-                        Yj: () => m,
-                        m: () => f
+                        Oc: () => v,
+                        So: () => y,
+                        iU: () => _,
+                        k5: () => k,
+                        uU: () => f
                     });
                     var a = o(637),
                         i = o.n(a),
                         r = o(780),
-                        l = o(352),
+                        l = o(300),
                         s = o(904),
                         c = o(96),
                         d = o(500),
                         u = o.n(d),
-                        p = o(416),
-                        h = o.n(p),
-                        g = e([s, c]);
-                    [s, c] = g.then ? (await g)() : g;
-                    const w = e => u().create({
-                            baseURL: s.CY,
+                        h = o(416),
+                        g = o.n(h),
+                        p = e([s, c]);
+                    [s, c] = p.then ? (await p)() : p;
+                    const w = e => m(e, s.CY),
+                        b = e => m(e, s.xy),
+                        m = (e, t) => u().create({
+                            baseURL: t,
                             headers: {
                                 Authorization: `Bearer ${e}`,
                                 "Content-Type": "application/json",
                                 "Access-Control-Allow-Origin": "*",
                                 Accept: "application/json"
                             }
                         }),
-                        b = e => u().create({
-                            baseURL: s.xy,
-                            headers: {
-                                Authorization: `Bearer ${e}`,
-                                "Content-Type": "application/json",
-                                "Access-Control-Allow-Origin": "*",
-                                Accept: "application/json"
-                            }
-                        }),
-                        m = async (e, t) => {
+                        f = async (e, t) => {
                             try {
-                                const o = h()(t),
+                                const o = g()(t),
                                     n = o.version_id,
                                     a = o.lab_id;
                                 console.log(`Fetching lab model for lab_id: ${a}, version_id: ${n}`);
-                                const i = `${o.lab_name}.ipynb`.replace(/^.*[\\/]/, ""),
+                                const i = `${o.lab_name}.ipynb`,
                                     r = await e.get(`api/v1/labs/${a}/lab_versions/${n}/download?timestamp=${(new Date).getTime()}`).then((e => (console.log("Lab model fetched successfully"), e.data)));
                                 return l.Dialog.flush(), {
                                     labFilename: i,
                                     body: r
                                 }
                             } catch (e) {
                                 throw "Failed to fetch notebook"
                             }
                         }, y = async (e, t, o, n) => {
                             if (!await (0, r.WA)("Publishing your lab onto Skills Network...").then((e => !0)).catch((e => !1))) return;
                             (0, r.Sc)("Publishing your changes...");
-                            const a = h()(n),
+                            const a = g()(n),
                                 s = a.version_id,
                                 d = a.lab_id;
                             await (0, c.ol)(t, o);
                             const u = await (0, c.gv)(t, o),
-                                p = new(i());
-                            return p.append("publish", "true"), p.append("draft[changelog]", "updated notebook"), p.append("file", u), console.log(`Posting lab model to AWB for lab_id: ${d}, version_id: ${s}`), new Promise((async (t, o) => {
-                                await e.post(`api/v1/labs/${d}/lab_versions/${s}/drafts`, p).then((e => {
+                                h = new(i());
+                            return h.append("publish", "true"), h.append("draft[changelog]", "updated notebook"), h.append("file", u), console.log(`Posting lab model to AWB for lab_id: ${d}, version_id: ${s}`), new Promise((async (t, o) => {
+                                await e.post(`api/v1/labs/${d}/lab_versions/${s}/drafts`, h).then((e => {
                                     console.log(`Successfully Pushed Lab Version for lab id: ${d}, ver: ${s}`, e), l.Dialog.flush(), (0, r.g3)(), t()
                                 })).catch((e => {
                                     l.Dialog.flush(), (0, r.KQ)(), o(new Error("Failed to post lab model"))
                                 }))
                             }))
-                        }, f = e => e.get(`v1/labs?timestamp=${(new Date).getTime()}`).then((e => (l.Dialog.flush(), e.data))).catch((e => {
+                        }, _ = e => e.get(`v1/labs?timestamp=${(new Date).getTime()}`).then((e => (l.Dialog.flush(), e.data))).catch((e => {
                             throw "Failed to fetch notebook"
-                        })), _ = e => {
+                        })), v = e => {
                             const t = new URL(e);
                             return 0 === t.searchParams.size && t.searchParams.append("timestamp", (new Date).getTime().toString()), u().get(t.toString(), {
                                 headers: {
                                     "Cache-Control": "no-cache",
                                     Expires: "0",
                                     "Access-Control-Allow-Origin": "*",
                                     Accept: "application/json"
                                 }
                             }).then((e => (l.Dialog.flush(), e))).catch((e => {
                                 throw "Failed to fetch notebook"
                             }))
-                        }, v = async (e, t, o) => {
+                        }, k = async (e, t, o) => {
                             if (!await (0, r.WA)("Publishing your lab onto Skills Network...").then((e => !0)).catch((e => !1))) return;
                             (0, r.Sc)("Publishing your changes..."), console.log("Updating lab commit ID"), await (0, c.ol)(t, o);
                             const n = await (0, c.gv)(t, o);
                             return console.log("Posting lab model to ATLAS"), new Promise((async (t, o) => {
                                 await e.post("v1/labs", {
                                     body: n
                                 }).then((e => {
@@ -281,85 +274,88 @@
                 }
             }))
         },
         964: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
-                        c: () => w
+                        c: () => b
                     });
-                    var a = o(792),
+                    var a = o(452),
                         i = o(760),
-                        r = o(352),
-                        l = o(464),
-                        s = o(608),
-                        c = o(780),
-                        d = o(904),
-                        u = o(96),
-                        p = o(416),
-                        h = o.n(p),
-                        g = e([d, u]);
-                    [d, u] = g.then ? (await g)() : g;
-                    const w = {
+                        r = o(300),
+                        l = o(628),
+                        s = o(736),
+                        c = o(568),
+                        d = o(780),
+                        u = o(904),
+                        h = o(96),
+                        g = o(416),
+                        p = o.n(g),
+                        w = e([u, h]);
+                    [u, h] = w.then ? (await w)() : w;
+                    const b = {
                         id: "skillsnetwork_jupyter_extension:menu",
                         autoStart: !0,
-                        requires: [a.IMainMenu, r.ICommandPalette, l.INotebookTracker, s.IDocumentManager],
-                        activate: async (e, t, o, n, a) => {
-                            if (console.log("skillsnetwork_jupyter_extension:menu extension activated"), d.Mh === d.a.LEARN) return;
+                        requires: [a.IMainMenu, r.ICommandPalette, l.INotebookTracker, s.IDocumentManager, c.IDefaultFileBrowser],
+                        activate: async (e, t, o, n, a, r) => {
+                            if (console.log("skillsnetwork_jupyter_extension:menu extension activated"), u.Mh === u.a.LEARN) return;
                             const {
-                                commands: r
-                            } = e, l = "mainMenu:editLabFromToken";
-                            r.addCommand(l, {
+                                commands: l
+                            } = e, s = "mainMenu:editLabFromToken";
+                            l.addCommand(s, {
                                 label: "Edit a Lab",
                                 execute: t => {
-                                    b(0, a, e.serviceManager.contents)
+                                    m(0, a, e.serviceManager.contents, r)
                                 }
                             }), o.addItem({
-                                command: l,
+                                command: s,
                                 category: "skillsNetwork",
                                 args: {
                                     origin: "from the palette"
                                 }
                             });
-                            const s = new i.Menu({
-                                commands: r
+                            const c = new i.Menu({
+                                commands: l
                             });
-                            s.title.label = "Skills Network", t.addMenu(s, !0, {
+                            c.title.label = "Skills Network", t.addMenu(c, !0, {
                                 rank: 80
-                            }), s.addItem({
-                                command: l,
+                            }), c.addItem({
+                                command: s,
                                 args: {}
                             })
                         }
                     };
 
-                    function b(e, t, o) {
-                        const n = document.createElement("div"),
-                            a = document.createElement("label");
-                        a.textContent = "Enter your authorization token";
-                        const l = document.createElement("input");
-                        l.className = "jp-mod-styled", n.appendChild(a), n.appendChild(l), (0, r.showDialog)({
+                    function m(e, t, o, n) {
+                        const a = document.createElement("div"),
+                            l = document.createElement("label");
+                        l.textContent = "Enter your authorization token";
+                        const s = document.createElement("input");
+                        s.className = "jp-mod-styled", a.appendChild(l), a.appendChild(s), (0, r.showDialog)({
                             title: "Edit a Lab",
                             body: new i.Widget({
-                                node: n
+                                node: a
                             }),
                             buttons: [r.Dialog.cancelButton(), r.Dialog.okButton()]
                         }).then((async e => {
                             if (e.button.accept) {
-                                console.log("Token dialog accepted, loading lab..."), (0, c.E3)("Loading up your lab...");
-                                const e = l.value;
-                                "version_id" in h()(e) ? (console.log("Token contains version_id, opening independent lab..."), await (0, u.op)(e, t, o)) : (console.log("Token does not contain version_id, opening lab..."), await (0, u.UJ)(e, t, o))
+                                console.log("Token dialog accepted, loading lab..."), (0, d.E3)("Loading up your lab...");
+                                const e = s.value;
+                                let a = "NO_TOKEN",
+                                    i = "NO_TOKEN";
+                                "version_id" in p()(e) ? (console.log("Token contains version_id, opening AWB lab..."), i = e) : (console.log("Token does not contain version_id, opening Atlas lab..."), a = e), await (0, h.UJ)(a, i, "Token Launch", t, o, n)
                             }
                         })).catch((e => {
-                            r.Dialog.flush(), (0, c.Zm)(), console.error("Error occurred while importing lab:", e)
+                            r.Dialog.flush(), (0, d.Zm)(), console.error("Error occurred while importing lab:", e)
                         }))
                     }
                     n()
-                } catch (m) {
-                    n(m)
+                } catch (f) {
+                    n(f)
                 }
             }))
         },
         864: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
@@ -382,15 +378,15 @@
                                 }(this, s, e, "f")
                         }
                         launch() {
                             const e = a.Gq.TOKENS.get(function(e, t, o, n) {
                                     if ("a" === o && !n) throw new TypeError("Private accessor was defined without a getter");
                                     if ("function" == typeof t ? e !== t || !n : !t.has(e)) throw new TypeError("Cannot read private member from an object whose class did not declare it");
                                     return "m" === o ? n : "a" === o ? n.call(e) : n ? n.value : t.get(e)
-                                }(this, s, "f").split("/").pop() || ""),
+                                }(this, s, "f") || ""),
                                 t = e ? r()(e) : {},
                                 o = document.createElement("a");
                             o.href = "project_id" in t ? `${a.o7}?atlas_token=${e}` : `${a.CS}?lab_version_id=${t.version_id}`, o.target = "_blank", document.body.appendChild(o), o.click(), document.body.removeChild(o)
                         }
                     }
                     s = new WeakMap, n()
                 } catch (e) {
@@ -402,15 +398,15 @@
             o.d(t, {
                 c: () => n
             });
             const n = {
                 id: "skillsnetwork_jupyter_extension:theme",
                 description: "Theme toggle plugin for Skills Network Authoring Extension",
                 autoStart: !0,
-                requires: [o(352).IThemeManager],
+                requires: [o(300).IThemeManager],
                 activate: (e, t) => {
                     console.log("Activating skillsnetwork_jupyter_extension theme toggle plugin!"), window.addEventListener("message", (e => {
                             "update_theme" === e.data.type && (console.log("Message received in the iframe:", e.data), "light" === e.data.color ? t.setTheme("JupyterLab Light") : t.setTheme("JupyterLab Dark"))
                         })),
                         function() {
                             try {
                                 return window.self !== window.top
@@ -423,65 +419,66 @@
                 }
             }
         },
         808: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
-                        c: () => v
+                        c: () => k
                     });
-                    var a = o(608),
-                        i = o(208),
-                        r = o(352),
+                    var a = o(736),
+                        i = o(568),
+                        r = o(300),
                         l = o(96),
                         s = o(508),
                         c = o(480),
                         d = o(780),
                         u = o(904),
-                        p = o(416),
-                        h = o.n(p),
-                        g = o(464),
+                        h = o(416),
+                        g = o.n(h),
+                        p = o(628),
                         w = o(864),
-                        b = e([u, c, l, w]);
-                    [u, c, l, w] = b.then ? (await b)() : b;
-                    const m = {
+                        b = o(468),
+                        m = e([u, c, l, w]);
+                    [u, c, l, w] = m.then ? (await m)() : m;
+                    const f = {
                         id: "skillsnetwork_jupyter_extension:toolbar",
                         description: "Toolbar plugin for Skills Network Authoring Extension",
                         autoStart: !0,
-                        requires: [g.INotebookTracker, a.IDocumentManager, i.IDefaultFileBrowser],
-                        activate: _
+                        requires: [p.INotebookTracker, a.IDocumentManager, i.IDefaultFileBrowser],
+                        activate: v
                     };
                     async function y(e) {
                         e.forEach((e => {
                             e.dispose()
                         }))
                     }
-                    class f {
+                    class _ {
                         createNew(e, t) {
                             if (u.Gq.SHOW_PUBLISH_BUTTON_FOR !== t.path) return new s.DisposableDelegate((() => {}));
                             {
                                 const o = async () => {
-                                    const o = t.path.split("/").pop() || "",
+                                    const o = t.path,
                                         n = u.Gq.TOKENS.get(o);
                                     if (void 0 === n) return console.log(`[ButtonExtension] No token found for filename: ${o}`), void await (0, r.showDialog)({
                                         title: "Publishing Restricted",
                                         body: `Only the lab '${u.Gq.TOKENS.keys().next().value}' can be published during this editing session.`,
                                         buttons: [r.Dialog.okButton({
                                             label: "Dismiss"
                                         })]
                                     });
-                                    "version_id" in h()(n) ? await (0, c.I7)((0, c.CU)(n), e, t, n) : await (0, c.E$)((0, c.GK)(n), e, t)
+                                    "version_id" in g()(n) ? await (0, c.So)((0, c.CU)(n), e, t, n) : await (0, c.k5)((0, c.GK)(n), e, t)
                                 }, n = async () => {
                                     const o = await (0, l.gv)(e, t),
                                         n = new Blob([o], {
                                             type: "application/x-ipynb+json"
                                         }),
                                         a = URL.createObjectURL(n),
                                         i = document.createElement("a");
-                                    i.setAttribute("download", t.path), i.setAttribute("href", a), document.body.appendChild(i), i.click(), document.body.removeChild(i), URL.revokeObjectURL(a)
+                                    i.setAttribute("download", b.PathExt.basename(t.path)), i.setAttribute("href", a), document.body.appendChild(i), i.click(), document.body.removeChild(i), URL.revokeObjectURL(a)
                                 }, a = new r.ToolbarButton({
                                     className: "download-lab-button",
                                     label: "Download Notebook",
                                     onClick: n,
                                     tooltip: "Download the current notebook ipynb file to your local system"
                                 }), i = new r.ToolbarButton({
                                     className: "publish-lab-button",
@@ -496,15 +493,15 @@
                                 });
                                 return e.toolbar.insertItem(8, "download", a), e.toolbar.insertItem(9, "sn-file-library", d), e.toolbar.insertItem(10, "publish", i), new s.DisposableDelegate((() => {
                                     a.dispose(), i.dispose(), d.dispose()
                                 }))
                             }
                         }
                     }
-                    async function _(e, t, o, n) {
+                    async function v(e, t, o, n) {
                         console.log("Activating skillsnetwork_jupyter_extension button plugin!");
                         const a = await (0, u.sd)();
                         if (console.log("Using default kernel:", u.Gq.PY_KERNEL_NAME), u.Mh === u.a.LEARN) {
                             if (u.Ut !== u.mW.JUPYTERLITE) return;
                             return console.log("skillsnetwork_jupyter_extension:toolbar extension activated"), void(u.wr ? (await e.serviceManager.ready, e.restored.then((async () => {
                                 await y(t);
                                 try {
@@ -512,44 +509,42 @@
                                 } catch (e) {
                                     console.error("Error opening lab:", e), r.Dialog.flush(), (0, d.Zm)()
                                 }
                             }))) : console.log("No valid notebook URL found..."))
                         }
                         const i = u.qK,
                             s = u.AP;
-                        console.log("skillsnetwork_jupyter_extension:toolbar extension activated"), e.docRegistry.addWidgetExtension("Notebook", new f), await e.serviceManager.ready, e.restored.then((async () => {
-                            if (await y(t), "NO_TOKEN" !== i && a !== u.mW.LOCAL) try {
-                                await (0, l.UJ)(i, o, e.serviceManager.contents)
-                            } catch (e) {
-                                console.error("Error opening lab with Atlas token:", e), r.Dialog.flush(), (0, d.Zm)()
-                            } else if ("NO_TOKEN" !== s && a !== u.mW.LOCAL) try {
-                                await (0, l.op)(s, o, e.serviceManager.contents)
+                        console.log("skillsnetwork_jupyter_extension:toolbar extension activated"), e.docRegistry.addWidgetExtension("Notebook", new _);
+                        let c = "";
+                        null !== u.aQ && (c = (0, l.eC)(u.aQ), console.log("Authoring lab file path:", c)), await e.serviceManager.ready, e.restored.then((async () => {
+                            if (await y(t), a !== u.mW.LOCAL && ("NO_TOKEN" !== i || "NO_TOKEN" !== s)) try {
+                                await (0, l.UJ)(i, s, c, o, e.serviceManager.contents, n)
                             } catch (e) {
-                                console.error("Error opening lab with AWB token:", e), r.Dialog.flush(), (0, d.Zm)()
+                                console.error("Error opening lab with Atlas/AWB token:", e), r.Dialog.flush(), (0, d.Zm)()
                             }
                         }))
                     }
-                    const v = m;
+                    const k = f;
                     n()
                 } catch (E) {
                     n(E)
                 }
             }))
         },
         96: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
-                        UJ: () => y,
+                        UJ: () => m,
+                        eC: () => E,
                         gv: () => u,
-                        ol: () => h,
-                        op: () => m,
+                        ol: () => g,
                         wO: () => f
                     });
-                    var a = o(352),
+                    var a = o(300),
                         i = o(944),
                         r = o(904),
                         l = o(480),
                         s = e([r, l]);
                     [r, l] = s.then ? (await s)() : s;
                     const c = e => {
                             const t = e.model.toJSON().source,
@@ -591,15 +586,15 @@
                                     cells: o,
                                     metadata: n,
                                     nbformat: a,
                                     nbformat_minor: i
                                 };
                             return JSON.stringify(l, null, 2)
                         },
-                        p = async (e, t) => {
+                        h = async (e, t) => {
                             t = i.C.removeSlash(t);
                             const o = i.C.dirname(t),
                                 n = [];
                             o.split("/").reduce(((e, t) => {
                                 const o = i.C.removeSlash(e + "/" + t);
                                 return n.push(o), o
                             }), ""), console.log(n);
@@ -612,25 +607,25 @@
                                 const n = await e.newUntitled({
                                     path: "",
                                     type: "directory"
                                 });
                                 await e.rename(n.path, t)
                             }
                         };
-                    async function h(e, t) {
+                    async function g(e, t) {
                         const o = await b(e, t),
-                            n = await S(o);
+                            n = await N(o);
                         await t.ready, t.model.setMetadata(r.Gq.PREV_PUB_HASH, n), t.save().then((() => {
                             console.log("Notebook saved with updated commit ID.")
                         })).catch((e => {
                             console.error("Failed to save notebook with updated commit ID:", e)
                         }))
                     }
 
-                    function g(e) {
+                    function p(e) {
                         var t, o, n, a, i, l, s;
                         return "string" == typeof e && (e = JSON.parse(e)), "object" != typeof e || null === e || !("metadata" in e) && !("content" in e) ? (console.error("Lab content is of unknown type: ", typeof e, "\n Value: \n", e), "") : null !== (s = null !== (n = null === (o = null === (t = e.metadata) || void 0 === t ? void 0 : t[r.Gq.PREV_PUB_HASH]) || void 0 === o ? void 0 : o.toString()) && void 0 !== n ? n : null === (l = null === (i = null === (a = e.content) || void 0 === a ? void 0 : a.metadata) || void 0 === i ? void 0 : i[r.Gq.PREV_PUB_HASH]) || void 0 === l ? void 0 : l.toString()) && void 0 !== s ? s : ""
                     }
 
                     function w(e) {
                         var t;
                         if ("string" == typeof e) try {
@@ -645,55 +640,58 @@
                     const b = (e, t) => {
                             const o = [];
                             return e.content.widgets.forEach((e => {
                                 const t = d(e);
                                 o.push(t)
                             })), JSON.stringify(o, null, 2)
                         },
-                        m = async (e, t, o) => {
-                            const {
-                                labFilename: n,
-                                body: a
-                            } = await (0, l.Yj)((0, l.CU)(e), e);
-                            let i, s = `${n}`;
-                            return r.Ut !== r.mW.JUPYTERLITE ? (s = `./${s}`, await E(s, o, t), await v(s, a, o, t)) : await t.deleteFile(s), r.Gq.SHOW_PUBLISH_BUTTON_FOR = n, r.Gq.TOKENS.set(n, e), i = await T(s, o) ? t.openOrReveal(n) : await _(t, n, a), i
-                        }, y = async (e, t, o) => {
-                            const {
-                                instructions_file_path: n,
-                                body: a
-                            } = await (0, l.m)((0, l.GK)(e)), i = L(n);
-                            let s, c = `${i}`;
-                            return r.Ut !== r.mW.JUPYTERLITE ? (c = `./${c}`, await E(c, o, t), await v(c, a, o, t)) : await t.deleteFile(c), r.Gq.SHOW_PUBLISH_BUTTON_FOR = i, r.Gq.TOKENS.set(i, e), s = await T(c, o) ? t.openOrReveal(i) : await _(t, i, JSON.parse(a)), s
+                        m = async (e, t, o, n, a, i) => {
+                            let s, c, d, u;
+                            if ("NO_TOKEN" !== e)({
+                                instructions_file_path: s,
+                                body: c
+                            } = await (0, l.iU)((0, l.GK)(e))), d = s, u = e;
+                            else {
+                                if ("NO_TOKEN" === t) throw Error("No valid token found.");
+                                ({
+                                    labFilename: d,
+                                    body: c
+                                } = await (0, l.uU)((0, l.CU)(t), t)), u = t
+                            }
+                            let g = `${d}`;
+                            "" !== o ? (g = `${o}/${g}`, await h(n, g), i.model.path !== o && (console.log(`Opening /${o} in file browser`), await i.model.cd(`/${o}`))) : await i.model.cd("/");
+                            let p, w = g;
+                            return r.Ut !== r.mW.JUPYTERLITE ? (w = `./${g}`, await v(g, a, n), await _(w, c, a, n)) : await n.deleteFile(w), r.Gq.SHOW_PUBLISH_BUTTON_FOR = g, r.Gq.TOKENS.set(g, u), p = await L(w, a) ? n.openOrReveal(g) : await y(n, g, "NO_TOKEN" !== e ? JSON.parse(c) : c), p
                         }, f = async (e, t, o, n, i) => {
                             const r = await (0, l.Oc)(e),
                                 s = r.data;
-                            if (!N(s)) throw Error(`content of ${e} is not a valid JSON! Please let the author know about this issue!`);
+                            if (!S(s)) throw Error(`content of ${e} is not a valid JSON! Please let the author know about this issue!`);
                             const c = Date.parse(r.headers["last-modified"] || "");
                             if (console.log(`last-modified date of ${e} extracted from headers:`, c), !(t && t.endsWith(".ipynb") || (console.log(`filePath from query (which is ${t}) is either missing or doesn't end with .ipynb. Trying to use the pathname from ${e} as filePath...`), (t = decodeURI(new URL(e).pathname)).endsWith(".ipynb")))) throw Error(`pathname of ${e} (which is ${t}) doesn't end with .ipynb. A notebook can't be created.`);
-                            console.log("filePath:", t), await p(o, t), console.log(`Opening ${t} in filebrowser`), await i.model.cd(t.substring(0, t.lastIndexOf("/")));
-                            const d = await T(t, n);
+                            console.log("filePath:", t), await h(o, t), console.log(`Opening ${t} in filebrowser`), await i.model.cd(t.substring(0, t.lastIndexOf("/")));
+                            const d = await L(t, n);
                             let u;
                             return d ? (console.log("last-modified date of", t, "extracted from notebook:", Date.parse(d.last_modified)), (!c || c > Date.parse(d.last_modified)) && (await (0, a.showDialog)({
                                 title: "Newer version of notebook available",
                                 body: `A newer version of the lab is available. Would you like to load the latest version? The current state of the notebook ${t} will be saved with a .backup.ipynb extension.`,
                                 buttons: [a.Dialog.cancelButton(), a.Dialog.okButton({
                                     label: "Use the newer version"
                                 })]
-                            })).button.accept ? (console.log("Opening newer version of notebook"), await o.overwrite(t, t.slice(0, t.lastIndexOf(".ipynb")) + ".backup.ipynb"), u = await _(o, t, s)) : (console.log("Opening existing notebook"), u = o.openOrReveal(t)), u) : (console.log("Creating a new notebook"), u = await _(o, t, s), u)
-                        }, _ = async (e, t, o) => {
+                            })).button.accept ? (console.log("Opening newer version of notebook"), await o.overwrite(t, t.slice(0, t.lastIndexOf(".ipynb")) + ".backup.ipynb"), u = await y(o, t, s)) : (console.log("Opening existing notebook"), u = o.openOrReveal(t)), u) : (console.log("Creating a new notebook"), u = await y(o, t, s), u)
+                        }, y = async (e, t, o) => {
                             const n = e.createNew(t, "notebook", {
                                 name: r.Gq.PY_KERNEL_NAME
                             });
                             if (void 0 === n) throw Error("Error loading lab");
                             return await k(n, o), n
                         };
-                    async function v(e, t, o, n) {
-                        const i = await T(e, o);
-                        if (i && g(t) !== g(i)) try {
-                            await R(i, o, n), await (0, a.showDialog)({
+                    async function _(e, t, o, n) {
+                        const i = await L(e, o);
+                        if (i && p(t) !== p(i)) try {
+                            await U(i, o, n), await (0, a.showDialog)({
                                 title: "Your Lab was Updated",
                                 body: `The newest published version of "${e}" is loaded. Your previous version has been backed up under "${e}${r.Gq.BACKUP_EXT}.ipynb"`,
                                 buttons: [a.Dialog.okButton({
                                     label: "Dismiss"
                                 })]
                             })
                         } catch (t) {
@@ -702,79 +700,82 @@
                                 body: `While trying to load your lab: "${e}", we found that you have another file named "${e}" that already exists in this folder, please delete it or rename it so we can load your published version"`,
                                 buttons: [a.Dialog.okButton({
                                     label: "Dismiss"
                                 })]
                             })
                         }
                     }
-                    async function E(e, t, o) {
-                        const n = await T(e, t);
-                        n && (await U(e, o), w(n) && await t.delete(e))
+                    async function v(e, t, o) {
+                        const n = await L(e, t);
+                        n && (await A(e, o), w(n) && await t.delete(e))
                     }
                     const k = async (e, t, o) => {
-                        if (await e.context.ready, "local" !== o) {
+                        if (await e.context.ready, o !== r.mW.LOCAL) {
                             e.context.model.fromJSON(t);
                             try {
                                 await e.context.save()
                             } catch (e) {
                                 console.error("[loadLabContents] Error saving notebook:", e)
                             }
-                        } else console.error("[loadLabContents] Notebook model is not initialized or authoring environment is local.")
-                    }, L = e => (null != e ? e : r.Gq.DEFAULT_LAB_NAME).replace(/^.*[\\/]/, "");
-                    async function T(e, t) {
+                        } else console.error("[loadLabContents] Notebook model is not initialized or environment is local.")
+                    }, E = e => {
+                        let t = e;
+                        return "" !== i.C.extname(e) && (t = i.C.dirname(e)), t = i.C.removeSlash(t), t.replace(/\/+$/, "")
+                    };
+                    async function L(e, t) {
                         try {
                             return await t.get(e)
                         } catch (e) {
                             if (e instanceof Error) {
                                 const t = e;
                                 if (t.response && 404 !== t.response.status) throw console.error("Error checking for existent backup file: ", e), e;
                                 return null
                             }
                             throw console.error("[getFile] Unexpected error type:", e), e
                         }
                     }
-                    async function A(e, t) {
+                    async function T(e, t) {
                         const o = t.findWidget(e);
                         if (o) try {
                             o.context.model.dirty && await o.context.save(), o.close()
                         } catch (e) {
                             console.error("[saveAndCloseOpenFiles] Error saving or closing widget:", e)
                         }
                     }
-                    async function U(e, t) {
+                    async function A(e, t) {
                         const o = t.findWidget(e);
                         if (o) try {
                             const e = t.contextForWidget(o);
                             e && e.model && (e.model.dirty = !1), o.close()
                         } catch (e) {
                             console.error("[closeWithoutSaving] Error closing widget:", e)
                         }
                     }
-                    async function R(e, t, o) {
+                    async function U(e, t, o) {
                         const n = e.path,
                             a = n.split(".").pop(),
                             i = `${n.replace(/\.[^/.]+$/,"")}${r.Gq.BACKUP_EXT}.${a}`;
-                        if (await T(i, t)) try {
+                        if (await L(i, t)) try {
                             await t.delete(i)
                         } catch (e) {
                             console.error("[convertFileToBackup] Error deleting existing backup file:", e)
                         }
                         try {
-                            await A(n, o), await t.rename(n, i)
+                            await T(n, o), await t.rename(n, i)
                         } catch (e) {
                             console.error("[convertFileToBackup] Error renaming file to backup:", e)
                         }
                     }
-                    async function S(e) {
+                    async function N(e) {
                         const t = (new TextEncoder).encode(e),
                             o = await crypto.subtle.digest("SHA-256", t);
                         return Array.from(new Uint8Array(o)).map((e => e.toString(16).padStart(2, "0"))).join("")
                     }
 
-                    function N(e) {
+                    function S(e) {
                         e = "string" != typeof e ? JSON.stringify(e) : e;
                         try {
                             e = JSON.parse(e)
                         } catch (e) {
                             return !1
                         }
                         return "object" == typeof e && null !== e
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -172,15 +172,15 @@
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        736: (e, t, n) => {
+        355: (e, t, n) => {
             n.r(t);
             var r = n(596),
                 o = n.n(r),
                 a = n(520),
                 s = n.n(a),
                 c = n(176),
                 i = n.n(c),
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.add80f4969ddadebc0ba.js` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.deab4c15018528576b5d.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b, m, y, g, w, _, k, j, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, b, v, m, y, g, w, _, k, j, S = {
             344: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./extension": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
-                        "./style": () => t.e(736).then((() => () => t(736)))
+                        "./style": () => t.e(736).then((() => () => t(355)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -37,20 +37,20 @@
         return S[e](t, t.exports, E), t.exports
     }
     E.m = S, E.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
     }, E.a = (o, a, i) => {
         var u;
         i && ((u = []).d = -1);
-        var l, f, s, d = new Set,
-            p = o.exports,
-            c = new Promise(((e, r) => {
-                s = r, f = e
+        var l, s, f, d = new Set,
+            c = o.exports,
+            p = new Promise(((e, r) => {
+                f = r, s = e
             }));
-        c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
+        p[r] = c, p[e] = e => (u && e(u), d.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
             var a;
             l = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
                         var a = [];
                         a.d = 0, o.then((e => {
@@ -65,71 +65,71 @@
                 var u = {};
                 return u[e] = e => {}, u[r] = o, u
             })))(o);
             var i = () => l.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
-                f = new Promise((r => {
+                s = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
-            return a.r ? f : i()
-        }), (e => (e ? s(c[t] = e) : f(p), n(u)))), u && u.d < 0 && (u.d = 0)
+            return a.r ? s : i()
+        }), (e => (e ? f(p[t] = e) : s(c), n(u)))), u && u.d < 0 && (u.d = 0)
     }, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return E.d(r, {
             a: r
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        496: "fe9a7d2284d4fc77abac",
+        496: "9f74bf3e410d1c115cd7",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
-        736: "7b5f76df818add15df8b",
+        736: "1176de539f275bcd21aa",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e] + ".js?v=" + {
-        496: "fe9a7d2284d4fc77abac",
+        496: "9f74bf3e410d1c115cd7",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
-        736: "7b5f76df818add15df8b",
+        736: "1176de539f275bcd21aa",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork_jupyter_extension:", E.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == e || s.getAttribute("data-webpack") == a + t) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -155,15 +155,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.2.1-rc0", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc0", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -206,84 +206,85 @@
             a.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? a.pop() + " " + a.pop() : l(i))
         }
         return u();
 
         function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, f = (e, r) => {
+    }, s = (e, r) => {
         if (0 in e) {
             r = i(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
             for (var o = 0, a = 1, u = !0;; a++, o++) {
-                var l, s, d = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (s = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
-                if ("u" == s) {
+                var l, f, d = a < e.length ? (typeof e[a])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
+                if ("u" == f) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == s)
+                    if (d == f)
                         if (a <= t) {
                             if (l != e[a]) return !1
                         } else {
                             if (n ? l > e[a] : l < e[a]) return !1;
                             l != e[a] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (n || a <= t) return !1;
                     u = !1, a--
                 } else {
-                    if (a <= t || s < d != n) return !1;
+                    if (a <= t || f < d != n) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? f(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? s(h, r) : !p())
         }
-        return !!c()
-    }, s = (e, r) => {
+        return !!p()
+    }, f = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
-    }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
+    }, c = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", p = (e, r, t, n) => {
         var o = d(e, t);
-        return f(n, o) || v(p(e, t, o, n)), b(e[t][o])
+        return s(n, o) || b(c(e, t, o, n)), v(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !f(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, v = e => {
+        return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
+    }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, b = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
+    }, v = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (s(e, t), c(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (f(e, t), p(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && h(r, t, n);
-        return a ? b(a) : o()
+        return a ? v(a) : o()
     })), w = {}, _ = {
-        208: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
-        348: () => y("default", "@jupyterlab/services", [1, 7, 1, 5]),
-        352: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
+        300: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
         416: () => g("default", "jwt-decode", [1, 3, 1, 2], (() => E.e(648).then((() => () => E(648))))),
-        464: () => y("default", "@jupyterlab/notebook", [1, 4, 1, 5]),
+        420: () => y("default", "@jupyterlab/services", [1, 7, 1, 8]),
+        452: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
+        468: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
         500: () => g("default", "axios", [1, 1, 6, 0], (() => E.e(636).then((() => () => E(636))))),
         508: () => y("default", "@lumino/disposable", [1, 2, 0, 0]),
-        608: () => y("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
+        568: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
+        628: () => y("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
         637: () => g("default", "form-data", [1, 4, 0, 0], (() => E.e(956).then((() => () => E(956))))),
-        760: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        792: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 5])
+        736: () => y("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
+        760: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])
     }, k = {
-        496: [208, 348, 352, 416, 464, 500, 508, 608, 637, 760, 792]
+        496: [300, 416, 420, 452, 468, 500, 508, 568, 628, 637, 736, 760]
     }, j = {}, E.f.consumes = (e, r) => {
         E.o(k, e) && k[e].forEach((e => {
             if (E.o(w, e)) return r.push(w[e]);
             if (!j[e]) {
                 var t = r => {
                     w[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json` & `skillsnetwork_jupyter_extension-2.3.0rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/config.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/dialog.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/handler.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/handler.ts`

 * *Files 6% similar despite different names*

```diff
@@ -12,59 +12,60 @@
 import { Dialog } from '@jupyterlab/apputils';
 import { ATLAS_BASE_URL, AWB_BASE_URL } from './config';
 import { getFileContents, updateLabCommitID } from './tools';
 import axios from 'axios';
 import jwt_decode from 'jwt-decode';
 
 export const atlasAxiosHandler = (lab_token: string): AxiosInstance => {
-  const atlasClient = axios.create({
-    baseURL: ATLAS_BASE_URL,
-    headers: {
-      Authorization: `Bearer ${lab_token}`,
-      'Content-Type': 'application/json',
-      'Access-Control-Allow-Origin': '*',
-      Accept: 'application/json'
-    }
-  });
-  return atlasClient;
+  return axiosHandler(lab_token, ATLAS_BASE_URL);
 };
 
 export const awbAxiosHandler = (lab_token: string): AxiosInstance => {
-  const awbClient = axios.create({
-    baseURL: AWB_BASE_URL,
+  return axiosHandler(lab_token, AWB_BASE_URL);
+};
+
+/**
+ * Generic Axios client
+ *
+ * @param lab_token JWT Bearer token
+ * @param baseURL Base URL
+ * @returns Axios client to make requests with
+ */
+const axiosHandler = (lab_token: string, baseURL: string): AxiosInstance => {
+  const client = axios.create({
+    baseURL,
     headers: {
       Authorization: `Bearer ${lab_token}`,
       'Content-Type': 'application/json',
       'Access-Control-Allow-Origin': '*',
       Accept: 'application/json'
     }
   });
-  return awbClient;
+  return client;
 };
 
 /**
  * GET the lab model / JSON that represents a .ipynb file/notebook from AWB
  *
  * @param awbAxiosHandler Axios client that contains a JWT Bearer token
  * @param lab_token JWT Bearer token
- * @returns Promise<void>
  */
-export const getIndependentLabModel = async (
+export const getAwbLabModel = async (
   awbAxiosHandler: AxiosInstance,
   lab_token: string
 ) => {
   try {
     const token_info = jwt_decode(lab_token) as { [key: string]: any };
     const version_id = token_info.version_id;
     const lab_id = token_info.lab_id;
 
     console.log(
       `Fetching lab model for lab_id: ${lab_id}, version_id: ${version_id}`
     );
-    const labFilename = `${token_info.lab_name}.ipynb`.replace(/^.*[\\/]/, '');
+    const labFilename = `${token_info.lab_name}.ipynb`;
     const instructions = await awbAxiosHandler
       // The timestamp query parameter is necessary to prevent caching
       .get(
         `api/v1/labs/${lab_id}/lab_versions/${version_id}/download?timestamp=${new Date().getTime()}`
       )
       .then(result => {
         console.log('Lab model fetched successfully');
@@ -81,17 +82,16 @@
 /**
  * POST the lab model / JSON from the .ipynb file/notebook to AWB
  *
  * @param awbAxiosHandler Axios client that contains a JWT Bearer token
  * @param panel Notebook panel
  * @param context Notebook context
  * @param lab_token lab token
- * @returns Promise<void>
  */
-export const postIndependentLabModel = async (
+export const postAwbLabModel = async (
   awbAxiosHandler: AxiosInstance,
   panel: NotebookPanel,
   context: DocumentRegistry.IContext<INotebookModel>,
   lab_token: string
 ): Promise<void> => {
   const confirmation_status = await showConfirmationStatus(
     'Publishing your lab onto Skills Network...'
@@ -142,31 +142,35 @@
   });
 };
 
 /**
  * GET the lab model / JSON that represents a .ipynb file/notebook from ATLAS
  *
  * @param axiosHandler Axios client that contains a JWT Bearer token
- * @returns Promise<void>
  */
-export const getLabModel = (axiosHandler: AxiosInstance) => {
+export const getAtlasLabModel = (axiosHandler: AxiosInstance) => {
   return (
     axiosHandler
       // The timestamp query parameter is necessary to prevent caching
       .get(`v1/labs?timestamp=${new Date().getTime()}`)
       .then(result => {
         Dialog.flush(); // remove spinner
         return result.data;
       })
       .catch(error => {
         throw 'Failed to fetch notebook';
       })
   );
 };
 
+/**
+ * GET the lab model / JSON that represents a .ipynb file/notebook from a URL
+ *
+ * @param notebook_url URL of the notebook
+ */
 export const getLearnerLabModel = (notebook_url: string) => {
   const url = new URL(notebook_url);
 
   // Adding a query parameter does not work when pulling from our private COS bucket which has authentication parameters
   if (url.searchParams.size === 0) {
     // The timestamp query parameter is necessary to prevent caching,
     // the headers are not sufficient on their own
@@ -192,17 +196,16 @@
 
 /**
  * POST the lab model / JSON from the .ipynb file/notebook to ATLAS
  *
  * @param axiosHandler Axios client that contains a JWT Bearer token
  * @param panel Notebook panel
  * @param context Notebook context
- * @returns Promise<void>
  */
-export const postLabModel = async (
+export const postAtlasLabModel = async (
   axiosHandler: AxiosInstance,
   panel: NotebookPanel,
   context: DocumentRegistry.IContext<INotebookModel>
 ): Promise<void> => {
   const confirmation_status = await showConfirmationStatus(
     'Publishing your lab onto Skills Network...'
   )
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/sn-file-library.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/sn-file-library.ts`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   #contextPath: string;
 
   constructor(contextPath: string) {
     this.#contextPath = contextPath;
   }
 
   launch() {
-    const token = Globals.TOKENS.get(this.#contextPath.split('/').pop() || '');
+    const token = Globals.TOKENS.get(this.#contextPath || '');
     const token_info = token
       ? (jwt_decode(token) as { [key: string]: any })
       : {};
     const anchor = document.createElement('a');
 
     if ('project_id' in token_info) {
       anchor.href = `${SN_FILE_LIBRARY_URL}?atlas_token=${token}`;
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/tools.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/tools.ts`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import { Contents } from '@jupyterlab/services';
 import * as nbformat from '@jupyterlab/nbformat';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { PathExt } from '@jupyterlab/coreutils/lib/path';
 import { ENV_TYPE, EnvType, Globals } from './config';
 import {
   atlasAxiosHandler,
-  getLabModel,
+  getAtlasLabModel,
   awbAxiosHandler,
-  getIndependentLabModel,
+  getAwbLabModel,
   getLearnerLabModel
 } from './handler';
 
 export interface ICellData {
   cell_type: string;
   id: string;
   metadata: {};
@@ -268,108 +268,104 @@
     const cellData = getCellContentsOmitID(cell);
     allCells.push(cellData);
   });
 
   return JSON.stringify(allCells, null, 2);
 };
 
-export const openIndependentLab = async (
+/**
+ * Opens a lab from Atlas or AWB
+ *
+ * @param atlas_token the Atlas token (or 'NO_TOKEN')
+ * @param awb_token the AWB token (or 'NO_TOKEN')
+ * @param dirPath the directory path to open the lab in
+ * @param docManager the JupyterLab document manager
+ * @param contentsManager the JupyterLab contents manager
+ * @param fileBrowser the JupyterLab file browser
+ * @returns the notebook panel
+ */
+export const openLab = async (
+  atlas_token: string,
   awb_token: string,
+  dirPath: string,
   docManager: IDocumentManager,
-  contentsManager: Contents.IManager
+  contentsManager: Contents.IManager,
+  fileBrowser: IDefaultFileBrowser
 ): Promise<NotebookPanel> => {
-  const { labFilename, body: instructions_content } =
-    await getIndependentLabModel(awbAxiosHandler(awb_token), awb_token);
-
-  let filePath = `${labFilename}`;
-
-  if (ENV_TYPE !== EnvType.JUPYTERLITE) {
-    // Outside of JupyterLite we want to use a relative path for some things
-    filePath = `./${filePath}`;
-    // We also want to delete the file if it is empty and create a backup if needed
-    await deleteIfEmptyFile(filePath, contentsManager, docManager);
-    await checkAndBackupSaveFile(
-      filePath,
-      instructions_content,
-      contentsManager,
-      docManager
-    );
+  let instructions_file_path: string;
+  let instructions_content: string;
+  let labFilename: string;
+  let token: string;
+
+  if (atlas_token !== 'NO_TOKEN') {
+    ({ instructions_file_path, body: instructions_content } =
+      await getAtlasLabModel(atlasAxiosHandler(atlas_token)));
+    labFilename = instructions_file_path;
+    token = atlas_token;
+  } else if (awb_token !== 'NO_TOKEN') {
+    ({ labFilename, body: instructions_content } = await getAwbLabModel(
+      awbAxiosHandler(awb_token),
+      awb_token
+    ));
+    token = awb_token;
   } else {
-    // Inside of JupyterLite we don't want persistent storage for authors, so we delete the existing file if it exists
-    await docManager.deleteFile(filePath);
+    throw Error('No valid token found.');
   }
 
-  // Set the publish button to only show for the lab with title labFilename
-  Globals.SHOW_PUBLISH_BUTTON_FOR = labFilename;
-  // Set the publish button to only work for the lab with title labFilename
-  Globals.TOKENS.set(labFilename, awb_token);
+  let filePath = `${labFilename}`;
 
-  const prevFile: Contents.IModel | null = await getFile(
-    filePath,
-    contentsManager
-  );
-  let nbPanel: NotebookPanel | undefined;
-  if (!prevFile) {
-    nbPanel = await createNotebook(
-      docManager,
-      labFilename,
-      instructions_content
-    );
+  if (dirPath !== '') {
+    filePath = `${dirPath}/${filePath}`;
+    await ensureSubFoldersExist(docManager, filePath);
+
+    if (fileBrowser.model.path !== dirPath) {
+      console.log(`Opening /${dirPath} in file browser`);
+      await fileBrowser.model.cd(`/${dirPath}`);
+    }
   } else {
-    nbPanel = docManager.openOrReveal(labFilename) as NotebookPanel;
+    await fileBrowser.model.cd('/');
   }
 
-  return nbPanel;
-};
-
-export const openLab = async (
-  token: string,
-  docManager: IDocumentManager,
-  contentsManager: Contents.IManager
-): Promise<NotebookPanel> => {
-  const { instructions_file_path, body: instructions_content } =
-    await getLabModel(atlasAxiosHandler(token));
-
-  const labFilename = getLabFileName(instructions_file_path);
-  let filePath = `${labFilename}`;
+  let potentialRelativePath = filePath;
 
   if (ENV_TYPE !== EnvType.JUPYTERLITE) {
     // Outside of JupyterLite we want to use a relative path for some things
-    filePath = `./${filePath}`;
+    potentialRelativePath = `./${filePath}`;
     // We also want to delete the file if it is empty and create a backup if needed
     await deleteIfEmptyFile(filePath, contentsManager, docManager);
     await checkAndBackupSaveFile(
-      filePath,
-      instructions_content,
+      potentialRelativePath,
+      instructions_content as ILabContent,
       contentsManager,
       docManager
     );
   } else {
     // Inside of JupyterLite we don't want persistent storage for authors, so we delete the existing file if it exists
-    await docManager.deleteFile(filePath);
+    await docManager.deleteFile(potentialRelativePath);
   }
 
-  // Set the publish button to only show for the lab with title labFilename
-  Globals.SHOW_PUBLISH_BUTTON_FOR = labFilename;
-  // Set the publish button to only work for the lab with title labFilename
-  Globals.TOKENS.set(labFilename, token);
+  // Set the publish button to only show for the opened lab
+  Globals.SHOW_PUBLISH_BUTTON_FOR = filePath;
+  Globals.TOKENS.set(filePath, token);
 
   const prevFile: Contents.IModel | null = await getFile(
-    filePath,
+    potentialRelativePath,
     contentsManager
   );
   let nbPanel: NotebookPanel | undefined;
   if (!prevFile) {
     nbPanel = await createNotebook(
       docManager,
-      labFilename,
-      JSON.parse(instructions_content)
+      filePath,
+      atlas_token !== 'NO_TOKEN'
+        ? JSON.parse(instructions_content)
+        : instructions_content
     );
   } else {
-    nbPanel = docManager.openOrReveal(labFilename) as NotebookPanel;
+    nbPanel = docManager.openOrReveal(filePath) as NotebookPanel;
   }
 
   return nbPanel;
 };
 
 export const openLearnerLab = async (
   notebookUrl: string,
@@ -556,42 +552,48 @@
     }
   }
 }
 
 export const loadLabContents = async (
   widget: NotebookPanel,
   notebook_content: nbformat.INotebookContent,
-  author_env?: string
+  env?: string
 ): Promise<void> => {
   // Wait for widget to initalize correctly before making changes
   await widget.context.ready;
 
-  if (author_env !== 'local') {
+  if (env !== EnvType.LOCAL) {
     // Load content
     widget.context.model.fromJSON(notebook_content);
     // Save content
     try {
-      // TODO: Minor Bug that can confuse user - after loading and saving,
-      // user is still prompted to save because JLabs updates the saved ipynb's metadata
       await widget.context.save();
     } catch (error) {
       console.error('[loadLabContents] Error saving notebook:', error);
     }
   } else {
     console.error(
-      '[loadLabContents] Notebook model is not initialized or authoring environment is local.'
+      '[loadLabContents] Notebook model is not initialized or environment is local.'
     );
   }
 };
 
-export const getLabFileName = (lab_filepath: any): string => {
-  const labFilePath = lab_filepath ?? Globals.DEFAULT_LAB_NAME;
-  // Extract filename from filepath
-  // TODO: This is required as the createNew method will not automatically create the parent directories
-  return labFilePath.replace(/^.*[\\/]/, '');
+/**
+ * Takes a file path and returns the directory path (no filename if it was included)
+ * @param filePath
+ */
+export const getAuthorLabFilePath = (filePath: string): string => {
+  let dir = filePath;
+  // Check if the path includes a filename and remove it if so
+  if (PathExt.extname(filePath) !== '') {
+    dir = PathExt.dirname(filePath);
+  }
+  dir = PathExt.removeSlash(dir);
+  // Remove any trailing slashes
+  return dir.replace(/\/+$/, '');
 };
 
 /**
  * Renames a file to filename.backup.ipynb and overwrites any files with the same name.
  *
  * @param {string} path - path to string.
  * @param {ContentsManager} contentsManager - The JupyterLab contents manager.
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/menu/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/menu/index.ts`

 * *Files 17% similar despite different names*

```diff
@@ -4,30 +4,38 @@
 } from '@jupyterlab/application';
 import { IMainMenu } from '@jupyterlab/mainmenu';
 import { Menu, Widget } from '@lumino/widgets';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { ICommandPalette } from '@jupyterlab/apputils';
+import { IDefaultFileBrowser } from '@jupyterlab/filebrowser';
 import { Contents } from '@jupyterlab/services';
 import { show_spinner, showFailureImportLabDialog } from '../dialog';
 import { MODE, Mode } from '../config';
-import { openIndependentLab, openLab } from '../tools';
+import { openLab } from '../tools';
 import jwt_decode from 'jwt-decode';
 
 const menu: JupyterFrontEndPlugin<void> = {
   id: 'skillsnetwork_jupyter_extension:menu',
   autoStart: true,
-  requires: [IMainMenu, ICommandPalette, INotebookTracker, IDocumentManager],
+  requires: [
+    IMainMenu,
+    ICommandPalette,
+    INotebookTracker,
+    IDocumentManager,
+    IDefaultFileBrowser
+  ],
   activate: async (
     app: JupyterFrontEnd,
     mainMenu: IMainMenu,
     palette: ICommandPalette,
     notebookTracker: INotebookTracker,
-    docManager: IDocumentManager
+    docManager: IDocumentManager,
+    fileBrowser: IDefaultFileBrowser
   ) => {
     console.log('skillsnetwork_jupyter_extension:menu extension activated');
 
     if (MODE === Mode.LEARN) {
       return;
     }
 
@@ -36,15 +44,16 @@
     const commandID = 'mainMenu:editLabFromToken';
     commands.addCommand(commandID, {
       label: 'Edit a Lab',
       execute: (args: any) => {
         showTokenDialog(
           notebookTracker,
           docManager,
-          app.serviceManager.contents
+          app.serviceManager.contents,
+          fileBrowser
         );
       }
     });
 
     const category = 'skillsNetwork';
     palette.addItem({
       command: commandID,
@@ -66,15 +75,16 @@
 };
 
 export default menu;
 
 function showTokenDialog(
   notebookTracker: INotebookTracker,
   docManager: IDocumentManager,
-  contentsManager: Contents.IManager
+  contentsManager: Contents.IManager,
+  fileBrowser: IDefaultFileBrowser
 ): void {
   // Generate Dialog body
   const bodyDialog = document.createElement('div');
   const nameLabel = document.createElement('label');
   nameLabel.textContent = 'Enter your authorization token';
   const tokenInput = document.createElement('input');
   tokenInput.className = 'jp-mod-styled';
@@ -90,21 +100,35 @@
       if (result.button.accept) {
         console.log('Token dialog accepted, loading lab...');
         show_spinner('Loading up your lab...');
 
         const token = tokenInput.value;
 
         const token_info = jwt_decode(token) as { [key: string]: any };
+
+        let atlas_token = 'NO_TOKEN';
+        let awb_token = 'NO_TOKEN';
+
         if ('version_id' in token_info) {
-          console.log('Token contains version_id, opening independent lab...');
-          await openIndependentLab(token, docManager, contentsManager);
+          console.log('Token contains version_id, opening AWB lab...');
+          awb_token = token;
         } else {
-          console.log('Token does not contain version_id, opening lab...');
-          await openLab(token, docManager, contentsManager);
+          console.log(
+            'Token does not contain version_id, opening Atlas lab...'
+          );
+          atlas_token = token;
         }
+        await openLab(
+          atlas_token,
+          awb_token,
+          'Token Launch',
+          docManager,
+          contentsManager,
+          fileBrowser
+        );
       }
     })
     .catch(e => {
       Dialog.flush(); //remove spinner
       showFailureImportLabDialog();
       console.error('Error occurred while importing lab:', e);
     });
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/theme/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/theme/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/src/toolbar/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc0/src/toolbar/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { IDefaultFileBrowser } from '@jupyterlab/filebrowser';
 import { Dialog, showDialog, ToolbarButton } from '@jupyterlab/apputils';
 import {
   getFileContents,
+  getAuthorLabFilePath,
   openLab,
-  openIndependentLab,
   openLearnerLab
 } from '../tools';
 import { IDisposable, DisposableDelegate } from '@lumino/disposable';
 import {
   atlasAxiosHandler,
-  postLabModel,
+  postAtlasLabModel,
   awbAxiosHandler,
-  postIndependentLabModel
+  postAwbLabModel
 } from '../handler';
 import { showFailureImportLabDialog } from '../dialog';
 import { Globals, EnvType, Mode, ENV_TYPE, FILE_PATH } from '../config';
 import {
   ATLAS_TOKEN,
   AWB_TOKEN,
   SET_DEFAULT_LAB_NAME_AND_KERNEL,
@@ -34,14 +34,15 @@
 import {
   NotebookPanel,
   INotebookModel,
   INotebookTracker
 } from '@jupyterlab/notebook';
 
 import { SkillsNetworkFileLibrary } from '../sn-file-library';
+import { PathExt } from '@jupyterlab/coreutils';
 
 /**
  * The plugin registration information.
  */
 const toolbar: JupyterFrontEndPlugin<void> = {
   id: 'skillsnetwork_jupyter_extension:toolbar',
   description: 'Toolbar plugin for Skills Network Authoring Extension',
@@ -79,54 +80,48 @@
     context: DocumentRegistry.IContext<INotebookModel>
   ): IDisposable {
     if (Globals.SHOW_PUBLISH_BUTTON_FOR !== context.path) {
       // This is not a Skills Network Lab notebook so return a no-op disposable
       return new DisposableDelegate(() => {});
     } else {
       // This is a Skills Network Lab notebook so add the publish button
-      const start = async () => {
+      const publish = async () => {
         // POST to Atlas the file contents/lab model
         const fullPath: string = context.path;
-        const filename: string = fullPath.split('/').pop() || '';
-        const token = Globals.TOKENS.get(filename);
+        const token = Globals.TOKENS.get(fullPath);
         if (token === undefined) {
           console.log(
-            `[ButtonExtension] No token found for filename: ${filename}`
+            `[ButtonExtension] No token found for filename: ${fullPath}`
           );
           await showDialog({
             title: 'Publishing Restricted',
             body: `Only the lab '${
               Globals.TOKENS.keys().next().value
             }' can be published during this editing session.`,
             buttons: [Dialog.okButton({ label: 'Dismiss' })]
           });
           return;
         }
 
         const token_info = jwt_decode(token) as { [key: string]: any };
 
         if ('version_id' in token_info) {
-          await postIndependentLabModel(
-            awbAxiosHandler(token),
-            panel,
-            context,
-            token
-          );
+          await postAwbLabModel(awbAxiosHandler(token), panel, context, token);
         } else {
-          await postLabModel(atlasAxiosHandler(token), panel, context);
+          await postAtlasLabModel(atlasAxiosHandler(token), panel, context);
         }
       };
 
       const download = async () => {
         const file = await getFileContents(panel, context);
         const blob = new Blob([file], { type: 'application/x-ipynb+json' });
         const url = URL.createObjectURL(blob);
 
         const link = document.createElement('a');
-        link.setAttribute('download', context.path);
+        link.setAttribute('download', PathExt.basename(context.path));
         link.setAttribute('href', url);
 
         document.body.appendChild(link);
         link.click();
 
         document.body.removeChild(link);
         URL.revokeObjectURL(url);
@@ -138,15 +133,15 @@
         onClick: download,
         tooltip: 'Download the current notebook ipynb file to your local system'
       });
 
       const publishButton = new ToolbarButton({
         className: 'publish-lab-button',
         label: 'Publish on SN',
-        onClick: start,
+        onClick: publish,
         tooltip: 'Publish Lab'
       });
 
       const snFileLibraryButton = new ToolbarButton({
         className: 'sn-file-library-button',
         label: 'SN File Library',
         onClick: () => new SkillsNetworkFileLibrary(context.path).launch(),
@@ -217,35 +212,40 @@
   const awb_token = AWB_TOKEN as string;
 
   console.log('skillsnetwork_jupyter_extension:toolbar extension activated');
 
   // Only show toolbar buttons for the lab that's launched via token
   app.docRegistry.addWidgetExtension('Notebook', new ButtonExtension());
 
+  let dirPath = '';
+
+  if (FILE_PATH !== null) {
+    dirPath = getAuthorLabFilePath(FILE_PATH);
+    console.log('Authoring lab file path:', dirPath);
+  }
+
   // Try to load up a notebook when author is using the browser tool (not in local)
   await app.serviceManager.ready;
   app.restored.then(async () => {
     await cleanUpEnvironment(notebookTracker);
-    if (atlas_token !== 'NO_TOKEN' && env_type !== EnvType.LOCAL) {
-      try {
-        await openLab(atlas_token, docManager, app.serviceManager.contents);
-      } catch (e) {
-        console.error('Error opening lab with Atlas token:', e);
-        Dialog.flush(); // remove spinner
-        showFailureImportLabDialog();
-      }
-    } else if (awb_token !== 'NO_TOKEN' && env_type !== EnvType.LOCAL) {
+    if (
+      env_type !== EnvType.LOCAL &&
+      (atlas_token !== 'NO_TOKEN' || awb_token !== 'NO_TOKEN')
+    ) {
       try {
-        await openIndependentLab(
+        await openLab(
+          atlas_token,
           awb_token,
+          dirPath,
           docManager,
-          app.serviceManager.contents
+          app.serviceManager.contents,
+          fileBrowser
         );
       } catch (e) {
-        console.error('Error opening lab with AWB token:', e);
+        console.error('Error opening lab with Atlas/AWB token:', e);
         Dialog.flush(); // remove spinner
         showFailureImportLabDialog();
       }
     }
   });
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/static/extension_demo.gif` & `skillsnetwork_jupyter_extension-2.3.0rc0/static/extension_demo.gif`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/.gitignore` & `skillsnetwork_jupyter_extension-2.3.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/LICENSE` & `skillsnetwork_jupyter_extension-2.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/README.md` & `skillsnetwork_jupyter_extension-2.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/pyproject.toml` & `skillsnetwork_jupyter_extension-2.3.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.2.1rc0/PKG-INFO` & `skillsnetwork_jupyter_extension-2.3.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skillsnetwork_jupyter_extension
-Version: 2.2.1rc0
+Version: 2.3.0rc0
 Dynamic: Keywords
 Summary: JupterLab/JupyerLite extension for Skills Network Labs
 Project-URL: Homepage, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/issues
 Project-URL: Repository, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension.git
 Author-email: IBM Skills Network <skills.network@ibm.com>
 License:                                  Apache License
```

