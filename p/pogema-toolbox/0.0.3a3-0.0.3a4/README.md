# Comparing `tmp/pogema_toolbox-0.0.3a3.tar.gz` & `tmp/pogema_toolbox-0.0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema_toolbox-0.0.3a3.tar", last modified: Thu Apr 18 12:54:41 2024, max compression
+gzip compressed data, was "pogema_toolbox-0.0.3a4.tar", last modified: Fri May  3 15:54:42 2024, max compression
```

## Comparing `pogema_toolbox-0.0.3a3.tar` & `pogema_toolbox-0.0.3a4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.663657 pogema_toolbox-0.0.3a3/
--rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-18 12:54:41.662527 pogema_toolbox-0.0.3a3/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema_toolbox-0.0.3a3/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.647186 pogema_toolbox-0.0.3a3/pogema_toolbox/
--rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-04-18 12:52:07.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/algorithm_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/config_variant_generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2247 2024-04-18 12:48:29.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/create_env.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/eval_utils.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11792 2024-04-18 12:52:14.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/evaluator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/fix_num_threads_issue.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.653595 pogema_toolbox-0.0.3a3/pogema_toolbox/maps/
--rw-r--r--   0 skrynnik   (503) staff       (20)     2501 2024-04-15 14:00:58.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/maps/default-maps.yaml
--rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/registry.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/results_holder.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.660562 pogema_toolbox-0.0.3a3/pogema_toolbox/views/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_multi_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_tabular.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.661795 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-18 12:54:41.663765 pogema_toolbox-0.0.3a3/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema_toolbox-0.0.3a3/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.301425 pogema_toolbox-0.0.3a4/
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-03 15:54:42.300927 pogema_toolbox-0.0.3a4/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema_toolbox-0.0.3a4/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.293492 pogema_toolbox-0.0.3a4/pogema_toolbox/
+-rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-05-03 15:53:57.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      401 2024-05-03 15:52:20.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/algorithm_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/config_variant_generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2247 2024-04-18 12:48:29.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/create_env.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/eval_utils.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    14691 2024-05-03 15:53:15.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/evaluator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/fix_num_threads_issue.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.296678 pogema_toolbox-0.0.3a4/pogema_toolbox/maps/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2501 2024-04-15 14:00:58.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/maps/default-maps.yaml
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/registry.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/results_holder.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.299953 pogema_toolbox-0.0.3a4/pogema_toolbox/views/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_multi_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_tabular.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-05-03 15:54:42.300495 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-05-03 15:54:42.000000 pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-05-03 15:54:42.301486 pogema_toolbox-0.0.3a4/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema_toolbox-0.0.3a4/setup.py
```

### Comparing `pogema_toolbox-0.0.3a3/LICENSE` & `pogema_toolbox-0.0.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/PKG-INFO` & `pogema_toolbox-0.0.3a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/config_variant_generator.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/config_variant_generator.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/create_env.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/create_env.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/eval_utils.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/evaluator.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/evaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from pogema_toolbox.registry import ToolboxRegistry
 
 from pogema_toolbox.views.view_multi_plot import process_multi_plot_view, MultiPlotView
 from pogema_toolbox.views.view_plot import process_plot_view, PlotView
 from pogema_toolbox.views.view_tabular import process_table_view, TabularView
 from pogema_toolbox.results_holder import ResultsHolder
 
