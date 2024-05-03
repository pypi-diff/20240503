# Comparing `tmp/linopy-0.3.8.tar.gz` & `tmp/linopy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linopy-0.3.8.tar", last modified: Mon Mar 11 09:57:55 2024, max compression
+gzip compressed data, was "linopy-0.3.9.tar", last modified: Fri May  3 15:23:37 2024, max compression
```

## Comparing `linopy-0.3.8.tar` & `linopy-0.3.9.tar`

### file list

```diff
@@ -1,162 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.365292 linopy-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)   180224 2024-03-11 09:57:51.000000 linopy-0.3.8/.coverage
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-11 09:57:51.000000 linopy-0.3.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.337292 linopy-0.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.341292 linopy-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-11 09:57:51.000000 linopy-0.3.8/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-11 09:57:51.000000 linopy-0.3.8/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-11 09:57:51.000000 linopy-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-11 09:57:51.000000 linopy-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-11 09:57:51.000000 linopy-0.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-11 09:57:51.000000 linopy-0.3.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-11 09:57:51.000000 linopy-0.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-03-11 09:57:55.365292 linopy-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-11 09:57:51.000000 linopy-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.341292 linopy-0.3.8/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   188981 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark-absolute.png
--rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   179946 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark-overhead.png
--rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark_resource-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   149975 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark_resource-absolute.png
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark_resource-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   132957 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/benchmark_resource-overhead.png
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/environment.fixed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.341292 linopy-0.3.8/benchmark/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/notebooks/plot-benchmarks.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.345292 linopy-0.3.8/benchmark/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1450 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1537 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_jump.jl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1456 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2043 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmark_pyomo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.345292 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1050 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/concat-benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.345292 linopy-0.3.8/benchmark/scripts/leftovers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmark-linopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.349292 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.349292 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (127)   103087 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (127)    26681 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    18332 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (127)   381819 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/leftovers/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/merge-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      399 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      287 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      399 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/run-pyomo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1023 2024-03-11 09:57:51.000000 linopy-0.3.8/benchmark/scripts/write-lp-file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.353292 linopy-0.3.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.353292 linopy-0.3.8/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    57997 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/benchmark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/create-a-model-with-coordinates.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/create-a-model.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/creating-constraints.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/creating-expressions.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/creating-variables.nblink
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/gurobi-double-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/infeasible-model.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    49959 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/manipulating-models.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/migrating-from-pyomo.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/solve-on-remote.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/syntax.rst
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/testing-framework.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/transport-tutorial.nblink
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-11 09:57:51.000000 linopy-0.3.8/doc/user-guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.357292 linopy-0.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/create-a-model-with-coordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/create-a-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/creating-constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/creating-expressions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/creating-variables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/infeasible-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/manipulating-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/migrating-from-pyomo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/solve-on-remote.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/testing-framework.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18181 2024-03-11 09:57:51.000000 linopy-0.3.8/examples/transport-tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.357292 linopy-0.3.8/linopy/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    56248 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23197 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    39351 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/monkey_patch_xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    39273 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    37594 2024-03-11 09:57:51.000000 linopy-0.3.8/linopy/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.361292 linopy-0.3.8/linopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 09:57:55.000000 linopy-0.3.8/linopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-11 09:57:51.000000 linopy-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 09:57:55.365292 linopy-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-11 09:57:51.000000 linopy-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:57:55.361292 linopy-0.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_inconsistency_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    19789 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_quadratic_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_scalar_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_scalar_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_variable_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-11 09:57:51.000000 linopy-0.3.8/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.240109 linopy-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)   180224 2024-05-03 15:23:32.000000 linopy-0.3.9/.coverage
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 15:23:32.000000 linopy-0.3.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.212109 linopy-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.216109 linopy-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-03 15:23:32.000000 linopy-0.3.9/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 15:23:32.000000 linopy-0.3.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-03 15:23:32.000000 linopy-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-03 15:23:32.000000 linopy-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 15:23:32.000000 linopy-0.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-03 15:23:32.000000 linopy-0.3.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 15:23:32.000000 linopy-0.3.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-03 15:23:37.240109 linopy-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-03 15:23:32.000000 linopy-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.220109 linopy-0.3.9/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   188981 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   179946 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark_resource-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   149975 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark_resource-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark_resource-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   132957 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/benchmark_resource-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/environment.fixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.220109 linopy-0.3.9/benchmark/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/notebooks/plot-benchmarks.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.220109 linopy-0.3.9/benchmark/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1450 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1537 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_jump.jl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1456 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1965 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2043 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmark_pyomo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.220109 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1050 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/concat-benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.224109 linopy-0.3.9/benchmark/scripts/leftovers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmark-linopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.224109 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.224109 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103087 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26681 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    18332 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   381819 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/leftovers/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/merge-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      399 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      287 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      399 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/run-pyomo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1023 2024-05-03 15:23:32.000000 linopy-0.3.9/benchmark/scripts/write-lp-file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.228109 linopy-0.3.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.228109 linopy-0.3.9/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    57997 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/benchmark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/create-a-model-with-coordinates.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/create-a-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/creating-constraints.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/creating-expressions.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/creating-variables.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/gurobi-double-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/infeasible-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    49959 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/manipulating-models.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/migrating-from-pyomo.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30300 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/solve-on-remote.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/syntax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/testing-framework.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/transport-tutorial.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-03 15:23:32.000000 linopy-0.3.9/doc/user-guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.232109 linopy-0.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/create-a-model-with-coordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/create-a-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/creating-constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10887 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/creating-expressions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/creating-variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/infeasible-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/manipulating-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/migrating-from-pyomo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/solve-on-remote.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/testing-framework.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-05-03 15:23:32.000000 linopy-0.3.9/examples/transport-tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.236109 linopy-0.3.9/linopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56807 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39426 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/monkey_patch_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40058 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39465 2024-05-03 15:23:32.000000 linopy-0.3.9/linopy/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.236109 linopy-0.3.9/linopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 15:23:37.000000 linopy-0.3.9/linopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-03 15:23:32.000000 linopy-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:23:37.240109 linopy-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:23:37.236109 linopy-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13147 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_inconsistency_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23456 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_quadratic_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_scalar_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_scalar_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_variable_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-03 15:23:32.000000 linopy-0.3.9/test/test_variables.py
```

### Comparing `linopy-0.3.8/.coverage` & `linopy-0.3.9/.coverage`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/.github/workflows/CI.yaml` & `linopy-0.3.9/.github/workflows/CI.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     strategy:
       fail-fast: false
       matrix:
         python-version:
         - 3.9
         - "3.10"
         - "3.11"
-        # - "3.12"
+        - "3.12"
         os:
         - ubuntu-latest
         - macos-latest
         - windows-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
@@ -51,15 +51,14 @@
     - name: Install windows dependencies
       if: matrix.os == 'windows-latest'
       run: |
         choco install glpk
 
     - name: Install dependencies for python ${{ matrix.python-version }}
       run: |
-        python -m pip install --upgrade pip
         pip install -e .[dev,solvers]
 
     - name: Lint with flake8
       run: |
         pip install flake8
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics --exclude=benchmark/scripts
```

### Comparing `linopy-0.3.8/.github/workflows/deploy.yml` & `linopy-0.3.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/.pre-commit-config.yaml` & `linopy-0.3.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
     -   id: check-merge-conflict
 -   repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.4.2
     hooks:
     -   id: black
     # Current docformatter version has a problem with urls (it's annoying)
 # -   repo: https://github.com/PyCQA/docformatter
 #     rev: v1.6.0.rc1
 #     hooks:
 #     -   id: docformatter
