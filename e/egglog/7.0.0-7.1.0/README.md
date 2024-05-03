# Comparing `tmp/egglog-7.0.0.tar.gz` & `tmp/egglog-7.1.0.tar.gz`

## Comparing `egglog-7.0.0.tar` & `egglog-7.1.0.tar`

### file list

```diff
@@ -1,113 +1,115 @@
--rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 egglog-7.0.0/Cargo.toml
--rw-r--r--   0     1001      127     2111 2024-04-27 01:52:05.000000 egglog-7.0.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3816 2024-04-27 01:52:05.000000 egglog-7.0.0/.github/workflows/version.yml
--rw-r--r--   0     1001      127      776 2024-04-27 01:52:05.000000 egglog-7.0.0/.gitignore
--rw-r--r--   0     1001      127     1000 2024-04-27 01:52:05.000000 egglog-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      825 2024-04-27 01:52:05.000000 egglog-7.0.0/.readthedocs.yaml
--rw-r--r--   0     1001      127     1438 2024-04-27 01:52:05.000000 egglog-7.0.0/CITATION.cff
--rw-r--r--   0     1001      127     1070 2024-04-27 01:52:05.000000 egglog-7.0.0/LICENSE
--rw-r--r--   0     1001      127     1420 2024-04-27 01:52:05.000000 egglog-7.0.0/README.md
--rw-r--r--   0     1001      127      388 2024-04-27 01:52:05.000000 egglog-7.0.0/conftest.py
--rw-r--r--   0     1001      127       71 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/.gitignore
--rw-r--r--   0     1001      127      484 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/_templates/comments.html
--rw-r--r--   0     1001      127    13795 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/changelog.md
--rw-r--r--   0     1001      127     5603 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/conf.py
--rw-r--r--   0     1001      127      149 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/environment.yml
--rw-r--r--   0     1001      127       13 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/.gitignore
--rw-r--r--   0     1001      127  1093641 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_07_presentation.ipynb
--rw-r--r--   0     1001      127   114752 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_11_09_portland_state.ipynb
--rw-r--r--   0     1001      127   260924 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_11_17_pytensor.ipynb
--rw-r--r--   0     1001      127   789680 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb
--rw-r--r--   0     1001      127    72312 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure-1.png
--rw-r--r--   0     1001      127   193296 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure-2.png
--rw-r--r--   0     1001      127     8470 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure.md
--rw-r--r--   0     1001      127  1048406 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2024_03_17_community_talk.ipynb
--rw-r--r--   0     1001      127   288149 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/2024_03_17_map.svg
--rw-r--r--   0     1001      127    30290 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/big_graph.svg
--rw-r--r--   0     1001      127     1402 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/define_and_define.md
--rw-r--r--   0     1001      127   657446 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/ecosystem-graph.png
--rw-r--r--   0     1001      127   184123 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/egg.png
--rw-r--r--   0     1001      127    64006 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/indexing_pushdown.ipynb
--rw-r--r--   0     1001      127   117358 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/moa.png
--rw-r--r--   0     1001      127     1551 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/optional_values.md
--rw-r--r--   0     1001      127   420307 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation/pldi_2023_presentation.ipynb
--rw-r--r--   0     1001      127      121 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/explanation.md
--rw-r--r--   0     1001      127      807 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/how-to-guides.md
--rw-r--r--   0     1001      127     1924 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/index.md
--rw-r--r--   0     1001      127     1226 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/bindings.md
--rw-r--r--   0     1001      127      708 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/contributing.md
--rw-r--r--   0     1001      127    16713 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/egglog-translation.md
--rw-r--r--   0     1001      127     1555 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/high-level.md
--rw-r--r--   0     1001      127    11130 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/python-integration.md
--rw-r--r--   0     1001      127     1188 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference/usage.md
--rw-r--r--   0     1001      127      594 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/reference.md
--rw-r--r--   0     1001      127    75257 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/tutorials/getting-started.ipynb
--rw-r--r--   0     1001      127    14545 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/tutorials/screenshot-1.png
--rw-r--r--   0     1001      127    91888 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/tutorials/screenshot-2.png
--rw-r--r--   0     1001      127   801962 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/tutorials/sklearn.ipynb
--rw-r--r--   0     1001      127       94 2024-04-27 01:52:05.000000 egglog-7.0.0/docs/tutorials.md
--rw-r--r--   0     1001      127     2623 2024-04-27 01:52:05.000000 egglog-7.0.0/increment_version.py
--rw-r--r--   0     1001      127     5122 2024-04-27 01:52:05.000000 egglog-7.0.0/pyproject.toml
--rw-r--r--   0     1001      127      237 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/__init__.py
--rw-r--r--   0     1001      127    11062 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/bindings.pyi
--rw-r--r--   0     1001      127    11499 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/builtins.py
--rw-r--r--   0     1001      127      168 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/config.py
--rw-r--r--   0     1001      127     5971 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/conversion.py
--rw-r--r--   0     1001      127    14840 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/declarations.py
--rw-r--r--   0     1001      127    61331 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/egraph.py
--rw-r--r--   0     1001      127    17274 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/egraph_state.py
--rw-r--r--   0     1001      127      232 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/README.rst
--rw-r--r--   0     1001      127       31 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/__init__.py
--rw-r--r--   0     1001      127      695 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/bool.py
--rw-r--r--   0     1001      127      966 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/eqsat_basic.py
--rw-r--r--   0     1001      127      492 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/fib.py
--rw-r--r--   0     1001      127     8208 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/lambda_.py
--rw-r--r--   0     1001      127     4961 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/matrix.py
--rw-r--r--   0     1001      127     4042 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/ndarrays.py
--rw-r--r--   0     1001      127     2119 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/resolution.py
--rw-r--r--   0     1001      127      618 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/examples/schedule_demo.py
--rw-r--r--   0     1001      127       49 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/__init__.py
--rw-r--r--   0     1001      127    39938 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/array_api.py
--rw-r--r--   0     1001      127     1250 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/array_api_jit.py
--rw-r--r--   0     1001      127     2852 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/array_api_numba.py
--rw-r--r--   0     1001      127    19209 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/array_api_program_gen.py
--rw-r--r--   0     1001      127    11874 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/program_gen.py
--rw-r--r--   0     1001      127      749 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/exp/siu_examples.py
--rw-r--r--   0     1001      127     1305 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/graphviz_widget.py
--rw-r--r--   0     1001      127     1213 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/ipython_magic.py
--rw-r--r--   0     1001      127    16633 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/pretty.py
--rw-r--r--   0     1001      127        0 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/py.typed
--rw-r--r--   0     1001      127    18256 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/runtime.py
--rw-r--r--   0     1001      127     1853 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/thunk.py
--rw-r--r--   0     1001      127     5550 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/type_constraint_solver.py
--rw-r--r--   0     1001      127       96 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/widget.css
--rw-r--r--   0     1001      127     1971 2024-04-27 01:52:05.000000 egglog-7.0.0/python/egglog/widget.js
--rw-r--r--   0     1001      127       24 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/__init__.py
--rw-r--r--   0     1001      127     4324 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py
--rw-r--r--   0     1001      127     1978 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py
--rw-r--r--   0     1001      127     4399 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py
--rw-r--r--   0     1001      127      110 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/__snapshots__/test_program_gen/test_to_string.py
--rw-r--r--   0     1001      127      606 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/conftest.py
--rw-r--r--   0     1001      127     5485 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_array_api.py
--rw-r--r--   0     1001      127     7775 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_bindings.py
--rw-r--r--   0     1001      127     2100 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_convert.py
--rw-r--r--   0     1001      127    15870 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_high_level.py
--rw-r--r--   0     1001      127     1020 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_modules.py
--rw-r--r--   0     1001      127     4810 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_pretty.py
--rw-r--r--   0     1001      127     2178 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_program_gen.py
--rw-r--r--   0     1001      127     3552 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_py_object_sort.py
--rw-r--r--   0     1001      127     3524 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_runtime.py
--rw-r--r--   0     1001      127     1999 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_type_constraint_solver.py
--rw-r--r--   0     1001      127     1126 2024-04-27 01:52:05.000000 egglog-7.0.0/python/tests/test_typing.py
--rw-r--r--   0     1001      127       31 2024-04-27 01:52:05.000000 egglog-7.0.0/rust-toolchain.toml
--rw-r--r--   0     1001      127    22966 2024-04-27 01:52:05.000000 egglog-7.0.0/src/conversions.rs
--rw-r--r--   0     1001      127     7739 2024-04-27 01:52:05.000000 egglog-7.0.0/src/egraph.rs
--rw-r--r--   0     1001      127     1516 2024-04-27 01:52:05.000000 egglog-7.0.0/src/error.rs
--rw-r--r--   0     1001      127      945 2024-04-27 01:52:05.000000 egglog-7.0.0/src/lib.rs
--rw-r--r--   0     1001      127    18937 2024-04-27 01:52:05.000000 egglog-7.0.0/src/py_object_sort.rs
--rw-r--r--   0     1001      127     1010 2024-04-27 01:52:05.000000 egglog-7.0.0/src/serialize.rs
--rw-r--r--   0     1001      127     7878 2024-04-27 01:52:05.000000 egglog-7.0.0/src/utils.rs
--rw-r--r--   0     1001      127      323 2024-04-27 01:52:05.000000 egglog-7.0.0/stubtest_allow
--rw-r--r--   0     1001      127      464 2024-04-27 01:52:05.000000 egglog-7.0.0/test-data/unit/check-high-level.test
--rw-r--r--   0     1001      127    35195 2024-04-27 01:52:49.000000 egglog-7.0.0/Cargo.lock
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 egglog-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 egglog-7.1.0/Cargo.toml
+-rw-r--r--   0     1001      127      640 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     2147 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3872 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/workflows/version.yml
+-rw-r--r--   0     1001      127      776 2024-05-03 20:47:31.000000 egglog-7.1.0/.gitignore
+-rw-r--r--   0     1001      127     1000 2024-05-03 20:47:31.000000 egglog-7.1.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      825 2024-05-03 20:47:31.000000 egglog-7.1.0/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1438 2024-05-03 20:47:31.000000 egglog-7.1.0/CITATION.cff
+-rw-r--r--   0     1001      127     1070 2024-05-03 20:47:31.000000 egglog-7.1.0/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-05-03 20:47:31.000000 egglog-7.1.0/README.md
+-rw-r--r--   0     1001      127      388 2024-05-03 20:47:31.000000 egglog-7.1.0/conftest.py
+-rw-r--r--   0     1001      127       71 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/.gitignore
+-rw-r--r--   0     1001      127      484 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/_templates/comments.html
+-rw-r--r--   0     1001      127    14715 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/changelog.md
+-rw-r--r--   0     1001      127     5603 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/conf.py
+-rw-r--r--   0     1001      127      149 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/environment.yml
+-rw-r--r--   0     1001      127       13 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/.gitignore
+-rw-r--r--   0     1001      127  1093641 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_07_presentation.ipynb
+-rw-r--r--   0     1001      127   114752 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_09_portland_state.ipynb
+-rw-r--r--   0     1001      127   260924 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_17_pytensor.ipynb
+-rw-r--r--   0     1001      127   789680 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb
+-rw-r--r--   0     1001      127    72312 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-1.png
+-rw-r--r--   0     1001      127   193296 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-2.png
+-rw-r--r--   0     1001      127     8470 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure.md
+-rw-r--r--   0     1001      127  1048406 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2024_03_17_community_talk.ipynb
+-rw-r--r--   0     1001      127   288149 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2024_03_17_map.svg
+-rw-r--r--   0     1001      127    30290 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/big_graph.svg
+-rw-r--r--   0     1001      127     1402 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/define_and_define.md
+-rw-r--r--   0     1001      127   657446 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/ecosystem-graph.png
+-rw-r--r--   0     1001      127   184123 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/egg.png
+-rw-r--r--   0     1001      127    64006 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/indexing_pushdown.ipynb
+-rw-r--r--   0     1001      127   117358 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/moa.png
+-rw-r--r--   0     1001      127     1551 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/optional_values.md
+-rw-r--r--   0     1001      127   420307 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/pldi_2023_presentation.ipynb
+-rw-r--r--   0     1001      127      121 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation.md
+-rw-r--r--   0     1001      127      807 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/how-to-guides.md
+-rw-r--r--   0     1001      127     1924 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/index.md
+-rw-r--r--   0     1001      127     1226 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/bindings.md
+-rw-r--r--   0     1001      127      708 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/contributing.md
+-rw-r--r--   0     1001      127    16713 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/egglog-translation.md
+-rw-r--r--   0     1001      127     1555 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/high-level.md
+-rw-r--r--   0     1001      127    12708 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/python-integration.md
+-rw-r--r--   0     1001      127     1188 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/usage.md
+-rw-r--r--   0     1001      127      594 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference.md
+-rw-r--r--   0     1001      127    75257 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0     1001      127    14545 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/screenshot-1.png
+-rw-r--r--   0     1001      127    91888 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/screenshot-2.png
+-rw-r--r--   0     1001      127   801962 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/sklearn.ipynb
+-rw-r--r--   0     1001      127       94 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials.md
+-rw-r--r--   0     1001      127     2623 2024-05-03 20:47:31.000000 egglog-7.1.0/increment_version.py
+-rw-r--r--   0     1001      127     5077 2024-05-03 20:47:31.000000 egglog-7.1.0/pyproject.toml
+-rw-r--r--   0     1001      127      237 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/__init__.py
+-rw-r--r--   0     1001      127    11237 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/bindings.pyi
+-rw-r--r--   0     1001      127    12617 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/builtins.py
+-rw-r--r--   0     1001      127      168 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/config.py
+-rw-r--r--   0     1001      127     6151 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/conversion.py
+-rw-r--r--   0     1001      127    15559 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/declarations.py
+-rw-r--r--   0     1001      127    64303 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/egraph.py
+-rw-r--r--   0     1001      127    19618 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/egraph_state.py
+-rw-r--r--   0     1001      127      232 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/README.rst
+-rw-r--r--   0     1001      127       31 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/__init__.py
+-rw-r--r--   0     1001      127      695 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/bool.py
+-rw-r--r--   0     1001      127      966 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/eqsat_basic.py
+-rw-r--r--   0     1001      127      492 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/fib.py
+-rw-r--r--   0     1001      127     8208 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/lambda_.py
+-rw-r--r--   0     1001      127     4961 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/matrix.py
+-rw-r--r--   0     1001      127     4042 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/ndarrays.py
+-rw-r--r--   0     1001      127     2119 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/resolution.py
+-rw-r--r--   0     1001      127      618 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/schedule_demo.py
+-rw-r--r--   0     1001      127       49 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/__init__.py
+-rw-r--r--   0     1001      127    40040 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api.py
+-rw-r--r--   0     1001      127     1250 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_jit.py
+-rw-r--r--   0     1001      127     2852 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_numba.py
+-rw-r--r--   0     1001      127    19209 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_program_gen.py
+-rw-r--r--   0     1001      127    11874 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/program_gen.py
+-rw-r--r--   0     1001      127      749 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/siu_examples.py
+-rw-r--r--   0     1001      127     1305 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/graphviz_widget.py
+-rw-r--r--   0     1001      127     1213 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/ipython_magic.py
+-rw-r--r--   0     1001      127    18607 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/pretty.py
+-rw-r--r--   0     1001      127        0 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/py.typed
+-rw-r--r--   0     1001      127    22465 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/runtime.py
+-rw-r--r--   0     1001      127     1823 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/thunk.py
+-rw-r--r--   0     1001      127     5550 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/type_constraint_solver.py
+-rw-r--r--   0     1001      127       96 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/widget.css
+-rw-r--r--   0     1001      127     1971 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/widget.js
+-rw-r--r--   0     1001      127       24 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__init__.py
+-rw-r--r--   0     1001      127     4324 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py
+-rw-r--r--   0     1001      127     1978 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py
+-rw-r--r--   0     1001      127     4399 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py
+-rw-r--r--   0     1001      127      110 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_program_gen/test_to_string.py
+-rw-r--r--   0     1001      127      606 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/conftest.py
+-rw-r--r--   0     1001      127     5485 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_array_api.py
+-rw-r--r--   0     1001      127     7775 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_bindings.py
+-rw-r--r--   0     1001      127     2100 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_convert.py
+-rw-r--r--   0     1001      127    16272 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_high_level.py
+-rw-r--r--   0     1001      127     1020 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_modules.py
+-rw-r--r--   0     1001      127     4810 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_pretty.py
+-rw-r--r--   0     1001      127     2178 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_program_gen.py
+-rw-r--r--   0     1001      127     3552 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_py_object_sort.py
+-rw-r--r--   0     1001      127     3629 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_runtime.py
+-rw-r--r--   0     1001      127     1999 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_type_constraint_solver.py
+-rw-r--r--   0     1001      127     1126 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_typing.py
+-rw-r--r--   0     1001      127     4292 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_unstable_fn.py
+-rw-r--r--   0     1001      127       31 2024-05-03 20:47:31.000000 egglog-7.1.0/rust-toolchain.toml
+-rw-r--r--   0     1001      127    23443 2024-05-03 20:47:31.000000 egglog-7.1.0/src/conversions.rs
+-rw-r--r--   0     1001      127     7760 2024-05-03 20:47:31.000000 egglog-7.1.0/src/egraph.rs
+-rw-r--r--   0     1001      127     1516 2024-05-03 20:47:31.000000 egglog-7.1.0/src/error.rs
+-rw-r--r--   0     1001      127      945 2024-05-03 20:47:31.000000 egglog-7.1.0/src/lib.rs
+-rw-r--r--   0     1001      127    19045 2024-05-03 20:47:31.000000 egglog-7.1.0/src/py_object_sort.rs
+-rw-r--r--   0     1001      127     1010 2024-05-03 20:47:31.000000 egglog-7.1.0/src/serialize.rs
+-rw-r--r--   0     1001      127     7878 2024-05-03 20:47:31.000000 egglog-7.1.0/src/utils.rs
+-rw-r--r--   0     1001      127      323 2024-05-03 20:47:31.000000 egglog-7.1.0/stubtest_allow
+-rw-r--r--   0     1001      127      464 2024-05-03 20:47:31.000000 egglog-7.1.0/test-data/unit/check-high-level.test
+-rw-r--r--   0     1001      127    35419 2024-05-03 20:48:21.000000 egglog-7.1.0/Cargo.lock
+-rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 egglog-7.1.0/PKG-INFO
```

