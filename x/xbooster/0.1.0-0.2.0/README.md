# Comparing `tmp/xbooster-0.1.0.tar.gz` & `tmp/xbooster-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbooster-0.1.0.tar", max compression
+gzip compressed data, was "xbooster-0.2.0.tar", max compression
```

## Comparing `xbooster-0.1.0.tar` & `xbooster-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-02-14 10:37:37.681440 xbooster-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     4232 2024-02-14 12:52:23.363020 xbooster-0.1.0/README.md
--rw-r--r--   0        0        0      727 2024-02-14 13:11:03.501584 xbooster-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-02-13 14:22:51.544451 xbooster-0.1.0/xbooster/.DS_Store
--rw-r--r--   0        0        0       17 2024-02-13 21:49:27.431142 xbooster-0.1.0/xbooster/__init__.py
--rw-r--r--   0        0        0     6911 2024-02-13 21:49:27.456857 xbooster-0.1.0/xbooster/_parser.py
--rw-r--r--   0        0        0     5690 2024-02-13 21:49:45.590482 xbooster-0.1.0/xbooster/_utils.py
--rw-r--r--   0        0        0    28641 2024-02-14 09:53:56.565516 xbooster-0.1.0/xbooster/constructor.py
--rw-r--r--   0        0        0    22243 2024-02-14 11:33:13.017619 xbooster-0.1.0/xbooster/explainer.py
--rw-r--r--   0        0        0     5176 1970-01-01 00:00:00.000000 xbooster-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-14 10:37:37.681440 xbooster-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0    16771 2024-05-03 11:06:56.522410 xbooster-0.2.0/README.md
+-rw-r--r--   0        0        0      746 2024-05-02 12:29:40.770207 xbooster-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-02-13 14:22:51.544451 xbooster-0.2.0/xbooster/.DS_Store
+-rw-r--r--   0        0        0       17 2024-02-13 21:49:27.431142 xbooster-0.2.0/xbooster/__init__.py
+-rw-r--r--   0        0        0     6911 2024-02-13 21:49:27.456857 xbooster-0.2.0/xbooster/_parser.py
+-rw-r--r--   0        0        0    12457 2024-04-30 18:54:22.550733 xbooster-0.2.0/xbooster/_utils.py
+-rw-r--r--   0        0        0    28641 2024-02-14 09:53:56.565516 xbooster-0.2.0/xbooster/constructor.py
+-rw-r--r--   0        0        0    41429 2024-05-02 10:43:56.668725 xbooster-0.2.0/xbooster/explainer.py
+-rw-r--r--   0        0        0    17755 1970-01-01 00:00:00.000000 xbooster-0.2.0/PKG-INFO
```

### Comparing `xbooster-0.1.0/LICENSE.md` & `xbooster-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xbooster-0.1.0/pyproject.toml` & `xbooster-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xbooster"
-version = "0.1.0"
+version = "0.2.0"
 description = "Explainable Boosted Scoring"
 authors = ["Denis Burakov <dennyemb@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
@@ -12,25 +12,26 @@
 duckdb = "^0.9.2"
 ipykernel = "6.25.2"
 matplotlib = "^3.8.0"
 numpy = "1.26.0"
 pandas = "2.0.3"
 pylint = "^3.0.3"
 scipy = "^1.11.4"
+scikit-learn = "^1.3.0"
 shap = "^0.44.0"
 xgboost = "^2.0.0"
-optbinning = "^0.19.0"
 pytest = "^8.0.0"
 pre-commit = "^3.6.1"
+jupyter = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.25.2"
 pytest = "^8.0.0"
 black = "^24.2.0"
 
 [tool.black]
-line-length = 100
+line-length = 60
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xbooster-0.1.0/xbooster/.DS_Store` & `xbooster-0.2.0/xbooster/.DS_Store`

 * *Files identical despite different names*

### Comparing `xbooster-0.1.0/xbooster/_parser.py` & `xbooster-0.2.0/xbooster/_parser.py`

 * *Files identical despite different names*

### Comparing `xbooster-0.1.0/xbooster/constructor.py` & `xbooster-0.2.0/xbooster/constructor.py`

 * *Files identical despite different names*