```

### Comparing `linopy-0.3.8/LICENSE.txt` & `linopy-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/PKG-INFO` & `linopy-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Linear optimization with N-D labeled arrays in Python
-Home-page: https://github.com/PyPSA/linopy
-Author: Fabian Hofmann
-Author-email: hofmann@fias.uni-frankfurt.de
-License: MIT
+Author-email: Fabian Hofmann <fabianmarikhofmann@gmail.com>
+Project-URL: Homepage, https://github.com/PyPSA/linopy
+Project-URL: Source, https://github.com/PyPSA/linopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -41,18 +40,19 @@
 Requires-Dist: netcdf4; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: paramiko; extra == "dev"
 Requires-Dist: gurobipy; extra == "dev"
 Requires-Dist: highspy; extra == "dev"
 Provides-Extra: solvers
 Requires-Dist: gurobipy; extra == "solvers"
-Requires-Dist: highspy; extra == "solvers"
-Requires-Dist: cplex; extra == "solvers"
+Requires-Dist: highspy>=1.5.0; python_version < "3.12" and extra == "solvers"
+Requires-Dist: highspy>=1.7.1.dev1; python_version >= "3.12" and extra == "solvers"
+Requires-Dist: cplex; (platform_system != "Darwin" and python_version < "3.12") and extra == "solvers"
 Requires-Dist: mosek; extra == "solvers"
-Requires-Dist: mindoptpy; extra == "solvers"
+Requires-Dist: mindoptpy; python_version < "3.12" and extra == "solvers"
 Requires-Dist: coptpy; extra == "solvers"
 Requires-Dist: xpress; (platform_system != "Darwin" and python_version < "3.11") and extra == "solvers"
 Requires-Dist: pyscipopt; platform_system != "Darwin" and extra == "solvers"
 
 # linopy: Optimization with array-like variables and constraints
 
 [![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License](https://img.shields.io/pypi/l/linopy.svg)](LICENSE.txt) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
@@ -60,15 +60,15 @@
 **linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Benchmarks
 
 **linopy** is designed to be fast and efficient. The following benchmark compares the performance of **linopy** with the alternative popular optimization packages.
 
-![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTAxNTAzMDYsIm5iZiI6MTcxMDE1MDAwNiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMzExVDA5NDAwNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBlNzU4NTYxOTQ2ZjdmYmFiMjBjMGNkNTIzYjk5NzhmMWYzODRhMzE2YzAwMDEzMTc5ZWJlNmE1MzMzMTRmNzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.pVhJRAuZJB982o5h85zCFp8aQixW9wl3Bo3bemf0MlU)
+![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQ3NDY1NzYsIm5iZiI6MTcxNDc0NjI3NiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA1MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNTAzVDE0MjQzNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ3M2Q5MTMxY2EzNTI4OTUzNDViMzUzZTkyOGQ0MzliYTYxNjc2ODdhNDFjODRiNmE4OGIwNWI0MWZlNDZmMWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.WFHwXmalW05hSm0oxWGmAEnVvcdFyCvQMxDJB7v3yBk)
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) continuous or binary variables with **coordinates**, e.g. time, consumers, etc.
```

### Comparing `linopy-0.3.8/README.md` & `linopy-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 **linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Benchmarks
 
 **linopy** is designed to be fast and efficient. The following benchmark compares the performance of **linopy** with the alternative popular optimization packages.
 
-![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTAxNTAzMDYsIm5iZiI6MTcxMDE1MDAwNiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMzExVDA5NDAwNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBlNzU4NTYxOTQ2ZjdmYmFiMjBjMGNkNTIzYjk5NzhmMWYzODRhMzE2YzAwMDEzMTc5ZWJlNmE1MzMzMTRmNzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.pVhJRAuZJB982o5h85zCFp8aQixW9wl3Bo3bemf0MlU)
+![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQ3NDY1NzYsIm5iZiI6MTcxNDc0NjI3NiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA1MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNTAzVDE0MjQzNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ3M2Q5MTMxY2EzNTI4OTUzNDViMzUzZTkyOGQ0MzliYTYxNjc2ODdhNDFjODRiNmE4OGIwNWI0MWZlNDZmMWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.WFHwXmalW05hSm0oxWGmAEnVvcdFyCvQMxDJB7v3yBk)
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) continuous or binary variables with **coordinates**, e.g. time, consumers, etc.
```

### Comparing `linopy-0.3.8/benchmark/README.md` & `linopy-0.3.9/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/Snakefile` & `linopy-0.3.9/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark-absolute.pdf` & `linopy-0.3.9/benchmark/benchmark-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark-absolute.png` & `linopy-0.3.9/benchmark/benchmark-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark-overhead.pdf` & `linopy-0.3.9/benchmark/benchmark-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark-overhead.png` & `linopy-0.3.9/benchmark/benchmark-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark_resource-absolute.pdf` & `linopy-0.3.9/benchmark/benchmark_resource-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark_resource-absolute.png` & `linopy-0.3.9/benchmark/benchmark_resource-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark_resource-overhead.pdf` & `linopy-0.3.9/benchmark/benchmark_resource-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/benchmark_resource-overhead.png` & `linopy-0.3.9/benchmark/benchmark_resource-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/environment.fixed.yaml` & `linopy-0.3.9/benchmark/environment.fixed.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/notebooks/plot-benchmarks.py.ipynb` & `linopy-0.3.9/benchmark/notebooks/plot-benchmarks.py.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_cvxpy.py` & `linopy-0.3.9/benchmark/scripts/benchmark_cvxpy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_gurobipy.py` & `linopy-0.3.9/benchmark/scripts/benchmark_gurobipy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_jump.jl` & `linopy-0.3.9/benchmark/scripts/benchmark_jump.jl`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_linopy.py` & `linopy-0.3.9/benchmark/scripts/benchmark_linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_ortools.py` & `linopy-0.3.9/benchmark/scripts/benchmark_ortools.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_pulp.py` & `linopy-0.3.9/benchmark/scripts/benchmark_pulp.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmark_pyomo.py` & `linopy-0.3.9/benchmark/scripts/benchmark_pyomo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.3.9/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/concat-benchmarks.py` & `linopy-0.3.9/benchmark/scripts/concat-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmark-linopy.py` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmark-linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.3.9/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/leftovers/common.py` & `linopy-0.3.9/benchmark/scripts/leftovers/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/merge-benchmarks.py` & `linopy-0.3.9/benchmark/scripts/merge-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/plot-benchmarks.py` & `linopy-0.3.9/benchmark/scripts/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/benchmark/scripts/write-lp-file.py` & `linopy-0.3.9/benchmark/scripts/write-lp-file.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/Makefile` & `linopy-0.3.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/_static/theme_overrides.css` & `linopy-0.3.9/doc/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/api.rst` & `linopy-0.3.9/doc/api.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/benchmark.png` & `linopy-0.3.9/doc/benchmark.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/benchmark.rst` & `linopy-0.3.9/doc/benchmark.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/conf.py` & `linopy-0.3.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/contributing.rst` & `linopy-0.3.9/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/gurobi-double-logging.rst` & `linopy-0.3.9/doc/gurobi-double-logging.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/index.rst` & `linopy-0.3.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/logo.pdf` & `linopy-0.3.9/doc/logo.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/logo.png` & `linopy-0.3.9/doc/logo.png`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/logo.py` & `linopy-0.3.9/doc/logo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/make.bat` & `linopy-0.3.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/prerequisites.rst` & `linopy-0.3.9/doc/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/doc/release_notes.rst` & `linopy-0.3.9/doc/release_notes.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 Release Notes
 =============
 
-.. Upcoming Version
-.. ----------------
+Upcoming Version
+----------------
+
+
+Version 0.3.8
+-------------
+
+
+* The matrices accessor of the `Model` class now has a new function `dual` which returns the dual values of the constraints if the underlying model was optimized and dual values are existent.
+
+* The Variables class now has a new function `get_solver_attribute` which parses solver-specific attributes of the variables. For now, this function only works for Gurobi `solver_model`s. For example, the function allows retrieving the variable fields `SAObjUp` or `RC`.
+
+* The constraint assignment with a `LinearExpression` and a constant value when using the pattern `model.add_constraints(lhs_with_constant, sign, rhs)` was fixed. Before, the constant value was not added to the right-hand-side properly which led to the wrong constraint behavior. This is fixed now.
+
+* `nan`s in constants is now handled more consistently. These are ignored when in the addition of expressions (effectively filled by zero). In a future version, this might change to align the propagation of `nan`s with tools like numpy/pandas/xarray.
+
+* Up to now the `rhs` argument in the `add_constraints` function was not supporting an expression as an input type. This is now added.
+
+* Linopy now supports python 3.12.
+
+**Deprecations**
+
+* The argument `dims` in the `.sum` function of variables and expressions was deprecated in favor of the `dim` argument. This aligns the argument name with the xarray convention.
 
 Version 0.3.8
 -------------
 
 **New Features**
 
 * The LinearExpression and QuadraticExpression class have a new attribute `solution` which returns the optimal values of the expression if the underlying model was optimized.
```

