# Comparing `tmp/spark_on_k8s-0.5.1.tar.gz` & `tmp/spark_on_k8s-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_on_k8s-0.5.1.tar", max compression
+gzip compressed data, was "spark_on_k8s-0.5.2.tar", max compression
```

## Comparing `spark_on_k8s-0.5.1.tar` & `spark_on_k8s-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2024-04-30 22:25:34.590385 spark_on_k8s-0.5.1/LICENSE
--rw-r--r--   0        0        0    11213 2024-04-30 22:25:34.590385 spark_on_k8s-0.5.1/README.md
--rw-r--r--   0        0        0     2366 2024-04-30 22:25:51.374422 spark_on_k8s-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       58 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/airflow/__init__.py
--rw-r--r--   0        0        0    14892 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/airflow/operators.py
--rw-r--r--   0        0        0     3114 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/airflow/triggers.py
--rw-r--r--   0        0        0     1190 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/__init__.py
--rw-r--r--   0        0        0     1744 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/app.py
--rw-r--r--   0        0        0     1472 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/apps.py
--rw-r--r--   0        0        0      728 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/configuration.py
--rw-r--r--   0        0        0     1305 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/main.py
--rw-r--r--   0        0        0     6750 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/__init__.py
--rw-r--r--   0        0        0      587 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/static/app_logs.css
--rw-r--r--   0        0        0      758 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/static/apps.css
--rw-r--r--   0        0        0     1416 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/templates/app_logs.html
--rw-r--r--   0        0        0     2953 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/templates/apps.html
--rw-r--r--   0        0        0      368 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/templates/error.html
--rw-r--r--   0        0        0      542 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/__init__.py
--rw-r--r--   0        0        0     1621 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/api.py
--rw-r--r--   0        0        0     6601 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/app.py
--rw-r--r--   0        0        0      690 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/apps.py
--rw-r--r--   0        0        0      553 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/namespace.py
--rw-r--r--   0        0        0     8686 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/cli/options.py
--rw-r--r--   0        0        0    27728 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/client.py
--rw-r--r--   0        0        0        0 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/k8s/__init__.py
--rw-r--r--   0        0        0     3135 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/k8s/async_client.py
--rw-r--r--   0        0        0     2849 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/k8s/sync_client.py
--rw-r--r--   0        0        0        0 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/__init__.py
--rw-r--r--   0        0        0    19764 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/app_manager.py
--rw-r--r--   0        0        0     9617 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/async_app_manager.py
--rw-r--r--   0        0        0     4048 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/configuration.py
--rw-r--r--   0        0        0      488 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/logging_mixin.py
--rw-r--r--   0        0        0     3956 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/setup_namespace.py
--rw-r--r--   0        0        0      842 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/spark_app_status.py
--rw-r--r--   0        0        0      141 2024-04-30 22:25:34.594385 spark_on_k8s-0.5.1/spark_on_k8s/utils/types.py
--rw-r--r--   0        0        0    13060 1970-01-01 00:00:00.000000 spark_on_k8s-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-03 12:14:02.577140 spark_on_k8s-0.5.2/LICENSE
+-rw-r--r--   0        0        0    11213 2024-05-03 12:14:02.577140 spark_on_k8s-0.5.2/README.md
+-rw-r--r--   0        0        0     2366 2024-05-03 12:14:18.773167 spark_on_k8s-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/__init__.py
+-rw-r--r--   0        0        0    15115 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/operators.py
+-rw-r--r--   0        0        0     3114 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/airflow/triggers.py
+-rw-r--r--   0        0        0     1190 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/__init__.py
+-rw-r--r--   0        0        0     1744 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/app.py
+-rw-r--r--   0        0        0     1472 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/apps.py
+-rw-r--r--   0        0        0      728 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/configuration.py
+-rw-r--r--   0        0        0     1305 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/main.py
+-rw-r--r--   0        0        0     6750 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/app_logs.css
+-rw-r--r--   0        0        0      758 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/apps.css
+-rw-r--r--   0        0        0     1416 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/app_logs.html
+-rw-r--r--   0        0        0     2953 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/apps.html
+-rw-r--r--   0        0        0      368 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/error.html
+-rw-r--r--   0        0        0      542 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/api.py
+-rw-r--r--   0        0        0     6601 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/app.py
+-rw-r--r--   0        0        0      690 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/apps.py
+-rw-r--r--   0        0        0      553 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/namespace.py
+-rw-r--r--   0        0        0     8686 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/cli/options.py
+-rw-r--r--   0        0        0    27728 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/client.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/async_client.py
+-rw-r--r--   0        0        0     2849 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/k8s/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/__init__.py
+-rw-r--r--   0        0        0    19764 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/app_manager.py
+-rw-r--r--   0        0        0     9617 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/async_app_manager.py
+-rw-r--r--   0        0        0     4048 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/configuration.py
+-rw-r--r--   0        0        0      488 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/logging_mixin.py
+-rw-r--r--   0        0        0     3956 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/setup_namespace.py
+-rw-r--r--   0        0        0      842 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/spark_app_status.py
+-rw-r--r--   0        0        0      141 2024-05-03 12:14:02.585140 spark_on_k8s-0.5.2/spark_on_k8s/utils/types.py
+-rw-r--r--   0        0        0    13060 1970-01-01 00:00:00.000000 spark_on_k8s-0.5.2/PKG-INFO
```

### Comparing `spark_on_k8s-0.5.1/LICENSE` & `spark_on_k8s-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/README.md` & `spark_on_k8s-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/pyproject.toml` & `spark_on_k8s-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-on-k8s"
-version = "0.5.1"
+version = "0.5.2"
 description = "A Python package to submit and manage Apache Spark applications on Kubernetes."
 authors = ["Hussein Awala <hussein@awala.fr>"]
 readme = "README.md"
 repository = "https://github.com/hussein-awala/spark-on-k8s"
 keywords = ["spark", "kubernetes", "k8s", "spark-submit", "spark-on-k8s"]
 license = "Apache-2.0"
 packages = [{include = "spark_on_k8s"}]