+from concurrent.futures import ProcessPoolExecutor
+
 
 def run_episode(env, algo):
     """
     Runs an episode in the environment using the given algorithm.
 
     Args:
         env: The environment to run the episode in.
@@ -158,26 +160,98 @@
     import dask.distributed as dd
     initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
 
     num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
     cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1, nthreads=1, )
     client = dd.Client(cluster, timeout="120s")  # Connect the client to the cluster
 
+    ToolboxRegistry.get_maps()
+    registry_state = ToolboxRegistry.get_state()
+
     futures = []
     for left, right in split_on_chunks(len(env_configs), initialized_algo_config.num_process):
-        future = client.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name, pure=False)
+        future = client.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name, registry_state, pure=False)
         futures.append(future)
 
     results = client.gather(futures)  # Gather the results from the distributed tasks
     client.close()  # Close the Dask client and cluster
     cluster.close()
     results = np.concatenate(results).tolist()
     return results
 
 
+def balanced_multiprocess_backend(algo_config, env_configs, full_algo_name):
+    """
+    Runs the algorithm in a balanced manner using multiple processes.
+
+    Args:
+        algo_config: Configuration for the algorithm.
+        env_configs: List of environment configurations.
+        full_algo_name: Full name of the algorithm.
+
+    Returns:
+        List: Results of running the algorithm on the environments.
+    """
+    initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
+
+    num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
+    balanced_buckets = get_balanced_buckets_indexes(env_configs, num_process)
+
+    # Getting maps to initialize registry (if not) and  avoid multiple loading
+    ToolboxRegistry.get_maps()
+    registry_state = ToolboxRegistry.get_state()
+
+    with ProcessPoolExecutor(num_process) as executor:
+        future2stuff = []
+        for bucket in balanced_buckets:
+            # select config from env_configs by their id from bucket
+            bucket_configs = [env_configs[idx] for idx in bucket]
+            future2stuff.append(
+                executor.submit(sequential_backend, algo_config, bucket_configs, full_algo_name, registry_state))
+
+        # Reorder the results according to the original order of env_configs
+        ordered_results = [None for _ in range(len(env_configs))]
+        for idx, future in enumerate(future2stuff):
+            bucket = balanced_buckets[idx]
+            bucket_results = future.result()
+            for i, env_idx in enumerate(bucket):
+                ordered_results[env_idx] = bucket_results[i]
+
+    return ordered_results
+
+
+def multiprocess_backend(algo_config, env_configs, full_algo_name):
+    """
+    Runs the algorithm in parallel using multiple processes.
+
+    Args:
+        algo_config: Configuration for the algorithm.
+        env_configs: List of environment configurations.
+        full_algo_name: Full name of the algorithm.
+
+    Returns:
+        List: Results of running the algorithm on the environments.
+    """
+    initialized_algo_config = ToolboxRegistry.create_algorithm_config(algo_config['name'], **algo_config)
+
+    ToolboxRegistry.get_maps()
+    registry_state = ToolboxRegistry.get_state()
+
+    results = []
+    num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
+    with ProcessPoolExecutor(num_process) as executor:
+        future2stuff = []
+        for left, right in split_on_chunks(len(env_configs), initialized_algo_config.num_process):
+            future2stuff.append(
+                executor.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name, registry_state))
+        for future in future2stuff:
+            results += future.result()
+    return results
+
+
 def balanced_dask_backend(algo_config, env_configs, full_algo_name):
     """
     Runs the algorithm in a balanced manner using Dask for distributed computing.
 
     Args:
         algo_config: Configuration for the algorithm.
         env_configs: List of environment configurations.
@@ -195,21 +269,21 @@
     balanced_buckets = get_balanced_buckets_indexes(env_configs, num_process)
 
     cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1, nthreads=1)
     client = dd.Client(cluster, timeout="120s")  # Connect the client to the cluster
 
     futures = []
 
-    # Getting maps to initialize registry (if not) and  avoid multiple loading
     ToolboxRegistry.get_maps()
     registry_state = ToolboxRegistry.get_state()
 
     for bucket in balanced_buckets:
         bucket_configs = [env_configs[idx] for idx in bucket]
-        future = client.submit(sequential_backend, algo_config, bucket_configs, full_algo_name, registry_state, pure=False)
+        future = client.submit(sequential_backend, algo_config, bucket_configs, full_algo_name, registry_state,
+                               pure=False)
         futures.append(future)
 
     results = client.gather(futures)
     client.close()
     cluster.close()
 
     # Reorder the results according to the original order of env_configs
@@ -289,20 +363,20 @@
     results = []
     for key, algo_cfg in evaluation_config['algorithms'].items():
         p_algo_cfg = ToolboxRegistry.create_algorithm_config(algo_cfg['name'], **algo_cfg)
         logger.info(f'Starting: {key}, {algo_cfg}')
         start_time = time.monotonic()
         if p_algo_cfg.parallel_backend == 'sequential':
             metrics = sequential_backend(algo_cfg, environment_configs, key)
-        # elif p_algo_cfg.parallel_backend == 'multiprocessing':
-        #     metrics = multiprocess_backend(algo_cfg, environment_configs, key)
+        elif p_algo_cfg.parallel_backend == 'multiprocessing':
+            metrics = multiprocess_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'dask':
             metrics = dask_backend(algo_cfg, environment_configs, key)
-        # elif p_algo_cfg.parallel_backend == 'balanced_multiprocessing':
-        #     metrics = balanced_multiprocess_backend(algo_cfg, environment_configs, key)
+        elif p_algo_cfg.parallel_backend == 'balanced_multiprocessing':
+            metrics = balanced_multiprocess_backend(algo_cfg, environment_configs, key)
         elif p_algo_cfg.parallel_backend == 'balanced_dask':
             metrics = balanced_dask_backend(algo_cfg, environment_configs, key)
         else:
             raise ValueError(f'Unknown parallel backend: {p_algo_cfg.parallel_backend}')
         algo_results = join_metrics_and_configs(metrics, environment_configs, env_grid_search, algo_cfg, key)
         if eval_dir:
             save_path = Path(eval_dir) / f'{key}.json'
```

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/maps/default-maps.yaml` & `pogema_toolbox-0.0.3a4/pogema_toolbox/maps/default-maps.yaml`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/registry.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/registry.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_multi_plot.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_multi_plot.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_plot.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_plot.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_tabular.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_tabular.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_utils.py` & `pogema_toolbox-0.0.3a4/pogema_toolbox/views/view_utils.py`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/PKG-INFO` & `pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/SOURCES.txt` & `pogema_toolbox-0.0.3a4/pogema_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pogema_toolbox-0.0.3a3/setup.py` & `pogema_toolbox-0.0.3a4/setup.py`

 * *Files identical despite different names*