### Comparing `linopy-0.3.8/doc/syntax.rst` & `linopy-0.3.9/doc/syntax.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 In order to compare the syntax between different API's, let's initialize the following problem in the different API's:
 
 .. math::
 
     & \min \;\; \sum_{i,j} 2 x_{i,j} + \; y_{i,j} \\
     s.t. & \\
-    & x_{i,j} - y_{i,j} \; \ge \; i \qquad \forall \; i,j \in \{1,...,N\} \\
+    & x_{i,j} - y_{i,j} \; \ge \; i-1 \qquad \forall \; i,j \in \{1,...,N\} \\
     & x_{i,j} + y_{i,j} \; \ge \; 0 \qquad \forall \; i,j \in \{1,...,N\}
 
 
 
 
 
 In ``JuMP`` the formulation translates to the following code:
@@ -21,17 +21,17 @@
 
     using JuMP
 
     function create_model(N)
         m = Model()
         @variable(m, x[1:N, 1:N])
         @variable(m, y[1:N, 1:N])
-        @constraint(m, [i=1:N, j=1:N], x[i, j] - y[i, j] >= i)
-        @constraint(m, [i=1:N, j=1:N], x[i, j] + y[i, j] >= 0)
-        @objective(m, Min, sum(2 * x[i, j] + y[i, j] for i in 1:N, j in 1:N))
+        @constraint(m, x - y .>= 0:(N-1))
+        @constraint(m, x + y .>= 0)
+        @objective(m, Min, 2 * sum(x) + sum(y))
         return m
     end
 
 The same model in ``linopy`` is initialized by
 
  .. code-block:: python
 
@@ -44,15 +44,15 @@
          x = m.add_variables(coords=[arange(N), arange(N)])
          y = m.add_variables(coords=[arange(N), arange(N)])
          m.add_constraints(x - y >= arange(N))
          m.add_constraints(x + y >= 0)
          m.add_objective((2 * x).sum() + y.sum())
          return m
 
-Note that the syntax is quiet similar. An important difference lays in the fact that ``linopy`` operates all arithmetic operations on **variable arrays**, while the JuMP syntax uses control variables `i` and `j`.
+Note that the syntax is quite similar.
 
 In ``Pyomo`` the code would look like
 
  .. code-block:: python
 
      from numpy import arange
      from pyomo.environ import ConcreteModel, Constraint, Objective, Set, Var
```

### Comparing `linopy-0.3.8/doc/user-guide.rst` & `linopy-0.3.9/doc/user-guide.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/create-a-model-with-coordinates.ipynb` & `linopy-0.3.9/examples/create-a-model-with-coordinates.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/create-a-model.ipynb` & `linopy-0.3.9/examples/create-a-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/creating-constraints.ipynb` & `linopy-0.3.9/examples/creating-constraints.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/creating-expressions.ipynb` & `linopy-0.3.9/examples/creating-expressions.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/creating-variables.ipynb` & `linopy-0.3.9/examples/creating-variables.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/infeasible-model.ipynb` & `linopy-0.3.9/examples/infeasible-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/manipulating-models.ipynb` & `linopy-0.3.9/examples/manipulating-models.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/migrating-from-pyomo.ipynb` & `linopy-0.3.9/examples/migrating-from-pyomo.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/solve-on-remote.ipynb` & `linopy-0.3.9/examples/solve-on-remote.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/testing-framework.ipynb` & `linopy-0.3.9/examples/testing-framework.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/examples/transport-tutorial.ipynb` & `linopy-0.3.9/examples/transport-tutorial.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995273109243697%*

 * *Differences: {"'cells'": '{18: {\'source\': [\'x.sum(dim="Markets") <= a\']}, 20: {\'source\': {insert: [(7, '*

 * *            '\'con = x.sum(dim="Markets") <= a\\n\'), (10, \'con = x.sum(dim="Canning Plants") >= '*

 * *            "b\\n')], delete: [10, 7]}}}"}*

```diff
@@ -291,15 +291,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "x.sum(dims=\"Markets\") <= a"
+                "x.sum(dim=\"Markets\") <= a"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The output nicely confirms that this is indeed the constraint we want to implement, so we add it to the model:"
@@ -316,18 +316,18 @@
                 "## Define contraints ##\n",
                 "# supply(i)   observe supply limit at plant i\n",
                 "# supply(i) .. sum (j, x(i,j)) =l= a(i)\n",
                 "\n",
                 "# demand(j)   satisfy demand at market j ;\n",
                 "# demand(j) .. sum(i, x(i,j)) =g= b(j);\n",
                 "\n",
-                "con = x.sum(dims=\"Markets\") <= a\n",
+                "con = x.sum(dim=\"Markets\") <= a\n",
                 "con1 = m.add_constraints(con, name=\"Observe supply limit at plant i\")\n",
                 "\n",
-                "con = x.sum(dims=\"Canning Plants\") >= b\n",
+                "con = x.sum(dim=\"Canning Plants\") >= b\n",
                 "con2 = m.add_constraints(con, name=\"Satisfy demand at market j\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `linopy-0.3.8/linopy/__init__.py` & `linopy-0.3.9/linopy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Mar 10 11:03:06 2021.
 
 @author: fabulous
 """
 
+from importlib.metadata import version
+
+__version__ = version("linopy")
+
 # Note: For intercepting multiplications between xarray dataarrays, Variables and Expressions
 # we need to extend their __mul__ functions with a quick special case
 import linopy.monkey_patch_xarray
 from linopy import model, remote
 from linopy.config import options
 from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
 from linopy.constraints import Constraint
 from linopy.expressions import LinearExpression, QuadraticExpression, merge
 from linopy.io import read_netcdf
 from linopy.model import Model, Variable, available_solvers
 from linopy.objective import Objective
 from linopy.remote import RemoteHandler
-from linopy.version import version as __version__
```

### Comparing `linopy-0.3.8/linopy/common.py` & `linopy-0.3.9/linopy/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/config.py` & `linopy-0.3.9/linopy/config.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/constants.py` & `linopy-0.3.9/linopy/constants.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/constraints.py` & `linopy-0.3.9/linopy/constraints.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/expressions.py` & `linopy-0.3.9/linopy/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 import functools
 import logging
 from dataclasses import dataclass, field
 from itertools import product, zip_longest
 from typing import Any, Mapping, Optional, Union
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 import xarray.core.groupby
 import xarray.core.rolling
 from numpy import array, nan
@@ -183,15 +184,15 @@
             arrays = [group, group.groupby(group).cumcount()]
             idx = pd.MultiIndex.from_arrays(
                 arrays, names=[group_name, GROUPED_TERM_DIM]
             )
             coords = Coordinates.from_pandas_multiindex(idx, group_dim)
             ds = self.data.assign_coords(coords)
             ds = ds.unstack(group_dim, fill_value=LinearExpression._fill_value)
-            ds = LinearExpression._sum(ds, dims=GROUPED_TERM_DIM)
+            ds = LinearExpression._sum(ds, dim=GROUPED_TERM_DIM)
 
             if int_map is not None:
                 index = ds.indexes["group"].map({v: k for k, v in int_map.items()})
                 index.names = orig_group.columns
                 index.name = group_name
                 coords = Coordinates.from_pandas_multiindex(index, group_name)
                 ds = xr.Dataset(ds.assign_coords(coords))
@@ -272,15 +273,15 @@
     Multiplying:
 
     >>> type(3 * expr)
     <class 'linopy.expressions.LinearExpression'>
 
     Summation over dimensions
 
-    >>> type(expr.sum(dims="dim_0"))
+    >>> type(expr.sum(dim="dim_0"))
     <class 'linopy.expressions.LinearExpression'>
     """
 
     __slots__ = ("_data", "_model")
     __array_ufunc__ = None
     __array_priority__ = 10000
 
