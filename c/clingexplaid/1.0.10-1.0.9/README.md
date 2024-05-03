# Comparing `tmp/clingexplaid-1.0.10.tar.gz` & `tmp/clingexplaid-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clingexplaid-1.0.10.tar", last modified: Fri May  3 12:57:29 2024, max compression
+gzip compressed data, was "clingexplaid-1.0.9.tar", last modified: Tue Apr 30 16:00:13 2024, max compression
```

## Comparing `clingexplaid-1.0.10.tar` & `clingexplaid-1.0.9.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.028432 clingexplaid-1.0.10/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.004431 clingexplaid-1.0.10/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/DEPLOYMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/LIMITATIONS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-03 12:57:29.028432 clingexplaid-1.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/_static/logo-dark-mode.png
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/_static/logo-light-mode.png
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/doc/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/doc/content/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/content/encodings/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/content/encodings/instance.md
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/content/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/content/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/doc/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.008432 clingexplaid-1.0.10/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.012431 clingexplaid-1.0.10/examples/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/graph_coloring/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/graph_coloring/encoding.lp
--rw-r--r--   0 runner    (1001) docker     (127)    42851 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/graph_coloring/graph_coloring_example.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/graph_coloring/instance.lp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.016431 clingexplaid-1.0.10/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/bad_mucs.lp
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/sat.lp
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/simple.lp
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/soup.lp
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/sudoku_4x4.lp
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/sudoku_encoding.lp
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/sudoku_encoding_2.lp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.016431 clingexplaid-1.0.10/examples/misc/test/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test/blob.lp
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test.lp
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test2.lp
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test3.lp
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test4.lp
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/test_inert.lp
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/x.lp
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/misc/zero_arity_assumptions.lp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.016431 clingexplaid-1.0.10/examples/queens/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/queens/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/queens/encoding.lp
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/queens/instance.lp
--rw-r--r--   0 runner    (1001) docker     (127)    19603 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/queens/queens_example.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.016431 clingexplaid-1.0.10/examples/sudoku/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/sudoku/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/sudoku/encoding.lp
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/sudoku/instance.lp
--rw-r--r--   0 runner    (1001) docker     (127)    36797 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/examples/sudoku/sudoku_example.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:57:29.028432 clingexplaid-1.0.10/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.008432 clingexplaid-1.0.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.016431 clingexplaid-1.0.10/src/clingexplaid/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/cli/clingo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/muc/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/muc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/muc/core_computer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/propagators/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/propagators/propagator_decision_order.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_assumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_optimization_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_rule_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_rule_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/unsat_constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/unsat_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/unsat_constraints/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/unsat_constraints/unsat_constraint_computer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.020431 clingexplaid-1.0.10/src/clingexplaid/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/src/clingexplaid/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.024432 clingexplaid-1.0.10/src/clingexplaid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-03 12:57:28.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-03 12:57:29.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:57:28.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 12:57:28.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 12:57:28.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 12:57:28.000000 clingexplaid-1.0.10/src/clingexplaid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.024432 clingexplaid-1.0.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.024432 clingexplaid-1.0.10/tests/clingexplaid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:29.024432 clingexplaid-1.0.10/tests/clingexplaid/res/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program.lp
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_constants.lp
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_constraints.lp
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_decision_order.lp
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_multi_muc.lp
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_optimization.lp
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_rules.lp
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/test_program_unsat_constraints.lp
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_assumptions_all.lp
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_assumptions_certain_signatures.lp
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_constraints.lp
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_constraints_id.lp
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_facts.lp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_optimization.lp
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_rule_ids.lp
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/res/transformed_program_rules_split.lp
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/test_muc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/test_unsat_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/clingexplaid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-03 12:57:23.000000 clingexplaid-1.0.10/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.747514 clingexplaid-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.723515 clingexplaid-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/DEPLOYMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-30 16:00:13.747514 clingexplaid-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/_static/logo-dark-mode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/_static/logo-light-mode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/doc/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/doc/content/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/content/encodings/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/content/encodings/instance.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/content/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/content/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/doc/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.727515 clingexplaid-1.0.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.731515 clingexplaid-1.0.9/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/graph_coloring/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/graph_coloring/encoding.lp
+-rw-r--r--   0 runner    (1001) docker     (127)    42851 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/graph_coloring/graph_coloring_example.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/graph_coloring/instance.lp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.735514 clingexplaid-1.0.9/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/bad_mucs.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/sat.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/simple.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/soup.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/sudoku_4x4.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/sudoku_encoding.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/sudoku_encoding_2.lp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.735514 clingexplaid-1.0.9/examples/misc/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test/blob.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test2.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test3.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test4.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/test_inert.lp
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/x.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/misc/zero_arity_assumptions.lp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.735514 clingexplaid-1.0.9/examples/queens/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/queens/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/queens/encoding.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/queens/instance.lp
+-rw-r--r--   0 runner    (1001) docker     (127)    19603 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/queens/queens_example.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.735514 clingexplaid-1.0.9/examples/sudoku/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/sudoku/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/sudoku/encoding.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/sudoku/instance.lp
+-rw-r--r--   0 runner    (1001) docker     (127)    36797 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/examples/sudoku/sudoku_example.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 16:00:13.747514 clingexplaid-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.727515 clingexplaid-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.735514 clingexplaid-1.0.9/src/clingexplaid/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.739514 clingexplaid-1.0.9/src/clingexplaid/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/cli/clingo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.739514 clingexplaid-1.0.9/src/clingexplaid/muc/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/muc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/muc/core_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.739514 clingexplaid-1.0.9/src/clingexplaid/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/propagators/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/propagators/propagator_decision_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.739514 clingexplaid-1.0.9/src/clingexplaid/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_assumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_optimization_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_rule_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_rule_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.739514 clingexplaid-1.0.9/src/clingexplaid/unsat_constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/unsat_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/unsat_constraints/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/unsat_constraints/unsat_constraint_computer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.743514 clingexplaid-1.0.9/src/clingexplaid/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/src/clingexplaid/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.747514 clingexplaid-1.0.9/src/clingexplaid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 16:00:13.000000 clingexplaid-1.0.9/src/clingexplaid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.743514 clingexplaid-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.743514 clingexplaid-1.0.9/tests/clingexplaid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:13.747514 clingexplaid-1.0.9/tests/clingexplaid/res/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_constants.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_constraints.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_decision_order.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_multi_muc.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_optimization.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_rules.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/test_program_unsat_constraints.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_assumptions_all.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_assumptions_certain_signatures.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_constraints.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_constraints_id.lp
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_facts.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_optimization.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_rule_ids.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/res/transformed_program_rules_split.lp
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/test_muc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/test_unsat_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/clingexplaid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 16:00:07.000000 clingexplaid-1.0.9/tests/test_main.py
```

### Comparing `clingexplaid-1.0.10/.github/workflows/deploy.yml` & `clingexplaid-1.0.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/.github/workflows/test.yml` & `clingexplaid-1.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/.pre-commit-config.yaml` & `clingexplaid-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/CONTRIBUTING.md` & `clingexplaid-1.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/DEPLOYMENT.md` & `clingexplaid-1.0.9/DEPLOYMENT.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/LICENSE` & `clingexplaid-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/TODO.md` & `clingexplaid-1.0.9/TODO.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/Makefile` & `clingexplaid-1.0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/_static/css/custom.css` & `clingexplaid-1.0.9/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/_static/logo-dark-mode.png` & `clingexplaid-1.0.9/doc/_static/logo-dark-mode.png`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/_static/logo-light-mode.png` & `clingexplaid-1.0.9/doc/_static/logo-light-mode.png`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/conf.py` & `clingexplaid-1.0.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/doc/content/installation.md` & `clingexplaid-1.0.9/doc/content/installation.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/graph_coloring/README.md` & `clingexplaid-1.0.9/examples/graph_coloring/README.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/graph_coloring/graph_coloring_example.svg` & `clingexplaid-1.0.9/examples/graph_coloring/graph_coloring_example.svg`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/misc/sudoku_encoding.lp` & `clingexplaid-1.0.9/examples/misc/sudoku_encoding.lp`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/misc/x.lp` & `clingexplaid-1.0.9/examples/misc/x.lp`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/queens/README.md` & `clingexplaid-1.0.9/examples/queens/README.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/queens/queens_example.svg` & `clingexplaid-1.0.9/examples/queens/queens_example.svg`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/sudoku/README.md` & `clingexplaid-1.0.9/examples/sudoku/README.md`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/examples/sudoku/sudoku_example.svg` & `clingexplaid-1.0.9/examples/sudoku/sudoku_example.svg`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/noxfile.py` & `clingexplaid-1.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/pyproject.toml` & `clingexplaid-1.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,47 +4,28 @@
     "setuptools-scm",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clingexplaid"
 authors = [
-    { name = "Hannes Weichelt", email = "hweichelt@uni-potsdam.de" },
-    { name = "Susana Hahn", email = "susuhahnml@yahoo.com.mx" }
+    { name = "Hannes Weichelt", email = "hweichelt@uni-potsdam.de" }
 ]