```

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/airflow/operators.py` & `spark_on_k8s-0.5.2/spark_on_k8s/airflow/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,20 @@
                 poll_interval=self.poll_interval,
             )
         elif self.app_waiter == "log":
             spark_app_manager.stream_logs(
                 namespace=self.namespace,
                 pod_name=self._driver_pod_name,
             )
+            # wait for termination status
+            spark_app_manager.wait_for_app(
+                namespace=self.namespace,
+                pod_name=self._driver_pod_name,
+                poll_interval=1,
+            )
         app_status = spark_app_manager.app_status(
             namespace=self.namespace,
             pod_name=self._driver_pod_name,
         )
         if app_status == "Succeeded":
             return app_status
         raise AirflowException(f"The job finished with status: {app_status}")
```

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/airflow/triggers.py` & `spark_on_k8s-0.5.2/spark_on_k8s/airflow/triggers.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/__init__.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/app.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/apps.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/configuration.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/main.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/main.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/__init__.py` & `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/static/app_logs.css` & `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/app_logs.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/static/apps.css` & `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/static/apps.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/templates/app_logs.html` & `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/app_logs.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/api/webserver/templates/apps.html` & `spark_on_k8s-0.5.2/spark_on_k8s/api/webserver/templates/apps.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/__init__.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/api.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/api.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/app.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/apps.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/namespace.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/cli/options.py` & `spark_on_k8s-0.5.2/spark_on_k8s/cli/options.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/client.py` & `spark_on_k8s-0.5.2/spark_on_k8s/client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/k8s/async_client.py` & `spark_on_k8s-0.5.2/spark_on_k8s/k8s/async_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/k8s/sync_client.py` & `spark_on_k8s-0.5.2/spark_on_k8s/k8s/sync_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/utils/app_manager.py` & `spark_on_k8s-0.5.2/spark_on_k8s/utils/app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/utils/async_app_manager.py` & `spark_on_k8s-0.5.2/spark_on_k8s/utils/async_app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/utils/configuration.py` & `spark_on_k8s-0.5.2/spark_on_k8s/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/utils/setup_namespace.py` & `spark_on_k8s-0.5.2/spark_on_k8s/utils/setup_namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/spark_on_k8s/utils/spark_app_status.py` & `spark_on_k8s-0.5.2/spark_on_k8s/utils/spark_app_status.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.5.1/PKG-INFO` & `spark_on_k8s-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-on-k8s
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Python package to submit and manage Apache Spark applications on Kubernetes.
 Home-page: https://github.com/hussein-awala/spark-on-k8s
 License: Apache-2.0
 Keywords: spark,kubernetes,k8s,spark-submit,spark-on-k8s
 Author: Hussein Awala
 Author-email: hussein@awala.fr
 Requires-Python: >=3.8,<4.0
```

