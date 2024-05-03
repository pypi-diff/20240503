# Comparing `tmp/krypt-0.1.1.tar.gz` & `tmp/krypt-0.1.2.tar.gz`

## Comparing `krypt-0.1.1.tar` & `krypt-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 krypt-0.1.1/tox.ini
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 krypt-0.1.1/.github/workflows/python-build.yml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 krypt-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/krypt.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 krypt-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/__main__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/main.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/parser.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/init.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/seal.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/unseal.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/argument_parsers/__init__.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/argument_parsers/init.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/argument_parsers/seal.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/argument_parsers/unseal.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/preflight_checks/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/preflight_checks/init.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/preflight_checks/seal.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/actions/preflight_checks/unseal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/pki/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/pki/decryptor.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/pki/encryptor.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/pki/keypair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/util/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/util/git_util.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/util/meta_util.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/util/path_util.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 krypt-0.1.1/krypt/util/zip_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 krypt-0.1.1/tests/test_main.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 krypt-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 krypt-0.1.1/LICENSE
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 krypt-0.1.1/README.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 krypt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 krypt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 krypt-0.1.2/tox.ini
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 krypt-0.1.2/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 krypt-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/krypt.iml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 krypt-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/__main__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/main.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/parser.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/init.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/seal.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/unseal.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/argument_parsers/__init__.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/argument_parsers/init.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/argument_parsers/seal.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/argument_parsers/unseal.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/preflight_checks/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/preflight_checks/init.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/preflight_checks/seal.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/actions/preflight_checks/unseal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/pki/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/pki/decryptor.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/pki/encryptor.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/pki/keypair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/util/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/util/git_util.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/util/meta_util.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/util/path_util.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 krypt-0.1.2/krypt/util/zip_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krypt-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 krypt-0.1.2/tests/test_main.py
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 krypt-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 krypt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 krypt-0.1.2/README.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 krypt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 krypt-0.1.2/PKG-INFO
```

### Comparing `krypt-0.1.1/.github/workflows/python-build.yml` & `krypt-0.1.2/.github/workflows/python-build.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 name: Build Python Package
 
-on: push
+on:
+  pull_request:
+    branches:
+    - main
+  push:
+    branches:
+    - main
 
 permissions:
   contents: read
 
 jobs:
   build:
-
-    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-latest]
+    runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build tox pex
+        pip install tox pex
     - name: Run checks with tox
       run: tox
     - name: Build an executable with pex
-      run: mkdir bin && pex . -o bin/krypt -e krypt.main:launch
+      run: mkdir bin && pex . -o bin/krypt-${{ runner.os }} -r deps.txt -e krypt.main:launch
     - name: Upload krypt executable
       uses: actions/upload-artifact@v4
       with:
-        name: krypt
-        path: bin/krypt
+        name: krypt-${{ runner.os }}
+        path: bin/krypt-${{ runner.os }}
         retention-days: 7
-
```

### Comparing `krypt-0.1.1/.github/workflows/python-publish.yml` & `krypt-0.1.2/.github/workflows/python-publish.yml`

 * *Files 24% similar despite different names*

```diff
@@ -5,40 +5,54 @@
     types: [published]
 
 permissions:
   contents: write
   id-token: write
 
 jobs:
-  build_and_deploy:
-
-    runs-on: ubuntu-latest
-    environment: release
+  build:
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-latest]
+    runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build tox pex
+        pip install pex tox
     - name: Run checks with tox
       run: tox
-    - name: Build package
-      run: python -m build
-    - name: Publish package distributions to PyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
     - name: Build an executable with pex
-      run: mkdir bin && pex . -o bin/krypt -e krypt.main:launch
+      run: mkdir bin && pex . -o bin/krypt-${{ runner.os }} -r deps.txt -e krypt.main:launch
     - name: Upload krypt executable
       uses: actions/upload-artifact@v4
       with:
-        name: krypt
-        path: bin/krypt
+        name: krypt-${{ runner.os }}
+        path: bin/krypt-${{ runner.os }}
         retention-days: 7
-    - name: Add the executable to release assets
-      uses: softprops/action-gh-release@v2
+
+  deploy:
+    runs-on: ubuntu-latest
+    needs: build
+
+    environment: release
+
+    steps:
+    - uses: actions/checkout@v4
+    - name: Set up Python
+      uses: actions/setup-python@v5
       with:
-        files: bin/krypt
+        python-version: '3.x'
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install build
+    - name: Build package
+      run: python -m build
+    - name: Publish package distributions to PyPI
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `krypt-0.1.1/krypt/__init__.py` & `krypt-0.1.2/krypt/__init__.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/main.py` & `krypt-0.1.2/krypt/main.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/parser.py` & `krypt-0.1.2/krypt/parser.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/__init__.py` & `krypt-0.1.2/krypt/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/init.py` & `krypt-0.1.2/krypt/actions/init.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/seal.py` & `krypt-0.1.2/krypt/actions/seal.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/unseal.py` & `krypt-0.1.2/krypt/actions/unseal.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/argument_parsers/init.py` & `krypt-0.1.2/krypt/actions/argument_parsers/init.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/argument_parsers/seal.py` & `krypt-0.1.2/krypt/actions/argument_parsers/seal.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/argument_parsers/unseal.py` & `krypt-0.1.2/krypt/actions/argument_parsers/unseal.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/preflight_checks/__init__.py` & `krypt-0.1.2/krypt/actions/preflight_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/preflight_checks/init.py` & `krypt-0.1.2/krypt/actions/preflight_checks/init.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/actions/preflight_checks/unseal.py` & `krypt-0.1.2/krypt/actions/preflight_checks/unseal.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/pki/keypair.py` & `krypt-0.1.2/krypt/pki/keypair.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/util/git_util.py` & `krypt-0.1.2/krypt/util/git_util.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/util/meta_util.py` & `krypt-0.1.2/krypt/util/meta_util.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/util/path_util.py` & `krypt-0.1.2/krypt/util/path_util.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/krypt/util/zip_util.py` & `krypt-0.1.2/krypt/util/zip_util.py`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/.gitignore` & `krypt-0.1.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -168,7 +168,8 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+deps.txt
```

### Comparing `krypt-0.1.1/LICENSE` & `krypt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/README.md` & `krypt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `krypt-0.1.1/pyproject.toml` & `krypt-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krypt"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Kubermate", email="168834048+kubermate@users.noreply.github.com" },
 ]
 description = "A helper tool for file encryption in Git repositories primarily aimed at encrypting Kubernetes secrets and other sensitive information to be later used in a CI/CD pipeline"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `krypt-0.1.1/PKG-INFO` & `krypt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: krypt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A helper tool for file encryption in Git repositories primarily aimed at encrypting Kubernetes secrets and other sensitive information to be later used in a CI/CD pipeline
 Project-URL: Homepage, https://github.com/kubertools/krypt
 Project-URL: Issues, https://github.com/kubertools/krypt/issues
 Author-email: Kubermate <168834048+kubermate@users.noreply.github.com>
 License-File: LICENSE
 Keywords: ci/cd pipeline,encryption,gitops,kubernetes,secrets
 Classifier: Development Status :: 4 - Beta
```