@@ -667,52 +668,63 @@
         reference or the model is not optimized.
         """
         vals = self._map_solution()
         sol = (self.coeffs * vals).sum(TERM_DIM) + self.const
         return sol.rename("solution")
 
     @classmethod
-    def _sum(cls, expr: Union["LinearExpression", Dataset], dims=None) -> Dataset:
+    def _sum(cls, expr: Union["LinearExpression", Dataset], dim=None) -> Dataset:
         data = _expr_unwrap(expr)
 
-        if dims is None:
+        if dim is None:
             vars = DataArray(data.vars.data.ravel(), dims=TERM_DIM)
             coeffs = DataArray(data.coeffs.data.ravel(), dims=TERM_DIM)
             const = data.const.sum()
             ds = xr.Dataset({"vars": vars, "coeffs": coeffs, "const": const})
         else:
-            dims = [d for d in np.atleast_1d(dims) if d != TERM_DIM]
+            dim = [d for d in np.atleast_1d(dim) if d != TERM_DIM]
             ds = (
                 data[["coeffs", "vars"]]
-                .reset_index(dims, drop=True)
+                .reset_index(dim, drop=True)
                 .rename({TERM_DIM: STACKED_TERM_DIM})
-                .stack({TERM_DIM: [STACKED_TERM_DIM] + dims}, create_index=False)
+                .stack({TERM_DIM: [STACKED_TERM_DIM] + dim}, create_index=False)
             )
-            ds["const"] = data.const.sum(dims)
+            ds["const"] = data.const.sum(dim)
 
         return ds
 
-    def sum(self, dims=None, drop_zeros=False) -> "LinearExpression":
+    def sum(self, dim=None, drop_zeros=False, **kwargs) -> "LinearExpression":
         """
         Sum the expression over all or a subset of dimensions.
 
         This stack all terms of the dimensions, that are summed over, together.
 
         Parameters
         ----------
-        dims : str/list, optional
+        dim : str/list, optional
             Dimension(s) to sum over. The default is None which results in all
             dimensions.
+        dims : str/list, optional
+            Deprecated. Use ``dim`` instead.
 
         Returns
         -------
         linopy.LinearExpression
             Summed expression.
         """
-        res = self.__class__(self._sum(self, dims=dims), self.model)
+        if dim is None and "dims" in kwargs:
+            dim = kwargs.pop("dims")
+            warn(
+                "The `dims` argument in `.sum` is deprecated. Use `dim` instead.",
+                DeprecationWarning,
+            )
+        if kwargs:
+            raise ValueError(f"Unknown keyword argument(s): {kwargs}")
+
+        res = self.__class__(self._sum(self, dim=dim), self.model)
 
         if drop_zeros:
             res = res.densify_terms()
 
         return res
 
     def cumsum(
@@ -1233,14 +1245,16 @@
 
     drop = exprwrap(Dataset.drop)
 
     drop_sel = exprwrap(Dataset.drop_sel)
 
     drop_isel = exprwrap(Dataset.drop_isel)
 
+    expand_dims = exprwrap(Dataset.expand_dims)
+
     ffill = exprwrap(Dataset.ffill)
 
     sel = exprwrap(Dataset.sel)
 
     isel = exprwrap(Dataset.isel)
 
     shift = exprwrap(Dataset.shift)
@@ -1251,14 +1265,16 @@
 
     rename = exprwrap(Dataset.rename)
 
     rename_dims = exprwrap(Dataset.rename_dims)
 
     roll = exprwrap(Dataset.roll)
 
+    stack = exprwrap(Dataset.stack)
+
 
 @forward_as_properties(data=["attrs", "coords", "indexes", "sizes"])
 class QuadraticExpression(LinearExpression):
     """
     A quadratic expression consisting of terms of coefficients and variables.
 
     The QuadraticExpression class is a subclass of LinearExpression which allows to
@@ -1371,18 +1387,18 @@
         reference or the model is not optimized.
         """
         vals = self._map_solution()
         sol = (self.coeffs * vals.prod(FACTOR_DIM)).sum(TERM_DIM) + self.const
         return sol.rename("solution")
 
     @classmethod
-    def _sum(cls, expr: "QuadraticExpression", dims=None) -> Dataset:
+    def _sum(cls, expr: "QuadraticExpression", dim=None) -> Dataset:
         data = _expr_unwrap(expr)
-        dims = dims or list(set(data.dims) - set(HELPER_DIMS))
-        return LinearExpression._sum(expr, dims)
+        dim = dim or list(set(data.dims) - set(HELPER_DIMS))
+        return LinearExpression._sum(expr, dim)
 
     def to_constraint(self, sign, rhs):
         raise NotImplementedError(
             "Quadratic expressions cannot be used in constraints."
         )
 
     @property
@@ -1537,15 +1553,16 @@
             "compat": "override",
         }
         if override:
             kwargs["join"] = "override"
 
     if dim == TERM_DIM:
         ds = xr.concat([d[["coeffs", "vars"]] for d in data], dim, **kwargs)
-        const = xr.concat([d["const"] for d in data], dim, **kwargs).sum(TERM_DIM)
+        subkwargs = {**kwargs, "fill_value": 0}
+        const = xr.concat([d["const"] for d in data], dim, **subkwargs).sum(TERM_DIM)
         ds["const"] = const
     elif dim == FACTOR_DIM:
         ds = xr.concat([d[["vars"]] for d in data], dim, **kwargs)
         coeffs = xr.concat([d["coeffs"] for d in data], dim, **kwargs).prod(FACTOR_DIM)
         ds["coeffs"] = coeffs
         const = xr.concat([d["const"] for d in data], dim, **kwargs).prod(FACTOR_DIM)
         ds["const"] = const
```

### Comparing `linopy-0.3.8/linopy/io.py` & `linopy-0.3.9/linopy/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,21 @@
         )
         for (l, u) in zip(M.lb, M.ub)
     ]
     blx = [b if b > -np.inf else 0.0 for b in M.lb]
     bux = [b if b < np.inf else 0.0 for b in M.ub]
     task.putvarboundslice(0, model.nvars, bkx, blx, bux)
 
+    if len(model.binaries.labels) + len(model.integers.labels) > 0:
+        idx = [i for (i, v) in enumerate(M.vtypes) if v in ["B", "I"]]
+        task.putvartypelist(idx, [mosek.variabletype.type_int] * len(idx))
+        if len(model.binaries.labels) > 0:
+            bidx = [i for (i, v) in enumerate(M.vtypes) if v == "B"]
+            task.putvarboundlistconst(bidx, mosek.boundkey.ra, 0.0, 1.0)
+
     ## Constraints
 
     if len(model.constraints) > 0:
         names = "c" + M.clabels.astype(str).astype(object)
         for i, n in enumerate(names):
             task.putconname(i, n)
         bkc = [
@@ -392,15 +399,15 @@
         )
         task.putconboundslice(0, model.ncons, bkc, blc, buc)
 
     ## Objective
     if model.is_quadratic:
         Q = (0.5 * tril(M.Q + M.Q.transpose())).tocoo()
         task.putqobj(Q.row, Q.col, Q.data)
-    task.putclist(np.arange(model.nvars), M.c)
+    task.putclist(list(np.arange(model.nvars)), M.c)
 
     if model.objective.sense == "max":
         task.putobjsense(mosek.objsense.maximize)
     else:
         task.putobjsense(mosek.objsense.minimize)
     return task
 
@@ -508,15 +515,15 @@
         Q = triu(Q)
         Q = Q.tocsr()
         num_vars = Q.shape[0]
         h.passHessian(num_vars, Q.nnz, 1, Q.indptr, Q.indices, Q.data)
 
     # change objective sense
     if m.objective.sense == "max":
-        h.changeObjectiveSense(highspy.highs_bindings.ObjSense.kMaximize)
+        h.changeObjectiveSense(highspy.ObjSense.kMaximize)
 
     return h
 
 
 def to_block_files(m, fn):
     """
     Write out the linopy model to a block structured output.
