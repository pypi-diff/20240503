# Comparing `tmp/tea_tasting-0.0.3.tar.gz` & `tmp/tea_tasting-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tea_tasting-0.0.3.tar", last modified: Sun Apr 21 13:48:01 2024, max compression
+gzip compressed data, was "tea_tasting-0.0.4.tar", last modified: Fri May  3 16:05:16 2024, max compression
```

## Comparing `tea_tasting-0.0.3.tar` & `tea_tasting-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/LICENSE
--rw-r--r--   0        0        0    14620 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/README.md
--rw-r--r--   0        0        0     3015 2024-04-21 13:48:01.136269 tea_tasting-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      392 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/__init__.py
--rw-r--r--   0        0        0        6 2024-04-21 13:48:01.132269 tea_tasting-0.0.3/src/tea_tasting/_version.txt
--rw-r--r--   0        0        0    11760 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/aggr.py
--rw-r--r--   0        0        0     2986 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/config.py
--rw-r--r--   0        0        0    13295 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/datasets.py
--rw-r--r--   0        0        0     6812 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/experiment.py
--rw-r--r--   0        0        0      350 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/__init__.py
--rw-r--r--   0        0        0     8605 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/base.py
--rw-r--r--   0        0        0    12534 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/mean.py
--rw-r--r--   0        0        0     4104 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/proportion.py
--rw-r--r--   0        0        0     8999 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/utils.py
--rw-r--r--   0        0        0      390 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/version.py
--rw-r--r--   0        0        0        0 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_base.py
--rw-r--r--   0        0        0     8593 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_mean.py
--rw-r--r--   0        0        0     4241 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_proportion.py
--rw-r--r--   0        0        0     6431 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_aggr.py
--rw-r--r--   0        0        0     1504 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_config.py
--rw-r--r--   0        0        0     3538 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_datasets.py
--rw-r--r--   0        0        0    10574 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_experiment.py
--rw-r--r--   0        0        0     6349 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_utils.py
--rw-r--r--   0        0        0      779 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_version.py
--rw-r--r--   0        0        0    15834 1970-01-01 00:00:00.000000 tea_tasting-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-03 16:04:35.196043 tea_tasting-0.0.4/LICENSE
+-rw-r--r--   0        0        0    14634 2024-05-03 16:04:35.196043 tea_tasting-0.0.4/README.md
+-rw-r--r--   0        0        0     3086 2024-05-03 16:05:16.760676 tea_tasting-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1033 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/__init__.py
+-rw-r--r--   0        0        0        6 2024-05-03 16:05:16.756676 tea_tasting-0.0.4/src/tea_tasting/_version.txt
+-rw-r--r--   0        0        0    12060 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/aggr.py
+-rw-r--r--   0        0        0     5084 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/config.py
+-rw-r--r--   0        0        0    17874 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/datasets.py
+-rw-r--r--   0        0        0    21570 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/experiment.py
+-rw-r--r--   0        0        0      772 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/metrics/__init__.py
+-rw-r--r--   0        0        0     8660 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/metrics/base.py
+-rw-r--r--   0        0        0    15229 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/metrics/mean.py
+-rw-r--r--   0        0        0     5100 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/metrics/proportion.py
+-rw-r--r--   0        0        0    11422 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/utils.py
+-rw-r--r--   0        0        0      390 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/src/tea_tasting/version.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/metrics/__init__.py
+-rw-r--r--   0        0        0    10600 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/metrics/test_base.py
+-rw-r--r--   0        0        0     8584 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/metrics/test_mean.py
+-rw-r--r--   0        0        0     4241 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/metrics/test_proportion.py
+-rw-r--r--   0        0        0     6431 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_aggr.py
+-rw-r--r--   0        0        0     1504 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_config.py
+-rw-r--r--   0        0        0     3538 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_datasets.py
+-rw-r--r--   0        0        0    14664 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_experiment.py
+-rw-r--r--   0        0        0     7202 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0      779 2024-05-03 16:04:35.200043 tea_tasting-0.0.4/tests/test_version.py
+-rw-r--r--   0        0        0    15849 1970-01-01 00:00:00.000000 tea_tasting-0.0.4/PKG-INFO
```

### Comparing `tea_tasting-0.0.3/LICENSE` & `tea_tasting-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/README.md` & `tea_tasting-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 - Sample ratio mismatch check.
 
 **tea-tasting** calculates statistics within data backends such as BigQuery, ClickHouse, PostgreSQL, Snowflake, Spark, and other of 20+ backends supported by [Ibis](https://ibis-project.org/). This approach eliminates the need to import granular data into a Python environment, though Pandas DataFrames are also supported.
 
 **tea-tasting** is still in alpha, but already includes all the features listed above. The following features are coming soon:
 
 - More statistical tests:
-  - Bootstrap.
-  - Quantile test (using Bootstrap).
-  - Asymptotic and exact tests for frequency data.
-  - Mann–Whitney U test.
+    - Bootstrap.
+    - Quantile test (using Bootstrap).
+    - Asymptotic and exact tests for frequency data.
+    - Mann–Whitney U test.
 - Power analysis.
 - A/A tests and simulations.
 - Pretty output for experiment results (round etc.).
 - More documentation and examples.
 
 ## Installation
 
@@ -109,17 +109,17 @@
 Use the `Mean` class to compare averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
 
 Use the `RatioOfMeans` class to compare ratios of averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
 
 Use the following parameters of `Mean` and `RatioOfMeans` to customize the analysis:
 
 - `alternative`: Alternative hypothesis. The following options are available:
-  - `"two-sided"` (default): the means are unequal.
-  - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
-  - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
+    - `"two-sided"` (default): the means are unequal.
+    - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
+    - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
 - `confidence_level`: Confidence level of the confidence interval. Default is `0.95`.
 - `equal_var`: Defines whether equal variance is assumed. If `True`, pooled variance is used for the calculation of the standard error of the difference between two means. Default is `False`.
 - `use_t`: Defines whether to use the Student's t-distribution (`True`) or the Normal distribution (`False`). Default is `True`.
 
 Example usage:
 
 ```python
```

### Comparing `tea_tasting-0.0.3/pyproject.toml` & `tea_tasting-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 name = "tea-tasting"
 dynamic = []
 description = "A Python package for statistical analysis of A/B tests."
 authors = [
     { name = "Evgeny Ivanov", email = "ivanov.evgeny.n@gmail.com" },
 ]
 dependencies = [
-    "ibis-framework[pandas]>=7,<9",
-    "numpy>=1.25,<2",
+    "ibis-framework[pandas]>=7,<10",
+    "numpy>=1.25,<3",
     "pandas>=2,<3",
     "scipy>=1.10,<2",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Typing :: Typed",
 ]
-version = "0.0.3"
+version = "0.0.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/tea-tasting"
 
@@ -45,14 +45,18 @@
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
 package-dir = "src"
 
 [tool.pdm.dev-dependencies]
+docs = [
+    "mkdocs-material",
+    "mkdocstrings[crystal,python]",
+]
 lint = [
     "ruff",
     "pyright",
 ]
 test = [
     "pytest",
     "coverage[toml]",
```

### Comparing `tea_tasting-0.0.3/src/tea_tasting/aggr.py` & `tea_tasting-0.0.4/src/tea_tasting/aggr.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 _COUNT = "_count"
 _MEAN = "_mean__{}"
 _VAR = "_var__{}"
 _COV = "_cov__{}__{}"
 _DEMEAN = "_demean__{}"
 
 
-class Aggregates(tea_tasting.utils.ReprMixin):
-    """Aggregated statistics."""
+class Aggregates(tea_tasting.utils.ReprMixin):  # noqa: D101
     count_: int | None
     mean_: dict[str, float | int]
     var_: dict[str, float | int]
     cov_: dict[tuple[str, str], float | int]
 
     def __init__(
         self,
@@ -47,70 +46,76 @@
         """
         self.count_ = count_
         self.mean_ = mean_
         self.var_ = var_
         self.cov_ = {_sorted_tuple(*k): v for k, v in cov_.items()}
 
     def with_zero_div(self) -> Aggregates:
-        """Return aggregates, which don't raise an error on division by zero.
+        """Return aggregates that do not raise an error on division by zero.
 
         Division by zero returns:
-            nan if numerator == 0,
-            inf if numerator > 0,
-            -inf if numerator < 0.
+            - `nan` if numerator is equal to `0`,
+            - `inf` if numerator is greater than `0`,
+            - `-inf` if numerator is less than `0`.
         """
         return Aggregates(
             count_=None if self.count_ is None else tea_tasting.utils.Int(self.count_),
             mean_={k: tea_tasting.utils.numeric(v) for k, v in self.mean_.items()},
             var_={k: tea_tasting.utils.numeric(v) for k, v in self.var_.items()},
             cov_={k: tea_tasting.utils.numeric(v) for k, v in self.cov_.items()},
         )
 
     def count(self) -> int:
         """Sample size (number of observations).
 
         Raises:
-            RuntimeError: Count is None (it wasn't defined at init).
+            RuntimeError: Count is `None` (if it was not defined during initialization).
 
         Returns:
             Sample size (number of observations).
         """
         if self.count_ is None:
             raise RuntimeError("Count is None.")
         return self.count_
 
     def mean(self, name: str | None) -> float | int:
         """Sample mean.
 
+        Assume the variable is a constant `1` if the variable name is `None`.
+
         Args:
             name: Variable name.
 
         Returns:
             Sample mean.
         """
         if name is None:
             return 1
         return self.mean_[name]
 
     def var(self, name: str | None) -> float | int:
         """Sample variance.
 
+        Assume the variable is a constant if the variable name is `None`.
+
         Args:
             name: Variable name.
 
         Returns:
             Sample variance.
         """
         if name is None:
             return 0
         return self.var_[name]
 
     def cov(self, left: str | None, right: str | None) -> float | int:
         """Sample covariance.
 
+        Assume the variable is a constant if the variable name is `None`.
+
         Args:
             left: First variable name.
             right: Second variable name.
 
         Returns:
             Sample covariance.
         """
@@ -121,24 +126,24 @@
     def ratio_var(
         self,
         numer: str | None,
         denom: str | None,
     ) -> float | int:
         """Sample variance of the ratio of two variables using the Delta method.
 
-        References:
-            [Delta method](https://en.wikipedia.org/wiki/Delta_method).
-            [Taylor expansions for the moments of functions of random variables](https://en.wikipedia.org/wiki/Taylor_expansions_for_the_moments_of_functions_of_random_variables).
-
         Args:
             numer: Numerator variable name.
             denom: Denominator variable name.
 
         Returns:
             Sample variance of the ratio of two variables.
+
+        References:
+            - [Delta method](https://en.wikipedia.org/wiki/Delta_method).
+            - [Taylor expansions for the moments of functions of random variables](https://en.wikipedia.org/wiki/Taylor_expansions_for_the_moments_of_functions_of_random_variables).
         """
         numer_mean_sq = self.mean(numer) * self.mean(numer)
         denom_mean_sq = self.mean(denom) * self.mean(denom)
         return (
             self.var(numer)
             - 2 * self.cov(numer, denom) * self.mean(numer) / self.mean(denom)
             + self.var(denom) * numer_mean_sq / denom_mean_sq
@@ -149,39 +154,39 @@
         left_numer: str | None,
         left_denom: str | None,
         right_numer: str | None,
         right_denom: str | None,
     ) -> float | int:
         """Sample covariance of the ratios of variables using the Delta method.
 
-        References:
-            [Delta method](https://en.wikipedia.org/wiki/Delta_method).
-            [Taylor expansions for the moments of functions of random variables](https://en.wikipedia.org/wiki/Taylor_expansions_for_the_moments_of_functions_of_random_variables).
-
         Args:
             left_numer: First numerator variable name.
             left_denom: First denominator variable name.
             right_numer: Second numerator variable name.
             right_denom: Second denominator variable name.
 
         Returns:
             Sample covariance of the ratios of variables.
+
+        References:
+            - [Delta method](https://en.wikipedia.org/wiki/Delta_method).
+            - [Taylor expansions for the moments of functions of random variables](https://en.wikipedia.org/wiki/Taylor_expansions_for_the_moments_of_functions_of_random_variables).
         """
         left_ratio_of_means = self.mean(left_numer) / self.mean(left_denom)
         right_ratio_of_means = self.mean(right_numer) / self.mean(right_denom)
         return (
             self.cov(left_numer, right_numer)
             - self.cov(left_numer, right_denom) * right_ratio_of_means
             - self.cov(left_denom, right_numer) * left_ratio_of_means
             + self.cov(left_denom, right_denom)
                 * left_ratio_of_means * right_ratio_of_means
         ) / self.mean(left_denom) / self.mean(right_denom)
 
     def __add__(self, other: Aggregates) -> Aggregates:
-        """Calculate aggregated statistics of the concatenation of two samples.
+        """Calculate the aggregated statistics of the concatenation of two samples.
 
         Samples are assumed to be independent.
 
         Args:
             other: Aggregated statistics of the second sample.
 
         Returns:
@@ -250,21 +255,21 @@
     data: ibis.expr.types.Table | pd.DataFrame,
     group_col: str | None,
     has_count: bool,
     mean_cols: Sequence[str],
     var_cols: Sequence[str],
     cov_cols: Sequence[tuple[str, str]],
 ) -> dict[Any, Aggregates] | Aggregates:
-    """Read aggregated statistics from an Ibis Table or a Pandas DataFrame.
+    """Extract aggregated statistics from an Ibis Table or a Pandas DataFrame.
 
     Args:
         data: Granular data.
         group_col: Column name to group by before aggregation.
-            If None, total aggregates are calculated.
-        has_count: If True, calculate the sample size.
+            If `None`, total aggregates are calculated.
+        has_count: If `True`, calculate the sample size.
         mean_cols: Column names for calculation of sample means.
         var_cols: Column names for calculation of sample variances.
         cov_cols: Pairs of column names for calculation of sample covariances.
 
     Returns:
         Aggregated statistics.
     """
```

### Comparing `tea_tasting-0.0.3/src/tea_tasting/metrics/base.py` & `tea_tasting-0.0.4/src/tea_tasting/metrics/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,50 +29,50 @@
     def analyze(
         self,
         data: pd.DataFrame | ibis.expr.types.Table,
         control: Any,
         treatment: Any,
         variant: str,
     ) -> R:
-        """Analyze metric in an experiment.
+        """Analyze a metric in an experiment.
 
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
         Returns:
             Analysis result.
         """
         ...
 
 
 class AggrCols(NamedTuple):
-    """Columns to aggregate for a metric analysis.
+    """Columns to be aggregated for a metric analysis.
 
     Attributes:
-        has_count: If True, include the sample size.
+        has_count: If `True`, include the sample size.
         mean_cols: Column names for calculation of sample means.
         var_cols: Column names for calculation of sample variances.
         cov_cols: Pairs of column names for calculation of sample covariances.
     """
     has_count: bool = False
     mean_cols: Sequence[str] = ()
     var_cols: Sequence[str] = ()
     cov_cols: Sequence[tuple[str, str]] = ()
 
     def __or__(self, other: AggrCols) -> AggrCols:
-        """Combine columns, exclude duplicates.
+        """Merge two aggregation column specifications.
 
         Args:
             other: Second objects.
 
         Returns:
-            Combined columns.
+            Merged column specifications.
         """
         return AggrCols(
             has_count=self.has_count or other.has_count,
             mean_cols=tuple({*self.mean_cols, *other.mean_cols}),
             var_cols=tuple({*self.var_cols, *other.var_cols}),
             cov_cols=tuple({
                 tea_tasting.aggr._sorted_tuple(*cols)
@@ -94,15 +94,15 @@
 
 
 class MetricBaseAggregated(MetricBase[R]):
     """Base class for metrics, which are analyzed using aggregated statistics."""
     @property
     @abc.abstractmethod
     def aggr_cols(self) -> AggrCols:
-        """Columns to aggregate for a metric analysis."""
+        """Columns to be aggregated for a metric analysis."""
         ...
 
     @overload
     def analyze(
         self,
         data: dict[Any, tea_tasting.aggr.Aggregates],
         control: Any,
@@ -125,15 +125,15 @@
         self,
         data: pd.DataFrame | ibis.expr.types.Table | dict[
             Any, tea_tasting.aggr.Aggregates],
         control: Any,
         treatment: Any,
         variant: str | None = None,
     ) -> R:
-        """Analyze metric in an experiment.
+        """Analyze a metric in an experiment.
 
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
@@ -173,52 +173,52 @@
     aggr_cols: AggrCols,
     variant: str | None = None,
 ) ->  dict[Any, tea_tasting.aggr.Aggregates]:
     """Aggregate experimental data by variants.
 
     Args:
         data: Experimental data.
-        aggr_cols: Columns to aggregate.
+        aggr_cols: Columns to be aggregated.
         variant: Variant column name.
 
     Raises:
-        ValueError: variant is None, while aggregated data are not provided.
+        ValueError: The variant parameter is required but was not provided.
         TypeError: data is not an instance of DataFrame, Table,
-            or a dictionary if Aggregates.
+            or a dictionary of Aggregates.
 
     Returns:
         Experimental data as a dictionary of Aggregates.
     """
     if isinstance(data, dict) and all(
         isinstance(v, tea_tasting.aggr.Aggregates) for v in data.values()  # type: ignore
     ):
         return data
 
     if variant is None:
-        raise ValueError("variant is None, but should be an instance of str.")
+        raise ValueError("The variant parameter is required but was not provided.")
 
     if not isinstance(data, pd.DataFrame | ibis.expr.types.Table):
         raise TypeError(
             f"data is a {type(data)}, but must be an instance of"
-            " DataFrame, Table, or a dictionary if Aggregates.",
+            " DataFrame, Table, or a dictionary of Aggregates.",
         )
 
     return tea_tasting.aggr.read_aggregates(
         data=data,
         group_col=variant,
         **aggr_cols._asdict(),
     )
 
 
 class MetricBaseGranular(MetricBase[R]):
     """Base class for metrics, which are analyzed using granular data."""
     @property
     @abc.abstractmethod
     def cols(self) -> Sequence[str]:
-        """Columns to fetch for a metric analysis."""
+        """Columns to be fetched for a metric analysis."""
         ...
 
     @overload
     def analyze(
         self,
         data: dict[Any, pd.DataFrame],
         control: Any,
@@ -240,15 +240,15 @@
     def analyze(
         self,
         data: pd.DataFrame | ibis.expr.types.Table | dict[Any, pd.DataFrame],
         control: Any,
         treatment: Any,
         variant: str | None = None,
     ) -> R:
-        """Analyze metric in an experiment.
+        """Analyze a metric in an experiment.
 
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
@@ -292,28 +292,28 @@
 
     Args:
         data: Experimental data.
         cols: Columns to read.
         variant: Variant column name.
 
     Raises:
-        ValueError: variant is None, while granular data are not provided.
+        ValueError: The variant parameter is required but was not provided.
         TypeError: data is not an instance of DataFrame, Table,
             or a dictionary if DataFrames.
 
     Returns:
         Experimental data as a dictionary of DataFrames.
     """
     if isinstance(data, dict) and all(
         isinstance(v, pd.DataFrame) for v in data.values()  # type: ignore
     ):
         return data
 
     if variant is None:
-        raise ValueError("variant is None, but should be an instance of str.")
+        raise ValueError("The variant parameter is required but was not provided.")
 
     if isinstance(data, ibis.expr.types.Table):
         data = data.select(*cols, variant).to_pandas()
 
     if not isinstance(data, pd.DataFrame):
         raise TypeError(
             f"data is a {type(data)}, but must be an instance of"
```

### Comparing `tea_tasting-0.0.3/src/tea_tasting/metrics/mean.py` & `tea_tasting-0.0.4/src/tea_tasting/metrics/mean.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Analysis of means."""
+"""Metrics for the analysis of means."""
 # ruff: noqa: PD901
 
 from __future__ import annotations
 
 import math
 from typing import TYPE_CHECKING, NamedTuple
 
@@ -14,16 +14,16 @@
 import tea_tasting.utils
 
 
 if TYPE_CHECKING:
     from typing import Literal
 
 
-class MeansResult(NamedTuple):
-    """Result of an analysis of means.
+class MeanResult(NamedTuple):
+    """Result of the analysis of means.
 
     Attributes:
         control: Control mean.
         treatment: Treatment mean.
         effect_size: Absolute effect size. Difference between two means.
         effect_size_ci_lower: Lower bound of the absolute effect size
             confidence interval.
@@ -46,49 +46,84 @@
     rel_effect_size: float
     rel_effect_size_ci_lower: float
     rel_effect_size_ci_upper: float
     pvalue: float
     statistic: float
 
 
-class RatioOfMeans(MetricBaseAggregated[MeansResult]):
-    """Ratio of means."""
-
+class RatioOfMeans(MetricBaseAggregated[MeanResult]):  # noqa: D101
     def __init__(  # noqa: PLR0913
         self,
         numer: str,
         denom: str | None = None,
         numer_covariate: str | None = None,
         denom_covariate: str | None = None,
         *,
         alternative: Literal["two-sided", "greater", "less"] | None = None,
         confidence_level: float | None = None,
         equal_var: bool | None = None,
         use_t: bool | None = None,
     ) -> None:
-        """Ratio of means.
+        """Metric for the analysis of ratios of means.
 
         Args:
             numer: Numerator column name.
             denom: Denominator column name.
             numer_covariate: Covariate numerator column name.
             denom_covariate: Covariate denominator column name.
-            alternative: Alternative hypothesis. Options:
-                "two-sided": the means are unequal.
-                "greater": the mean in the treatment variant is greater than the mean
-                    in the control variant.
-                "less": the mean in the treatment variant is less than the mean
-                    in the control variant.
+            alternative: Alternative hypothesis.
             confidence_level: Confidence level for the confidence interval.
-            equal_var: Defines whether equal variance is assumed. If True,
+            equal_var: Defines whether equal variance is assumed. If `True`,
                 pooled variance is used for the calculation of the standard error
                 of the difference between two means.
-            use_t: Defines whether to use the Student's t-distribution (True) or
-                the Normal distribution (False).
-        """
+            use_t: Defines whether to use the Student's t-distribution (`True`) or
+                the Normal distribution (`False`).
+
+        Alternative hypothesis options:
+            - `"two-sided"`: the means are unequal,
+            - `"greater"`: the mean in the treatment variant is greater than the mean
+                in the control variant,
+            - `"less"`: the mean in the treatment variant is less than the mean
+                in the control variant.
+
+        Examples:
+            ```python
+            import tea_tasting as tt
+
+
+            experiment = tt.Experiment(
+                orders_per_session=tt.RatioOfMeans("orders", "sessions"),
+            )
+
+            data = tt.make_users_data(seed=42)
+            result = experiment.analyze(data)
+            print(result)
+            #>             metric control treatment rel_effect_size rel_effect_size_ci pvalue
+            #> orders_per_session   0.266     0.289            8.8%      [-0.89%, 19%] 0.0762
+            ```
+
+            With CUPED:
+
+            ```python
+            experiment = tt.Experiment(
+                orders_per_session=tt.RatioOfMeans(
+                    "orders",
+                    "sessions",
+                    "orders_covariate",
+                    "sessions_covariate",
+                ),
+            )
+
+            data = tt.make_users_data(seed=42, covariates=True)
+            result = experiment.analyze(data)
+            print(result)
+            #>             metric control treatment rel_effect_size rel_effect_size_ci  pvalue
+            #> orders_per_session   0.262     0.293             12%        [4.2%, 21%] 0.00229
+            ```
+        """  # noqa: E501
         self.numer = tea_tasting.utils.check_scalar(numer, "numer", typ=str)
         self.denom = tea_tasting.utils.check_scalar(denom, "denom", typ=str | None)
         self.numer_covariate = tea_tasting.utils.check_scalar(
             numer_covariate, "numer_covariate", typ=str | None)
         self.denom_covariate = tea_tasting.utils.check_scalar(
             denom_covariate, "denom_covariate", typ=str | None)
         self.alternative = (
@@ -111,15 +146,15 @@
             if use_t is not None
             else tea_tasting.config.get_config("use_t")
         )
 
 
     @property
     def aggr_cols(self) -> AggrCols:
-        """Columns to aggregate for a metric analysis."""
+        """Columns to be aggregated for a metric analysis."""
         cols = tuple(
             col for col in (
                 self.numer,
                 self.denom,
                 self.numer_covariate,
                 self.denom_covariate,
             )
@@ -138,16 +173,16 @@
         )
 
 
     def analyze_aggregates(
         self,
         control: tea_tasting.aggr.Aggregates,
         treatment: tea_tasting.aggr.Aggregates,
-    ) -> MeansResult:
-        """Analyze metric in an experiment using aggregated statistics.
+    ) -> MeanResult:
+        """Analyze a metric in an experiment using aggregated statistics.
 
         Args:
             control: Control data.
             treatment: Treatment data.
 
         Returns:
             Analysis result.
@@ -214,15 +249,15 @@
         self,
         contr_mean: float,
         contr_var: float,
         contr_count: int,
         treat_mean: float,
         treat_var: float,
         treat_count: int,
-    ) -> MeansResult:
+    ) -> MeanResult:
         scale, distr = self._scale_and_distr(
             contr_var=contr_var,
             contr_count=contr_count,
             treat_var=treat_var,
             treat_count=treat_count,
         )
         log_scale, log_distr = self._scale_and_distr(
@@ -256,15 +291,15 @@
 
             rel_half_ci = math.exp(log_scale * log_distr.ppf(q))
             means_ratio_ci_lower = means_ratio / rel_half_ci
             means_ratio_ci_upper = means_ratio * rel_half_ci
 
             pvalue = 2 * distr.sf(abs(statistic))
 
-        return MeansResult(
+        return MeanResult(
             control=contr_mean,
             treatment=treat_mean,
             effect_size=effect_size,
             effect_size_ci_lower=effect_size_ci_lower,
             effect_size_ci_upper=effect_size_ci_upper,
             rel_effect_size=means_ratio - 1,
             rel_effect_size_ci_lower=means_ratio_ci_lower - 1,
@@ -302,44 +337,82 @@
             distr = scipy.stats.t(df=df)
         else:
             distr = scipy.stats.norm()
 
         return scale, distr
 
 
-class Mean(RatioOfMeans):
-    """Value mean."""
+class Mean(RatioOfMeans):  # noqa: D101
     def __init__(
         self,
         value: str,
         covariate: str | None = None,
         *,
         alternative: Literal["two-sided", "greater", "less"] | None = None,
         confidence_level: float | None = None,
         equal_var: bool | None = None,
         use_t: bool | None = None,
     ) -> None:
-        """Value mean.
+        """Metric for the analysis of means.
 
         Args:
             value: Metric value column name.
             covariate: Metric covariate column name.
-            alternative: Alternative hypothesis. Options:
-                "two-sided": the means are unequal.
-                "greater": the mean in the treatment variant is greater than the mean
-                    in the control variant.
-                "less": the mean in the treatment variant is less than the mean
-                    in the control variant.
+            alternative: Alternative hypothesis.
             confidence_level: Confidence level for the confidence interval.
-            equal_var: Defines whether equal variance is assumed. If True,
+            equal_var: Defines whether equal variance is assumed. If `True`,
                 pooled variance is used for the calculation of the standard error
                 of the difference between two means.
-            use_t: Defines whether to use the Student's t-distribution (True) or
-                the Normal distribution (False).
-        """
+            use_t: Defines whether to use the Student's t-distribution (`True`) or
+                the Normal distribution (`False`).
+
+        Alternative hypothesis options:
+            - `"two-sided"`: the means are unequal,
+            - `"greater"`: the mean in the treatment variant is greater than the mean
+                in the control variant,
+            - `"less"`: the mean in the treatment variant is less than the mean
+                in the control variant.
+
+        Examples:
+            ```python
+            import tea_tasting as tt
+
+
+            experiment = tt.Experiment(
+                orders_per_user=tt.Mean("orders"),
+                revenue_per_user=tt.Mean("revenue"),
+            )
+
+            data = tt.make_users_data(seed=42)
+            result = experiment.analyze(data)
+            print(result)
+            #>           metric control treatment rel_effect_size rel_effect_size_ci pvalue
+            #>  orders_per_user   0.530     0.573            8.0%       [-2.0%, 19%]  0.118
+            #> revenue_per_user    5.24      5.73            9.3%       [-2.4%, 22%]  0.123
+            ```
+
+            With CUPED:
+
+            ```python
+            import tea_tasting as tt
+
+
+            experiment = tt.Experiment(
+                orders_per_user=tt.Mean("orders", "orders_covariate"),
+                revenue_per_user=tt.Mean("revenue", "revenue_covariate"),
+            )
+
+            data = tt.make_users_data(seed=42, covariates=True)
+            result = experiment.analyze(data)
+            print(result)
+            #>           metric control treatment rel_effect_size rel_effect_size_ci  pvalue
+            #>  orders_per_user   0.523     0.581             11%        [2.9%, 20%] 0.00733
+            #> revenue_per_user    5.12      5.85             14%        [3.8%, 26%] 0.00675
+            ```
+        """  # noqa: E501
         super().__init__(
             numer=value,
             denom=None,
             numer_covariate=covariate,
             denom_covariate=None,
             alternative=alternative,
             confidence_level=confidence_level,
```

### Comparing `tea_tasting-0.0.3/src/tea_tasting/metrics/proportion.py` & `tea_tasting-0.0.4/src/tea_tasting/metrics/proportion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Analysis of proportions."""
+"""Metrics for the analysis of proportions."""
 
 from __future__ import annotations
 
 import math
 from typing import TYPE_CHECKING, NamedTuple
 
 import scipy.stats
@@ -33,64 +33,97 @@
         pvalue: P-value
     """
     control: float
     treatment: float
     pvalue: float
 
 
-class SampleRatio(MetricBaseAggregated[SampleRatioResult]):
-    """Sample ratio mismatch check."""
-
+class SampleRatio(MetricBaseAggregated[SampleRatioResult]):  # noqa: D101
     def __init__(
         self,
         ratio: float | int | dict[Any, float | int] = 1,
         *,
         method: Literal["auto", "binom", "norm"] = "auto",
         correction: bool = True,
     ) -> None:
-        """Sample ratio mismatch check.
+        """Metric for sample ratio mismatch check.
 
         Args:
-            ratio: Expected ratio of the number of observation in treatment
-                relative to control.
-            method: Statistical test used for calculation of p-value. Options:
-                "auto": Apply exact binomial test if the total number of observations
-                    is < 1000, or normal approximation otherwise.
-                "binom": Apply exact binomial test.
-                "norm": Apply normal approximation of the binomial distribution.
-            correction: If True, add continuity correction.
+            ratio: Expected ratio of the number of observations in the treatment
+                relative to the control.
+            method: Statistical test used for calculation of p-value.
+            correction: If `True`, add continuity correction.
                 Only for normal approximation.
+
+        Method options:
+            - `"auto"`: Apply exact binomial test if the total number of observations
+                is < 1000; or normal approximation otherwise.
+            - `"binom"`: Apply exact binomial test.
+            - `"norm"`: Apply normal approximation of the binomial distribution.
+
+        Examples:
+            ```python
+            import tea_tasting as tt
+
+
+            experiment = tt.Experiment(
+                sample_ratio=tt.SampleRatio(),
+            )
+
+            data = tt.make_users_data(seed=42)
+            result = experiment.analyze(data)
+            print(result.to_string(("control", "treatment", "pvalue")))
+            #>       metric control treatment pvalue
+            #> sample_ratio    2023      1977  0.477
+            ```
+
+            Different expected ratio:
+
+            ```python
+            import tea_tasting as tt
+
+
+            experiment = tt.Experiment(
+                sample_ratio=tt.SampleRatio(0.5),
+            )
+
+            data = tt.make_users_data(seed=42)
+            result = experiment.analyze(data)
+            print(result.to_string(("control", "treatment", "pvalue")))
+            #>       metric control treatment    pvalue
+            #> sample_ratio    2023      1977 3.26e-103
+            ```
         """
         if isinstance(ratio, dict):
             for val in ratio.values():
                 tea_tasting.utils.auto_check(val, "ratio")
         else:
             tea_tasting.utils.auto_check(ratio, "ratio")
         self.ratio = ratio
 
         self.method = tea_tasting.utils.check_scalar(
-            method, "method", typ=str, is_in={"auto", "binom", "norm"})
+            method, "method", typ=str, in_={"auto", "binom", "norm"})
         self.correction = tea_tasting.utils.auto_check(correction, "correction")
 
 
     @property
     def aggr_cols(self) -> AggrCols:
-        """Columns to aggregate for a metric analysis."""
+        """Columns to be aggregated for a metric analysis."""
         return AggrCols(has_count=True)
 
 
     def analyze(
         self,
         data: pd.DataFrame | ibis.expr.types.Table | dict[
             Any, tea_tasting.aggr.Aggregates],
         control: Any,
         treatment: Any,
         variant: str | None = None,
     ) -> SampleRatioResult:
-        """Perform sample ratio mismatch check.
+        """Perform a sample ratio mismatch check.
 
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
@@ -133,9 +166,9 @@
 
 
     def analyze_aggregates(
         self,
         control: tea_tasting.aggr.Aggregates,
         treatment: tea_tasting.aggr.Aggregates,
     ) -> SampleRatioResult:
-        """Method stub for compatibility with the base class."""
+        """Stub method for compatibility with the base class."""
         raise NotImplementedError
```

### Comparing `tea_tasting-0.0.3/tests/metrics/test_base.py` & `tea_tasting-0.0.4/tests/metrics/test_base.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/tests/metrics/test_mean.py` & `tea_tasting-0.0.4/tests/metrics/test_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,28 +110,28 @@
 
 def test_ratio_of_means_analyze_table(table: ibis.expr.types.Table):
     metric = tea_tasting.metrics.mean.RatioOfMeans(
         numer="orders",
         numer_covariate="orders_covariate",
     )
     result = metric.analyze(table, 0, 1, variant="variant")
-    assert isinstance(result, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(result, tea_tasting.metrics.mean.MeanResult)
 
 def test_ratio_of_means_analyze_df(dataframe: pd.DataFrame):
     metric = tea_tasting.metrics.mean.RatioOfMeans(
         numer="orders",
         denom="sessions",
     )
     result = metric.analyze(dataframe, 0, 1, variant="variant")
-    assert isinstance(result, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(result, tea_tasting.metrics.mean.MeanResult)
 
 def test_ratio_of_means_analyze_basic(data: dict[str, tea_tasting.aggr.Aggregates]):
     metric = tea_tasting.metrics.mean.RatioOfMeans(numer="orders")
     result = metric.analyze(data, 0, 1)
-    assert isinstance(result, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(result, tea_tasting.metrics.mean.MeanResult)
     assert result.control == pytest.approx(0.5660377358490566)
     assert result.treatment == pytest.approx(0.3829787234042553)
     assert result.effect_size == pytest.approx(-0.18305901244480127)
     assert result.effect_size_ci_lower == pytest.approx(-0.5004359360326984)
     assert result.effect_size_ci_upper == pytest.approx(0.13431791114309583)
     assert result.rel_effect_size == pytest.approx(-0.32340425531914896)
     assert result.rel_effect_size_ci_lower == pytest.approx(-0.6593351111187646)
@@ -145,15 +145,15 @@
     metric = tea_tasting.metrics.mean.RatioOfMeans(
         numer="orders",
         denom="sessions",
         alternative="greater",
         equal_var=True,
     )
     result = metric.analyze(data, 0, 1)
-    assert isinstance(result, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(result, tea_tasting.metrics.mean.MeanResult)
     assert result.control == pytest.approx(0.2857142857142857)
     assert result.treatment == pytest.approx(0.20224719101123595)
     assert result.effect_size == pytest.approx(-0.08346709470304975)
     assert result.effect_size_ci_lower == pytest.approx(-0.21187246704082818)
     assert result.effect_size_ci_upper == float("inf")
     assert result.rel_effect_size == pytest.approx(-0.2921348314606741)
     assert result.rel_effect_size_ci_lower == pytest.approx(-0.5852384654309937)
@@ -169,15 +169,15 @@
         denom="sessions",
         numer_covariate="orders_covariate",
         denom_covariate="sessions_covariate",
         alternative="less",
         use_t=False,
     )
     result = metric.analyze(data, 0, 1)
-    assert isinstance(result, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(result, tea_tasting.metrics.mean.MeanResult)
     assert result.control == pytest.approx(0.25572348175909004)
     assert result.treatment == pytest.approx(0.23549786496156158)
     assert result.effect_size == pytest.approx(-0.020225616797528462)
     assert result.effect_size_ci_lower == float("-inf")
     assert result.effect_size_ci_upper == pytest.approx(0.07287939184944564)
     assert result.rel_effect_size == pytest.approx(-0.07909174651619377)
     assert result.rel_effect_size_ci_lower == float("-inf")
@@ -203,19 +203,19 @@
         equal_var=True,
         use_t=False,
     )
     _compare_results(metric.analyze(data, 0, 1), ratio_metric.analyze(data, 0, 1))
 
 
 def _compare_results(
-    left: tea_tasting.metrics.mean.MeansResult,
-    right: tea_tasting.metrics.mean.MeansResult,
+    left: tea_tasting.metrics.mean.MeanResult,
+    right: tea_tasting.metrics.mean.MeanResult,
 ) -> None:
-    assert isinstance(left, tea_tasting.metrics.mean.MeansResult)
-    assert isinstance(right, tea_tasting.metrics.mean.MeansResult)
+    assert isinstance(left, tea_tasting.metrics.mean.MeanResult)
+    assert isinstance(right, tea_tasting.metrics.mean.MeanResult)
     assert left.control == pytest.approx(right.control)
     assert left.treatment == pytest.approx(right.treatment)
     assert left.effect_size == pytest.approx(right.effect_size)
     assert left.effect_size_ci_lower == pytest.approx(right.effect_size_ci_lower)
     assert left.effect_size_ci_upper == pytest.approx(right.effect_size_ci_upper)
     assert left.rel_effect_size == pytest.approx(right.rel_effect_size)
     assert left.rel_effect_size_ci_lower == pytest.approx(
```

### Comparing `tea_tasting-0.0.3/tests/metrics/test_proportion.py` & `tea_tasting-0.0.4/tests/metrics/test_proportion.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/tests/test_aggr.py` & `tea_tasting-0.0.4/tests/test_aggr.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/tests/test_config.py` & `tea_tasting-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/tests/test_datasets.py` & `tea_tasting-0.0.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/tests/test_experiment.py` & `tea_tasting-0.0.4/tests/test_experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -128,14 +128,42 @@
         tea_tasting.experiment.ExperimentResult,
     ],
 ) -> tea_tasting.experiment.ExperimentResult:
     return get_result((10, 11, 1), (20, 22, 2))
 
 
 @pytest.fixture
+def result2() -> tea_tasting.experiment.ExperimentResult:
+    class MetricResultTuple(NamedTuple):
+        control: float
+        treatment: float
+        rel_effect_size: float
+        rel_effect_size_ci_lower: float
+        rel_effect_size_ci_upper: float
+        pvalue: float
+
+    return tea_tasting.experiment.ExperimentResult(
+        metric_tuple=MetricResultTuple(
+            control=4.4444,
+            treatment=5.5555,
+            rel_effect_size=0.2,
+            rel_effect_size_ci_lower=0.12345,
+            rel_effect_size_ci_upper=float("inf"),
+            pvalue=0.23456,
+        ),
+        metric_dict={
+            "control": 9.9999,
+            "treatment": 11.111,
+            "rel_effect_size": 0.11111,
+            "rel_effect_size_ci_lower": 0,
+        },
+    )
+
+
+@pytest.fixture
 def results(
     result: tea_tasting.experiment.ExperimentResult,
 ) -> tea_tasting.experiment.ExperimentResults:
     return tea_tasting.experiment.ExperimentResults({(0, 1): result})
 
 
 @pytest.fixture
@@ -185,14 +213,122 @@
             "control": (10, 20),
             "treatment": (11, 22),
             "effect_size": (1, 2),
         }),
     )
 
 
+def test_experiment_result_to_pretty(result2: tea_tasting.experiment.ExperimentResult):
+    pd.testing.assert_frame_equal(
+        result2.to_pretty(),
+        pd.DataFrame((
+            {
+                "metric": "metric_tuple",
+                "control": "4.44",
+                "treatment": "5.56",
+                "rel_effect_size": "20%",
+                "rel_effect_size_ci": "[12%, ∞]",
+                "pvalue": "0.235",
+            },
+            {
+                "metric": "metric_dict",
+                "control": "10.0",
+                "treatment": "11.1",
+                "rel_effect_size": "11%",
+                "rel_effect_size_ci": "[0.0%, -]",
+                "pvalue": "-",
+            },
+        )),
+    )
+
+
+def test_experiment_result_to_string(result2: tea_tasting.experiment.ExperimentResult):
+    assert result2.to_string() == pd.DataFrame((
+        {
+            "metric": "metric_tuple",
+            "control": "4.44",
+            "treatment": "5.56",
+            "rel_effect_size": "20%",
+            "rel_effect_size_ci": "[12%, ∞]",
+            "pvalue": "0.235",
+        },
+        {
+            "metric": "metric_dict",
+            "control": "10.0",
+            "treatment": "11.1",
+            "rel_effect_size": "11%",
+            "rel_effect_size_ci": "[0.0%, -]",
+            "pvalue": "-",
+        },
+    )).to_string(index=False)
+
+
+def test_experiment_result_str(result2: tea_tasting.experiment.ExperimentResult):
+    assert str(result2) == pd.DataFrame((
+        {
+            "metric": "metric_tuple",
+            "control": "4.44",
+            "treatment": "5.56",
+            "rel_effect_size": "20%",
+            "rel_effect_size_ci": "[12%, ∞]",
+            "pvalue": "0.235",
+        },
+        {
+            "metric": "metric_dict",
+            "control": "10.0",
+            "treatment": "11.1",
+            "rel_effect_size": "11%",
+            "rel_effect_size_ci": "[0.0%, -]",
+            "pvalue": "-",
+        },
+    )).to_string(index=False)
+
+
+def test_experiment_result_to_html(result2: tea_tasting.experiment.ExperimentResult):
+    assert result2.to_html() == pd.DataFrame((
+        {
+            "metric": "metric_tuple",
+            "control": "4.44",
+            "treatment": "5.56",
+            "rel_effect_size": "20%",
+            "rel_effect_size_ci": "[12%, ∞]",
+            "pvalue": "0.235",
+        },
+        {
+            "metric": "metric_dict",
+            "control": "10.0",
+            "treatment": "11.1",
+            "rel_effect_size": "11%",
+            "rel_effect_size_ci": "[0.0%, -]",
+            "pvalue": "-",
+        },
+    )).to_html(index=False)
+
+
+def test_experiment_result_repr_html(result2: tea_tasting.experiment.ExperimentResult):
+    assert result2._repr_html_() == pd.DataFrame((
+        {
+            "metric": "metric_tuple",
+            "control": "4.44",
+            "treatment": "5.56",
+            "rel_effect_size": "20%",
+            "rel_effect_size_ci": "[12%, ∞]",
+            "pvalue": "0.235",
+        },
+        {
+            "metric": "metric_dict",
+            "control": "10.0",
+            "treatment": "11.1",
+            "rel_effect_size": "11%",
+            "rel_effect_size_ci": "[0.0%, -]",
+            "pvalue": "-",
+        },
+    )).to_html(index=False)
+
+
 def test_experiment_init_default():
     metrics = {
         "avg_sessions": _Metric("sessions"),
         "avg_orders": _MetricAggregated("orders"),
         "avg_revenue": _MetricGranular("revenue"),
     }
     experiment = tea_tasting.experiment.Experiment(metrics)  # type: ignore
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tea_tasting-0.0.3/tests/test_utils.py` & `tea_tasting-0.0.4/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
 def test_check_scalar_lt():
     assert tea_tasting.utils.check_scalar(1, lt=2) == 1
     with pytest.raises(ValueError, match="must be <"):
         tea_tasting.utils.check_scalar(1, lt=1)
 
 def test_check_scalar_is_in():
-    assert tea_tasting.utils.check_scalar(1, is_in={0, 1}) == 1
+    assert tea_tasting.utils.check_scalar(1, in_={0, 1}) == 1
     with pytest.raises(ValueError, match="must be in"):
-        tea_tasting.utils.check_scalar(1, is_in={0, 2})
+        tea_tasting.utils.check_scalar(1, in_={0, 2})
 
 
 def test_auto_check_alternative():
     assert tea_tasting.utils.auto_check("two-sided", "alternative") == "two-sided"
     with pytest.raises(TypeError):
         tea_tasting.utils.auto_check(2, "alternative")
     with pytest.raises(ValueError, match="must be in"):
@@ -73,14 +73,30 @@
 
 def test_auto_check_use_t():
     assert tea_tasting.utils.auto_check(False, "use_t") is False
     with pytest.raises(TypeError):
         tea_tasting.utils.auto_check(0, "use_t")
 
 
+def test_format_num():
+    assert tea_tasting.utils.format_num(1.2345) == "1.23"
+    assert tea_tasting.utils.format_num(0.9999) == "1.00"
+    assert tea_tasting.utils.format_num(1.2345, sig=2) == "1.2"
+    assert tea_tasting.utils.format_num(0.12345, pct=True) == "12.3%"
+    assert tea_tasting.utils.format_num(None) == "-"
+    assert tea_tasting.utils.format_num(float("nan")) == "-"
+    assert tea_tasting.utils.format_num(float("inf")) == "∞"
+    assert tea_tasting.utils.format_num(float("-inf")) == "-∞"
+    assert tea_tasting.utils.format_num(0.00012345) == "1.23e-04"
+    assert tea_tasting.utils.format_num(0.00099999) == "1.00e-03"
+    assert tea_tasting.utils.format_num(12345, thousands_sep=" ") == "12 345"
+    assert tea_tasting.utils.format_num(1.2345, decimal_point=",") == "1,23"
+    assert tea_tasting.utils.format_num(0) == "0.00"
+
+
 def test_div():
     assert tea_tasting.utils.div(1, 2) == 0.5
     assert tea_tasting.utils.div(1, 0, 3) == 3
     assert math.isnan(tea_tasting.utils.div(0, 0))
     assert tea_tasting.utils.div(1, 0) == float("inf")
     assert tea_tasting.utils.div(-1, 0) == float("-inf")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tea_tasting-0.0.3/tests/test_version.py` & `tea_tasting-0.0.4/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.3/PKG-INFO` & `tea_tasting-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tea-tasting
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for statistical analysis of A/B tests.
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Typing :: Typed
 Project-URL: Source, https://github.com/e10v/tea-tasting
 Requires-Python: >=3.10
-Requires-Dist: ibis-framework[pandas]<9,>=7
-Requires-Dist: numpy<2,>=1.25
+Requires-Dist: ibis-framework[pandas]<10,>=7
+Requires-Dist: numpy<3,>=1.25
 Requires-Dist: pandas<3,>=2
 Requires-Dist: scipy<2,>=1.10
 Description-Content-Type: text/markdown
 
 # tea-tasting: statistical analysis of A/B tests
 
 [![CI](https://github.com/e10v/tea-tasting/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/e10v/tea-tasting/actions/workflows/ci.yml)
@@ -47,18 +47,18 @@
 - Sample ratio mismatch check.
 
 **tea-tasting** calculates statistics within data backends such as BigQuery, ClickHouse, PostgreSQL, Snowflake, Spark, and other of 20+ backends supported by [Ibis](https://ibis-project.org/). This approach eliminates the need to import granular data into a Python environment, though Pandas DataFrames are also supported.
 
 **tea-tasting** is still in alpha, but already includes all the features listed above. The following features are coming soon:
 
 - More statistical tests:
-  - Bootstrap.
-  - Quantile test (using Bootstrap).
-  - Asymptotic and exact tests for frequency data.
-  - Mann–Whitney U test.
+    - Bootstrap.
+    - Quantile test (using Bootstrap).
+    - Asymptotic and exact tests for frequency data.
+    - Mann–Whitney U test.
 - Power analysis.
 - A/A tests and simulations.
 - Pretty output for experiment results (round etc.).
 - More documentation and examples.
 
 ## Installation
 
@@ -139,17 +139,17 @@
 Use the `Mean` class to compare averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
 
 Use the `RatioOfMeans` class to compare ratios of averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
 
 Use the following parameters of `Mean` and `RatioOfMeans` to customize the analysis:
 
 - `alternative`: Alternative hypothesis. The following options are available:
-  - `"two-sided"` (default): the means are unequal.
-  - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
-  - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
+    - `"two-sided"` (default): the means are unequal.
+    - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
+    - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
 - `confidence_level`: Confidence level of the confidence interval. Default is `0.95`.
 - `equal_var`: Defines whether equal variance is assumed. If `True`, pooled variance is used for the calculation of the standard error of the difference between two means. Default is `False`.
 - `use_t`: Defines whether to use the Student's t-distribution (`True`) or the Normal distribution (`False`). Default is `True`.
 
 Example usage:
 
 ```python
```

