# Comparing `tmp/synthx-1.1.1.tar.gz` & `tmp/synthx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-1.1.1.tar", max compression
+gzip compressed data, was "synthx-1.2.0.tar", max compression
```

## Comparing `synthx-1.1.1.tar` & `synthx-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.1.1/README.md
--rw-r--r--   0        0        0     1270 2024-05-02 15:33:38.187018 synthx-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.1.1/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.1.1/synthx/core/__init__.py
--rw-r--r--   0        0        0    12500 2024-05-02 15:33:38.187244 synthx-1.1.1/synthx/core/dataset.py
--rw-r--r--   0        0        0     8907 2024-04-30 09:13:02.339542 synthx-1.1.1/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.1.1/synthx/core/sample.py
--rw-r--r--   0        0        0      923 2024-04-30 09:13:40.939358 synthx-1.1.1/synthx/errors/__init__.py
--rw-r--r--   0        0        0    11370 2024-05-02 15:33:38.187471 synthx-1.1.1/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.1.1/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.1.1/synthx/stats/norm.py
--rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.1.1/synthx/stats/p.py
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7544 2024-04-30 07:29:11.374218 synthx-1.2.0/README.md
+-rw-r--r--   0        0        0     1270 2024-05-03 02:09:11.373632 synthx-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-1.2.0/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-1.2.0/synthx/core/__init__.py
+-rw-r--r--   0        0        0    12500 2024-05-02 15:34:22.114713 synthx-1.2.0/synthx/core/dataset.py
+-rw-r--r--   0        0        0     9572 2024-05-03 02:09:11.373875 synthx-1.2.0/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-1.2.0/synthx/core/sample.py
+-rw-r--r--   0        0        0      923 2024-04-30 09:13:40.939358 synthx-1.2.0/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    11905 2024-05-03 02:09:11.374112 synthx-1.2.0/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-1.2.0/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-1.2.0/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1053 2024-04-23 18:47:48.800391 synthx-1.2.0/synthx/stats/p.py
+-rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 synthx-1.2.0/PKG-INFO
```

### Comparing `synthx-1.1.1/README.md` & `synthx-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/pyproject.toml` & `synthx-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "1.1.1"
+version = "1.2.0"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-1.1.1/synthx/core/dataset.py` & `synthx-1.2.0/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/synthx/core/result.py` & `synthx-1.2.0/synthx/core/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,26 @@
     """Synthetic control result."""
 
     def __init__(
         self,
         *,
         dataset: sx.Dataset,
         control_unit_weights: np.ndarray,
+        scales: np.ndarray,
     ) -> None:
         """Initialize SyntheticControlResult.
 
         Args:
             dataset (sx.Dataset): The dataset used for synthetic control analysis.
             control_unit_weights (np.ndarray): The weights of control units.
+            scales (np.ndarray): The weights to get both graph close.
         """
         self.dataset = dataset
         self.control_unit_weights = control_unit_weights
+        self.scales = scales
 
     @property
     def df_test(self) -> pl.DataFrame:
         """Get data in test group as a DataFrame.
 
         Returns:
             pl.DataFrame: dataframe of test group.
@@ -91,15 +94,18 @@
             columns=self.dataset.unit_column,
             values=self.dataset.y_column,
         ).drop(self.dataset.time_column)
         arr_control_pivoted = df_control_pivoted.to_numpy()
         control_unit_weight = self.control_unit_weights[
             self.dataset.intervention_units.index(intervention_unit)
         ]
-        return np.sum(arr_control_pivoted * control_unit_weight, axis=1)
+        y_control = np.sum(arr_control_pivoted * control_unit_weight, axis=1)
+        scale = self.scales[self.dataset.intervention_units.index(intervention_unit)]
+        print(scale, y_control)
+        return scale * y_control
 
     def estimate_effects(self) -> list[float]:
         """Estimate the effects of the intervention.
 
         Returns:
             list[float]: The estimated effect of the intervention.
         """
@@ -119,14 +125,15 @@
                 time_column=self.dataset.time_column,
                 y_column=self.dataset.y_column,
                 covariate_columns=self.dataset.covariate_columns,
                 intervention_units=self.dataset.intervention_units,
                 intervention_time=0,
             ),
             control_unit_weights=self.control_unit_weights,
+            scales=self.scales,
         )
         # dataset after intervention
         post_df = self.dataset.data.filter(
             self.dataset.data[self.dataset.time_column] >= self.dataset.intervention_time
         )
         post_result = SyntheticControlResult(
             dataset=sx.Dataset(
@@ -135,22 +142,26 @@
                 time_column=self.dataset.time_column,
                 y_column=self.dataset.y_column,
                 covariate_columns=self.dataset.covariate_columns,
                 intervention_units=self.dataset.intervention_units,
                 intervention_time=0,
             ),
             control_unit_weights=self.control_unit_weights,
+            scales=self.scales,
         )
         return [
-            np.mean(
-                post_result.y_test(intervention_unit) - post_result.y_control(intervention_unit)
-            )
-            - np.mean(
-                pre_result.y_test(intervention_unit) - pre_result.y_control(intervention_unit)
+            (
+                np.mean(
+                    post_result.y_test(intervention_unit) - post_result.y_control(intervention_unit)
+                )
+                - np.mean(
+                    pre_result.y_test(intervention_unit) - pre_result.y_control(intervention_unit)
+                )
             )
+            / np.mean(pre_result.y_test(intervention_unit))
             for intervention_unit in self.dataset.intervention_units
         ]
 
     def validation_differences(self) -> Optional[list[float]]:
         """Calculate the difference between training and validation.
 
         Returns:
@@ -170,14 +181,15 @@
                 time_column=self.dataset.time_column,
                 y_column=self.dataset.y_column,
                 covariate_columns=self.dataset.covariate_columns,
                 intervention_units=self.dataset.intervention_units,
                 intervention_time=0,
             ),
             control_unit_weights=self.control_unit_weights,
+            scales=self.scales,
         )
         # dataset in the validation period
         val_df = self.dataset.data.filter(
             (self.dataset.data[self.dataset.time_column] >= self.dataset.validation_time)
             & (self.dataset.data[self.dataset.time_column] < self.dataset.intervention_time)
         )
         val_result = SyntheticControlResult(
@@ -187,21 +199,27 @@
                 time_column=self.dataset.time_column,
                 y_column=self.dataset.y_column,
                 covariate_columns=self.dataset.covariate_columns,
                 intervention_units=self.dataset.intervention_units,
                 intervention_time=0,
             ),
             control_unit_weights=self.control_unit_weights,
+            scales=self.scales,
         )
 
         return [
-            np.mean(val_result.y_test(intervention_unit) - val_result.y_control(intervention_unit))
-            - np.mean(
-                pre_result.y_test(intervention_unit) - pre_result.y_control(intervention_unit)
+            (
+                np.mean(
+                    val_result.y_test(intervention_unit) - val_result.y_control(intervention_unit)
+                )
+                - np.mean(
+                    pre_result.y_test(intervention_unit) - pre_result.y_control(intervention_unit)
+                )
             )
+            / np.mean(pre_result.y_test(intervention_unit))
             for intervention_unit in self.dataset.intervention_units
         ]
 
     def plot(self, save: Optional[str] = None) -> None:
         """Plot the target variable over time for both test and control units.
 
         Args:
```

### Comparing `synthx-1.1.1/synthx/core/sample.py` & `synthx-1.2.0/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/synthx/errors/__init__.py` & `synthx-1.2.0/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/synthx/method.py` & `synthx-1.2.0/synthx/method.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             ((pl.col(variable) - pl.col(variable).min()) / pl.col(variable).std()).alias(variable)
         )
 
     # dataframe for control
     df_control = df.filter(condition_training_time & condition_control_units)
 
     control_unit_weights: list[np.ndarray] = []
+    scales: list[np.ndarray] = []
     for intervention_unit in dataset.intervention_units:
         condition_test_unit = df[dataset.unit_column] == intervention_unit
         df_test = df.filter(condition_training_time & condition_test_unit)
 
         # optimize unit weights
         def objective(unit_weights: np.ndarray) -> float:
             diff = 0
@@ -98,16 +99,27 @@
 
         if not solution.success:
             raise NoFeasibleModelError(
                 f'synthetic control optimization failed: test unit {intervention_unit}'
             )
         control_unit_weights.append(solution.x)
 
+        # scale
+        y_test = df_test[dataset.y_column].to_numpy()
+        df_control_pivoted = df_control.pivot(
+            index=dataset.time_column, columns=dataset.unit_column, values=dataset.y_column
+        ).drop(dataset.time_column)
+        arr_control_pivoted = df_control_pivoted.to_numpy()
+        y_control = np.sum(arr_control_pivoted * solution.x, axis=1)
+        scales.append(np.sum(y_test * y_control) / np.sum(y_control * y_control))
+
     return sx.SyntheticControlResult(
-        dataset=dataset, control_unit_weights=np.asarray(control_unit_weights)
+        dataset=dataset,
+        control_unit_weights=np.asarray(control_unit_weights),
+        scales=np.asarray(scales),
     )
 
 
 def placebo_test(
     dataset: sx.Dataset, n_jobs: int = -1
 ) -> tuple[list[float], list[float], sx.SyntheticControlResult, list[sx.SyntheticControlResult]]:
     """Perform a placebo test to assess the significance of the intervention effect.
```

### Comparing `synthx-1.1.1/synthx/stats/norm.py` & `synthx-1.2.0/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/synthx/stats/p.py` & `synthx-1.2.0/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-1.1.1/PKG-INFO` & `synthx-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

