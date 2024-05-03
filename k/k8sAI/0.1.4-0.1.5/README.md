# Comparing `tmp/k8sai-0.1.4.tar.gz` & `tmp/k8sai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8sai-0.1.4.tar", last modified: Fri May  3 08:23:33 2024, max compression
+gzip compressed data, was "k8sai-0.1.5.tar", last modified: Fri May  3 08:24:37 2024, max compression
```

## Comparing `k8sai-0.1.4.tar` & `k8sai-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.851215 k8sai-0.1.4/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.4/LICENSE
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.4/MANIFEST.in
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:23:33.850968 k8sai-0.1.4/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.4/README.md
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.840852 k8sai-0.1.4/k8sAI/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.4/k8sAI/__init__.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.842278 k8sai-0.1.4/k8sAI/kuberag/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.4/k8sAI/kuberag/__init__.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     2680 2024-05-03 03:56:55.000000 k8sai-0.1.4/k8sAI/kuberag/chat.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.842403 k8sai-0.1.4/k8sAI/kuberag/embeddings/
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.850518 k8sai-0.1.4/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.4/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.4/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.4/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.4/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
--rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.4/k8sAI/kuberag/embeddings/chroma.sqlite3
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3501 2024-05-03 01:47:59.000000 k8sai-0.1.4/k8sAI/kuberag/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.4/k8sAI/kuberag/retriever.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.4/k8sAI/kuberag/tool_handler.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     6926 2024-05-03 06:45:53.000000 k8sai-0.1.4/k8sAI/kuberag/tools.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     4345 2024-05-03 06:43:38.000000 k8sai-0.1.4/k8sAI/main.py
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      139 2024-05-03 06:42:49.000000 k8sai-0.1.4/k8sAI/util.py
-drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:23:33.850690 k8sai-0.1.4/k8sAI.egg-info/
--rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/PKG-INFO
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/entry_points.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       78 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/requires.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-03 08:23:33.000000 k8sai-0.1.4/k8sAI.egg-info/top_level.txt
--rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-03 08:23:33.851255 k8sai-0.1.4/setup.cfg
--rw-r--r--   0 wilsonspearman   (501) staff       (20)      752 2024-05-03 08:11:27.000000 k8sai-0.1.4/setup.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.659787 k8sai-0.1.5/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)    34523 2024-05-01 19:17:58.000000 k8sai-0.1.5/LICENSE
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       45 2024-05-02 00:01:57.000000 k8sai-0.1.5/MANIFEST.in
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:24:37.659487 k8sai-0.1.5/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3311 2024-05-02 00:16:00.000000 k8sai-0.1.5/README.md
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.633052 k8sai-0.1.5/k8sAI/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:29:38.000000 k8sai-0.1.5/k8sAI/__init__.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.635602 k8sai-0.1.5/k8sAI/kuberag/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-04-30 19:56:40.000000 k8sai-0.1.5/k8sAI/kuberag/__init__.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     2680 2024-05-03 03:56:55.000000 k8sai-0.1.5/k8sAI/kuberag/chat.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.635830 k8sai-0.1.5/k8sAI/kuberag/embeddings/
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.658833 k8sai-0.1.5/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  6284000 2024-05-01 22:10:06.000000 k8sai-0.1.5/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/data_level0.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      100 2024-05-01 22:10:05.000000 k8sai-0.1.5/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/header.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4000 2024-05-01 22:10:06.000000 k8sai-0.1.5/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/length.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        0 2024-05-01 22:10:05.000000 k8sai-0.1.5/k8sAI/kuberag/embeddings/8e153713-b589-4b93-8e0f-cae56950b20d/link_lists.bin
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)  3272704 2024-04-30 23:46:31.000000 k8sai-0.1.5/k8sAI/kuberag/embeddings/chroma.sqlite3
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3501 2024-05-03 01:47:59.000000 k8sai-0.1.5/k8sAI/kuberag/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      746 2024-05-02 00:01:57.000000 k8sai-0.1.5/k8sAI/kuberag/retriever.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     1810 2024-05-02 05:42:12.000000 k8sai-0.1.5/k8sAI/kuberag/tool_handler.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     6926 2024-05-03 06:45:53.000000 k8sai-0.1.5/k8sAI/kuberag/tools.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     4345 2024-05-03 06:43:38.000000 k8sai-0.1.5/k8sAI/main.py
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      139 2024-05-03 06:42:49.000000 k8sai-0.1.5/k8sAI/util.py
+drwxr-xr-x   0 wilsonspearman   (501) staff       (20)        0 2024-05-03 08:24:37.659083 k8sai-0.1.5/k8sAI.egg-info/
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)     3766 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      751 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        1 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       42 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       78 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/requires.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)        6 2024-05-03 08:24:37.000000 k8sai-0.1.5/k8sAI.egg-info/top_level.txt
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)       38 2024-05-03 08:24:37.659833 k8sai-0.1.5/setup.cfg
+-rw-r--r--   0 wilsonspearman   (501) staff       (20)      752 2024-05-03 08:24:33.000000 k8sai-0.1.5/setup.py
```

### Comparing `k8sai-0.1.4/LICENSE` & `k8sai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/PKG-INFO` & `k8sai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.4
+Version: 0.1.5
 Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `k8sai-0.1.4/README.md` & `k8sai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/chat.py` & `k8sai-0.1.5/k8sAI/kuberag/chat.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/embeddings/chroma.sqlite3` & `k8sai-0.1.5/k8sAI/kuberag/embeddings/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/main.py` & `k8sai-0.1.5/k8sAI/kuberag/main.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/retriever.py` & `k8sai-0.1.5/k8sAI/kuberag/retriever.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/tool_handler.py` & `k8sai-0.1.5/k8sAI/kuberag/tool_handler.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/kuberag/tools.py` & `k8sai-0.1.5/k8sAI/kuberag/tools.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI/main.py` & `k8sai-0.1.5/k8sAI/main.py`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/k8sAI.egg-info/PKG-INFO` & `k8sai-0.1.5/k8sAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8sAI
-Version: 0.1.4
+Version: 0.1.5
 Summary: A conversational AI for Kubernetes users.
 Home-page: https://github.com/wilson090/k8sAI
 Author: Wilson Spearman
 Author-email: wilsonspearman@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `k8sai-0.1.4/k8sAI.egg-info/SOURCES.txt` & `k8sai-0.1.5/k8sAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k8sai-0.1.4/setup.py` & `k8sai-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 setup(
     name="k8sAI",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     description="A conversational AI for Kubernetes users.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Wilson Spearman",
     author_email="wilsonspearman@gmail.com",
     url="https://github.com/wilson090/k8sAI",
```