### Comparing `egglog-7.0.0/Cargo.toml` & `egglog-7.1.0/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [package]
 name = "egglog-python"
-version = "7.0.0"
+version = "7.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "egglog_python"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21", features = ["extension-module"] }
 
 # https://github.com/egraphs-good/egglog/compare/ceed816e9369570ffed9feeba157b19471dda70d...main
-egglog = { git = "https://github.com/egraphs-good/egglog", rev = "0113af1d6476b75d4319591cc3d675f96a71cdc5" }
+egglog = { git = "https://github.com/egraphs-good/egglog", rev = "fb4a9f114f9bb93154d6eff0dbab079b5cb4ebb6" }
 # egglog = { git = "https://github.com/oflatt/egg-smol", branch = "oflatt-fast-terms" }
 # egglog = { git = "https://github.com/saulshanabrook/egg-smol", rev = "38b3014b34399cc78887ede09c845b2a5d6c7d19" }
 egraph-serialize = { git = "https://github.com/egraphs-good/egraph-serialize", rev = "5838c036623e91540831745b1574539e01c8cb23" }
 serde_json = "*"
 pyo3-log = "0.10.0"
-log = "0.4.20"
-lalrpop-util = { version = "0.20.0", features = ["lexer"] }
+log = "0.4.21"
+lalrpop-util = { version = "0.20.2", features = ["lexer"] }
 ordered-float = "*"
-uuid = { version = "1.7.0", features = ["v4"] }
+uuid = { version = "1.8.0", features = ["v4"] }
 num-rational = "*"
 
 [package.metadata.maturin]
 name = "egglog.bindings"
 
 # Use unreleased version of egraph-serialize in egglog as well
 [patch.crates-io]
```

### Comparing `egglog-7.0.0/.github/workflows/CI.yml` & `egglog-7.1.0/.github/workflows/CI.yml`

 * *Files 9% similar despite different names*

```diff
@@ -24,57 +24,57 @@
           - "3.11"
           - "3.10"
     steps:
       - uses: actions/checkout@v4
       - uses: dtolnay/rust-toolchain@1.71.1
       - uses: Swatinem/rust-cache@v2
       - name: Setup python ${{ matrix.py }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.py }}
           cache: "pip"
       - run: pip install -e .[test]
       - run: pytest --benchmark-disable -vvv
   mypy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: dtolnay/rust-toolchain@1.71.1
       - uses: Swatinem/rust-cache@v2
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
           cache: "pip"
       - run: pip install -e .[test] mypy pre-commit
-      - run: pre-commit run --hook-stage manual mypy
-      - run: pre-commit run --hook-stage manual stubtest
+      - run: pre-commit run --hook-stage manual --all-files mypy
+      - run: pre-commit run --hook-stage manual --all-files stubtest
   benchmark:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: dtolnay/rust-toolchain@1.71.1
       - uses: Swatinem/rust-cache@v2
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
       - run: pip install -e .[test]
       - uses: CodSpeedHQ/action@v2
         with:
           token: ${{ secrets.CODSPEED_TOKEN }}
           run: pytest -vvv -n auto
   docs:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: dtolnay/rust-toolchain@1.71.1
       - uses: Swatinem/rust-cache@v2
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
           cache: "pip"
       - name: Install graphviz
         run: |
           sudo apt-get update
           sudo apt-get install -y graphviz
       - run: pip install -e .[docs] pre-commit
-      - run: pre-commit run --hook-stage manual docs
+      - run: pre-commit run --hook-stage manual --all-files docs
```

### Comparing `egglog-7.0.0/.github/workflows/version.yml` & `egglog-7.1.0/.github/workflows/version.yml`

 * *Files 6% similar despite different names*

```diff
@@ -49,72 +49,73 @@
     name: build linux
     runs-on: ubuntu-latest
     needs: [bump]
     steps:
       - uses: actions/checkout@v4
         with:
           ref: version-${{ needs.bump.outputs.version }}
-      - uses: PyO3/maturin-action@v1.40.1
+      - uses: PyO3/maturin-action@v1.42.1
         with:
           manylinux: auto
           command: build
           args: --release --sdist -o dist --find-interpreter
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-linux
           path: dist
 
   windows:
     name: build windows
     runs-on: windows-latest
     needs: [bump]
     steps:
       - uses: actions/checkout@v4
         with:
           ref: version-${{ needs.bump.outputs.version }}
-      - uses: PyO3/maturin-action@v1.40.1
+      - uses: PyO3/maturin-action@v1.42.1
         with:
           command: build
           args: --release -o dist --find-interpreter
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-windows
           path: dist
 
   macos:
     name: build macos
     runs-on: macos-latest
     needs: [bump]
     steps:
       - uses: actions/checkout@v4
         with:
           ref: version-${{ needs.bump.outputs.version }}
-      - uses: PyO3/maturin-action@v1.40.1
+      - uses: PyO3/maturin-action@v1.42.1
         with:
           command: build
           args: --release -o dist --universal2 --find-interpreter
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/') || (github.event_name == 'workflow_dispatch')
     needs: [macos, windows, linux]
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v4
         with:
-          name: wheels
+          pattern: wheels-*
+          merge-multiple: true
       - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1.40.1
+        uses: PyO3/maturin-action@v1.42.1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --skip-existing *
   tag-and-merge:
     runs-on: ubuntu-latest
```

### Comparing `egglog-7.0.0/.gitignore` & `egglog-7.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/.pre-commit-config.yaml` & `egglog-7.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/.readthedocs.yaml` & `egglog-7.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/CITATION.cff` & `egglog-7.1.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/LICENSE` & `egglog-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/README.md` & `egglog-7.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `egglog` Python wrapper
 