```

### Comparing `linopy-0.3.8/linopy/matrices.py` & `linopy-0.3.9/linopy/matrices.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,14 +78,28 @@
         if not self._parent.status == "ok":
             raise ValueError("Model is not optimized.")
         if "solution" not in self.flat_vars:
             del self.flat_vars  # clear cache
         df = self.flat_vars
         return create_vector(df.key, df.solution, fill_value=np.nan)
 
+    @cached_property
+    def dual(self):
+        "Vector of dual values of all non-missing constraints."
+        if not self._parent.status == "ok":
+            raise ValueError("Model is not optimized.")
+        if "dual" not in self.flat_cons:
+            del self.flat_cons  # clear cache
+        df = self.flat_cons
+        if "dual" not in df:
+            raise AttributeError(
+                "Underlying is optimized but does not have dual values stored."
+            )
+        return create_vector(df.key, df.dual, fill_value=np.nan)
+
     @property
     def ub(self):
         "Vector of upper bounds of all non-missing variables."
         df = self.flat_vars
         return create_vector(df.key, df.upper)
 
     @property
```

### Comparing `linopy-0.3.8/linopy/model.py` & `linopy-0.3.9/linopy/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         "_connameCounter",
         "_blocks",
         # TODO: check if these should not be mutable
         "_chunk",
         "_force_dim_names",
         "_solver_dir",
         "solver_model",
+        "solver_name",
         "matrices",
     )
 
     def __init__(self, solver_dir=None, chunk=None, force_dim_names=False):
         """
         Initialize the linopy model.
 
@@ -533,20 +534,18 @@
         if name in self.constraints:
             raise ValueError(f"Constraint '{name}' already assigned to model")
         elif name is None:
             name = f"con{self._connameCounter}"
             self._connameCounter += 1
         if sign is not None:
             sign = maybe_replace_signs(as_dataarray(sign))
-        if rhs is not None:
-            rhs = as_dataarray(rhs)
 
         if isinstance(lhs, LinearExpression):
             assert_sign_rhs_not_None(lhs, sign, rhs)
-            data = lhs.data.assign(sign=sign, rhs=rhs)
+            data = lhs.to_constraint(sign, rhs).data
         elif callable(lhs):
             assert coords is not None, "`coords` must be given when lhs is a function"
             rule = lhs
             assert_sign_rhs_are_None(lhs, sign, rhs)
             data = Constraint.from_rule(self, rule, coords).data
         elif isinstance(lhs, AnonymousScalarConstraint):
             assert_sign_rhs_are_None(lhs, sign, rhs)
@@ -979,28 +978,29 @@
             Whether to keep all temporary files like lp file, solution file.
             This argument is ignored for the logger file `log_fn`. The default
             is False.
         env : gurobi.Env, optional
             Existing environment passed to the solver (e.g. `gurobipy.Env`).
             Currently only in use for Gurobi. The default is None.
         sanitize_zeros : bool, optional
-            Whether to set terms with zero coeffficient as missing.
+            Whether to set terms with zero coefficient as missing.
             This will remove unneeded overhead in the lp file writing.
             The default is True.
         remote : linopy.remote.RemoteHandler
             Remote handler to use for solving model on a server. Note that when
             solving on a rSee
             linopy.remote.RemoteHandler for more details.
         **solver_options : kwargs
             Options passed to the solver.
 
         Returns
         -------
-        linopy.Model
-            Optimized model.
+        status : tuple
+            Tuple containing the status and termination condition of the
+            optimization process.
         """
         if remote:
             solved = remote.solve_on_remote(
                 self,
                 solver_name=solver_name,
                 io_api=io_api,
                 problem_fn=problem_fn,
@@ -1076,14 +1076,15 @@
 
         result.info()
 
         self.objective._value = result.solution.objective
         self.status = result.status.status.value
         self.termination_condition = result.status.termination_condition.value
         self.solver_model = result.solver_model
+        self.solver_name = solver_name
 
         if not result.status.is_ok:
             return result.status.status.value, result.status.termination_condition.value
 
         # map solution and dual to original shape which includes missing values
         sol = result.solution.primal.copy()
         sol.loc[-1] = nan
```

### Comparing `linopy-0.3.8/linopy/monkey_patch_xarray.py` & `linopy-0.3.9/linopy/monkey_patch_xarray.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/objective.py` & `linopy-0.3.9/linopy/objective.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/remote.py` & `linopy-0.3.9/linopy/remote.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/solvers.py` & `linopy-0.3.9/linopy/solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import contextlib
 import io
 import logging
 import os
 import re
 import subprocess as sub
+import sys
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from linopy.constants import (
     Result,
@@ -124,15 +125,15 @@
 def maybe_adjust_objective_sign(solution, sense, io_api):
     if sense == "min":
         return
 
     if np.isnan(solution.objective):
         return
 
-    if io_api == "mps":
+    if io_api == "mps" and sys.version_info < (3, 12):
         logger.info(
             "Adjusting objective sign due to switched coefficients in MPS file."
         )
         solution.objective *= -1
 
 
 def set_int_index(series):
@@ -171,14 +172,20 @@
     options, run 'cbc' in your shell
     """
     if io_api is not None and io_api not in ["lp", "mps"]:
         raise ValueError(
             "Keyword argument `io_api` has to be one of `lp`, `mps' or None"
         )
 
+    # CBC does not like the OBJSENSE line in MPS files, which new highspy versions write
+    if io_api == "mps" and model.sense == "max" and sys.version_info >= (3, 12):
+        raise ValueError(
+            "GLPK does not support maximization in MPS format for Python 3.12+"
+        )
+
     problem_fn = model.to_file(problem_fn)
 
     # printingOptions is about what goes in solution file
     command = f"cbc -printingOptions all -import {problem_fn} "
 
     if warmstart_fn:
         command += f"-basisI {warmstart_fn} "
@@ -278,14 +285,20 @@
     }
 
     if io_api is not None and io_api not in ["lp", "mps"]:
         raise ValueError(
             "Keyword argument `io_api` has to be one of `lp`, `mps` or None"
         )
 
+    # GLPK does not like the OBJSENSE line in MPS files, which new highspy versions write
+    if io_api == "mps" and model.sense == "max" and sys.version_info >= (3, 12):
+        raise ValueError(
+            "GLPK does not support maximization in MPS format for Python 3.12+"
+        )
+
     problem_fn = model.to_file(problem_fn)
     suffix = problem_fn.suffix[1:]
 
     os.makedirs(os.path.dirname(solution_fn), exist_ok=True)
 
     # TODO use --nopresol argument for non-optimal solution output
     command = f"glpsol --{suffix} {problem_fn} --output {solution_fn} "
@@ -354,15 +367,14 @@
             .pipe(set_int_index)
         )
         f.close()
         return Solution(sol, dual, objective)
 
     solution = safe_get_solution(status, get_solver_solution)
     maybe_adjust_objective_sign(solution, model.objective.sense, io_api)
-
     return Result(status, solution)
 
 
 def run_highs(
     model,
     io_api=None,
     problem_fn=None,
@@ -382,15 +394,15 @@
 
     . The full list of solver options is documented at
     https://www.maths.ed.ac.uk/hall/HiGHS/HighsOptions.set .
 
     Some exemplary options are:
 
         * presolve : "choose" by default - "on"/"off" are alternatives.
-        * solver :"choose" by default - "simplex"/"ipm" are alternatives.
+        * solver :"choose" by default - "simplex"/"ipm"/"pdlp" are alternatives. Only "choose" solves MIP / QP!
         * parallel : "choose" by default - "on"/"off" are alternatives.
         * time_limit : inf by default.
 
     Returns
     -------
     status : string,
         SolverStatus.ok or SolverStatus.warning
@@ -399,20 +411,23 @@
     variables_sol : series
     constraints_dual : series
     objective : float
     """
     CONDITION_MAP = {}
 
     if warmstart_fn:
-        logger.warning("Warmstart not available with HiGHS solver. Ignore argument.")
+        logger.warning("Warmstart not implemented. Ignoring argument.")
 
-    if solver_options.get("solver") in ["simplex", "ipm"] and model.type == "QP":
+    if solver_options.get("solver") in ["simplex", "ipm", "pdlp"] and model.type in [
+        "QP",
+        "MILP",
+    ]:
         logger.warning(
-            "The HiGHS solver ignores quadratic terms if the solver is set to 'simplex' or 'ipm'. "
-            "Drop the solver option or use 'choose' to enable quadratic terms."
+            "The HiGHS solver ignores quadratic terms / integrality if the solver is set to 'simplex', 'ipm' or 'pdlp'. "
+            "Drop the solver option or use 'choose' to enable quadratic terms / integrality."
         )
 
     if io_api is None or io_api in ["lp", "mps"]:
         model.to_file(problem_fn)
         h = highspy.Highs()
         h.readModel(maybe_convert_path(problem_fn))
     elif io_api == "direct":
@@ -743,15 +758,17 @@
         sol = pd.Series({v.name: s[v] for v in m.getVars()})
         sol.drop(["quadobjvar", "qmatrixvar"], errors="ignore", inplace=True, axis=0)
         sol = set_int_index(sol)
 
         cons = m.getConss()
         if len(cons) != 0:
             dual = pd.Series({c.name: m.getDualSolVal(c) for c in cons})
-            dual = dual[dual.index.str.startswith("c")]
+            dual = dual[
+                dual.index.str.startswith("c") & ~dual.index.str.startswith("cf")
+            ]
             dual = set_int_index(dual)
         else:
             logger.warning("Dual values of MILP couldn't be parsed")
             dual = pd.Series(dtype=float)
 
         return Solution(sol, dual, objective)
 
@@ -894,17 +911,16 @@
     }
 
     if io_api is not None and io_api not in ["lp", "mps", "direct"]:
         raise ValueError(
             "Keyword argument `io_api` has to be one of `lp`, `mps`, `direct` or None"
         )
 
-    problem_fn = model.to_file(problem_fn)
-
     if io_api != "direct" and io_api is not None:
+        problem_fn = model.to_file(problem_fn)
         problem_fn = maybe_convert_path(problem_fn)
     log_fn = maybe_convert_path(log_fn)
     warmstart_fn = maybe_convert_path(warmstart_fn)
     basis_fn = maybe_convert_path(basis_fn)
 
     with contextlib.ExitStack() as stack:
         if env is None:
```

### Comparing `linopy-0.3.8/linopy/testing.py` & `linopy-0.3.9/linopy/testing.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/linopy/variables.py` & `linopy-0.3.9/linopy/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     print_coord,
     print_single_variable,
     save_join,
     to_dataframe,
 )
 from linopy.config import options
 from linopy.constants import TERM_DIM