-maintainers = [{ name = "Hannes Weichelt", email = "hweichelt@uni-potsdam.de" }]
-description = "Tools to aid the development of explanation systems using clingo"
+description = "A template project."
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dynamic = [ "version" ]
 readme = "README.md"
 dependencies = [
 	"clingo>=5.7.1",
     "autoflake",
 ]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed",
-]
 
 [project.urls]
-Homepage = "https://github.com/potassco/clingo-explaid"
-Source = "https://github.com/potassco/clingo-explaid"
-"Issues" = "https://github.com/potassco/clingo-explaid/issues"
+Homepage = "https://github.com/krr-up/clingo-explaid"
 
 [project.optional-dependencies]
 format = [ "black", "isort", "autoflake" ]
 lint_pylint = [ "pylint" ]
 typecheck = [ "types-setuptools", "mypy" ]
 test = [ "coverage[toml]" ]
 doc = [ "sphinx", "furo", "nbsphinx", "sphinx_copybutton", "myst-parser" ]
```

### Comparing `clingexplaid-1.0.10/src/clingexplaid/cli/clingo_app.py` & `clingexplaid-1.0.9/src/clingexplaid/cli/clingo_app.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/muc/core_computer.py` & `clingexplaid-1.0.9/src/clingexplaid/muc/core_computer.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/propagators/propagator_decision_order.py` & `clingexplaid-1.0.9/src/clingexplaid/propagators/propagator_decision_order.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/__init__.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_assumption.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_assumption.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_constraint.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_constraint.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_fact.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_fact.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_optimization_remover.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_optimization_remover.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_rule_id.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_rule_id.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/transformers/transformer_rule_splitter.py` & `clingexplaid-1.0.9/src/clingexplaid/transformers/transformer_rule_splitter.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/unsat_constraints/unsat_constraint_computer.py` & `clingexplaid-1.0.9/src/clingexplaid/unsat_constraints/unsat_constraint_computer.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/utils/__init__.py` & `clingexplaid-1.0.9/src/clingexplaid/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/utils/logging.py` & `clingexplaid-1.0.9/src/clingexplaid/utils/logging.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid/utils/parser.py` & `clingexplaid-1.0.9/src/clingexplaid/utils/parser.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/src/clingexplaid.egg-info/SOURCES.txt` & `clingexplaid-1.0.9/src/clingexplaid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.md
 CONTRIBUTING.md
 DEPLOYMENT.md
 DEVELOPMENT.md
 LICENSE
-LIMITATIONS.md
 README.md
 TODO.md
 noxfile.py
 pyproject.toml
 .github/workflows/deploy.yml
 .github/workflows/test.yml
 doc/Makefile
```

### Comparing `clingexplaid-1.0.10/tests/clingexplaid/test_muc.py` & `clingexplaid-1.0.9/tests/clingexplaid/test_muc.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/tests/clingexplaid/test_transformers.py` & `clingexplaid-1.0.9/tests/clingexplaid/test_transformers.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/tests/clingexplaid/test_unsat_constraints.py` & `clingexplaid-1.0.9/tests/clingexplaid/test_unsat_constraints.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/tests/clingexplaid/test_utils.py` & `clingexplaid-1.0.9/tests/clingexplaid/test_utils.py`

 * *Files identical despite different names*

### Comparing `clingexplaid-1.0.10/tests/test_main.py` & `clingexplaid-1.0.9/tests/test_main.py`

 * *Files identical despite different names*