-[![Documentation Status](https://readthedocs.org/projects/egglog-python/badge/?version=latest)](https://egglog-python.readthedocs.io/en/latest/?badge=latest) [![Test](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![CodSpeed Badge](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://codspeed.io/egraphs-good/egglog-python)
+[![Documentation Status](https://readthedocs.org/projects/egglog-python/badge/?version=latest)](https://egglog-python.readthedocs.io/latest/?badge=latest) [![Test](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![CodSpeed Badge](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://codspeed.io/egraphs-good/egglog-python)
 
 `egglog` is a Python package that provides bindings to the Rust library [`egglog`](https://github.com/egraphs-good/egglog/),
 allowing you to use e-graphs in Python for optimization, symbolic computation, and analysis.
 
 Please see the [documentation](https://egglog-python.readthedocs.io/) for more information.
 
 Come say hello [on the e-graphs Zulip](https://egraphs.zulipchat.com/#narrow/stream/375765-egglog/) or [open an issue](https://github.com/egraphs-good/egglog-python/issues/new/choose)!
```

### Comparing `egglog-7.0.0/docs/changelog.md` & `egglog-7.1.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Changelog
 
 _This project uses semantic versioning_
 
 ## UNRELEASED
 
+## 7.1.0 (2024-05-03)
+
+## New Feaatures
+
+- Upgrade [egglog](https://github.com/egraphs-good/egglog/compare/0113af1d6476b75d4319591cc3d675f96a71cdc5...fb4a9f114f9bb93154d6eff0dbab079b5cb4ebb6) ([#143](https://github.com/egraphs-good/egglog-python/pull/143))
+  - Adds `bindings.UnstableCombinedRulset` to commands
+  - Adds `UnstableFn` sort
+- Adds support for first class functions as values using Python's built in `Callable` syntax and `partial`.
+- Adds way to combine ruleset with `r1 | r2` syntax or the experimental `unstable_combine_rulesets(*rs, name=None)` function.
+
+## Minor improvements
+
+- Fixes a bug where you could not write binary dunder methods (like `__add__`) that didn't have symetric arguments
+- Use function name as ruleset name by default when creating ruleset from function
+- Adds ability to refer to methods and property off of classes instead of only off of instances (i.e. `Math.__add__(x, y)`)
+
 ## 7.0.0 (2024-04-27)
 
 - Defers adding rules in functions until they are used, so that you can use types that are not present yet.
 - Removes ability to set custom default ruleset for egraph. Either just use the empty default ruleset or explicitly set it for every run
 - Automatically mark Python builtin operators as preserved if they must return a real Python value
 - Properly pretty print all items (rewrites, actions, exprs, etc) so that expressions are de-duplicated and state is handled correctly.
 - Add automatic releases from github manual action
```

### Comparing `egglog-7.0.0/docs/conf.py` & `egglog-7.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_07_presentation.ipynb` & `egglog-7.1.0/docs/explanation/2023_07_presentation.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_11_09_portland_state.ipynb` & `egglog-7.1.0/docs/explanation/2023_11_09_portland_state.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_11_17_pytensor.ipynb` & `egglog-7.1.0/docs/explanation/2023_11_17_pytensor.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb` & `egglog-7.1.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure-1.png` & `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-1.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure-2.png` & `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-2.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2023_12_02_congruence_closure.md` & `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2024_03_17_community_talk.ipynb` & `egglog-7.1.0/docs/explanation/2024_03_17_community_talk.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/2024_03_17_map.svg` & `egglog-7.1.0/docs/explanation/2024_03_17_map.svg`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/big_graph.svg` & `egglog-7.1.0/docs/explanation/big_graph.svg`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/define_and_define.md` & `egglog-7.1.0/docs/explanation/define_and_define.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/ecosystem-graph.png` & `egglog-7.1.0/docs/explanation/ecosystem-graph.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/egg.png` & `egglog-7.1.0/docs/explanation/egg.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/indexing_pushdown.ipynb` & `egglog-7.1.0/docs/explanation/indexing_pushdown.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/moa.png` & `egglog-7.1.0/docs/explanation/moa.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/optional_values.md` & `egglog-7.1.0/docs/explanation/optional_values.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/explanation/pldi_2023_presentation.ipynb` & `egglog-7.1.0/docs/explanation/pldi_2023_presentation.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/how-to-guides.md` & `egglog-7.1.0/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/index.md` & `egglog-7.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference/bindings.md` & `egglog-7.1.0/docs/reference/bindings.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference/contributing.md` & `egglog-7.1.0/docs/reference/contributing.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference/egglog-translation.md` & `egglog-7.1.0/docs/reference/egglog-translation.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference/high-level.md` & `egglog-7.1.0/docs/reference/high-level.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference/python-integration.md` & `egglog-7.1.0/docs/reference/python-integration.md`

 * *Files 4% similar despite different names*

```diff
@@ -384,7 +384,45 @@
 mutate_egraph
 ```
 
 Any function which mutates its first argument must return `None`. In egglog, this is translated into a function which
 returns the type of its first argument.
 
 Note that dunder methods such as `__setitem__` will automatically be marked as mutating their first argument.
+
+## Functions as Values
+
+In Python, functions are first class objects, and can be passed around as values. You can use the builtin `Callable`
+type annotation to specify that a function is expected as an argument. You can then pass egglog functions directly
+and call them with rewrite rules. For example, here is how you could define a `MathList` class which supports mapping:
+
+```{code-cell} python
+from collections.abc import Callable
+from typing import ClassVar
+
+class MathList(Expr):
+    EMPTY: ClassVar[MathList]
+
+    def append(self, x: Math) -> MathList: ...
+
+    def map(self, fn: Callable[[Math], Math]) -> MathList: ...
+
+@ruleset
+def math_list_ruleset(xs: MathList, x: Math, f: Callable[[Math], Math]):
+    yield rewrite(MathList.EMPTY.map(f)).to(MathList.EMPTY)
+    yield rewrite(xs.append(x).map(f)).to(xs.map(f).append(f(x)))
+```
+
+To support partial application, you can use the builtin `functools.partial` function:
+
+```{code-cell} python
+from functools import partial
+
+x = MathList.EMPTY.append(Math(1))
+added_two = x.map(partial(Math.__add__, Math(2)))
+
+check_eq(added_two, MathList.EMPTY.append(Math(2) + Math(1)), math_list_ruleset.saturate())
+```
+
+Note that this is all built on the [unstable function support added as a sort to egglog](https://github.com/egraphs-good/egglog/pull/348).
+While this sort is exposed directly at the high level with the `UnstableFn` class, we don't reccomend depending on it directly, and instead
+using the builtin Python type annotations. This will allow us to change the implementation in the future without breaking user code.
```

### Comparing `egglog-7.0.0/docs/reference/usage.md` & `egglog-7.1.0/docs/reference/usage.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/reference.md` & `egglog-7.1.0/docs/reference.md`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/tutorials/getting-started.ipynb` & `egglog-7.1.0/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/tutorials/screenshot-1.png` & `egglog-7.1.0/docs/tutorials/screenshot-1.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/tutorials/screenshot-2.png` & `egglog-7.1.0/docs/tutorials/screenshot-2.png`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/docs/tutorials/sklearn.ipynb` & `egglog-7.1.0/docs/tutorials/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/increment_version.py` & `egglog-7.1.0/increment_version.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/pyproject.toml` & `egglog-7.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 dependencies = ["typing-extensions", "black", "graphviz"]
 
 [project.optional-dependencies]
 
 array = [
     "scikit-learn",
     "array_api_compat",
-    "numba==0.59.0rc1",
-    "llvmlite==0.42.0rc1",
+    "numba==0.59.1",
+    "llvmlite==0.42.0",
 ]
 dev = ["pre-commit", "ruff", "mypy", "anywidget[dev]", "egglog[docs,test]"]
 
 test = [
     "pytest",
     "mypy",
     "syrupy",
@@ -193,15 +193,14 @@
 [tool.mypy]
 ignore_missing_imports = true
 warn_redundant_casts = true
 check_untyped_defs = true
 strict_equality = true
 warn_unused_configs = true
 allow_redefinition = true
-enable_incomplete_feature = ["Unpack"]
 exclude = ["__snapshots__", "_build", "^conftest.py$"]
 
 [tool.maturin]
 python-source = "python"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
```

### Comparing `egglog-7.0.0/python/egglog/bindings.pyi` & `egglog-7.1.0/python/egglog/bindings.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -490,14 +490,20 @@
 
     def __init__(self, constructor: str, inputs: list[str]) -> None: ...
 
 @final
 class PrintOverallStatistics:
     def __init__(self) -> None: ...
 
+@final
+class UnstableCombinedRuleset:
+    name: str
+    rulesets: list[str]
+    def __init__(self, name: str, rulesets: list[str]) -> None: ...
+
 _Command: TypeAlias = (
     SetOption
     | Datatype
     | Declare
     | Sort
     | Function
     | AddRuleset
@@ -517,10 +523,11 @@
     | Push
     | Pop
     | Fail
     | Include
     | CheckProof
     | Relation
     | PrintOverallStatistics
+    | UnstableCombinedRuleset
 )
 
 def termdag_term_to_expr(termdag: TermDag, term: _Term) -> _Expr: ...
```

### Comparing `egglog-7.0.0/python/egglog/builtins.py` & `egglog-7.1.0/python/egglog/builtins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # mypy: disable-error-code="empty-body"
 """
 Builtin sorts and function to egg.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generic, Protocol, TypeAlias, TypeVar, Union
+from functools import partial
+from typing import TYPE_CHECKING, Generic, Protocol, TypeAlias, TypeVar, Union, overload
+
+from typing_extensions import TypeVarTuple, Unpack
 
 from .conversion import converter
 from .egraph import Expr, Unit, function, method
+from .runtime import RuntimeFunction
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 __all__ = [
     "i64",
     "i64Like",
@@ -27,14 +31,15 @@
     "Set",
     "Vec",
     "join",
     "PyObject",
     "py_eval",
     "py_exec",
     "py_eval_fn",
+    "UnstableFn",
 ]
 
 
 class String(Expr, builtin=True):
     def __init__(self, value: str) -> None: ...
 
     @method(egg_fn="replace")
@@ -457,7 +462,42 @@
 
 
 @function(builtin=True, egg_fn="py-exec")
 def py_exec(code: StringLike, globals: object = PyObject.dict(), locals: object = PyObject.dict()) -> PyObject:
     """
     Copies the locals, execs the Python code, and returns the locals with any updates.
     """
+
+
+TS = TypeVarTuple("TS")
+
+T1 = TypeVar("T1")
+T2 = TypeVar("T2")
+T3 = TypeVar("T3")
+
+
+class UnstableFn(Expr, Generic[T, Unpack[TS]], builtin=True):
+    @overload
+    def __init__(self, f: Callable[[Unpack[TS]], T]) -> None: ...
+
+    @overload
+    def __init__(self, f: Callable[[T1, Unpack[TS]], T], _a: T1, /) -> None: ...
+
+    @overload
+    def __init__(self, f: Callable[[T1, T2, Unpack[TS]], T], _a: T1, _b: T2, /) -> None: ...
+
+    # Removing due to bug in MyPy
+    # https://github.com/python/mypy/issues/17212
+    # @overload
+    # def __init__(self, f: Callable[[T1, T2, T3, Unpack[TS]], T], _a: T1, _b: T2, _c: T3, /) -> None: ...
+
+    # etc, for partial application
+
+    @method(egg_fn="unstable-fn")
+    def __init__(self, f, *partial) -> None: ...
+
+    @method(egg_fn="unstable-app")
+    def __call__(self, *args: Unpack[TS]) -> T: ...
+
+
+converter(RuntimeFunction, UnstableFn, UnstableFn)
+converter(partial, UnstableFn, lambda p: UnstableFn(p.func, *p.args))
```

### Comparing `egglog-7.0.0/python/egglog/conversion.py` & `egglog-7.1.0/python/egglog/conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, TypeVar, cast
+from typing import TYPE_CHECKING, NewType, TypeVar, cast
 
 from .declarations import *
 from .pretty import *
 from .runtime import *
 from .thunk import *
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from .declarations import HasDeclerations
     from .egraph import Expr
 
 __all__ = ["convert", "converter", "resolve_literal", "convert_to_same_type"]
 # Mapping from (source type, target type) to and function which takes in the runtimes values of the source and return the target
-CONVERSIONS: dict[tuple[type | JustTypeRef, JustTypeRef], tuple[int, Callable]] = {}
+TypeName = NewType("TypeName", str)
+CONVERSIONS: dict[tuple[type | TypeName, TypeName], tuple[int, Callable]] = {}
 # Global declerations to store all convertable types so we can query if they have certain methods or not
 # Defer it as a thunk so we can register conversions without triggering type signature loading
 CONVERSIONS_DECLS: Callable[[], Declarations] = Thunk.value(Declarations())
 
 T = TypeVar("T")
 V = TypeVar("V", bound="Expr")
 
@@ -30,20 +31,20 @@
 
 
 def converter(from_type: type[T], to_type: type[V], fn: Callable[[T], V], cost: int = 1) -> None:
     """
     Register a converter from some type to an egglog type.
     """
     to_type_name = process_tp(to_type)
-    if not isinstance(to_type_name, JustTypeRef):
+    if not isinstance(to_type_name, str):
         raise TypeError(f"Expected return type to be a egglog type, got {to_type_name}")
     _register_converter(process_tp(from_type), to_type_name, fn, cost)
 
 
-def _register_converter(a: type | JustTypeRef, b: JustTypeRef, a_b: Callable, cost: int) -> None:
+def _register_converter(a: type | TypeName, b: TypeName, a_b: Callable, cost: int) -> None:
     """
     Registers a converter from some type to an egglog type, if not already registered.
 
     Also adds transitive converters, i.e. if registering A->B and there is already B->C, then A->C will be registered.
     Also, if registering A->B and there is already D->A, then D->B will be registered.
     """
     if a == b:
@@ -90,45 +91,48 @@
     """
     Convert a source object to the same type as the target.
     """
     tp = target.__egg_typed_expr__.tp
     return resolve_literal(tp.to_var(), source)
 
 
-def process_tp(tp: type | RuntimeClass) -> JustTypeRef | type:
+def process_tp(tp: type | RuntimeClass) -> TypeName | type:
     """
     Process a type before converting it, to add it to the global declerations and resolve to a ref.
     """
     global CONVERSIONS_DECLS
     if isinstance(tp, RuntimeClass):
         CONVERSIONS_DECLS = Thunk.fn(_combine_decls, CONVERSIONS_DECLS, tp)
-        return tp.__egg_tp__.to_just()
+        egg_tp = tp.__egg_tp__
+        if egg_tp.args:
+            raise TypeError(f"Cannot register a converter for a generic type, got {tp}")
+        return TypeName(egg_tp.name)
     return tp
 
 
 def _combine_decls(d: Callable[[], Declarations], x: HasDeclerations) -> Declarations:
     return Declarations.create(d(), x)
 
 
-def min_convertable_tp(a: object, b: object, name: str) -> JustTypeRef:
+def min_convertable_tp(a: object, b: object, name: str) -> TypeName:
     """
     Returns the minimum convertable type between a and b, that has a method `name`, raising a ConvertError if no such type exists.
     """
     decls = CONVERSIONS_DECLS()
     a_tp = _get_tp(a)
     b_tp = _get_tp(b)
     a_converts_to = {
-        to: c for ((from_, to), (c, _)) in CONVERSIONS.items() if from_ == a_tp and decls.has_method(to.name, name)
+        to: c for ((from_, to), (c, _)) in CONVERSIONS.items() if from_ == a_tp and decls.has_method(to, name)
     }
     b_converts_to = {
-        to: c for ((from_, to), (c, _)) in CONVERSIONS.items() if from_ == b_tp and decls.has_method(to.name, name)
+        to: c for ((from_, to), (c, _)) in CONVERSIONS.items() if from_ == b_tp and decls.has_method(to, name)
     }
-    if isinstance(a_tp, JustTypeRef):
+    if isinstance(a_tp, str):
         a_converts_to[a_tp] = 0
-    if isinstance(b_tp, JustTypeRef):
+    if isinstance(b_tp, str):
         b_converts_to[b_tp] = 0
     common = set(a_converts_to) & set(b_converts_to)
     if not common:
         raise ConvertError(f"Cannot convert {a_tp} and {b_tp} to a common type")
     return min(common, key=lambda tp: a_converts_to[tp] + b_converts_to[tp])
 
 
@@ -139,34 +143,35 @@
 def resolve_literal(tp: TypeOrVarRef, arg: object) -> RuntimeExpr:
     arg_type = _get_tp(arg)
 
     # If we have any type variables, dont bother trying to resolve the literal, just return the arg
     try:
         tp_just = tp.to_just()
     except NotImplementedError:
-        # If this is a var, it has to be a runtime exprssions
+        # If this is a var, it has to be a runtime expession
         assert isinstance(arg, RuntimeExpr)
         return arg
-    if arg_type == tp_just:
+    tp_name = TypeName(tp_just.name)
+    if arg_type == tp_name:
         # If the type is an egg type, it has to be a runtime expr
         assert isinstance(arg, RuntimeExpr)
         return arg
     # Try all parent types as well, if we are converting from a Python type
     for arg_type_instance in arg_type.__mro__ if isinstance(arg_type, type) else [arg_type]:
         try:
-            fn = CONVERSIONS[(cast(JustTypeRef | type, arg_type_instance), tp_just)][1]
+            fn = CONVERSIONS[(cast(TypeName | type, arg_type_instance), tp_name)][1]
         except KeyError:
             continue
         break
     else:
-        raise ConvertError(f"Cannot convert {arg_type} to {tp_just}")
+        raise ConvertError(f"Cannot convert {arg_type} to {tp_name}")
     return fn(arg)
 
 
-def _get_tp(x: object) -> JustTypeRef | type:
+def _get_tp(x: object) -> TypeName | type:
     if isinstance(x, RuntimeExpr):
-        return x.__egg_typed_expr__.tp
+        return TypeName(x.__egg_typed_expr__.tp.name)
     tp = type(x)
     # If this value has a custom metaclass, let's use that as our index instead of the type
     if type(tp) != type:
         return type(tp)
     return tp
```

### Comparing `egglog-7.0.0/python/egglog/declarations.py` & `egglog-7.1.0/python/egglog/declarations.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     "CallableRef",
     "FunctionDecl",
     "RelationDecl",
     "ConstantDecl",
     "CallableDecl",
     "VarDecl",
     "PyObjectDecl",
+    "PartialCallDecl",
     "LitType",
     "LitDecl",
     "CallDecl",
     "ExprDecl",
     "TypedExprDecl",
     "ClassDecl",
     "RulesetDecl",
+    "CombinedRulesetDecl",
     "SaturateDecl",
     "RepeatDecl",
     "SequenceDecl",
     "RunDecl",
     "ScheduleDecl",
     "EqDecl",
     "ExprFactDecl",
@@ -63,14 +65,16 @@
     "ActionDecl",
     "RewriteDecl",
     "BiRewriteDecl",
     "RuleDecl",
     "RewriteOrRuleDecl",
     "ActionCommandDecl",
     "CommandDecl",
+    "SpecialFunctions",
+    "FunctionSignature",
 ]
 
 
 @dataclass
 class DelayedDeclerations:
     __egg_decls_thunk__: Callable[[], Declarations]
 
@@ -84,17 +88,14 @@
     @property
     def __egg_decls__(self) -> Declarations: ...
 
 
 DeclerationsLike: TypeAlias = Union[HasDeclerations, None, "Declarations"]
 
 
-# TODO: Make all ClassDecls take deferred type refs, which return new decls when resolving.
-
-
 def upcast_declerations(declerations_like: Iterable[DeclerationsLike]) -> list[Declarations]:
     d = []
     for l in declerations_like:
         if l is None:
             continue
         if isinstance(l, HasDeclerations):
             d.append(l.__egg_decls__)
@@ -106,15 +107,15 @@
 
 
 @dataclass
 class Declarations:
     _functions: dict[str, FunctionDecl | RelationDecl] = field(default_factory=dict)
     _constants: dict[str, ConstantDecl] = field(default_factory=dict)
     _classes: dict[str, ClassDecl] = field(default_factory=dict)
-    _rulesets: dict[str, RulesetDecl] = field(default_factory=lambda: {"": RulesetDecl([])})
+    _rulesets: dict[str, RulesetDecl | CombinedRulesetDecl] = field(default_factory=lambda: {"": RulesetDecl([])})
 
     @classmethod
     def create(cls, *others: DeclerationsLike) -> Declarations:
         others = upcast_declerations(others)
         if not others:
             return Declarations()
         first, *rest = others
@@ -192,24 +193,29 @@
     # These have to be seperate from class_methods so that printing them can be done easily
     class_variables: dict[str, ConstantDecl] = field(default_factory=dict)
     methods: dict[str, FunctionDecl] = field(default_factory=dict)
     properties: dict[str, FunctionDecl] = field(default_factory=dict)
     preserved_methods: dict[str, Callable] = field(default_factory=dict)
 
 
-@dataclass
+@dataclass(frozen=True)
 class RulesetDecl:
     rules: list[RewriteOrRuleDecl]
 
     # Make hashable so when traversing for pretty-fying we can know which rulesets we have already
     # made into strings
     def __hash__(self) -> int:
         return hash((type(self), tuple(self.rules)))
 
 
+@dataclass(frozen=True)
+class CombinedRulesetDecl:
+    rulesets: tuple[str, ...]
+
+
 # Have two different types of type refs, one that can include vars recursively and one that cannot.
 # We only use the one with vars for classmethods and methods, and the other one for egg references as
 # well as runtime values.
 @dataclass(frozen=True)
 class JustTypeRef:
     name: str
     args: tuple[JustTypeRef, ...] = ()
@@ -312,18 +318,20 @@
     arg_types: tuple[JustTypeRef, ...]
     # List of defaults. None for any arg which doesn't have one.
     arg_defaults: tuple[ExprDecl | None, ...]
     egg_name: str | None
 
     def to_function_decl(self) -> FunctionDecl:
         return FunctionDecl(
-            arg_types=tuple(a.to_var() for a in self.arg_types),
-            arg_names=tuple(f"__{i}" for i in range(len(self.arg_types))),
-            arg_defaults=self.arg_defaults,
-            return_type=TypeRefWithVars("Unit"),
+            FunctionSignature(
+                arg_types=tuple(a.to_var() for a in self.arg_types),
+                arg_names=tuple(f"__{i}" for i in range(len(self.arg_types))),
+                arg_defaults=self.arg_defaults,
+                return_type=TypeRefWithVars("Unit"),
+            ),
             egg_name=self.egg_name,
             default=LitDecl(None),
         )
 
 
 @dataclass(frozen=True)
 class ConstantDecl:
@@ -332,56 +340,61 @@
     """
 
     type_ref: JustTypeRef
     egg_name: str | None = None
 
     def to_function_decl(self) -> FunctionDecl:
         return FunctionDecl(
-            arg_types=(),
-            arg_names=(),
-            arg_defaults=(),
-            return_type=self.type_ref.to_var(),
+            FunctionSignature(return_type=self.type_ref.to_var()),
             egg_name=self.egg_name,
         )
 
 
+# special cases for partial function creation and application, which cannot use the normal python rules
+SpecialFunctions: TypeAlias = Literal["fn-partial", "fn-app"]
+
+
 @dataclass(frozen=True)
-class FunctionDecl:
-    # All args are delayed except for relations converted to function decls
-    arg_types: tuple[TypeOrVarRef, ...]
-    arg_names: tuple[str, ...]
+class FunctionSignature:
+    arg_types: tuple[TypeOrVarRef, ...] = ()
+    arg_names: tuple[str, ...] = ()
     # List of defaults. None for any arg which doesn't have one.
-    arg_defaults: tuple[ExprDecl | None, ...]
+    arg_defaults: tuple[ExprDecl | None, ...] = ()
     # If None, then the first arg is mutated and returned
-    return_type: TypeOrVarRef | None
+    return_type: TypeOrVarRef | None = None
     var_arg_type: TypeOrVarRef | None = None
 
+    @property
+    def semantic_return_type(self) -> TypeOrVarRef:
+        """
+        The type that is returned by the function, which wil be in the first arg if it mutates it.
+        """
+        return self.return_type or self.arg_types[0]
+
+    @property
+    def mutates(self) -> bool:
+        return self.return_type is None
+
+
+@dataclass(frozen=True)
+class FunctionDecl:
+    signature: FunctionSignature | SpecialFunctions = field(default_factory=FunctionSignature)
+
     # Egg params
     builtin: bool = False
     egg_name: str | None = None
     cost: int | None = None
     default: ExprDecl | None = None
     on_merge: tuple[ActionDecl, ...] = ()
     merge: ExprDecl | None = None
     unextractable: bool = False
 
     def to_function_decl(self) -> FunctionDecl:
         return self
 
-    @property
-    def semantic_return_type(self) -> TypeOrVarRef:
-        """
-        The type that is returned by the function, which wil be in the first arg if it mutates it.
-        """
-        return self.return_type or self.arg_types[0]
-
-    @property
-    def mutates(self) -> bool:
-        return self.return_type is None
-
 
 CallableDecl: TypeAlias = RelationDecl | ConstantDecl | FunctionDecl
 
 ##
 # Expressions
 ##
 
@@ -459,15 +472,28 @@
     def __eq__(self, other: object) -> bool:
         # Override eq to use cached hash for perf
         if not isinstance(other, CallDecl):
             return False
         return hash(self) == hash(other)
 
 
-ExprDecl: TypeAlias = VarDecl | LitDecl | CallDecl | PyObjectDecl
+@dataclass(frozen=True)
+class PartialCallDecl:
+    """
+    A partially applied function aka a function sort.
+
+    Note it does not need to have any args, in which case it's just a function pointer.
+
+    Seperated from the call decl so it's clear it is translated to a `unstable-fn` call.
+    """
+
+    call: CallDecl
+
+
+ExprDecl: TypeAlias = VarDecl | LitDecl | CallDecl | PyObjectDecl | PartialCallDecl
 
 
 @dataclass(frozen=True)
 class TypedExprDecl:
     tp: JustTypeRef
     expr: ExprDecl
```

### Comparing `egglog-7.0.0/python/egglog/egraph.py` & `egglog-7.1.0/python/egglog/egraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,27 +71,29 @@
     "expr_fact",
     "action_command",
     "Schedule",
     "run",
     "seq",
     "Command",
     "simplify",
+    "unstable_combine_rulesets",
     "check",
     "GraphvizKwargs",
     "Ruleset",
     "_RewriteBuilder",
     "_BirewriteBuilder",
     "_EqBuilder",
     "_NeBuilder",
     "_SetBuilder",
     "_UnionBuilder",
     "RewriteOrRule",
     "Fact",
     "Action",
     "Command",
+    "check_eq",
 ]
 
 T = TypeVar("T")
 P = ParamSpec("P")
 TYPE = TypeVar("TYPE", bound="type[Expr]")
 CALLABLE = TypeVar("CALLABLE", bound=Callable)
 EXPR = TypeVar("EXPR", bound="Expr")
@@ -141,14 +143,31 @@
     Simplify an expression by running the schedule.
     """
     if schedule:
         return EGraph().simplify(x, schedule)
     return EGraph().extract(x)
 
 
+def check_eq(x: EXPR, y: EXPR, schedule: Schedule | None = None) -> EGraph:
+    """
+    Verifies that two expressions are equal after running the schedule.
+    """
+    egraph = EGraph()
+    x_var = egraph.let("__check_eq_x", x)
+    y_var = egraph.let("__check_eq_y", y)
+    if schedule:
+        egraph.run(schedule)
+    fact = eq(x_var).to(y_var)
+    try:
+        egraph.check(fact)
+    except bindings.EggSmolError as err:
+        raise AssertionError(f"Failed {eq(x).to(y)}\n -> {ne(egraph.extract(x)).to(egraph.extract(y))})") from err
+    return egraph
+
+
 def check(x: FactLike, schedule: Schedule | None = None, *given: ActionLike) -> None:
     """
     Verifies that the fact is true given some assumptions and after running the schedule.
     """
     egraph = EGraph()
     if given:
         egraph.register(*given)
@@ -452,15 +471,15 @@
         )
         return RuntimeClass(decls_thunk, TypeRefWithVars(name))
 
     def __instancecheck__(cls, instance: object) -> bool:
         return isinstance(instance, RuntimeExpr)
 
 
-def _generate_class_decls(
+def _generate_class_decls(  # noqa: C901
     namespace: dict[str, Any], frame: FrameType, builtin: bool, egg_sort: str | None, cls_name: str
 ) -> Declarations:
     """
     Lazy constructor for class declerations to support classes with methods whose types are not yet defined.
     """
     parameters: list[TypeVar] = (
         # Get the generic params from the orig bases generic class
@@ -514,14 +533,24 @@
                 mutates = method_name in ALWAYS_MUTATES_SELF
         if preserve:
             cls_decl.preserved_methods[method_name] = fn
             continue
         locals = frame.f_locals
 
         def create_decl(fn: object, first: Literal["cls"] | TypeRefWithVars) -> FunctionDecl:
+            special_function_name: SpecialFunctions | None = (
+                "fn-partial" if egg_fn == "unstable-fn" else "fn-app" if egg_fn == "unstable-app" else None  # noqa: B023
+            )
+            if special_function_name:
+                return FunctionDecl(
+                    special_function_name,
+                    builtin=True,
+                    egg_name=egg_fn,  # noqa: B023
+                )
+
             return _fn_decl(
                 decls,
                 egg_fn,  # noqa: B023
                 fn,
                 locals,  # noqa: B023
                 default,  # noqa: B023
                 cost,  # noqa: B023
@@ -645,14 +674,18 @@
     is_init: bool = False,
     unextractable: bool = False,
 ) -> FunctionDecl:
     if not isinstance(fn, FunctionType):
         raise NotImplementedError(f"Can only generate function decls for functions not {fn}  {type(fn)}")
 
     hint_globals = fn.__globals__.copy()
+    # Copy Callable into global if not present bc sometimes it gets automatically removed by ruff to type only block
+    # https://docs.astral.sh/ruff/rules/typing-only-standard-library-import/
+    if "Callable" not in hint_globals:
+        hint_globals["Callable"] = Callable
 
     hints = get_type_hints(fn, hint_globals, hint_locals)
 
     params = list(signature(fn).parameters.values())
 
     # If this is an init function, or a classmethod, remove the first arg name
     if is_init or first_arg == "cls":
@@ -711,19 +744,21 @@
                 RuntimeExpr.__from_value__(decls, TypedExprDecl(return_type.to_just(), VarDecl("old"))),
                 RuntimeExpr.__from_value__(decls, TypedExprDecl(return_type.to_just(), VarDecl("new"))),
             )
         )
     )
     decls.update(*merge_action)
     return FunctionDecl(
-        return_type=None if mutates_first_arg else return_type,
-        var_arg_type=var_arg_type,
-        arg_types=arg_types,
-        arg_names=tuple(t.name for t in params),
-        arg_defaults=tuple(a.__egg_typed_expr__.expr if a is not None else None for a in arg_defaults),
+        FunctionSignature(
+            return_type=None if mutates_first_arg else return_type,
+            var_arg_type=var_arg_type,
+            arg_types=arg_types,
+            arg_names=tuple(t.name for t in params),
+            arg_defaults=tuple(a.__egg_typed_expr__.expr if a is not None else None for a in arg_defaults),
+        ),
         cost=cost,
         egg_name=egg_name,
         merge=merged.__egg_typed_expr__.expr if merged is not None else None,
         unextractable=unextractable,
         builtin=is_builtin,
         default=None if default is None else default.__egg_typed_expr__.expr,
         on_merge=tuple(a.action for a in merge_action),
@@ -929,21 +964,20 @@
         """
         return self.graphviz_svg()
 
     def display(self, **kwargs: Unpack[GraphvizKwargs]) -> None:
         """
         Displays the e-graph in the notebook.
         """
-        graphviz = self.graphviz(**kwargs)
         if IN_IPYTHON:
             from IPython.display import SVG, display
 
             display(SVG(self.graphviz_svg(**kwargs)))
         else:
-            graphviz.render(view=True, format="svg", quiet=True)
+            self.graphviz(**kwargs).render(view=True, format="svg", quiet=True)
 
     def input(self, fn: Callable[..., String], path: str) -> None:
         """
         Loads a CSV file and sets it as *input, output of the function.
         """
         ref, decls = resolve_callable(fn)
         self._add_decls(decls)
@@ -1055,15 +1089,15 @@
     def extract(self, expr: EXPR, include_cost: bool = False) -> EXPR | tuple[EXPR, int]:
         """
         Extract the lowest cost expression from the egraph.
         """
         runtime_expr = to_runtime_expr(expr)
         self._add_decls(runtime_expr)
         typed_expr = runtime_expr.__egg_typed_expr__
-        extract_report = self._run_extract(typed_expr.expr, 0)
+        extract_report = self._run_extract(typed_expr, 0)
 
         if not isinstance(extract_report, bindings.Best):
             msg = "No extract report saved"
             raise ValueError(msg)  # noqa: TRY004
         (new_typed_expr,) = self._state.exprs_from_egg(extract_report.termdag, [extract_report.term], typed_expr.tp)
 
         res = cast(EXPR, RuntimeExpr.__from_value__(self.__egg_decls__, new_typed_expr))
@@ -1075,23 +1109,24 @@
         """
         Extract multiple expressions from the egraph.
         """
         runtime_expr = to_runtime_expr(expr)
         self._add_decls(runtime_expr)
         typed_expr = runtime_expr.__egg_typed_expr__
 
-        extract_report = self._run_extract(typed_expr.expr, n)
+        extract_report = self._run_extract(typed_expr, n)
         if not isinstance(extract_report, bindings.Variants):
             msg = "Wrong extract report type"
             raise ValueError(msg)  # noqa: TRY004
         new_exprs = self._state.exprs_from_egg(extract_report.termdag, extract_report.terms, typed_expr.tp)
         return [cast(EXPR, RuntimeExpr.__from_value__(self.__egg_decls__, expr)) for expr in new_exprs]
 
-    def _run_extract(self, expr: ExprDecl, n: int) -> bindings._ExtractReport:
-        expr = self._state.expr_to_egg(expr)
+    def _run_extract(self, typed_expr: TypedExprDecl, n: int) -> bindings._ExtractReport:
+        self._state.type_ref_to_egg(typed_expr.tp)
+        expr = self._state.expr_to_egg(typed_expr.expr)
         self._egraph.run_program(bindings.ActionCommand(bindings.Extract(expr, bindings.Lit(bindings.Int(n)))))
         extract_report = self._egraph.extract_report()
         if not extract_report:
             msg = "No extract report saved"
             raise ValueError(msg)
         return extract_report
 
@@ -1272,16 +1307,18 @@
     rule_or_generator: RewriteOrRule | RewriteOrRuleGenerator | None = None,
     *rules: RewriteOrRule,
     name: None | str = None,
 ) -> Ruleset:
     """
     Creates a ruleset with the following rules.
 
-    If no name is provided, one is generated based on the current module
+    If no name is provided, try using the name of the funciton.
     """
+    if isinstance(rule_or_generator, FunctionType):
+        name = name or rule_or_generator.__name__
     r = Ruleset(name)
     if rule_or_generator is not None:
         r.register(rule_or_generator, *rules, _increase_frame=True)
     return r
 
 
 @dataclass
@@ -1384,21 +1421,57 @@
 
     def __str__(self) -> str:
         return pretty_decl(self._current_egg_decls, self.__egg_ruleset__, ruleset_name=self.name)
 
     def __repr__(self) -> str:
         return str(self)
 
+    def __or__(self, other: Ruleset | UnstableCombinedRuleset) -> UnstableCombinedRuleset:
+        return unstable_combine_rulesets(self, other)
+
     # Create a unique name if we didn't pass one from the user
     @property
     def __egg_name__(self) -> str:
         return self.name or f"ruleset_{id(self)}"
 
 
 @dataclass
+class UnstableCombinedRuleset(Schedule):
+    __egg_decls_thunk__: Callable[[], Declarations] = field(init=False)
+    schedule: RunDecl = field(init=False)
+    name: str | None
+    rulesets: InitVar[list[Ruleset | UnstableCombinedRuleset]]
+
+    def __post_init__(self, rulesets: list[Ruleset | UnstableCombinedRuleset]) -> None:
+        self.schedule = RunDecl(self.__egg_name__, ())
+        self.__egg_decls_thunk__ = Thunk.fn(self._create_egg_decls, *rulesets)
+
+    @property
+    def __egg_name__(self) -> str:
+        return self.name or f"combined_ruleset_{id(self)}"
+
+    def _create_egg_decls(self, *rulesets: Ruleset | UnstableCombinedRuleset) -> Declarations:
+        decls = Declarations.create(*rulesets)
+        decls._rulesets[self.__egg_name__] = CombinedRulesetDecl(tuple(r.__egg_name__ for r in rulesets))
+        return decls
+
+    def __or__(self, other: Ruleset | UnstableCombinedRuleset) -> UnstableCombinedRuleset:
+        return unstable_combine_rulesets(self, other)
+
+
+def unstable_combine_rulesets(
+    *rulesets: Ruleset | UnstableCombinedRuleset, name: str | None = None
+) -> UnstableCombinedRuleset:
+    """
+    Combine multiple rulesets into a single ruleset.
+    """
+    return UnstableCombinedRuleset(name, list(rulesets))
+
+
+@dataclass
 class RewriteOrRule:
     __egg_decls__: Declarations
     decl: RewriteOrRuleDecl
     ruleset: Ruleset | None = None
 
     def __str__(self) -> str:
         return pretty_decl(self.__egg_decls__, self.decl)
@@ -1552,17 +1625,17 @@
 def var(name: str, bound: type[EXPR]) -> EXPR:
     """Create a new variable with the given name and type."""
     return cast(EXPR, _var(name, bound))
 
 
 def _var(name: str, bound: object) -> RuntimeExpr:
     """Create a new variable with the given name and type."""
-    if not isinstance(bound, RuntimeClass):
-        raise TypeError(f"Unexpected type {type(bound)}")
-    return RuntimeExpr.__from_value__(bound.__egg_decls__, TypedExprDecl(bound.__egg_tp__.to_just(), VarDecl(name)))
+    decls = Declarations()
+    type_ref = resolve_type_annotation(decls, bound)
+    return RuntimeExpr.__from_value__(decls, TypedExprDecl(type_ref.to_just(), VarDecl(name)))
 
 
 def vars_(names: str, bound: type[EXPR]) -> Iterable[EXPR]:
     """Create variables with the given names and type."""
     for name in names.split(" "):
         yield var(name, bound)
 
@@ -1797,16 +1870,18 @@
 
 def _rewrite_or_rule_generator(gen: RewriteOrRuleGenerator, frame: FrameType) -> Iterable[RewriteOrRule]:
     """
     Returns a thunk which will call the function with variables of the type and name of the arguments.
     """
     # Get the local scope from where the function is defined, so that we can get any type hints that are in the scope
     # but not in the globals
-
-    hints = get_type_hints(gen, gen.__globals__, frame.f_locals)
+    globals = gen.__globals__.copy()
+    if "Callable" not in globals:
+        globals["Callable"] = Callable
+    hints = get_type_hints(gen, globals, frame.f_locals)
     args = [_var(p.name, hints[p.name]) for p in signature(gen).parameters.values()]
     return list(gen(*args))  # type: ignore[misc]
 
 
 FactLike = Fact | Expr
```

### Comparing `egglog-7.0.0/python/egglog/egraph_state.py` & `egglog-7.1.0/python/egglog/egraph_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,25 +83,34 @@
             case _:
                 assert_never(schedule)
 
     def ruleset_to_egg(self, name: str) -> None:
         """
         Registers a ruleset if it's not already registered.
         """
-        if name not in self.rulesets:
-            if name:
-                self.egraph.run_program(bindings.AddRuleset(name))
-            rules = self.rulesets[name] = set()
-        else:
-            rules = self.rulesets[name]
-        for rule in self.__egg_decls__._rulesets[name].rules:
-            if rule in rules:
-                continue
-            self.egraph.run_program(self.command_to_egg(rule, name))
-            rules.add(rule)
+        match self.__egg_decls__._rulesets[name]:
+            case RulesetDecl(rules):
+                if name not in self.rulesets:
+                    if name:
+                        self.egraph.run_program(bindings.AddRuleset(name))
+                    added_rules = self.rulesets[name] = set()
+                else:
+                    added_rules = self.rulesets[name]
+                for rule in rules:
+                    if rule in added_rules:
+                        continue
+                    self.egraph.run_program(self.command_to_egg(rule, name))
+                    added_rules.add(rule)
+            case CombinedRulesetDecl(rulesets):
+                if name in self.rulesets:
+                    return
+                self.rulesets[name] = set()
+                for ruleset in rulesets:
+                    self.ruleset_to_egg(ruleset)
+                self.egraph.run_program(bindings.UnstableCombinedRuleset(name, list(rulesets)))
 
     def command_to_egg(self, cmd: CommandDecl, ruleset: str) -> bindings._Command:
         match cmd:
             case ActionCommandDecl(action):
                 return bindings.ActionCommand(self.action_to_egg(action))
             case RewriteDecl(tp, lhs, rhs, conditions) | BiRewriteDecl(tp, lhs, rhs, conditions):
                 self.type_ref_to_egg(tp)
@@ -180,19 +189,21 @@
                 # Use function decleration instead of constant b/c constants cannot be extracted
                 # https://github.com/egraphs-good/egglog/issues/334
                 self.egraph.run_program(
                     bindings.Function(bindings.FunctionDecl(egg_name, bindings.Schema([], self.type_ref_to_egg(tp))))
                 )
             case FunctionDecl():
                 if not decl.builtin:
+                    signature = decl.signature
+                    assert isinstance(signature, FunctionSignature), "Cannot turn special function to egg"
                     egg_fn_decl = bindings.FunctionDecl(
                         egg_name,
                         bindings.Schema(
-                            [self.type_ref_to_egg(a.to_just()) for a in decl.arg_types],
-                            self.type_ref_to_egg(decl.semantic_return_type.to_just()),
+                            [self.type_ref_to_egg(a.to_just()) for a in signature.arg_types],
+                            self.type_ref_to_egg(signature.semantic_return_type.to_just()),
                         ),
                         self.expr_to_egg(decl.default) if decl.default else None,
                         self.expr_to_egg(decl.merge) if decl.merge else None,
                         [self.action_to_egg(a) for a in decl.on_merge],
                         decl.cost,
                         decl.unextractable,
                     )
@@ -208,27 +219,30 @@
         try:
             return self.type_ref_to_egg_sort[ref]
         except KeyError:
             pass
         decl = self.__egg_decls__._classes[ref.name]
         self.type_ref_to_egg_sort[ref] = egg_name = decl.egg_name or _generate_type_egg_name(ref)
         if not decl.builtin or ref.args:
-            self.egraph.run_program(
-                bindings.Sort(
-                    egg_name,
-                    (
-                        (
-                            self.type_ref_to_egg(JustTypeRef(ref.name)),
-                            [bindings.Var(self.type_ref_to_egg(a)) for a in ref.args],
-                        )
-                        if ref.args
-                        else None
-                    ),
-                )
-            )
+            if ref.args:
+                if ref.name == "UnstableFn":
+                    # UnstableFn is a special case, where the rest of args are collected into a call
+                    type_args: list[bindings._Expr] = [
+                        bindings.Call(
+                            self.type_ref_to_egg(ref.args[1]),
+                            [bindings.Var(self.type_ref_to_egg(a)) for a in ref.args[2:]],
+                        ),
+                        bindings.Var(self.type_ref_to_egg(ref.args[0])),
+                    ]
+                else:
+                    type_args = [bindings.Var(self.type_ref_to_egg(a)) for a in ref.args]
+                args = (self.type_ref_to_egg(JustTypeRef(ref.name)), type_args)
+            else:
+                args = None
+            self.egraph.run_program(bindings.Sort(egg_name, args))
         # For builtin classes, let's also make sure we have the mapping of all egg fn names for class methods, because
         # these can be created even without adding them to the e-graph, like `vec-empty` which can be extracted
         # even if you never use that function.
         if decl.builtin:
             for method in decl.class_methods:
                 self.callable_ref_to_egg(ClassMethodRef(ref.name, method))
 
@@ -288,14 +302,17 @@
                 res = bindings.Lit(l)
             case CallDecl(ref, args, _):
                 egg_fn = self.callable_ref_to_egg(ref)
                 egg_args = [self.typed_expr_to_egg(a) for a in args]
                 res = bindings.Call(egg_fn, egg_args)
             case PyObjectDecl(value):
                 res = GLOBAL_PY_OBJECT_SORT.store(value)
+            case PartialCallDecl(call_decl):
+                egg_fn_call = self.expr_to_egg(call_decl)
+                res = bindings.Call("unstable-fn", [bindings.Lit(bindings.String(egg_fn_call.name)), *egg_fn_call.args])
             case _:
                 assert_never(expr_decl.expr)
 
         self.expr_to_egg_cache[expr_decl] = res
         return res
 
     def exprs_from_egg(
@@ -367,51 +384,73 @@
         elif isinstance(term, bindings.TermLit):
             value = term.value
             expr_decl = LitDecl(None if isinstance(value, bindings.Unit) else value.value)
         elif isinstance(term, bindings.TermApp):
             if term.name == "py-object":
                 call = bindings.termdag_term_to_expr(self.termdag, term)
                 expr_decl = PyObjectDecl(self.state.egraph.eval_py_object(call))
+            if term.name == "unstable-fn":
+                # Get function name
+                fn_term, *arg_terms = term.args
+                fn_value = self.resolve_term(fn_term, JustTypeRef("String"))
+                assert isinstance(fn_value.expr, LitDecl)
+                fn_name = fn_value.expr.value
+                assert isinstance(fn_name, str)
+
+                # Resolve what types the partiallied applied args are
+                assert tp.name == "UnstableFn"
+                call_decl = self.from_call(tp.args[0], bindings.TermApp(fn_name, arg_terms))
+                expr_decl = PartialCallDecl(call_decl)
             else:
                 expr_decl = self.from_call(tp, term)
         else:
             assert_never(term)
         return TypedExprDecl(tp, expr_decl)
 
-    def from_call(self, tp: JustTypeRef, term: bindings.TermApp) -> CallDecl:
+    def from_call(
+        self,
+        tp: JustTypeRef,
+        term: bindings.TermApp,  # additional_arg_tps: tuple[JustTypeRef, ...]
+    ) -> CallDecl:
         """
         Convert a call to a CallDecl.
 
         There could be Python call refs which match the call, so we need to find the correct one.
+
+        The additional_arg_tps are known types for arguments that come after the term args, used to infer types
+        for partially applied functions, where we know the types of the later args, but not of the earlier ones where
+        we have values for.
         """
         # Find the first callable ref that matches the call
         for callable_ref in self.state.egg_fn_to_callable_refs[term.name]:
             # If this is a classmethod, we might need the type params that were bound for this type
             # This could be multiple types if the classmethod is ambiguous, like map create.
             possible_types: Iterable[JustTypeRef | None]
-            fn_decl = self.decls.get_callable_decl(callable_ref).to_function_decl()
+            signature = self.decls.get_callable_decl(callable_ref).to_function_decl().signature
+            assert isinstance(signature, FunctionSignature)
             if isinstance(callable_ref, ClassMethodRef):
                 possible_types = self.state._get_possible_types(callable_ref.class_name)
                 cls_name = callable_ref.class_name
             else:
                 possible_types = [None]
                 cls_name = None
             for possible_type in possible_types:
                 tcs = TypeConstraintSolver(self.decls)
                 if possible_type and possible_type.args:
                     tcs.bind_class(possible_type)
 
                 try:
                     arg_types, bound_tp_params = tcs.infer_arg_types(
-                        fn_decl.arg_types, fn_decl.semantic_return_type, fn_decl.var_arg_type, tp, cls_name
+                        signature.arg_types, signature.semantic_return_type, signature.var_arg_type, tp, cls_name
                     )
                 except TypeConstraintError:
                     continue
-                args: list[TypedExprDecl] = []
-                for a, tp in zip(term.args, arg_types, strict=False):
-                    try:
-                        res = self.cache[a]
-                    except KeyError:
-                        res = self.cache[a] = self.from_expr(tp, self.termdag.nodes[a])
-                    args.append(res)
-                return CallDecl(callable_ref, tuple(args), bound_tp_params)
+                args = tuple(self.resolve_term(a, tp) for a, tp in zip(term.args, arg_types, strict=False))
+                return CallDecl(callable_ref, args, bound_tp_params)
         raise ValueError(f"Could not find callable ref for call {term}")
+
+    def resolve_term(self, term_id: int, tp: JustTypeRef) -> TypedExprDecl:
+        try:
+            return self.cache[term_id]
+        except KeyError:
+            res = self.cache[term_id] = self.from_expr(tp, self.termdag.nodes[term_id])
+            return res
```

### Comparing `egglog-7.0.0/python/egglog/examples/bool.py` & `egglog-7.1.0/python/egglog/examples/bool.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/eqsat_basic.py` & `egglog-7.1.0/python/egglog/examples/eqsat_basic.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/lambda_.py` & `egglog-7.1.0/python/egglog/examples/lambda_.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/matrix.py` & `egglog-7.1.0/python/egglog/examples/matrix.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/ndarrays.py` & `egglog-7.1.0/python/egglog/examples/ndarrays.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/resolution.py` & `egglog-7.1.0/python/egglog/examples/resolution.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/examples/schedule_demo.py` & `egglog-7.1.0/python/egglog/examples/schedule_demo.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/exp/array_api.py` & `egglog-7.1.0/python/egglog/exp/array_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from egglog import *
 from egglog.bindings import EggSmolError
 from egglog.runtime import RuntimeExpr
 
 from .program_gen import *
 
 if TYPE_CHECKING:
-    from collections.abc import Iterator
+    from collections.abc import Callable, Iterator
     from types import ModuleType
 
 # Pretend that exprs are numbers b/c sklearn does isinstance checks
 numbers.Integral.register(RuntimeExpr)
 
 array_api_ruleset = ruleset(name="array_api_ruleset")
 array_api_schedule = array_api_ruleset.saturate()
@@ -253,42 +253,42 @@
 
     @method(preserve=True)
     def __iter__(self) -> Iterator[Int]:
         return iter(self[Int(i)] for i in range(len(self)))
 
     def __getitem__(self, i: Int) -> Int: ...
 
-    def product(self) -> Int: ...
+    def fold(self, init: Int, f: Callable[[Int, Int], Int]) -> Int: ...
 
 
 converter(
     tuple,
     TupleInt,
     lambda x: TupleInt(convert(x[0], Int)) + convert(x[1:], TupleInt)
     if len(x) > 1
     else TupleInt(convert(x[0], Int))
     if x
     else TupleInt.EMPTY,
 )
 
 
 @array_api_ruleset.register
-def _tuple_int(ti: TupleInt, ti2: TupleInt, i: Int, i2: Int, k: i64):
+def _tuple_int(ti: TupleInt, ti2: TupleInt, i: Int, i2: Int, k: i64, f: Callable[[Int, Int], Int]):
     return [
         rewrite(ti + TupleInt.EMPTY).to(ti),
         rewrite(TupleInt(i).length()).to(Int(1)),
         rewrite((ti + ti2).length()).to(ti.length() + ti2.length()),
         rewrite(TupleInt(i)[Int(0)]).to(i),
         rewrite((TupleInt(i) + ti)[Int(0)]).to(i),
         # Rule for indexing > 0
         rule(eq(i).to((TupleInt(i2) + ti)[Int(k)]), k > 0).then(union(i).with_(ti[Int(k - 1)])),
-        # Product
-        rewrite(TupleInt(i).product()).to(i),
-        rewrite((TupleInt(i) + ti).product()).to(i * ti.product()),
-        rewrite(TupleInt.EMPTY.product()).to(Int(1)),
+        # fold
+        rewrite(TupleInt.EMPTY.fold(i, f)).to(i),
+        rewrite(TupleInt(i2).fold(i, f)).to(f(i, i2)),
+        rewrite((TupleInt(i2) + ti).fold(i, f)).to(ti.fold(f(i, i2), f)),
     ]
 
 
 class OptionalInt(Expr):
     none: ClassVar[OptionalInt]
 
     @classmethod
@@ -1342,15 +1342,15 @@
     # yield rewrite(
     #     possible_values(reshape(a.index(shape, copy), ALL_INDICES)),
     # ).to(possible_values(a.index(ALL_INDICES)))
 
 
 @array_api_ruleset.register
 def _size(x: NDArray):
-    yield rewrite(x.size).to(x.shape.product())
+    yield rewrite(x.size).to(x.shape.fold(Int(1), Int.__mul__))
 
 
 @overload
 def try_evaling(expr: Expr, prim_expr: i64) -> int: ...
 
 
 @overload
```

### Comparing `egglog-7.0.0/python/egglog/exp/array_api_jit.py` & `egglog-7.1.0/python/egglog/exp/array_api_jit.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/exp/array_api_numba.py` & `egglog-7.1.0/python/egglog/exp/array_api_numba.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/exp/array_api_program_gen.py` & `egglog-7.1.0/python/egglog/exp/array_api_program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/exp/program_gen.py` & `egglog-7.1.0/python/egglog/exp/program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/exp/siu_examples.py` & `egglog-7.1.0/python/egglog/exp/siu_examples.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/graphviz_widget.py` & `egglog-7.1.0/python/egglog/graphviz_widget.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/ipython_magic.py` & `egglog-7.1.0/python/egglog/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/pretty.py` & `egglog-7.1.0/python/egglog/pretty.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 UNARY_METHODS = {
     "__pos__": "+",
     "__neg__": "-",
     "__invert__": "~",
 }
 
-AllDecls: TypeAlias = RulesetDecl | CommandDecl | ActionDecl | FactDecl | ExprDecl | ScheduleDecl
+AllDecls: TypeAlias = RulesetDecl | CombinedRulesetDecl | CommandDecl | ActionDecl | FactDecl | ExprDecl | ScheduleDecl
 
 
 def pretty_decl(
     decls: Declarations, decl: AllDecls, *, wrapping_fn: str | None = None, ruleset_name: str | None = None
 ) -> str:
     """
     Pretty print a decleration.
@@ -102,25 +102,29 @@
     Pretty print a callable reference, using a dummy value for
     the args if the function is not in the form `f(x, ...)`.
 
     To be used in the visualization.
     """
     # Pass in three dummy args, which are the max used for any operation that
     # is not a generic function call
-    args: list[ExprDecl] = [LitDecl(ARG_STR)] * 3
+    args: list[ExprDecl] = [VarDecl(ARG_STR)] * 3
     if first_arg:
         args.insert(0, first_arg)
     res = PrettyContext(decls, defaultdict(lambda: 0))._call_inner(
         ref, args, bound_tp_params=bound_tp_params, parens=False
     )
     # Either returns a function or a function with args. If args are provided, they would just be called,
     # on the function, so return them, because they are dummies
     return res[0] if isinstance(res, tuple) else res
 
 
+# TODO: Add a different pretty callable ref that doesnt fill in wholes but instead returns the function
+# so that things like Math.__add__ will be represented properly
+
+
 @dataclass
 class TraverseContext:
     """
     State for traversing expressions (or declerations that contain expressions), so we can know how many parents each
     expression has.
     """
 
@@ -166,14 +170,18 @@
             case CallDecl(_, exprs, _):
                 for e in exprs:
                     self(e.expr)
             case RunDecl(_, until):
                 if until:
                     for f in until:
                         self(f)
+            case PartialCallDecl(c):
+                self(c)
+            case CombinedRulesetDecl(_):
+                pass
             case _:
                 assert_never(decl)
 
         self._seen.add(decl)
 
 
 @dataclass
@@ -227,14 +235,17 @@
                     case str(s):
                         return repr(s) if unwrap_lit else f"String({s!r})", "String"
                 assert_never(value)
             case VarDecl(name):
                 return name, name
             case CallDecl(_, _, _):
                 return self._call(decl, parens)
+            case PartialCallDecl(CallDecl(ref, typed_args, _)):
+                arg_strs = (_pretty_callable(ref), *(self(a.expr, parens=False, unwrap_lit=True) for a in typed_args))
+                return f"UnstableFn({', '.join(arg_strs)})", "fn"
             case PyObjectDecl(value):
                 return repr(value) if unwrap_lit else f"PyObject({value!r})", "PyObject"
             case ActionCommandDecl(action):
                 return self(action), "action"
             case RewriteDecl(_, lhs, rhs, conditions) | BiRewriteDecl(_, lhs, rhs, conditions):
                 args = ", ".join(map(self, (rhs, *conditions)))
                 fn = "rewrite" if isinstance(decl, RewriteDecl) else "birewrite"
@@ -263,14 +274,18 @@
                 first, *rest = exprs
                 return f"eq({self(first)}).to({', '.join(map(self, rest))})", "fact"
             case RulesetDecl(rules):
                 if ruleset_name:
                     return f"ruleset(name={ruleset_name!r})", f"ruleset_{ruleset_name}"
                 args = ", ".join(map(self, rules))
                 return f"ruleset({args})", "ruleset"
+            case CombinedRulesetDecl(rulesets):
+                if ruleset_name:
+                    rulesets = (*rulesets, f"name={ruleset_name!r})")
+                return f"unstable_combine_rulesets({', '.join(rulesets)})", "combined_ruleset"
             case SaturateDecl(schedule):
                 return f"{self(schedule, parens=True)}.saturate()", "schedule"
             case RepeatDecl(schedule, times):
                 return f"{self(schedule, parens=True)} * {times}", "schedule"
             case SequenceDecl(schedules):
                 if len(schedules) == 2:
                     return f"{self(schedules[0], parens=True)} + {self(schedules[1], parens=True)}", "schedule"
@@ -298,27 +313,36 @@
         args = [a.expr for a in decl.args]
         ref = decl.callable
         # Special case !=
         if decl.callable == FunctionRef("!="):
             l, r = self(args[0]), self(args[1])
             return f"ne({l}).to({r})", "Unit"
         function_decl = self.decls.get_callable_decl(ref).to_function_decl()
+        signature = function_decl.signature
+
         # Determine how many of the last arguments are defaults, by iterating from the end and comparing the arg with the default
         n_defaults = 0
-        for arg, default in zip(
-            reversed(args), reversed(function_decl.arg_defaults), strict=not function_decl.var_arg_type
-        ):
-            if arg != default:
-                break
-            n_defaults += 1
+        # Dont try counting defaults for function application
+        if isinstance(signature, FunctionSignature):
+            for arg, default in zip(
+                reversed(args), reversed(signature.arg_defaults), strict=not signature.var_arg_type
+            ):
+                if arg != default:
+                    break
+                n_defaults += 1
         if n_defaults:
             args = args[:-n_defaults]
 
-        tp_name = function_decl.semantic_return_type.name
-        if function_decl.mutates:
+        # If this is a function application, the type is the first type arg of the function object
+        if signature == "fn-app":
+            tp_name = decl.args[0].tp.args[0].name
+        else:
+            assert isinstance(signature, FunctionSignature)
+            tp_name = signature.semantic_return_type.name
+        if isinstance(signature, FunctionSignature) and signature.mutates:
             first_arg = args[0]
             expr_str = self(first_arg)
             # copy an identifier expression iff it has multiple parents (b/c then we can't mutate it directly)
             has_multiple_parents = self.parents[first_arg] > 1
             self.names[decl] = expr_name = self._name_expr(tp_name, expr_str, copy_identifier=has_multiple_parents)
             # Set the first arg to be the name of the mutated arg and return the name
             args[0] = VarDecl(expr_name)
@@ -393,14 +417,36 @@
                 name = expr_str
         else:
             name = self._generate_name(tp_name)
             self.statements.append(f"{name} = {expr_str}")
         return name
 
 
+def _pretty_callable(ref: CallableRef) -> str:
+    """
+    Returns a function call as a string.
+    """
+    match ref:
+        case FunctionRef(name):
+            return name
+        case (
+            ClassMethodRef(class_name, method_name)
+            | MethodRef(class_name, method_name)
+            | PropertyRef(class_name, method_name)
+        ):
+            return f"{class_name}.{method_name}"
+        case ConstantRef(_):
+            msg = "Constants should not be callable"
+            raise NotImplementedError(msg)
+        case ClassVariableRef(_, _):
+            msg = "Class variables should not be callable"
+            raise NotADirectoryError(msg)
+    assert_never(ref)
+
+
 def _plot_line_length(expr: object):  # pragma: no cover
     """
     Plots the number of line lengths based on different max lengths
     """
     global MAX_LINE_LENGTH, LINE_DIFFERENCE
     import altair as alt
     import pandas as pd
```

### Comparing `egglog-7.0.0/python/egglog/runtime.py` & `egglog-7.1.0/python/egglog/runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 Note that all their internal fields are prefixed with __egg_ to avoid name collisions with user code, but will end in __
 so they are not mangled by Python and can be accessed by the user.
 """
 
 from __future__ import annotations
 
-from dataclasses import dataclass
+from collections.abc import Callable
+from dataclasses import dataclass, replace
 from inspect import Parameter, Signature
 from itertools import zip_longest
 from typing import TYPE_CHECKING, NoReturn, TypeVar, Union, cast, get_args, get_origin
 
 from .declarations import *
 from .pretty import *
 from .thunk import Thunk
 from .type_constraint_solver import *
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Iterable
+    from collections.abc import Iterable
 
     from .egraph import Expr
 
 __all__ = [
     "LIT_CLASS_NAMES",
     "resolve_callable",
     "resolve_type_annotation",
@@ -56,33 +57,42 @@
     "__rxor__": "__xor__",
     "__ror__": "__or__",
 }
 
 # Set this globally so we can get access to PyObject when we have a type annotation of just object.
 # This is the only time a type annotation doesn't need to include the egglog type b/c object is top so that would be redundant statically.
 _PY_OBJECT_CLASS: RuntimeClass | None = None
+# Same for functions
+_UNSTABLE_FN_CLASS: RuntimeClass | None = None
 
 T = TypeVar("T")
 
 
 def resolve_type_annotation(decls: Declarations, tp: object) -> TypeOrVarRef:
     """
     Resolves a type object into a type reference.
+
+    Any runtime type object decls will be add to those passed in.
     """
     if isinstance(tp, TypeVar):
         return ClassTypeVarRef(tp.__name__)
     # If there is a union, then we assume the first item is the type we want, and the others are types that can be converted to that type.
     if get_origin(tp) == Union:
         first, *_rest = get_args(tp)
         return resolve_type_annotation(decls, first)
 
     # If the type is `object` then this is assumed to be a PyObjectLike, i.e. converted into a PyObject
     if tp == object:
         assert _PY_OBJECT_CLASS
         return resolve_type_annotation(decls, _PY_OBJECT_CLASS)
+    # If the type is a `Callable` then convert it into a UnstableFn
+    if get_origin(tp) == Callable:
+        assert _UNSTABLE_FN_CLASS
+        args, ret = get_args(tp)
+        return resolve_type_annotation(decls, _UNSTABLE_FN_CLASS[(ret, *args)])
     if isinstance(tp, RuntimeClass):
         decls |= tp
         return tp.__egg_tp__
     raise TypeError(f"Unexpected type annotation {tp}")
 
 
 ##
@@ -91,17 +101,19 @@
 
 
 @dataclass
 class RuntimeClass(DelayedDeclerations):
     __egg_tp__: TypeRefWithVars
 
     def __post_init__(self) -> None:
-        global _PY_OBJECT_CLASS
-        if self.__egg_tp__.name == "PyObject":
+        global _PY_OBJECT_CLASS, _UNSTABLE_FN_CLASS
+        if (name := self.__egg_tp__.name) == "PyObject":
             _PY_OBJECT_CLASS = self
+        elif name == "UnstableFn" and not self.__egg_tp__.args:
+            _UNSTABLE_FN_CLASS = self
 
     def verify(self) -> None:
         if not self.__egg_tp__.args:
             return
 
         # Raise error if we have args, but they are the wrong number
         desired_args = self.__egg_decls__.get_class_decl(self.__egg_tp__.name).type_vars
@@ -109,34 +121,56 @@
             raise ValueError(f"Expected {desired_args} type args, got {len(self.__egg_tp__.args)}")
 
     def __call__(self, *args: object, **kwargs: object) -> RuntimeExpr | None:
         """
         Create an instance of this kind by calling the __init__ classmethod
         """
         # If this is a literal type, initializing it with a literal should return a literal
-        if self.__egg_tp__.name == "PyObject":
+        if (name := self.__egg_tp__.name) == "PyObject":
             assert len(args) == 1
             return RuntimeExpr.__from_value__(
                 self.__egg_decls__, TypedExprDecl(self.__egg_tp__.to_just(), PyObjectDecl(args[0]))
             )
-        if self.__egg_tp__.name in UNARY_LIT_CLASS_NAMES:
+        if name == "UnstableFn":
+            assert not kwargs
+            fn_arg, *partial_args = args
+            del args
+            # Assumes we don't have types set for UnstableFn w/ generics, that they have to be inferred
+
+            # 1. Create a runtime function for the first arg
+            assert isinstance(fn_arg, RuntimeFunction)
+            # 2. Call it with the partial args, and use untyped vars for the rest of the args
+            res = fn_arg(*partial_args, _egg_partial_function=True)
+            assert res is not None, "Mutable partial functions not supported"
+            # 3. Use the inferred return type and inferred rest arg types as the types of the function, and
+            #    the partially applied args as the args.
+            call = (res_typed_expr := res.__egg_typed_expr__).expr
+            return_tp = res_typed_expr.tp
+            assert isinstance(call, CallDecl), "partial function must be a call"
+            n_args = len(partial_args)
+            value = PartialCallDecl(replace(call, args=call.args[:n_args]))
+            remaining_arg_types = [a.tp for a in call.args[n_args:]]
+            type_ref = JustTypeRef("UnstableFn", (return_tp, *remaining_arg_types))
+            return RuntimeExpr.__from_value__(Declarations.create(self, res), TypedExprDecl(type_ref, value))
+
+        if name in UNARY_LIT_CLASS_NAMES:
             assert len(args) == 1
             assert isinstance(args[0], int | float | str | bool)
             return RuntimeExpr.__from_value__(
                 self.__egg_decls__, TypedExprDecl(self.__egg_tp__.to_just(), LitDecl(args[0]))
             )
-        if self.__egg_tp__.name == UNIT_CLASS_NAME:
+        if name == UNIT_CLASS_NAME:
             assert len(args) == 0
             return RuntimeExpr.__from_value__(
                 self.__egg_decls__, TypedExprDecl(self.__egg_tp__.to_just(), LitDecl(None))
             )
 
         return RuntimeFunction(
-            Thunk.value(self.__egg_decls__), ClassMethodRef(self.__egg_tp__.name, "__init__"), self.__egg_tp__.to_just()
-        )(*args, **kwargs)
+            Thunk.value(self.__egg_decls__), ClassMethodRef(name, "__init__"), self.__egg_tp__.to_just()
+        )(*args, **kwargs)  # type: ignore[arg-type]
 
     def __dir__(self) -> list[str]:
         cls_decl = self.__egg_decls__.get_class_decl(self.__egg_tp__.name)
         possible_methods = (
             list(cls_decl.class_methods) + list(cls_decl.class_variables) + list(cls_decl.preserved_methods)
         )
         if "__init__" in possible_methods:
@@ -180,14 +214,20 @@
                 self.__egg_decls__,
                 TypedExprDecl(return_tp.type_ref, CallDecl(ClassVariableRef(self.__egg_tp__.name, name))),
             )
         if name in cls_decl.class_methods:
             return RuntimeFunction(
                 Thunk.value(self.__egg_decls__), ClassMethodRef(self.__egg_tp__.name, name), self.__egg_tp__.to_just()
             )
+        # allow referencing properties and methods as class variables as well
+        if name in cls_decl.properties:
+            return RuntimeFunction(Thunk.value(self.__egg_decls__), PropertyRef(self.__egg_tp__.name, name))
+        if name in cls_decl.methods:
+            return RuntimeFunction(Thunk.value(self.__egg_decls__), MethodRef(self.__egg_tp__.name, name))
+
         msg = f"Class {self.__egg_tp__.name} has no method {name}"
         if name == "__ne__":
             msg += ". Did you mean to use the ne(...).to(...)?"
         raise AttributeError(msg) from None
 
     def __str__(self) -> str:
         return str(self.__egg_tp__)
@@ -203,54 +243,85 @@
 
 @dataclass
 class RuntimeFunction(DelayedDeclerations):
     __egg_ref__: CallableRef
     # bound methods need to store RuntimeExpr not just TypedExprDecl, so they can mutate the expr if required on self
     __egg_bound__: JustTypeRef | RuntimeExpr | None = None
 
-    def __call__(self, *args: object, **kwargs: object) -> RuntimeExpr | None:
+    def __call__(self, *args: object, _egg_partial_function: bool = False, **kwargs: object) -> RuntimeExpr | None:
         from .conversion import resolve_literal
 
         if isinstance(self.__egg_bound__, RuntimeExpr):
             args = (self.__egg_bound__, *args)
-        fn_decl = self.__egg_decls__.get_callable_decl(self.__egg_ref__).to_function_decl()
+        signature = self.__egg_decls__.get_callable_decl(self.__egg_ref__).to_function_decl().signature
+        decls = self.__egg_decls__.copy()
+        # Special case function application bc we dont support variadic generics yet generally
+        if signature == "fn-app":
+            fn, *rest_args = args
+            args = tuple(rest_args)
+            assert not kwargs
+            assert isinstance(fn, RuntimeExpr)
+            decls.update(fn)
+            function_value = fn.__egg_typed_expr__
+            fn_tp = function_value.tp
+            assert fn_tp.name == "UnstableFn"
+            fn_return_tp, *fn_arg_tps = fn_tp.args
+            signature = FunctionSignature(
+                tuple(tp.to_var() for tp in fn_arg_tps),
+                tuple(f"_{i}" for i in range(len(fn_arg_tps))),
+                (None,) * len(fn_arg_tps),
+                fn_return_tp.to_var(),
+            )
+        else:
+            function_value = None
+            assert isinstance(signature, FunctionSignature)
+
         # Turn all keyword args into positional args
-        bound = callable_decl_to_signature(fn_decl, self.__egg_decls__).bind(*args, **kwargs)
+        py_signature = to_py_signature(signature, self.__egg_decls__, _egg_partial_function)
+        bound = py_signature.bind(*args, **kwargs)
+        del kwargs
         bound.apply_defaults()
         assert not bound.kwargs
-        del args, kwargs
+        args = bound.args
 
         upcasted_args = [
             resolve_literal(cast(TypeOrVarRef, tp), arg)
-            for arg, tp in zip_longest(bound.args, fn_decl.arg_types, fillvalue=fn_decl.var_arg_type)
+            for arg, tp in zip_longest(args, signature.arg_types, fillvalue=signature.var_arg_type)
         ]
-
-        decls = Declarations.create(self, *upcasted_args)
+        decls.update(*upcasted_args)
 
         tcs = TypeConstraintSolver(decls)
         bound_tp = (
             None
             if self.__egg_bound__ is None
             else self.__egg_bound__.__egg_typed_expr__.tp
             if isinstance(self.__egg_bound__, RuntimeExpr)
             else self.__egg_bound__
         )
-        if bound_tp and bound_tp.args:
+        if (
+            bound_tp
+            and bound_tp.args
+            # Don't  bind class if we have a first class function arg, b/c we don't support that yet
+            and not function_value
+        ):
             tcs.bind_class(bound_tp)
         arg_exprs = tuple(arg.__egg_typed_expr__ for arg in upcasted_args)
         arg_types = [expr.tp for expr in arg_exprs]
         cls_name = bound_tp.name if bound_tp else None
         return_tp = tcs.infer_return_type(
-            fn_decl.arg_types, fn_decl.return_type or fn_decl.arg_types[0], fn_decl.var_arg_type, arg_types, cls_name
+            signature.arg_types, signature.semantic_return_type, signature.var_arg_type, arg_types, cls_name
         )
         bound_params = cast(JustTypeRef, bound_tp).args if isinstance(self.__egg_ref__, ClassMethodRef) else None
+        # If we were using unstable-app to call a funciton, add that function back as the first arg.
+        if function_value:
+            arg_exprs = (function_value, *arg_exprs)
         expr_decl = CallDecl(self.__egg_ref__, arg_exprs, bound_params)
         typed_expr_decl = TypedExprDecl(return_tp, expr_decl)
         # If there is not return type, we are mutating the first arg
-        if not fn_decl.return_type:
+        if not signature.return_type:
             first_arg = upcasted_args[0]
             first_arg.__egg_thunk__ = Thunk.value((decls, typed_expr_decl))
             return None
         return RuntimeExpr.__from_value__(decls, typed_expr_decl)
 
     def __str__(self) -> str:
         first_arg, bound_tp_params = None, None
@@ -258,27 +329,34 @@
             case RuntimeExpr(_):
                 first_arg = self.__egg_bound__.__egg_typed_expr__.expr
             case JustTypeRef(_, args):
                 bound_tp_params = args
         return pretty_callable_ref(self.__egg_decls__, self.__egg_ref__, first_arg, bound_tp_params)
 
 
-def callable_decl_to_signature(
-    decl: FunctionDecl,
-    decls: Declarations,
-) -> Signature:
+def to_py_signature(sig: FunctionSignature, decls: Declarations, optional_args: bool) -> Signature:
+    """
+    Convert to a Python signature.
+
+    If optional_args is true, then all args will be treated as optional, as if a default was provided that makes them
+    a var with that arg name as the value.
+
+    Used for partial application to try binding a function with only some of its args.
+    """
     parameters = [
         Parameter(
             n,
             Parameter.POSITIONAL_OR_KEYWORD,
-            default=RuntimeExpr.__from_value__(decls, TypedExprDecl(t.to_just(), d)) if d else Parameter.empty,
+            default=RuntimeExpr.__from_value__(decls, TypedExprDecl(t.to_just(), d if d is not None else VarDecl(n)))
+            if d is not None or optional_args
+            else Parameter.empty,
         )
-        for n, d, t in zip(decl.arg_names, decl.arg_defaults, decl.arg_types, strict=True)
+        for n, d, t in zip(sig.arg_names, sig.arg_defaults, sig.arg_types, strict=True)
     ]
-    if isinstance(decl, FunctionDecl) and decl.var_arg_type is not None:
+    if isinstance(sig, FunctionSignature) and sig.var_arg_type is not None:
         parameters.append(Parameter("__rest", Parameter.VAR_POSITIONAL))
     return Signature(parameters)
 
 
 # All methods which should return NotImplemented if they fail to resolve
 # From https://docs.python.org/3/reference/datamodel.html
 PARTIAL_METHODS = {
@@ -408,18 +486,22 @@
         # we want to find the "best" superparent (lowest cost) of the arg types to call with it, instead of just
         # using the arg type of the self arg.
         # This is neccesary so if we add like an int to a ndarray, it will upcast the int to an ndarray, instead of vice versa.
         if __name in PARTIAL_METHODS:
             try:
                 return call_method_min_conversion(self, args[0], __name)
             except ConvertError:
-                return NotImplemented
+                # Defer raising not imeplemented in case the dunder method is not symmetrical, then
+                # we use the standard process
+                pass
         if __name in class_decl.methods:
             fn = RuntimeFunction(Thunk.value(self.__egg_decls__), MethodRef(class_name, __name), self)
-            return fn(*args, **kwargs)
+            return fn(*args, **kwargs)  # type: ignore[arg-type]
+        if __name in PARTIAL_METHODS:
+            return NotImplemented
         raise TypeError(f"{class_name!r} object does not support {__name}")
 
     setattr(RuntimeExpr, name, _special_method)
 
 # For each of the reflected binary methods, translate to the corresponding non-reflected method
 for reflected, non_reflected in REFLECTED_BINARY_METHODS.items():
 
@@ -432,16 +514,16 @@
 
 def call_method_min_conversion(slf: object, other: object, name: str) -> RuntimeExpr | None:
     from .conversion import min_convertable_tp, resolve_literal
 
     # find a minimum type that both can be converted to
     # This is so so that calls like `-0.1 * Int("x")` work by upcasting both to floats.
     min_tp = min_convertable_tp(slf, other, name)
-    slf = resolve_literal(min_tp.to_var(), slf)
-    other = resolve_literal(min_tp.to_var(), other)
+    slf = resolve_literal(TypeRefWithVars(min_tp), slf)
+    other = resolve_literal(TypeRefWithVars(min_tp), other)
     method = RuntimeFunction(Thunk.value(slf.__egg_decls__), MethodRef(slf.__egg_class_name__, name), slf)
     return method(other)
 
 
 for name in ["__bool__", "__len__", "__complex__", "__int__", "__float__", "__iter__", "__index__"]:
 
     def _preserved_method(self: RuntimeExpr, __name: str = name):
```

### Comparing `egglog-7.0.0/python/egglog/thunk.py` & `egglog-7.1.0/python/egglog/thunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from typing_extensions import ParamSpec, TypeVarTuple, Unpack
+from typing_extensions import TypeVarTuple, Unpack
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 
 __all__ = ["Thunk"]
 
 T = TypeVar("T")
-P = ParamSpec("P")
 TS = TypeVarTuple("TS")
 
 
 @dataclass
 class Thunk(Generic[T, Unpack[TS]]):
     """
     Cached delayed function call.
```

### Comparing `egglog-7.0.0/python/egglog/type_constraint_solver.py` & `egglog-7.1.0/python/egglog/type_constraint_solver.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/egglog/widget.js` & `egglog-7.1.0/python/egglog/widget.js`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py` & `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py` & `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py` & `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/conftest.py` & `egglog-7.1.0/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_array_api.py` & `egglog-7.1.0/python/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_bindings.py` & `egglog-7.1.0/python/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_convert.py` & `egglog-7.1.0/python/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_high_level.py` & `egglog-7.1.0/python/tests/test_high_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -625,7 +625,26 @@
     def second(x: AA) -> AA: ...
 
     check(
         eq(first(AA())).to(second(AA())),
         rules,
         first(AA()),
     )
+
+
+def test_access_method_on_class():
+    class A(Expr):
+        def __init__(self) -> None: ...
+
+        def b(self, x: i64Like) -> A: ...
+
+    assert expr_parts(A.b(A(), 1)) == expr_parts(A().b(1))
+
+
+def test_access_property_on_class():
+    class A(Expr):
+        def __init__(self) -> None: ...
+
+        @property
+        def b(self) -> i64: ...
+
+    assert expr_parts(A.b(A())) == expr_parts(A().b)
```

### Comparing `egglog-7.0.0/python/tests/test_modules.py` & `egglog-7.1.0/python/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_pretty.py` & `egglog-7.1.0/python/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_program_gen.py` & `egglog-7.1.0/python/tests/test_program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_py_object_sort.py` & `egglog-7.1.0/python/tests/test_py_object_sort.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_runtime.py` & `egglog-7.1.0/python/tests/test_runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def test_function_call():
     decls = Declarations(
         _classes={
             "i64": ClassDecl(),
         },
         _functions={
-            "one": FunctionDecl((), (), (), TypeRefWithVars("i64")),
+            "one": FunctionDecl(FunctionSignature(return_type=TypeRefWithVars("i64"))),
         },
     )
     one = RuntimeFunction(Thunk.value(decls), FunctionRef("one"))
     assert (
         one().__egg_typed_expr__  # type: ignore[union-attr]
         == TypedExprDecl(JustTypeRef("i64"), CallDecl(FunctionRef("one")))
     )
@@ -41,15 +41,15 @@
     K, V = ClassTypeVarRef("K"), ClassTypeVarRef("V")
     decls = Declarations(
         _classes={
             "i64": ClassDecl(),
             "unit": ClassDecl(),
             "Map": ClassDecl(
                 type_vars=("K", "V"),
-                class_methods={"create": FunctionDecl((), (), (), TypeRefWithVars("Map", (K, V)))},
+                class_methods={"create": FunctionDecl(FunctionSignature(return_type=TypeRefWithVars("Map", (K, V))))},
             ),
         },
     )
     Map = RuntimeClass(Thunk.value(decls), TypeRefWithVars("Map"))
     with pytest.raises(TypeConstraintError):
         Map.create()  # type: ignore[operator]
     i64 = RuntimeClass(Thunk.value(decls), TypeRefWithVars("i64"))
@@ -65,25 +65,26 @@
 
 def test_expr_special():
     decls = Declarations(
         _classes={
             "i64": ClassDecl(
                 methods={
                     "__add__": FunctionDecl(
-                        (TypeRefWithVars("i64"), TypeRefWithVars("i64")),
-                        (
-                            "a",
-                            "b",
-                        ),
-                        (None, None),
-                        TypeRefWithVars("i64"),
+                        FunctionSignature(
+                            (TypeRefWithVars("i64"), TypeRefWithVars("i64")),
+                            ("a", "b"),
+                            (None, None),
+                            TypeRefWithVars("i64"),
+                        )
                     )
                 },
                 class_methods={
-                    "__init__": FunctionDecl((TypeRefWithVars("i64"),), ("self",), (None,), TypeRefWithVars("i64"))
+                    "__init__": FunctionDecl(
+                        FunctionSignature((TypeRefWithVars("i64"),), ("self",), (None,), TypeRefWithVars("i64"))
+                    )
                 },
             ),
         },
     )
     i64 = RuntimeClass(Thunk.value(decls), TypeRefWithVars("i64"))
     one = i64(1)
     res = one + one  # type: ignore[operator]
```

### Comparing `egglog-7.0.0/python/tests/test_type_constraint_solver.py` & `egglog-7.1.0/python/tests/test_type_constraint_solver.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/python/tests/test_typing.py` & `egglog-7.1.0/python/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/src/conversions.rs` & `egglog-7.1.0/src/conversions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,24 @@
             },
             egglog::ast::Command::Relation {constructor, inputs} => Relation {
                 constructor: constructor.to_string(),
                 inputs: inputs.iter().map(|i| i.to_string()).collect()
             };
         PrintOverallStatistics()
             _c -> egglog::ast::Command::PrintOverallStatistics,
-            egglog::ast::Command::PrintOverallStatistics => PrintOverallStatistics {}
+            egglog::ast::Command::PrintOverallStatistics => PrintOverallStatistics {};
+        UnstableCombinedRuleset(name: String, rulesets: Vec<String>)
+            r -> egglog::ast::Command::UnstableCombinedRuleset(
+                (&r.name).into(),
+                r.rulesets.iter().map(|i| i.into()).collect()
+            ),
+            egglog::ast::Command::UnstableCombinedRuleset(name, rulesets) => UnstableCombinedRuleset {
+                name: name.to_string(),
+                rulesets: rulesets.iter().map(|i| i.to_string()).collect()
+            }
     };
     egglog::ExtractReport: "{:?}" => ExtractReport {
         Best(termdag: TermDag, cost: usize, term: Term)
             b -> egglog::ExtractReport::Best {
                 termdag: (&b.termdag).into(),
                 cost: b.cost,
                 term: (&b.term).into()
```

### Comparing `egglog-7.0.0/src/egraph.rs` & `egglog-7.1.0/src/egraph.rs`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
 
     /// Run a series of commands on the EGraph.
     /// Returns a list of strings representing the output.
     /// An EggSmolError is raised if there is problem parsing or executing.
     #[pyo3(signature=(*commands))]
     fn run_program(&mut self, commands: Vec<Command>) -> EggResult<Vec<String>> {
         let commands: Vec<egglog::ast::Command> = commands.into_iter().map(|x| x.into()).collect();
-        info!("Running commands {:?}", commands);
+        for cmd in &commands {
+            info!("{}", cmd);
+        }
         if let Some(cmds) = &mut self.cmds {
             for cmd in &commands {
                 cmds.push_str(&cmd.to_string());
                 cmds.push('\n');
             }
         }
         let res = self.egraph.run_program(commands)?;
```

### Comparing `egglog-7.0.0/src/error.rs` & `egglog-7.1.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/src/lib.rs` & `egglog-7.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/src/py_object_sort.rs` & `egglog-7.1.0/src/py_object_sort.rs`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,15 @@
     fn get_type_constraints(&self) -> Box<dyn TypeConstraint> {
         AllEqualTypeConstraint::new(self.name())
             .with_all_arguments_sort(self.i64.clone())
             .with_output_sort(self.py_object.clone())
             .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let ident = match values {
             [id] => PyObjectIdent::Unhashable(i64::load(self.i64.as_ref(), id) as usize),
             [type_hash, hash] => PyObjectIdent::Hashable(
                 i64::load(self.i64.as_ref(), type_hash) as isize,
                 i64::load(self.i64.as_ref(), hash) as isize,
             ),
             _ => unreachable!(),
@@ -299,15 +299,15 @@
                 self.py_object.clone(),
                 self.py_object.clone(),
             ],
         )
         .into_box();
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let code: Symbol = Symbol::load(self.string.as_ref(), &values[0]);
         let res_obj: PyObject = Python::with_gil(|py| {
             let globals = self.py_object.load(values[1]);
             let globals = globals.downcast_bound::<PyDict>(py).unwrap();
             let locals = self.py_object.load(values[2]);
             let locals = locals.downcast_bound::<PyDict>(py).unwrap();
             py.eval_bound(code.into(), Some(globals), Some(locals))
@@ -340,15 +340,15 @@
                 self.py_object.clone(),
                 self.py_object.clone(),
             ],
         )
         .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let code: Symbol = Symbol::load(self.string.as_ref(), &values[0]);
         let code: &str = code.into();
         let locals: PyObject = Python::with_gil(|py| {
             let globals = self.py_object.load(values[1]);
             let globals = globals.downcast_bound::<PyDict>(py).unwrap();
             let locals = self.py_object.load(values[2]);
             // Copy the locals so we can mutate them and return them
@@ -382,15 +382,15 @@
     fn get_type_constraints(&self) -> Box<dyn TypeConstraint> {
         AllEqualTypeConstraint::new(self.name())
             .with_all_arguments_sort(self.py_object.clone())
             .with_output_sort(self.py_object.clone())
             .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let dict: PyObject = Python::with_gil(|py| {
             let dict = PyDict::new_bound(py);
             // Update the dict with the key-value pairs
             for i in values.chunks_exact(2) {
                 let key = self.py_object.load(i[0]);
                 let value = self.py_object.load(i[1]);
                 dict.set_item(key, value).unwrap();
@@ -415,15 +415,15 @@
     fn get_type_constraints(&self) -> Box<dyn TypeConstraint> {
         AllEqualTypeConstraint::new(self.name())
             .with_all_arguments_sort(self.py_object.clone())
             .with_output_sort(self.py_object.clone())
             .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let dict: PyObject = Python::with_gil(|py| {
             let dict = self.py_object.load(values[0]);
             // Copy the dict so we can mutate it and return it
             let dict = dict.downcast_bound::<PyDict>(py).unwrap().copy().unwrap();
             // Update the dict with the key-value pairs
             for i in values[1..].chunks_exact(2) {
                 let key = self.py_object.load(i[0]);
@@ -451,15 +451,15 @@
     fn get_type_constraints(&self) -> Box<dyn TypeConstraint> {
         SimpleTypeConstraint::new(
             self.name(),
             vec![self.py_object.clone(), self.string.clone()],
         )
         .into_box()
     }
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let obj: String =
             Python::with_gil(|py| self.py_object.load(values[0]).extract(py).unwrap());
         let symbol: Symbol = obj.into();
         symbol.store(self.string.as_ref())
     }
 }
 
@@ -479,15 +479,15 @@
         SimpleTypeConstraint::new(
             self.name(),
             vec![self.py_object.clone(), self.bool_.clone()],
         )
         .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let obj: bool = Python::with_gil(|py| self.py_object.load(values[0]).extract(py).unwrap());
         obj.store(self.bool_.as_ref())
     }
 }
 
 /// (py-from-string <str>)
 struct FromString {
@@ -505,15 +505,15 @@
         SimpleTypeConstraint::new(
             self.name(),
             vec![self.string.clone(), self.py_object.clone()],
         )
         .into_box()
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let str = Symbol::load(self.string.as_ref(), &values[0]).to_string();
         let obj: PyObject = Python::with_gil(|py| str.into_py(py));
         Some(self.py_object.store(obj))
     }
 }
 
 // (py-from-int <int>)
@@ -532,15 +532,15 @@
         return SimpleTypeConstraint::new(
             self.name(),
             vec![self.int.clone(), self.py_object.clone()],
         )
         .into_box();
     }
 
-    fn apply(&self, values: &[Value], _egraph: &EGraph) -> Option<Value> {
+    fn apply(&self, values: &[Value], _egraph: Option<&mut EGraph>) -> Option<Value> {
         let int = i64::load(self.int.as_ref(), &values[0]);
         let obj: PyObject = Python::with_gil(|py| int.into_py(py));
         Some(self.py_object.store(obj))
     }
 }
 
 /// Runs the code in the given context with a certain path.
```

### Comparing `egglog-7.0.0/src/serialize.rs` & `egglog-7.1.0/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/src/utils.rs` & `egglog-7.1.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.0.0/Cargo.lock` & `egglog-7.1.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0862016ff20d69b84ef8247369fabf5c008a7417002411897d40ee1f4532b873"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
@@ -281,15 +281,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "675e35c02a51bb4d4618cb4885b3839ce6d1787c97b664474d9208d074742e20"
 
 [[package]]
 name = "egglog"
 version = "0.1.0"
-source = "git+https://github.com/egraphs-good/egglog?rev=0113af1d6476b75d4319591cc3d675f96a71cdc5#0113af1d6476b75d4319591cc3d675f96a71cdc5"
+source = "git+https://github.com/egraphs-good/egglog?rev=fb4a9f114f9bb93154d6eff0dbab079b5cb4ebb6#fb4a9f114f9bb93154d6eff0dbab079b5cb4ebb6"
 dependencies = [
  "clap",
  "egraph-serialize",
  "env_logger",
  "generic_symbolic_expressions",
  "hashbrown 0.14.1",
  "indexmap",
@@ -308,15 +308,15 @@
  "smallvec",
  "symbol_table",
  "thiserror",
 ]
 
 [[package]]
 name = "egglog-python"
-version = "7.0.0"
+version = "7.1.0"
 dependencies = [
  "egglog",
  "egraph-serialize",
  "lalrpop-util",
  "log",
  "num-rational",
  "ordered-float",
@@ -483,17 +483,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indexmap"
-version = "2.0.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8adf3ddd720272c6ea8bf59463c04e0f93d0bbf7c5439b691bca2987e0270897"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.1",
  "serde",
 ]
 
 [[package]]
@@ -571,28 +571,28 @@
  "ena",
  "is-terminal",
  "itertools",
  "lalrpop-util",
  "petgraph",
  "pico-args",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.7.4",
  "string_cache",
  "term",
  "tiny-keccak",
  "unicode-xid",
 ]
 
 [[package]]
 name = "lalrpop-util"
-version = "0.20.0"
+version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f35c735096c0293d313e8f2a641627472b83d01b937177fe76e5e2708d31e0d"
+checksum = "507460a910eb7b32ee961886ff48539633b788a36b65692b95f225b844c82553"
 dependencies = [
- "regex",
+ "regex-automata",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
@@ -617,23 +617,23 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
@@ -755,15 +755,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc9fc1b9e7057baba189b5c626e2d6f40681ae5b6eb064dc7c7834101ec8123a"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pest_meta"
 version = "2.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1df74e9e7ec4053ceb980e7c0c8bd3594e977fde1af91daba9c928e8e8c6708d"
@@ -814,17 +814,17 @@
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.66"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -879,35 +879,35 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -967,42 +967,48 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.1"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
- "regex-syntax",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
+name = "regex-syntax"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
@@ -1033,37 +1039,37 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1128,17 +1134,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.32"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239814284fd6f1a4ffe4ca893952cdd93c224b6a1571c9a9eadd670295c0c9e2"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1193,15 +1199,15 @@
 name = "thiserror-impl"
 version = "1.0.49"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10712f02019e9288794769fba95cd6847df9874d49d871d062172f9dd41bc4cc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
@@ -1243,17 +1249,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
```

### Comparing `egglog-7.0.0/PKG-INFO` & `egglog-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egglog
-Version: 7.0.0
+Version: 7.1.0
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,25 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions
 Requires-Dist: black
 Requires-Dist: graphviz
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: mypy; extra == 'test'
+Requires-Dist: syrupy; extra == 'test'
+Requires-Dist: egglog[array]; extra == 'test'
+Requires-Dist: pytest-codspeed; extra == 'test'
+Requires-Dist: pytest-benchmark; extra == 'test'
+Requires-Dist: pytest-xdist; extra == 'test'
+Requires-Dist: scikit-learn; extra == 'array'
+Requires-Dist: array_api_compat; extra == 'array'
+Requires-Dist: numba==0.59.1; extra == 'array'
+Requires-Dist: llvmlite==0.42.0; extra == 'array'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-gallery; extra == 'docs'
 Requires-Dist: nbconvert; extra == 'docs'
 Requires-Dist: matplotlib; extra == 'docs'
 Requires-Dist: anywidget; extra == 'docs'
@@ -32,38 +43,27 @@
 Requires-Dist: sphinxcontrib-mermaid; extra == 'docs'
 Requires-Dist: ablog; extra == 'docs'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: anywidget[dev]; extra == 'dev'
 Requires-Dist: egglog[docs,test]; extra == 'dev'
-Requires-Dist: scikit-learn; extra == 'array'
-Requires-Dist: array_api_compat; extra == 'array'
-Requires-Dist: numba==0.59.0rc1; extra == 'array'
-Requires-Dist: llvmlite==0.42.0rc1; extra == 'array'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: mypy; extra == 'test'
-Requires-Dist: syrupy; extra == 'test'
-Requires-Dist: egglog[array]; extra == 'test'
-Requires-Dist: pytest-codspeed; extra == 'test'
-Requires-Dist: pytest-benchmark; extra == 'test'
-Requires-Dist: pytest-xdist; extra == 'test'
+Provides-Extra: test
+Provides-Extra: array
 Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: array
-Provides-Extra: test
 License-File: LICENSE
 Summary: e-graphs in Python built around the the egglog rust library
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # `egglog` Python wrapper
 
-[![Documentation Status](https://readthedocs.org/projects/egglog-python/badge/?version=latest)](https://egglog-python.readthedocs.io/en/latest/?badge=latest) [![Test](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![CodSpeed Badge](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://codspeed.io/egraphs-good/egglog-python)
+[![Documentation Status](https://readthedocs.org/projects/egglog-python/badge/?version=latest)](https://egglog-python.readthedocs.io/latest/?badge=latest) [![Test](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/egraphs-good/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![CodSpeed Badge](https://img.shields.io/endpoint?url=https://codspeed.io/badge.json)](https://codspeed.io/egraphs-good/egglog-python)
 
 `egglog` is a Python package that provides bindings to the Rust library [`egglog`](https://github.com/egraphs-good/egglog/),
 allowing you to use e-graphs in Python for optimization, symbolic computation, and analysis.
 
 Please see the [documentation](https://egglog-python.readthedocs.io/) for more information.
 
 Come say hello [on the e-graphs Zulip](https://egraphs.zulipchat.com/#narrow/stream/375765-egglog/) or [open an issue](https://github.com/egraphs-good/egglog-python/issues/new/choose)!
```