+from linopy.solvers import set_int_index
 
 logger = logging.getLogger(__name__)
 
 
 def varwrap(method, *default_args, **new_default_kwargs):
     @functools.wraps(method)
     def _varwrap(var, *args, **kwargs):
@@ -661,14 +662,47 @@
         """
         warn(
             "`Variable.sol` is deprecated. Use `Variable.solution` instead.",
             DeprecationWarning,
         )
         return self.solution
 
+    @has_optimized_model
+    def get_solver_attribute(self, attr):
+        """
+        Get an attribute from the solver model.
+
+        Parameters
+        ----------
+        attr : str
+            Name of the attribute to get.
+
+        Returns
+        -------
+        xr.DataArray
+        """
+        solver_model = self.model.solver_model
+        if self.model.solver_name != "gurobi":
+            raise NotImplementedError(
+                "Solver attribute getter only supports the Gurobi solver for now."
+            )
+
+        vals = pd.Series(
+            {v.VarName: getattr(v, attr) for v in solver_model.getVars()}, dtype=float
+        )
+        vals = set_int_index(vals)
+
+        idx = np.ravel(self.labels)
+        try:
+            vals = vals[idx].values.reshape(self.labels.shape)
+        except KeyError:
+            vals = vals.reindex(idx).values.reshape(self.labels.shape)
+
+        return DataArray(vals, self.coords)
+
     @property
     def flat(self):
         """
         Convert the variable to a pandas DataFrame.
 
         The resulting DataFrame represents a long table format of the variable
         with columns `labels`, `lower`, `upper` which are not masked.
@@ -688,33 +722,44 @@
         if any_nan.any():
             fields = ", ".join("`" + df.columns[any_nan] + "`")
             raise ValueError(
                 f"Variable `{self.name}` contains nan's in field(s) {fields}"
             )
         return df
 
-    def sum(self, dims=None):
+    def sum(self, dim=None, **kwargs):
         """
         Sum the variables over all or a subset of dimensions.
 
         This stack all terms of the dimensions, that are summed over, together.
         The function works exactly in the same way as ``LinearExpression.sum()``.
 
         Parameters
         ----------
-        dims : str/list, optional
+        dim : str/list, optional
             Dimension(s) to sum over. The default is None which results in all
             dimensions.
+        dims : str/list, optional
+            Deprecated. Use ``dim`` instead.
 
         Returns
         -------
         linopy.LinearExpression
             Summed expression.
         """
-        return self.to_linexpr().sum(dims)
+        if dim is None and "dims" in kwargs:
+            dim = kwargs.pop("dims")
+            warn(
+                "The `dims` argument is deprecated. Use `dim` instead.",
+                DeprecationWarning,
+            )
+        if kwargs:
+            raise ValueError(f"Unknown keyword argument(s): {kwargs}")
+
+        return self.to_linexpr().sum(dim)
 
     def diff(self, dim, n=1):
         """
         Calculate the n-th order discrete difference along the given dimension.
 
         This function works exactly in the same way as ``LinearExpression.diff()``.
 
@@ -871,24 +916,28 @@
 
     # drop = varwrap(Dataset.drop)
 
     drop_sel = varwrap(Dataset.drop_sel)
 
     drop_isel = varwrap(Dataset.drop_isel)
 
+    expand_dims = varwrap(Dataset.expand_dims)
+
     sel = varwrap(Dataset.sel)
 
     isel = varwrap(Dataset.isel)
 
     shift = varwrap(Dataset.shift, fill_value=_fill_value)
 
     rename = varwrap(Dataset.rename)
 
     roll = varwrap(Dataset.roll)
 
+    stack = varwrap(Dataset.stack)
+
 
 @dataclass(repr=False)
 @forward_as_properties(
     labels=[
         "attrs",
         "coords",
         "indexes",
@@ -1049,14 +1098,32 @@
     @property
     def solution(self):
         """
         Get the solution of variables.
         """
         return save_join(*[v.solution.rename(k) for k, v in self.items()])
 
+    @has_optimized_model
+    def get_solver_attribute(self, attr):
+        """
+        Get an attribute from the solver model.
+
+        Parameters
+        ----------
+        attr : str
+            Name of the attribute to get.
+
+        Returns
+        -------
+        xr.DataArray
+        """
+        return save_join(
+            *[v.get_solver_attribute(attr).rename(k) for k, v in self.items()]
+        )
+
     def get_name_by_label(self, label):
         """
         Get the variable name of the variable containing the passed label.
 
         Parameters
         ----------
         label : int
