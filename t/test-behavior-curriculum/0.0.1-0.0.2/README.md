# Comparing `tmp/test_behavior_curriculum-0.0.1.tar.gz` & `tmp/test_behavior_curriculum-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_behavior_curriculum-0.0.1.tar", last modified: Fri May  3 18:06:48 2024, max compression
+gzip compressed data, was "test_behavior_curriculum-0.0.2.tar", last modified: Fri May  3 18:30:15 2024, max compression
```

## Comparing `test_behavior_curriculum-0.0.1.tar` & `test_behavior_curriculum-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.413324 test_behavior_curriculum-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/workflows/tag_publish_upload.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.417324 test_behavior_curriculum-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-03 18:06:48.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-03 18:06:48.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:06:48.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 18:06:48.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 18:06:48.000000 test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:06:48.421324 test_behavior_curriculum-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 18:06:37.000000 test_behavior_curriculum-0.0.1/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.625495 test_behavior_curriculum-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.617495 test_behavior_curriculum-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.617495 test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.617495 test_behavior_curriculum-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/workflows/tag_publish_upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-03 18:30:15.625495 test_behavior_curriculum-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.617495 test_behavior_curriculum-0.0.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.621495 test_behavior_curriculum-0.0.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.621495 test_behavior_curriculum-0.0.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:30:15.625495 test_behavior_curriculum-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.617495 test_behavior_curriculum-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.621495 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 18:30:06.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.621495 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-03 18:30:15.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-03 18:30:15.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:30:15.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 18:30:15.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 18:30:15.000000 test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:30:15.621495 test_behavior_curriculum-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 18:30:05.000000 test_behavior_curriculum-0.0.2/tests/test_example.py
```

### Comparing `test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/.github/ISSUE_TEMPLATE/user-story.md` & `test_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/.github/workflows/init.yml` & `test_behavior_curriculum-0.0.2/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/.github/workflows/tag_publish_upload.yml` & `test_behavior_curriculum-0.0.2/.github/workflows/tag_publish_upload.yml`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,15 @@
   upload_curriculum:
     needs: [tag, publish]
     runs-on: ubuntu-latest
     permissions:
       id-token: write
       contents: read
     env:
-      AWS_AIND_BEHAVIOR_ROLE: 'arn:aws:iam::467914378000:role/AindBehaviorCurriculumBucketGithubRole'
+      AWS_AIND_BEHAVIOR_ROLE: ${{ secrets.AIND_AWS_BEHAVIOR_CURRICULUM_ROLE }}
       AWS_BEHAVIOR_CURRICULUM_BUCKET: 'aind-behavior-curriculum-prod-o5171v'
       AWS_REGION: 'us-west-2'
       TEMP_DIR: 'temp_dir'
       S3_PREFIX: 'curriculums'
       REPO_NAME: ${{ github.repository }}
       VERSION: ${{ needs.tag.outputs.new_version }}
 
@@ -109,17 +109,17 @@
       - name: Set up Python 3.11
         uses: actions/setup-python@v3
         with:
           python-version: 3.11
       - name: Configure aws credentials
         uses: aws-actions/configure-aws-credentials@v2
         with:
-          role-to-assume: ${{ env.AWS_AIND_BEHAVIOR_ROLE }}
+          role-to-assume: $AWS_AIND_BEHAVIOR_ROLE
           role-session-name: github-schema-upload-session
-          aws-region: ${{ env.AWS_REGION }}
+          aws-region: $AWS_REGION
       - name: Install dependencies
         run: |
           sudo apt install graphviz libgraphviz-dev -y
           python -m pip install -e .
           python -m pip install awscli
       - name: Upload curriculum and curriculum diagram
         # Upload curriculum if TEMP_DIR is not empty.
```

### Comparing `test_behavior_curriculum-0.0.1/.github/workflows/test_and_lint.yml` & `test_behavior_curriculum-0.0.2/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/.gitignore` & `test_behavior_curriculum-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/LICENSE` & `test_behavior_curriculum-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/PKG-INFO` & `test_behavior_curriculum-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.1/README.md` & `test_behavior_curriculum-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/Makefile` & `test_behavior_curriculum-0.0.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/make.bat` & `test_behavior_curriculum-0.0.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/source/_static/dark-logo.svg` & `test_behavior_curriculum-0.0.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/source/_static/favicon.ico` & `test_behavior_curriculum-0.0.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/source/_static/light-logo.svg` & `test_behavior_curriculum-0.0.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/doc_template/source/conf.py` & `test_behavior_curriculum-0.0.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/pyproject.toml` & `test_behavior_curriculum-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/PKG-INFO` & `test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-behavior-curriculum
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-behavior-curriculum-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `test_behavior_curriculum-0.0.1/src/test_behavior_curriculum.egg-info/SOURCES.txt` & `test_behavior_curriculum-0.0.2/src/test_behavior_curriculum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