```

### Comparing `linopy-0.3.8/linopy.egg-info/PKG-INFO` & `linopy-0.3.9/linopy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Linear optimization with N-D labeled arrays in Python
-Home-page: https://github.com/PyPSA/linopy
-Author: Fabian Hofmann
-Author-email: hofmann@fias.uni-frankfurt.de
-License: MIT
+Author-email: Fabian Hofmann <fabianmarikhofmann@gmail.com>
+Project-URL: Homepage, https://github.com/PyPSA/linopy
+Project-URL: Source, https://github.com/PyPSA/linopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -41,18 +40,19 @@
 Requires-Dist: netcdf4; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: paramiko; extra == "dev"
 Requires-Dist: gurobipy; extra == "dev"
 Requires-Dist: highspy; extra == "dev"
 Provides-Extra: solvers
 Requires-Dist: gurobipy; extra == "solvers"
-Requires-Dist: highspy; extra == "solvers"
-Requires-Dist: cplex; extra == "solvers"
+Requires-Dist: highspy>=1.5.0; python_version < "3.12" and extra == "solvers"
+Requires-Dist: highspy>=1.7.1.dev1; python_version >= "3.12" and extra == "solvers"
+Requires-Dist: cplex; (platform_system != "Darwin" and python_version < "3.12") and extra == "solvers"
 Requires-Dist: mosek; extra == "solvers"
-Requires-Dist: mindoptpy; extra == "solvers"
+Requires-Dist: mindoptpy; python_version < "3.12" and extra == "solvers"
 Requires-Dist: coptpy; extra == "solvers"
 Requires-Dist: xpress; (platform_system != "Darwin" and python_version < "3.11") and extra == "solvers"
 Requires-Dist: pyscipopt; platform_system != "Darwin" and extra == "solvers"
 
 # linopy: Optimization with array-like variables and constraints
 
 [![PyPI](https://img.shields.io/pypi/v/linopy)](https://pypi.org/project/linopy/) [![CI](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml/badge.svg)](https://github.com/FabianHofmann/linopy/actions/workflows/CI.yaml) [![License](https://img.shields.io/pypi/l/linopy.svg)](LICENSE.txt) [![doc](https://readthedocs.org/projects/linopy/badge/?version=latest)](https://linopy.readthedocs.io/en/latest/) [![codecov](https://codecov.io/gh/PyPSA/linopy/branch/master/graph/badge.svg?token=TT4EYFCCZX)](https://codecov.io/gh/PyPSA/linopy)
@@ -60,15 +60,15 @@
 **linopy** is an open-source python package that facilitates **optimization** with **real world data**. It builds a bridge between data analysis packages like [xarray](https://github.com/pydata/xarray) & [pandas](https://pandas.pydata.org/) and problem solvers like [cbc](https://projects.coin-or.org/Cbc), [gurobi](https://www.gurobi.com/) (see the full list below). **Linopy** supports **Linear, Integer, Mixed-Integer and Quadratic Programming** while aiming to make linear programming in Python easy, highly-flexible and performant.
 
 
 ## Benchmarks
 
 **linopy** is designed to be fast and efficient. The following benchmark compares the performance of **linopy** with the alternative popular optimization packages.
 
-![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTAxNTAzMDYsIm5iZiI6MTcxMDE1MDAwNiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAzMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMzExVDA5NDAwNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBlNzU4NTYxOTQ2ZjdmYmFiMjBjMGNkNTIzYjk5NzhmMWYzODRhMzE2YzAwMDEzMTc5ZWJlNmE1MzMzMTRmNzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.pVhJRAuZJB982o5h85zCFp8aQixW9wl3Bo3bemf0MlU)
+![Performance Benchmark](https://private-user-images.githubusercontent.com/19226431/311655091-e3b8a6b9-da72-407b-bd37-7c80ada39d46.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQ3NDY1NzYsIm5iZiI6MTcxNDc0NjI3NiwicGF0aCI6Ii8xOTIyNjQzMS8zMTE2NTUwOTEtZTNiOGE2YjktZGE3Mi00MDdiLWJkMzctN2M4MGFkYTM5ZDQ2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA1MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNTAzVDE0MjQzNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ3M2Q5MTMxY2EzNTI4OTUzNDViMzUzZTkyOGQ0MzliYTYxNjc2ODdhNDFjODRiNmE4OGIwNWI0MWZlNDZmMWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.WFHwXmalW05hSm0oxWGmAEnVvcdFyCvQMxDJB7v3yBk)
 
 
 ## Main features
 
 **linopy** is heavily based on [xarray](https://github.com/pydata/xarray) which allows for many flexible data-handling features:
 
 * Define (arrays of) continuous or binary variables with **coordinates**, e.g. time, consumers, etc.
```

### Comparing `linopy-0.3.8/linopy.egg-info/SOURCES.txt` & `linopy-0.3.9/linopy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CONTRIBUTING.md
 LICENSE.txt
 README.md
 pyproject.toml
-setup.py
 .github/workflows/CI.yaml
 .github/workflows/deploy.yml
 benchmark/README.md
 benchmark/Snakefile
 benchmark/benchmark-absolute.pdf
 benchmark/benchmark-absolute.png
 benchmark/benchmark-overhead.pdf
```

### Comparing `linopy-0.3.8/test/test_common.py` & `linopy-0.3.9/test/test_common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_constraint.py` & `linopy-0.3.9/test/test_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,23 @@
     m.add_constraints(lhs, EQUAL, 0, name="c2")
     assert m.constraints["c2"].vars.notnull().all()
     assert m.constraints["c2"].coeffs.notnull().all()
     assert (m.constraints["c2"].sign == EQUAL).all()
     assert (m.constraints["c2"].rhs == 0).all()
 
 
+def test_constraint_assignment_with_args_and_constant(m, x, y):
+    lhs = x + y + 10
+    m.add_constraints(lhs, EQUAL, 0, name="c2")
+    assert m.constraints["c2"].vars.notnull().all()
+    assert m.constraints["c2"].coeffs.notnull().all()
+    assert (m.constraints["c2"].sign == EQUAL).all()
+    assert (m.constraints["c2"].rhs == -10).all()
+
+
 def test_constraint_assignment_with_args_valid_sign(m, x, y):
     lhs = x + y
     for i, sign in enumerate([EQUAL, GREATER_EQUAL, LESS_EQUAL]):
         m.add_constraints(lhs, sign, 0, name=f"c{i}")
         assert m.constraints[f"c{i}"].vars.notnull().all()
         assert m.constraints[f"c{i}"].coeffs.notnull().all()
         assert (m.constraints[f"c{i}"].sign == sign).all()
```

### Comparing `linopy-0.3.8/test/test_constraints.py` & `linopy-0.3.9/test/test_constraints.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_io.py` & `linopy-0.3.9/test/test_io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_linear_expression.py` & `linopy-0.3.9/test/test_linear_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,24 @@
     res = expr.sum("dim_0", drop_zeros=True)
     assert res.nterm == 2
 
     res = expr.sum("dim_1", drop_zeros=True)
     assert res.nterm == 2
 
 
+def test_linear_expression_sum_warn_using_dims(z):
+    with pytest.warns(DeprecationWarning):
+        (1 * z).sum(dims="dim_0")
+
+
+def test_linear_expression_sum_warn_unknown_kwargs(z):
+    with pytest.raises(ValueError):
+        (1 * z).sum(unknown_kwarg="dim_0")
+
+
 def test_linear_expression_multiplication(x, y, z):
     expr = 10 * x + y + z
     mexpr = expr * 10
     assert (mexpr.coeffs.sel(dim_1=0, dim_0=0, _term=0) == 100).item()
 
     mexpr = 10 * expr
     assert (mexpr.coeffs.sel(dim_1=0, dim_0=0, _term=0) == 100).item()
@@ -552,14 +562,26 @@
 
     filled = filtered.fillna(10)
     assert isinstance(filled, LinearExpression)
     assert filled.const.sum() == 200
     assert filled.coeffs.isnull().sum() == 10
 
 
+def test_variable_expand_dims(v):
+    result = v.to_linexpr().expand_dims("new_dim")
+    assert isinstance(result, LinearExpression)
+    assert result.coord_dims == ("new_dim", "dim_2")
+
+
+def test_variable_stack(v):
+    result = v.to_linexpr().expand_dims("new_dim").stack(new=("new_dim", "dim_2"))
+    assert isinstance(result, LinearExpression)
+    assert result.coord_dims == ("new",)
+
+
 def test_linear_expression_diff(v):
     diff = v.to_linexpr().diff("dim_2")
     assert diff.nterm == 2
 
 
 @pytest.mark.parametrize("use_fallback", [True, False])
 def test_linear_expression_groupby(v, use_fallback):
```

### Comparing `linopy-0.3.8/test/test_matrices.py` & `linopy-0.3.9/test/test_matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_model.py` & `linopy-0.3.9/test/test_model.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_objective.py` & `linopy-0.3.9/test/test_objective.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_optimization.py` & `linopy-0.3.9/test/test_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 Created on Thu Mar 18 08:49:08 2021.
 
 @author: fabian
 """
 
 import logging
 import platform
+import sys
 
 import numpy as np
 import pandas as pd
 import pytest
+import xarray as xr
 from xarray.testing import assert_equal
 
 from linopy import GREATER_EQUAL, LESS_EQUAL, Model
 from linopy.solvers import available_solvers, quadratic_solvers
 
 logger = logging.getLogger(__name__)
 
@@ -328,27 +330,31 @@
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_setting(model, solver, io_api):
     assert model.objective.sense == "min"
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "ok"
     assert np.isclose(model.objective.value, 3.3)
+    assert model.solver_name == solver
 
     with pytest.warns(DeprecationWarning):
         assert np.isclose(model.objective_value, 3.3)
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_setting_sol_and_dual_accessor(model, solver, io_api):
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "ok"
     x = model["x"]
     assert_equal(x.solution, model.solution["x"])
     c = model.constraints["con1"]
     assert_equal(c.dual, model.dual["con1"])
+    # squeeze in dual getter in matrix
+    assert len(model.matrices.dual) == model.ncons
+    assert model.matrices.dual[0] == model.dual["con0"]
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_setting_expression_sol_accessor(model, solver, io_api):
     status, condition = model.solve(solver, io_api=io_api)
     assert status == "ok"
     x = model["x"]
@@ -375,17 +381,22 @@
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_model_maximization(model_maximization, solver, io_api):
     m = model_maximization
     assert m.objective.sense == "max"
     assert m.objective.value is None
-    status, condition = m.solve(solver, io_api=io_api)
-    assert status == "ok"
-    assert np.isclose(m.objective.value, 3.3)
+
+    if solver in ["cbc", "glpk"] and io_api == "mps" and sys.version_info >= (3, 12):
+        with pytest.raises(ValueError):
+            m.solve(solver, io_api=io_api)
+    else:
+        status, condition = m.solve(solver, io_api=io_api)
+        assert status == "ok"
+        assert np.isclose(m.objective.value, 3.3)
 
 
 @pytest.mark.parametrize("solver,io_api", params)
 def test_default_settings_chunked(model_chunked, solver, io_api):
     status, condition = model_chunked.solve(solver, io_api=io_api)
     assert status == "ok"
     assert np.isclose(model_chunked.objective.value, 3.3)
@@ -624,14 +635,26 @@
 
 @pytest.mark.parametrize("solver", available_solvers)
 def test_non_supported_solver_io(model, solver):
     with pytest.raises(ValueError):
         model.solve(solver, io_api="non_supported")
 
 
+@pytest.mark.parametrize("solver,io_api", params)
+def test_solver_attribute_getter(model, solver, io_api):
+    model.solve(solver)
+    if solver != "gurobi":
+        with pytest.raises(NotImplementedError):
+            model.variables.get_solver_attribute("RC")
+    else:
+        rc = model.variables.get_solver_attribute("RC")
+        assert isinstance(rc, xr.Dataset)
+        assert set(rc) == set(model.variables)
+
+
 # def init_model_large():
 #     m = Model()
 #     time = pd.Index(range(10), name="time")
 
 #     x = m.add_variables(name="x", lower=0, coords=[time])
 #     y = m.add_variables(name="y", lower=0, coords=[time])
 #     factor = pd.Series(time, index=time)
```

### Comparing `linopy-0.3.8/test/test_options.py` & `linopy-0.3.9/test/test_options.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_quadratic_expression.py` & `linopy-0.3.9/test/test_quadratic_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,23 +145,33 @@
     assert (expr.const == -5).all()
     assert expr.nterm == 2
 
 
 def test_quadratic_expression_sum(x, y):
     expr = x * y + x + 5
 
-    summed_expr = expr.sum(dims="dim_0")
+    summed_expr = expr.sum(dim="dim_0")
     assert isinstance(summed_expr, QuadraticExpression)
     assert not summed_expr.coord_dims
 
     summed_expr_all = expr.sum()
     assert isinstance(summed_expr_all, QuadraticExpression)
     assert not summed_expr_all.coord_dims
 
 
+def test_quadratic_expression_sum_warn_using_dims(x):
+    with pytest.warns(DeprecationWarning):
+        (x**2).sum(dims="dim_0")
+
+
+def test_quadratic_expression_sum_warn_unknown_kwargs(x):
+    with pytest.raises(ValueError):
+        (x**2).sum(unknown_kwarg="dim_0")
+
+
 def test_quadratic_expression_wrong_multiplication(x, y):
     with pytest.raises(TypeError):
         x * x * y
 
 
 def test_merge_linear_expression_and_quadratic_expression(x, y):
     linexpr = 10 * x + y + 5
```

### Comparing `linopy-0.3.8/test/test_repr.py` & `linopy-0.3.9/test/test_repr.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_scalar_constraint.py` & `linopy-0.3.9/test/test_scalar_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_scalar_linear_expression.py` & `linopy-0.3.9/test/test_scalar_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_variable.py` & `linopy-0.3.9/test/test_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,14 +139,24 @@
 
 
 def test_variable_sum(x):
     res = x.sum()
     assert res.nterm == 10
 
 
+def test_variable_sum_warn_using_dims(x):
+    with pytest.warns(DeprecationWarning):
+        x.sum(dims="first")
+
+
+def test_variable_sum_warn_unknown_kwargs(x):
+    with pytest.raises(ValueError):
+        x.sum(unknown_kwarg="first")
+
+
 def test_variable_where(x):
     x = x.where([True] * 4 + [False] * 6)
     assert isinstance(x, linopy.variables.Variable)
     assert x.labels[9] == x._fill_value["labels"]
 
     x = x.where([True] * 4 + [False] * 6, x[0])
     assert isinstance(x, linopy.variables.Variable)
@@ -200,17 +210,24 @@
     x = x.where([True] * 4 + [False] * 6)
     x = x.ffill("first")
     assert isinstance(x, linopy.variables.Variable)
     assert x.labels[9] == x.labels[3]
     assert x.labels[3] != x.labels[2]
 
 
-def test_variable_fillna(x):
-    result = x.fillna(x[0])
+def test_variable_expand_dims(x):
+    result = x.expand_dims("new_dim")
+    assert isinstance(result, linopy.variables.Variable)
+    assert result.dims == ("new_dim", "first")
+
+
+def test_variable_stack(x):
+    result = x.expand_dims("new_dim").stack(new=("new_dim", "first"))
     assert isinstance(result, linopy.variables.Variable)
+    assert result.dims == ("new",)
 
 
 def test_variable_sanitize(x):
     # convert intentionally to float with nans
     fill_value = {"labels": np.nan, "lower": np.nan, "upper": np.nan}
     x = x.where([True] * 4 + [False] * 6, fill_value)
     x = x.sanitize()
```

### Comparing `linopy-0.3.8/test/test_variable_assignment.py` & `linopy-0.3.9/test/test_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `linopy-0.3.8/test/test_variables.py` & `linopy-0.3.9/test/test_variables.py`

 * *Files identical despite different names*

