# Comparing `tmp/squlearn-0.7.1.tar.gz` & `tmp/squlearn-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squlearn-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "squlearn-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `squlearn-0.7.1.tar` & `squlearn-0.7.2.tar`

### file list

```diff
@@ -1,159 +1,161 @@
--rw-r--r--   0        0        0     5514 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2187 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      487 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      532 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/doc_checks.yml
--rw-r--r--   0        0        0      564 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/format.yml
--rw-r--r--   0        0        0      679 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1717 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      630 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0     3314 2024-04-19 13:32:49.108146 squlearn-0.7.1/.gitignore
--rw-r--r--   0        0        0     1452 2024-04-19 13:32:49.108146 squlearn-0.7.1/CITATION.cff
--rw-r--r--   0        0        0    11421 2024-04-19 13:32:49.108146 squlearn-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     3424 2024-04-19 13:32:49.108146 squlearn-0.7.1/README.md
--rw-r--r--   0        0        0      632 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/Makefile
--rw-r--r--   0        0        0      278 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/README.md
--rw-r--r--   0        0        0     4126 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0     2249 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/favicon.png
--rw-r--r--   0        0        0    12664 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/logo.png
--rw-r--r--   0        0        0    44296 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/qnn/qnn.svg
--rw-r--r--   0        0        0    36032 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/schematic.png
--rw-r--r--   0        0        0   121611 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_static/util/executor.png
--rw-r--r--   0        0        0      161 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/class.rst
--rw-r--r--   0        0        0      486 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/class_with_call.rst
--rw-r--r--   0        0        0      165 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/function.rst
--rw-r--r--   0        0        0     3542 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/conf.py
--rw-r--r--   0        0        0      146 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_kernel_digit_classification.nblink
--rw-r--r--   0        0        0       67 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_kernel_grid_search.nblink
--rw-r--r--   0        0        0      142 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_qnn_backend_mitigation.nblink
--rw-r--r--   0        0        0      148 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_quantum_bayesian_optimization.nblink
--rw-r--r--   0        0        0      223 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/examples_index.rst
--rw-r--r--   0        0        0      524 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/index.rst
--rw-r--r--   0        0        0      940 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/install/install.rst
--rw-r--r--   0        0        0     1018 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/make.bat
--rw-r--r--   0        0        0     5764 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/modules/classes.rst
--rw-r--r--   0        0        0       60 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/qiskit_settings.conf
--rw-r--r--   0        0        0      144 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/requirements.txt
--rw-r--r--   0        0        0      461 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0    10216 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/encoding_circuits.rst
--rw-r--r--   0        0        0    13519 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/executor.rst
--rw-r--r--   0        0        0    15401 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/kernel_methods.rst
--rw-r--r--   0        0        0     6098 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/observables.rst
--rw-r--r--   0        0        0    18179 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/quantum_neural_networks.rst
--rw-r--r--   0        0        0      165 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/user_guide_index.rst
--rw-r--r--   0        0        0    96711 2024-04-19 13:32:49.112146 squlearn-0.7.1/examples/encoding_circuits/layered_encoding_circuit.ipynb
--rw-r--r--   0        0        0    23998 2024-04-19 13:32:49.112146 squlearn-0.7.1/examples/encoding_circuits/pruning_example.ipynb
--rw-r--r--   0        0        0   552422 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/encoding_circuits/various_encoding_circuit.ipynb
--rw-r--r--   0        0        0     9791 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/executor/example_executor_qiskit.ipynb
--rw-r--r--   0        0        0     7553 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/integration/mlflow.ipynb
--rw-r--r--   0        0        0    40419 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_fidelity_kernel.ipynb
--rw-r--r--   0        0        0   392223 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_projected_kernel.ipynb
--rw-r--r--   0        0        0    57347 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_regularization_mitigation.ipynb
--rw-r--r--   0        0        0   132621 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpc_workflow.ipynb
--rw-r--r--   0        0        0    64202 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpr_optimization_workflow.ipynb
--rw-r--r--   0        0        0    64741 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpr_workflow.ipynb
--rw-r--r--   0        0        0    96580 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/classification_example.ipynb
--rw-r--r--   0        0        0    75008 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/example_adam.ipynb
--rw-r--r--   0        0        0    76093 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/example_minibatch.ipynb
--rw-r--r--   0        0        0   400751 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/example_qcnn_encoding_circuit.ipynb
--rw-r--r--   0        0        0   220203 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/regression_example.ipynb
--rw-r--r--   0        0        0   194050 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/regression_with_variance.ipynb
--rw-r--r--   0        0        0   147762 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/tutorials/images/encoding_circuit.png
--rw-r--r--   0        0        0    30308 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/pipeline.png
--rw-r--r--   0        0        0    97978 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/projected_quantum_kernel.png
--rw-r--r--   0        0        0   157564 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/quantum_bo.png
--rw-r--r--   0        0        0   503838 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/kernel_digit_classification.ipynb
--rw-r--r--   0        0        0   244971 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/kernel_grid_search.ipynb
--rw-r--r--   0        0        0    90619 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/kernel_regression.ipynb
--rw-r--r--   0        0        0   253985 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/qnn_backend_mitigation.ipynb
--rw-r--r--   0        0        0   745771 2024-04-19 13:32:49.136146 squlearn-0.7.1/examples/tutorials/quantum_bayesian_optimization.ipynb
--rw-r--r--   0        0        0     2034 2024-04-19 13:32:49.136146 squlearn-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      336 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/__init__.py
--rw-r--r--   0        0        0     9625 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
--rw-r--r--   0        0        0     6454 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
--rw-r--r--   0        0        0     7139 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
--rw-r--r--   0        0        0    10302 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
--rw-r--r--   0        0        0     6419 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
--rw-r--r--   0        0        0     5685 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
--rw-r--r--   0        0        0     3808 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
--rw-r--r--   0        0        0    31845 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
--rw-r--r--   0        0        0     8823 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
--rw-r--r--   0        0        0     4555 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
--rw-r--r--   0        0        0    12664 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_base.py
--rw-r--r--   0        0        0    13217 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
--rw-r--r--   0        0        0   125558 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/layered_encoding_circuit.py
--rw-r--r--   0        0        0    12914 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
--rw-r--r--   0        0        0     7106 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
--rw-r--r--   0        0        0      315 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/__init__.py
--rw-r--r--   0        0        0      161 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/__init__.py
--rw-r--r--   0        0        0    13444 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel.py
--rw-r--r--   0        0        0    12641 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
--rw-r--r--   0        0        0    15109 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_matrix_base.py
--rw-r--r--   0        0        0     1237 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_util.py
--rw-r--r--   0        0        0    28126 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/projected_quantum_kernel.py
--rw-r--r--   0        0        0     2626 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/regularization.py
--rw-r--r--   0        0        0      168 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/__init__.py
--rw-r--r--   0        0        0     5636 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qgpc.py
--rw-r--r--   0        0        0    12897 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qgpr.py
--rw-r--r--   0        0        0     9115 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qkrr.py
--rw-r--r--   0        0        0     5972 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qsvc.py
--rw-r--r--   0        0        0     5940 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qsvr.py
--rw-r--r--   0        0        0      190 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/__init__.py
--rw-r--r--   0        0        0      646 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_loss_base.py
--rw-r--r--   0        0        0     1323 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimization_base.py
--rw-r--r--   0        0        0     3675 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimizer.py
--rw-r--r--   0        0        0     2811 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/negative_log_likelihood.py
--rw-r--r--   0        0        0     2648 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/target_alignment.py
--rw-r--r--   0        0        0      579 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/__init__.py
--rw-r--r--   0        0        0    18957 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_base.py
--rw-r--r--   0        0        0    13837 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_derivatives.py
--rw-r--r--   0        0        0        0 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/__init__.py
--rw-r--r--   0        0        0     4154 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/custom_observable.py
--rw-r--r--   0        0        0     6619 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
--rw-r--r--   0        0        0     3331 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_pauli.py
--rw-r--r--   0        0        0     3449 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_probability.py
--rw-r--r--   0        0        0     4602 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_paulis.py
--rw-r--r--   0        0        0     4433 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_probabilities.py
--rw-r--r--   0        0        0      350 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/__init__.py
--rw-r--r--   0        0        0     7904 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/adam.py
--rw-r--r--   0        0        0     4606 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/approximated_gradients.py
--rw-r--r--   0        0        0     2822 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/optimizer_base.py
--rw-r--r--   0        0        0     6830 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/optimizers_wrapper.py
--rw-r--r--   0        0        0      486 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/__init__.py
--rw-r--r--   0        0        0     8625 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/barren_plateau_analysis.py
--rw-r--r--   0        0        0    12397 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/base_qnn.py
--rw-r--r--   0        0        0    28576 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/loss.py
--rw-r--r--   0        0        0     1650 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn.py
--rw-r--r--   0        0        0     4928 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_base.py
--rw-r--r--   0        0        0    38214 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_pennylane.py
--rw-r--r--   0        0        0    44856 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_qiskit.py
--rw-r--r--   0        0        0    10052 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/qnnc.py
--rw-r--r--   0        0        0     9069 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/qnnr.py
--rw-r--r--   0        0        0    19726 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/training.py
--rw-r--r--   0        0        0       92 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/util/__init__.py
--rw-r--r--   0        0        0     3841 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/util/data_preprocessing.py
--rw-r--r--   0        0        0    73387 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/executor.py
--rw-r--r--   0        0        0      548 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/__init__.py
--rw-r--r--   0        0        0    32033 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree.py
--rw-r--r--   0        0        0    17472 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree_derivative.py
--rw-r--r--   0        0        0    69544 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree_evaluate.py
--rw-r--r--   0        0        0      166 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/__init__.py
--rw-r--r--   0        0        0    24901 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_circuit.py
--rw-r--r--   0        0        0     1905 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_gates.py
--rw-r--r--   0        0        0     7776 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/qfi.py
--rw-r--r--   0        0        0     9207 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/encoding_circuit/test_layered_encoding_circuit.py
--rw-r--r--   0        0        0     6832 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qgpc.py
--rw-r--r--   0        0        0     7604 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qgpr.py
--rw-r--r--   0        0        0     6249 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qkrr.py
--rw-r--r--   0        0        0     6812 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qsvc.py
--rw-r--r--   0        0        0     6811 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qsvr.py
--rw-r--r--   0        0        0     4953 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_base_qnn.py
--rw-r--r--   0        0        0     7013 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_qnnc.py
--rw-r--r--   0        0        0     7055 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_qnnr.py
--rw-r--r--   0        0        0     6768 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_training.py
--rw-r--r--   0        0        0     5527 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/optree/test_optree_derivative.py
--rw-r--r--   0        0        0     9928 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/optree/test_optree_evaluate.py
--rw-r--r--   0        0        0     7337 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/test_executor.py
--rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 squlearn-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     5514 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2187 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      487 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      532 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/workflows/doc_checks.yml
+-rw-r--r--   0        0        0      564 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/workflows/format.yml
+-rw-r--r--   0        0        0      679 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1717 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      630 2024-05-03 11:03:32.152659 squlearn-0.7.2/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0     3314 2024-05-03 11:03:32.152659 squlearn-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1452 2024-05-03 11:03:32.152659 squlearn-0.7.2/CITATION.cff
+-rw-r--r--   0        0        0    11421 2024-05-03 11:03:32.152659 squlearn-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     3424 2024-05-03 11:03:32.152659 squlearn-0.7.2/README.md
+-rw-r--r--   0        0        0      632 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/Makefile
+-rw-r--r--   0        0        0      278 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/README.md
+-rw-r--r--   0        0        0     4126 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     2249 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/favicon.png
+-rw-r--r--   0        0        0    12664 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/logo.png
+-rw-r--r--   0        0        0    44296 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/qnn/qnn.svg
+-rw-r--r--   0        0        0    36032 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/schematic.png
+-rw-r--r--   0        0        0   121611 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_static/util/executor.png
+-rw-r--r--   0        0        0      161 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_templates/class.rst
+-rw-r--r--   0        0        0      486 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_templates/class_with_call.rst
+-rw-r--r--   0        0        0      165 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/_templates/function.rst
+-rw-r--r--   0        0        0     3568 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/conf.py
+-rw-r--r--   0        0        0      146 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/examples/example_kernel_digit_classification.nblink
+-rw-r--r--   0        0        0       67 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/examples/example_kernel_grid_search.nblink
+-rw-r--r--   0        0        0      142 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/examples/example_qnn_backend_mitigation.nblink
+-rw-r--r--   0        0        0      148 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/examples/example_quantum_bayesian_optimization.nblink
+-rw-r--r--   0        0        0      223 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/examples/examples_index.rst
+-rw-r--r--   0        0        0      524 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/index.rst
+-rw-r--r--   0        0        0      940 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/install/install.rst
+-rw-r--r--   0        0        0     1018 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/make.bat
+-rw-r--r--   0        0        0     5784 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/modules/classes.rst
+-rw-r--r--   0        0        0       60 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/qiskit_settings.conf
+-rw-r--r--   0        0        0      144 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/requirements.txt
+-rw-r--r--   0        0        0      461 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0    10216 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/encoding_circuits.rst
+-rw-r--r--   0        0        0    13519 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/executor.rst
+-rw-r--r--   0        0        0    15401 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/kernel_methods.rst
+-rw-r--r--   0        0        0     6098 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/observables.rst
+-rw-r--r--   0        0        0    18179 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/quantum_neural_networks.rst
+-rw-r--r--   0        0        0      165 2024-05-03 11:03:32.152659 squlearn-0.7.2/docs/user_guide/user_guide_index.rst
+-rw-r--r--   0        0        0    96711 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/encoding_circuits/layered_encoding_circuit.ipynb
+-rw-r--r--   0        0        0    32387 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/encoding_circuits/pruning_example.ipynb
+-rw-r--r--   0        0        0   552422 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/encoding_circuits/various_encoding_circuit.ipynb
+-rw-r--r--   0        0        0     9791 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/executor/example_executor_qiskit.ipynb
+-rw-r--r--   0        0        0     7553 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/integration/mlflow.ipynb
+-rw-r--r--   0        0        0    40419 2024-05-03 11:03:32.156659 squlearn-0.7.2/examples/kernel/example_fidelity_kernel.ipynb
+-rw-r--r--   0        0        0   392223 2024-05-03 11:03:32.160659 squlearn-0.7.2/examples/kernel/example_projected_kernel.ipynb
+-rw-r--r--   0        0        0    57347 2024-05-03 11:03:32.160659 squlearn-0.7.2/examples/kernel/example_regularization_mitigation.ipynb
+-rw-r--r--   0        0        0   132621 2024-05-03 11:03:32.160659 squlearn-0.7.2/examples/kernel/qgpc_workflow.ipynb
+-rw-r--r--   0        0        0    64202 2024-05-03 11:03:32.160659 squlearn-0.7.2/examples/kernel/qgpr_optimization_workflow.ipynb
+-rw-r--r--   0        0        0    64741 2024-05-03 11:03:32.160659 squlearn-0.7.2/examples/kernel/qgpr_workflow.ipynb
+-rw-r--r--   0        0        0    96580 2024-05-03 11:03:32.164659 squlearn-0.7.2/examples/qnn/classification_example.ipynb
+-rw-r--r--   0        0        0    75008 2024-05-03 11:03:32.164659 squlearn-0.7.2/examples/qnn/example_adam.ipynb
+-rw-r--r--   0        0        0    76093 2024-05-03 11:03:32.164659 squlearn-0.7.2/examples/qnn/example_minibatch.ipynb
+-rw-r--r--   0        0        0   530356 2024-05-03 11:03:32.164659 squlearn-0.7.2/examples/qnn/example_qcnn_encoding_circuit.ipynb
+-rw-r--r--   0        0        0   220203 2024-05-03 11:03:32.168659 squlearn-0.7.2/examples/qnn/regression_example.ipynb
+-rw-r--r--   0        0        0   194050 2024-05-03 11:03:32.168659 squlearn-0.7.2/examples/qnn/regression_with_variance.ipynb
+-rw-r--r--   0        0        0   147762 2024-05-03 11:03:32.168659 squlearn-0.7.2/examples/tutorials/images/encoding_circuit.png
+-rw-r--r--   0        0        0    30308 2024-05-03 11:03:32.168659 squlearn-0.7.2/examples/tutorials/images/pipeline.png
+-rw-r--r--   0        0        0    97978 2024-05-03 11:03:32.168659 squlearn-0.7.2/examples/tutorials/images/projected_quantum_kernel.png
+-rw-r--r--   0        0        0   157564 2024-05-03 11:03:32.172659 squlearn-0.7.2/examples/tutorials/images/quantum_bo.png
+-rw-r--r--   0        0        0   503838 2024-05-03 11:03:32.172659 squlearn-0.7.2/examples/tutorials/kernel_digit_classification.ipynb
+-rw-r--r--   0        0        0   244971 2024-05-03 11:03:32.176659 squlearn-0.7.2/examples/tutorials/kernel_grid_search.ipynb
+-rw-r--r--   0        0        0    90619 2024-05-03 11:03:32.176659 squlearn-0.7.2/examples/tutorials/kernel_regression.ipynb
+-rw-r--r--   0        0        0   253985 2024-05-03 11:03:32.176659 squlearn-0.7.2/examples/tutorials/qnn_backend_mitigation.ipynb
+-rw-r--r--   0        0        0   745771 2024-05-03 11:03:32.180659 squlearn-0.7.2/examples/tutorials/quantum_bayesian_optimization.ipynb
+-rw-r--r--   0        0        0     2084 2024-05-03 11:03:32.180659 squlearn-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/__init__.py
+-rw-r--r--   0        0        0     9625 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
+-rw-r--r--   0        0        0     6454 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
+-rw-r--r--   0        0        0     7139 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
+-rw-r--r--   0        0        0    10302 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
+-rw-r--r--   0        0        0     6419 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
+-rw-r--r--   0        0        0     5685 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
+-rw-r--r--   0        0        0     3808 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
+-rw-r--r--   0        0        0    31845 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
+-rw-r--r--   0        0        0     8823 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
+-rw-r--r--   0        0        0     4555 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
+-rw-r--r--   0        0        0    12664 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/encoding_circuit_base.py
+-rw-r--r--   0        0        0    13217 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
+-rw-r--r--   0        0        0   125558 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/layered_encoding_circuit.py
+-rw-r--r--   0        0        0    12914 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
+-rw-r--r--   0        0        0     7106 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
+-rw-r--r--   0        0        0      315 2024-05-03 11:03:32.180659 squlearn-0.7.2/src/squlearn/kernel/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/__init__.py
+-rw-r--r--   0        0        0    13571 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/fidelity_kernel.py
+-rw-r--r--   0        0        0    12642 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
+-rw-r--r--   0        0        0    15109 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/kernel_matrix_base.py
+-rw-r--r--   0        0        0     1237 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/kernel_util.py
+-rw-r--r--   0        0        0    28126 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/projected_quantum_kernel.py
+-rw-r--r--   0        0        0     2626 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/matrix/regularization.py
+-rw-r--r--   0        0        0      168 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/__init__.py
+-rw-r--r--   0        0        0     5636 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/qgpc.py
+-rw-r--r--   0        0        0    12897 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/qgpr.py
+-rw-r--r--   0        0        0     9115 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/qkrr.py
+-rw-r--r--   0        0        0     5972 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/qsvc.py
+-rw-r--r--   0        0        0     5940 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/ml/qsvr.py
+-rw-r--r--   0        0        0      190 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/__init__.py
+-rw-r--r--   0        0        0      646 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_loss_base.py
+-rw-r--r--   0        0        0     1323 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_optimization_base.py
+-rw-r--r--   0        0        0     3675 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_optimizer.py
+-rw-r--r--   0        0        0     2811 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/negative_log_likelihood.py
+-rw-r--r--   0        0        0     2648 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/kernel/optimization/target_alignment.py
+-rw-r--r--   0        0        0      579 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/__init__.py
+-rw-r--r--   0        0        0    18957 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_base.py
+-rw-r--r--   0        0        0    13837 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_derivatives.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/__init__.py
+-rw-r--r--   0        0        0     4154 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/custom_observable.py
+-rw-r--r--   0        0        0     6619 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
+-rw-r--r--   0        0        0     3331 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/single_pauli.py
+-rw-r--r--   0        0        0     3449 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/single_probability.py
+-rw-r--r--   0        0        0     4602 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/summed_paulis.py
+-rw-r--r--   0        0        0     4433 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/observables/observable_implemented/summed_probabilities.py
+-rw-r--r--   0        0        0      388 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/__init__.py
+-rw-r--r--   0        0        0     7904 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/adam.py
+-rw-r--r--   0        0        0     4606 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/approximated_gradients.py
+-rw-r--r--   0        0        0     2822 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/optimizer_base.py
+-rw-r--r--   0        0        0     6830 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/optimizers_wrapper.py
+-rw-r--r--   0        0        0    10576 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/optimizers/sglbo.py
+-rw-r--r--   0        0        0      486 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/__init__.py
+-rw-r--r--   0        0        0     8625 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/barren_plateau_analysis.py
+-rw-r--r--   0        0        0    11832 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/base_qnn.py
+-rw-r--r--   0        0        0    28576 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/loss.py
+-rw-r--r--   0        0        0     1650 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn.py
+-rw-r--r--   0        0        0     4920 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_base.py
+-rw-r--r--   0        0        0    38214 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_pennylane.py
+-rw-r--r--   0        0        0    44856 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_qiskit.py
+-rw-r--r--   0        0        0    10052 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/qnnc.py
+-rw-r--r--   0        0        0     9069 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/qnnr.py
+-rw-r--r--   0        0        0    19738 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/qnn/training.py
+-rw-r--r--   0        0        0       92 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/__init__.py
+-rw-r--r--   0        0        0     4478 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/data_preprocessing.py
+-rw-r--r--   0        0        0    73392 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/executor.py
+-rw-r--r--   0        0        0      548 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/optree/__init__.py
+-rw-r--r--   0        0        0    32033 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/optree/optree.py
+-rw-r--r--   0        0        0    17472 2024-05-03 11:03:32.184659 squlearn-0.7.2/src/squlearn/util/optree/optree_derivative.py
+-rw-r--r--   0        0        0    69544 2024-05-03 11:03:32.188659 squlearn-0.7.2/src/squlearn/util/optree/optree_evaluate.py
+-rw-r--r--   0        0        0      166 2024-05-03 11:03:32.188659 squlearn-0.7.2/src/squlearn/util/pennylane/__init__.py
+-rw-r--r--   0        0        0    26113 2024-05-03 11:03:32.188659 squlearn-0.7.2/src/squlearn/util/pennylane/pennylane_circuit.py
+-rw-r--r--   0        0        0     1905 2024-05-03 11:03:32.188659 squlearn-0.7.2/src/squlearn/util/pennylane/pennylane_gates.py
+-rw-r--r--   0        0        0     9208 2024-05-03 11:03:32.188659 squlearn-0.7.2/src/squlearn/util/qfi.py
+-rw-r--r--   0        0        0     9207 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/encoding_circuit/test_layered_encoding_circuit.py
+-rw-r--r--   0        0        0     6832 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/kernel/ml/test_qgpc.py
+-rw-r--r--   0        0        0     7604 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/kernel/ml/test_qgpr.py
+-rw-r--r--   0        0        0     6249 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/kernel/ml/test_qkrr.py
+-rw-r--r--   0        0        0     6812 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/kernel/ml/test_qsvc.py
+-rw-r--r--   0        0        0     6811 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/kernel/ml/test_qsvr.py
+-rw-r--r--   0        0        0      857 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/optimizers/test_sglbo.py
+-rw-r--r--   0        0        0     4953 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/qnn/test_base_qnn.py
+-rw-r--r--   0        0        0     7013 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/qnn/test_qnnc.py
+-rw-r--r--   0        0        0     7055 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/qnn/test_qnnr.py
+-rw-r--r--   0        0        0     6768 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/qnn/test_training.py
+-rw-r--r--   0        0        0     5527 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/util/optree/test_optree_derivative.py
+-rw-r--r--   0        0        0     9928 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/util/optree/test_optree_evaluate.py
+-rw-r--r--   0        0        0     7337 2024-05-03 11:03:32.188659 squlearn-0.7.2/tests/util/test_executor.py
+-rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 squlearn-0.7.2/PKG-INFO
```

### Comparing `squlearn-0.7.1/.github/CODE_OF_CONDUCT.md` & `squlearn-0.7.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/CONTRIBUTING.md` & `squlearn-0.7.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `squlearn-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/workflows/doc_checks.yml` & `squlearn-0.7.2/.github/workflows/doc_checks.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/workflows/format.yml` & `squlearn-0.7.2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/workflows/publish.yml` & `squlearn-0.7.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/workflows/publish_docs.yml` & `squlearn-0.7.2/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.github/workflows/tests.yaml` & `squlearn-0.7.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/.gitignore` & `squlearn-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/CITATION.cff` & `squlearn-0.7.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/LICENSE.txt` & `squlearn-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/README.md` & `squlearn-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/Makefile` & `squlearn-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/css/custom.css` & `squlearn-0.7.2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/favicon.png` & `squlearn-0.7.2/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/logo.png` & `squlearn-0.7.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/qnn/qnn.svg` & `squlearn-0.7.2/docs/_static/qnn/qnn.svg`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/schematic.png` & `squlearn-0.7.2/docs/_static/schematic.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/_static/util/executor.png` & `squlearn-0.7.2/docs/_static/util/executor.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/conf.py` & `squlearn-0.7.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,18 +102,18 @@
     "preamble": r"""
     \usepackage{braket}
     """,
 }
 
 # intersphinx
 intersphinx_mapping = {
-    "qiskit": ("https://qiskit.org/documentation/", None),
-    "qiskit-aer": ("https://qiskit.org/ecosystem/aer/", None),
+    "qiskit": ("https://docs.quantum.ibm.com/api/qiskit/", None),
+    "qiskit-aer": ("https://qiskit.github.io/qiskit-aer/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "sklearn": ("https://scikit-learn.org/stable/", None),
 }
 
-suppress_warnings = ["myst.header"]
+suppress_warnings = ["myst.header", "config.cache"]
 
 # base URL for sphinx_sitemap
 html_baseurl = "https://squlearn.github.io/"
 sitemap_url_scheme = "{link}"
```

### Comparing `squlearn-0.7.1/docs/index.rst` & `squlearn-0.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/install/install.rst` & `squlearn-0.7.2/docs/install/install.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/make.bat` & `squlearn-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/modules/classes.rst` & `squlearn-0.7.2/docs/modules/classes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,15 @@
    :toctree: generated/
    :template: class.rst
 
    optimizers.Adam
    optimizers.LBFGSB
    optimizers.SLSQP
    optimizers.SPSA
+   optimizers.SGLBO
 
 OpTree Data Structure
 ------------------------------------
 
 .. currentmodule:: squlearn
 
 .. autosummary::
```

### Comparing `squlearn-0.7.1/docs/user_guide/encoding_circuits.rst` & `squlearn-0.7.2/docs/user_guide/encoding_circuits.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/user_guide/executor.rst` & `squlearn-0.7.2/docs/user_guide/executor.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/user_guide/kernel_methods.rst` & `squlearn-0.7.2/docs/user_guide/kernel_methods.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/user_guide/observables.rst` & `squlearn-0.7.2/docs/user_guide/observables.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/docs/user_guide/quantum_neural_networks.rst` & `squlearn-0.7.2/docs/user_guide/quantum_neural_networks.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/encoding_circuits/layered_encoding_circuit.ipynb` & `squlearn-0.7.2/examples/encoding_circuits/layered_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/encoding_circuits/various_encoding_circuit.ipynb` & `squlearn-0.7.2/examples/encoding_circuits/various_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/executor/example_executor_qiskit.ipynb` & `squlearn-0.7.2/examples/executor/example_executor_qiskit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/integration/mlflow.ipynb` & `squlearn-0.7.2/examples/integration/mlflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/example_fidelity_kernel.ipynb` & `squlearn-0.7.2/examples/kernel/example_fidelity_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/example_projected_kernel.ipynb` & `squlearn-0.7.2/examples/kernel/example_projected_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/example_regularization_mitigation.ipynb` & `squlearn-0.7.2/examples/kernel/example_regularization_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/qgpc_workflow.ipynb` & `squlearn-0.7.2/examples/kernel/qgpc_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/qgpr_optimization_workflow.ipynb` & `squlearn-0.7.2/examples/kernel/qgpr_optimization_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/kernel/qgpr_workflow.ipynb` & `squlearn-0.7.2/examples/kernel/qgpr_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/qnn/classification_example.ipynb` & `squlearn-0.7.2/examples/qnn/classification_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/qnn/example_adam.ipynb` & `squlearn-0.7.2/examples/qnn/example_adam.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/qnn/example_minibatch.ipynb` & `squlearn-0.7.2/examples/qnn/example_minibatch.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/qnn/regression_example.ipynb` & `squlearn-0.7.2/examples/qnn/regression_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/qnn/regression_with_variance.ipynb` & `squlearn-0.7.2/examples/qnn/regression_with_variance.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/images/encoding_circuit.png` & `squlearn-0.7.2/examples/tutorials/images/encoding_circuit.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/images/pipeline.png` & `squlearn-0.7.2/examples/tutorials/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/images/projected_quantum_kernel.png` & `squlearn-0.7.2/examples/tutorials/images/projected_quantum_kernel.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/images/quantum_bo.png` & `squlearn-0.7.2/examples/tutorials/images/quantum_bo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/kernel_digit_classification.ipynb` & `squlearn-0.7.2/examples/tutorials/kernel_digit_classification.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/kernel_grid_search.ipynb` & `squlearn-0.7.2/examples/tutorials/kernel_grid_search.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/kernel_regression.ipynb` & `squlearn-0.7.2/examples/tutorials/kernel_regression.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/qnn_backend_mitigation.ipynb` & `squlearn-0.7.2/examples/tutorials/qnn_backend_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/examples/tutorials/quantum_bayesian_optimization.ipynb` & `squlearn-0.7.2/examples/tutorials/quantum_bayesian_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/pyproject.toml` & `squlearn-0.7.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "qiskit-aer>=0.12.0",
     "qiskit-algorithms>=0.3.0",
     "qiskit-ibm-runtime>=0.15.1",
     "qiskit-machine-learning>=0.6.1",
     "pennylane>=0.34.0",
     "scipy>=1.5",
     "scikit-learn>=1.0",
+    "scikit-optimize>=0.8",
     "tqdm>=4.0",
 ]
 requires-python = ">=3.9"
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = [
@@ -48,14 +49,15 @@
     "nbsphinx",
     "nbsphinx_link",
     "pylint",
     "pytest",
     "sphinx",
     "sphinxcontrib-spelling",
     "sphinx-rtd-theme",
+    "sphinx-sitemap",
     "jupyter-sphinx",
 ]
 examples = [
     "jupyter",
     "matplotlib>=3.5",
     "mlflow",
     "pandas",
```

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/__init__.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_base.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/encoding_circuit_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/layered_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/pruned_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/pruned_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py` & `squlearn-0.7.2/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/fidelity_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 from qiskit_algorithms.state_fidelities import ComputeUncompute
 from qiskit.circuit import ParameterVector
 
 from .kernel_matrix_base import KernelMatrixBase
 from ...encoding_circuit.encoding_circuit_base import EncodingCircuitBase
 from ...util.executor import Executor
+from ...util.data_preprocessing import convert_to_float64
 
 from .fidelity_kernel_pennylane import FidelityKernelPennyLane
 
 
 class FidelityKernel(KernelMatrixBase):
     """
     Fidelity Quantum Kernel.
@@ -238,14 +239,17 @@
         Returns:
             Returns the quantum kernel matrix as 2D numpy array.
         """
 
         if y is None:
             y = x
 
+        x = convert_to_float64(x)
+        y = convert_to_float64(y)
+
         if self._parameter_vector is not None:
             if self._parameters is None:
                 raise ValueError(
                     "Parameters have to been set with assign_parameters or as initial parameters!"
                 )
             self._quantum_kernel.assign_training_parameters(self._parameters)
```

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
                 Vector of training or test data for which the kernel matrix is evaluated
         Returns:
             Returns the quantum kernel matrix as 2D numpy array.
         """
 
         if y is None:
             y = x
+
         kernel_matrix = np.ones((x.shape[0], y.shape[0]))
 
         if self._executor.is_statevector:
             kernel_matrix = self._pennylane_evaluate_kernel_sv(x, y)
         else:
             kernel_matrix = self._pennylane_evaluate_kernel(x, y)
```

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_matrix_base.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/kernel_matrix_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_util.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/kernel_util.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/projected_quantum_kernel.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/projected_quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/matrix/regularization.py` & `squlearn-0.7.2/src/squlearn/kernel/matrix/regularization.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/ml/qgpc.py` & `squlearn-0.7.2/src/squlearn/kernel/ml/qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/ml/qgpr.py` & `squlearn-0.7.2/src/squlearn/kernel/ml/qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/ml/qkrr.py` & `squlearn-0.7.2/src/squlearn/kernel/ml/qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/ml/qsvc.py` & `squlearn-0.7.2/src/squlearn/kernel/ml/qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/ml/qsvr.py` & `squlearn-0.7.2/src/squlearn/kernel/ml/qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_loss_base.py` & `squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_loss_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimization_base.py` & `squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_optimization_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimizer.py` & `squlearn-0.7.2/src/squlearn/kernel/optimization/kernel_optimizer.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/optimization/negative_log_likelihood.py` & `squlearn-0.7.2/src/squlearn/kernel/optimization/negative_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/kernel/optimization/target_alignment.py` & `squlearn-0.7.2/src/squlearn/kernel/optimization/target_alignment.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/__init__.py` & `squlearn-0.7.2/src/squlearn/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_base.py` & `squlearn-0.7.2/src/squlearn/observables/observable_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_derivatives.py` & `squlearn-0.7.2/src/squlearn/observables/observable_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/custom_observable.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/custom_observable.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/ising_hamiltonian.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_pauli.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/single_pauli.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_probability.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/single_probability.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_paulis.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/summed_paulis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_probabilities.py` & `squlearn-0.7.2/src/squlearn/observables/observable_implemented/summed_probabilities.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/optimizers/adam.py` & `squlearn-0.7.2/src/squlearn/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/optimizers/approximated_gradients.py` & `squlearn-0.7.2/src/squlearn/optimizers/approximated_gradients.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/optimizers/optimizer_base.py` & `squlearn-0.7.2/src/squlearn/optimizers/optimizer_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/optimizers/optimizers_wrapper.py` & `squlearn-0.7.2/src/squlearn/optimizers/optimizers_wrapper.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/barren_plateau_analysis.py` & `squlearn-0.7.2/src/squlearn/qnn/barren_plateau_analysis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/base_qnn.py` & `squlearn-0.7.2/src/squlearn/qnn/base_qnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         parameter_seed: Union[int, None] = 0,
         caching: bool = True,
         pretrained: bool = False,
         callback: Union[Callable, str, None] = None,
         **kwargs,
     ) -> None:
         super().__init__()
+        self.encoding_circuit = encoding_circuit
+        self.operator = operator
         self.loss = loss
         self.optimizer = optimizer
         self.variance = variance
         self.shot_control = shot_control
         self.parameter_seed = parameter_seed
 
         if param_ini is None:
@@ -95,31 +97,14 @@
                 )
             else:
                 self.param_op_ini = operator.generate_initial_parameters(seed=parameter_seed + 1)
         else:
             self.param_op_ini = param_op_ini
         self._param_op = self.param_op_ini.copy()
 
-        """
-        operator_qubits = []
-        total_num_qubits = encoding_circuit.num_qubits
-        for obs in operator.get_operator([0]*operator.num_parameters).paulis:
-            for n_q,q in enumerate(str(obs)):
-                if q != "I":
-                    if n_q not in operator_qubits:
-                        operator_qubits.append(total_num_qubits-n_q-1)
-        print(operator_qubits)
-        circ_decomposed = None
-        circ = encoding_circuit.get_circuit([0]*encoding_circuit.num_features,[0]*encoding_circuit.num_parameters)
-        for instruction, qargs, cargs in encoding_circuit.get_circuit([0]*encoding_circuit.num_features,[0]*encoding_circuit.num_parameters).decompose().data:
-            if instruction.name == "measure":
-                for qubit in qargs:
-                    if encoding_circuit.find_bit(qubit)[0] in operator_qubits:
-                        raise ValueError("There are measurements in the operator on qubits which are already measured in the circuit. Please remove these measurements or adjust the in-circuit measurements.")
-        """
         if not isinstance(optimizer, SGDMixin) and any(
             param is not None for param in [batch_size, epochs, shuffle]
         ):
             warn(
                 f"{optimizer.__class__.__name__} is not of type SGDMixin, thus batch_size, epochs"
                 " and shuffle will be ignored."
             )
@@ -130,19 +115,14 @@
         self.opt_param_op = opt_param_op
 
         self.caching = caching
         self.pretrained = pretrained
 
         self.executor = executor
 
-        self._encoding_circuit_ini = encoding_circuit
-        self._operator_ini = operator
-
-        self._qnn = LowLevelQNN(encoding_circuit, operator, executor, result_caching=self.caching)
-
         self.shot_control = shot_control
         if self.shot_control is not None:
             self.shot_control.set_executor(self.executor)
 
         self.callback = callback
 
         if self.callback:
@@ -160,14 +140,16 @@
 
                 self.optimizer.set_callback(pbar_callback)
             elif isinstance(self.callback, str):
                 raise ValueError(f"Unknown callback string value {self.callback}")
             else:
                 raise TypeError(f"Unknown callback type {type(self.callback)}")
 
+        self._initialize_lowlevel_qnn()
+
         update_params = self.get_params().keys() & kwargs.keys()
         if update_params:
             self.set_params(**{key: kwargs[key] for key in update_params})
 
         self._is_fitted = self.pretrained
 
     def __getstate__(self):
@@ -195,49 +177,14 @@
         return self._qnn.num_parameters
 
     @property
     def num_parameters_observable(self) -> int:
         """Number of parameters of the observable."""
         return self._qnn.num_parameters_observable
 
-    @property
-    def encoding_circuit(self) -> EncodingCircuitBase:
-        """Encoding circuit."""
-        if isinstance(self._qnn._pqc, TranspiledEncodingCircuit):
-            return self._qnn._pqc._encoding_circuit
-        else:
-            return self._qnn._pqc
-
-    @encoding_circuit.setter
-    def encoding_circuit(self, encoding_circuit: EncodingCircuitBase):
-        """Set the encoding circuit."""
-        self._encoding_circuit_ini = encoding_circuit
-        self._qnn = LowLevelQNN(
-            self._encoding_circuit_ini,
-            self._operator_ini,
-            self.executor,
-            result_caching=self.caching,
-        )
-
-    @property
-    def operator(self) -> Union[ObservableBase, list[ObservableBase]]:
-        """Operator."""
-        return self._qnn._observable
-
-    @operator.setter
-    def operator(self, operator: Union[ObservableBase, list[ObservableBase]]):
-        """Set the operator."""
-        self._operator_ini = operator
-        self._qnn = LowLevelQNN(
-            self._encoding_circuit_ini,
-            self._operator_ini,
-            self.executor,
-            result_caching=self.caching,
-        )
-
     def fit(self, X: np.ndarray, y: np.ndarray, weights: np.ndarray = None) -> None:
         """Fit a new model to data.
 
         This method will reinitialize the models parameters and fit it to the provided data.
 
         Args:
             X: Input data
@@ -287,19 +234,58 @@
                 )
 
         # Set parameters
         self_params = params.keys() & self.get_params(deep=False).keys()
         for key in self_params:
             setattr(self, key, params[key])
 
+        initialize_qnn = False
+        if "encoding_circuit" in params or "operator" in params:
+            initialize_qnn = True
+
+        # Set encoding_circuit parameters
+        ec_params = params.keys() & self.encoding_circuit.get_params(deep=True).keys()
+        if ec_params:
+            self.encoding_circuit.set_params(**{key: params[key] for key in ec_params})
+            initialize_qnn = True
+
+        # Set parameters of the operator
+        if isinstance(self.operator, list):
+            op_params = set()
+            for i, operator in enumerate(self.operator):
+                param_dict = {}
+                for key, value in params.items():
+                    if key == "num_qubits":
+                        param_dict[key] = value
+                        op_params.add(key)
+                    else:
+                        if key.startswith("op" + str(i) + "__"):
+                            param_dict[key.split("__", 1)[1]] = value
+                        op_params.add(key)
+                if len(param_dict) > 0:
+                    operator.set_params(**param_dict)
+                    initialize_qnn = True
+        else:
+            op_params = params.keys() & self.operator.get_params(deep=True).keys()
+            if op_params:
+                self.operator.set_params(**{key: params[key] for key in op_params})
+                initialize_qnn = True
+
+        if initialize_qnn:
+            self._initialize_lowlevel_qnn()
+
         # Set parameters of the QNN
-        qnn_params = params.keys() & self._qnn.get_params(deep=True).keys()
+        qnn_params = (params.keys() & self._qnn.get_params(deep=True).keys()) - (
+            ec_params | op_params
+        )
         if qnn_params:
             self._qnn.set_params(**{key: params[key] for key in qnn_params})
+            initialize_qnn = True
 
+        if initialize_qnn:
             # If the number of parameters has changed, reinitialize the parameters
             if self.encoding_circuit.num_parameters != len(self.param_ini):
                 self.param_ini = self.encoding_circuit.generate_initial_parameters(
                     seed=self.parameter_seed
                 )
             if isinstance(self.operator, list):
                 num_op_parameters = sum(operator.num_parameters for operator in self.operator)
@@ -321,7 +307,12 @@
 
         return self
 
     @abstractmethod
     def _fit(self, X: np.ndarray, y: np.ndarray, weights: np.ndarray = None) -> None:
         """Internal fit function."""
         raise NotImplementedError()
+
+    def _initialize_lowlevel_qnn(self):
+        self._qnn = LowLevelQNN(
+            self.encoding_circuit, self.operator, self.executor, result_caching=self.caching
+        )
```

### Comparing `squlearn-0.7.1/src/squlearn/qnn/loss.py` & `squlearn-0.7.2/src/squlearn/qnn/loss.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn.py` & `squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_base.py` & `squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     def __init__(
         self,
         parameterized_quantum_circuit: EncodingCircuitBase,
         observable: Union[ObservableBase, list],
         executor: Executor,
     ) -> None:
-        self._pqc = copy.deepcopy(parameterized_quantum_circuit)
-        self._observable = copy.deepcopy(observable)
+        self._pqc = copy.copy(parameterized_quantum_circuit)
+        self._observable = copy.copy(observable)
         self._executor = executor
 
     @abc.abstractmethod
     def set_params(self, **params) -> None:
         """Set the parameters of the QNN."""
         raise NotImplementedError
```

### Comparing `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_pennylane.py` & `squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_pennylane.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_qiskit.py` & `squlearn-0.7.2/src/squlearn/qnn/lowlevel_qnn_qiskit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/qnnc.py` & `squlearn-0.7.2/src/squlearn/qnn/qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/qnnr.py` & `squlearn-0.7.2/src/squlearn/qnn/qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/qnn/training.py` & `squlearn-0.7.2/src/squlearn/qnn/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,25 +241,25 @@
     Returns:
         Optimized parameters of the PQC, and, if opt_param_op=True,
         the optimized parameters of the observable
     """
     if isinstance(weights, np.ndarray):
         weights_values = weights
     elif weights is None:
-        weights_values = np.ones(ground_truth.shape)
+        weights_values = np.ones(np.shape(ground_truth))
     else:
         raise TypeError(f"Unknown weight format: {type(weights)}")
 
     # Tell the loss function if the cost operator parameters are optimized
     loss.set_opt_param_op(opt_param_op)
 
-    if weights_values.shape != ground_truth.shape:
+    if weights_values.shape != np.shape(ground_truth):
         raise ValueError(
             f"Shape {weights_values.shape} of weight values doesn't match shape"
-            f" {ground_truth.shape} of reference values"
+            f" {np.shape(ground_truth)} of reference values"
         )
 
     # Preprocessing of the input values in case of lists
     if not isinstance(param_ini, np.ndarray):
         param = np.array([param_ini])
     else:
         param = param_ini
```

### Comparing `squlearn-0.7.1/src/squlearn/util/data_preprocessing.py` & `squlearn-0.7.2/src/squlearn/util/data_preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,15 +80,37 @@
             error = True
     else:
         error = True
 
     if error:
         raise ValueError("Wrong format of an input variable.")
 
-    return xx, multiple_inputs
+    return convert_to_float64(xx), multiple_inputs
+
+
+def convert_to_float64(x: Union[float, np.ndarray, list]) -> np.ndarray:
+    """Convert to float64 format, raise Error for complex values
+
+    Args:
+        x (Union[float, np.ndarray]): Data that is converted
+
+    Returns:
+        Converted numpy float64 array
+    """
+    if not isinstance(x, np.ndarray):
+        x = np.array(x)
+    if x.dtype != np.float64:
+        x = np.real_if_close(x)
+        if np.iscomplexobj(x):
+            raise ValueError(
+                "Only real values for parameters and features are supported in sQUlearn!"
+            )
+        x = np.array(x, dtype=np.float64)
+
+    return x
 
 
 def to_tuple(x: Union[float, np.ndarray, list, tuple], flatten: bool = True) -> Tuple:
     """Function for converting data into hashable tuples
 
     Args:
         x (Union[float,np.ndarray,list,tuple]): Input data.
```

### Comparing `squlearn-0.7.1/src/squlearn/util/executor.py` & `squlearn-0.7.2/src/squlearn/util/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -957,15 +957,15 @@
             job_pickle._api_client = None
             job_pickle._service = None
             job_pickle._ws_client_future = None
             job_pickle._ws_client = None
             try:
                 job_pickle._backend = str(job.backend())
             except (QiskitError, AttributeError):
-                job_pickle._backend = self.backend
+                job_pickle._backend = str(self.backend)
 
             # overwrite result function with the obtained result
             def result_():
                 return result
 
             job_pickle.result = result_
             self._cache.store_file(hash_value, job_pickle)
```

### Comparing `squlearn-0.7.1/src/squlearn/util/optree/__init__.py` & `squlearn-0.7.2/src/squlearn/util/optree/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/util/optree/optree.py` & `squlearn-0.7.2/src/squlearn/util/optree/optree.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/util/optree/optree_derivative.py` & `squlearn-0.7.2/src/squlearn/util/optree/optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/util/optree/optree_evaluate.py` & `squlearn-0.7.2/src/squlearn/util/optree/optree_evaluate.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_circuit.py` & `squlearn-0.7.2/src/squlearn/util/pennylane/pennylane_circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from qiskit.compiler import transpile
 from qiskit_aer import Aer
 
 import pennylane as qml
 import pennylane.numpy as pnp
 import pennylane.pauli as pauli
+from pennylane.operation import Observable as PennyLaneObservable
 
 from .pennylane_gates import qiskit_pennylane_gate_dict
 from ..executor import Executor
 
 
 def _get_sympy_interface():
     """
@@ -122,15 +123,22 @@
     Methods:
     --------
     """
 
     def __init__(
         self,
         circuit: QuantumCircuit,
-        observable: Union[None, SparsePauliOp, List[SparsePauliOp], str] = None,
+        observable: Union[
+            None,
+            SparsePauliOp,
+            List[SparsePauliOp],
+            str,
+            PennyLaneObservable,
+            List[PennyLaneObservable],
+        ] = None,
         executor: Executor = None,
     ) -> None:
 
         self._executor = executor
         if self._executor is None:
             self._executor = Executor("pennylane")
 
@@ -146,16 +154,23 @@
             self._pennylane_gates_param_function,
             self._pennylane_gates_wires,
             self._pennylane_conditions,
             self._pennylane_gates_parameters,
             self._pennylane_gates_parameters_dimensions,
         ) = self.build_circuit_instructions(self._qiskit_circuit)
 
+        self._is_qiskit_observable = False
+        if isinstance(observable, SparsePauliOp):
+            self._is_qiskit_observable = True
+        if isinstance(observable, list):
+            if all([isinstance(obs, SparsePauliOp) for obs in observable]):
+                self._is_qiskit_observable = True
+
         # Build circuit instructions for the pennylane observable from the qiskit circuit
-        if observable is not None and not isinstance(observable, str):
+        if self._is_qiskit_observable:
             (
                 self._pennylane_obs_param_function,
                 self._pennylane_words,
                 self._pennylane_obs_parameters,
                 self._pennylane_obs_parameters_dimensions,
             ) = self.build_observable_instructions(observable)
         else:
@@ -540,44 +555,56 @@
             # Defines the output of the circuit
             if self._qiskit_observable == None:
                 return qml.probs(wires=range(self._num_qubits))
             elif self._qiskit_observable == "probs":
                 return qml.probs(wires=range(self._num_qubits))
             elif self._qiskit_observable == "state":
                 return qml.state()
-            elif isinstance(self._qiskit_observable, list):
-                expval_list = []
-                for i, obs in enumerate(self._pennylane_words):
+            elif self._is_qiskit_observable:
+                if isinstance(self._qiskit_observable, list):
+                    expval_list = []
+                    for i, obs in enumerate(self._pennylane_words):
+                        if len(obs_param_list) > 0:
+                            coeff_list = []
+                            for coeff in self._pennylane_obs_param_function[i]:
+                                if callable(coeff):
+                                    evaluated_param = coeff(*obs_param_list)
+                                    coeff_list.append(evaluated_param)
+                                else:
+                                    coeff_list.append(coeff)
+                            expval_list.append(qml.expval(qml.Hamiltonian(coeff_list, obs)))
+                        else:
+                            # In case no parameters are present in the observable
+                            # Calculate the expectation value of sum of the observables
+                            # since this is more compatible with hardware backends
+                            if len(self._pennylane_words[i]) == 0:
+                                expval_list.append(0.0)
+                            else:
+                                expval_list.append(
+                                    qml.expval(sum([obs for obs in self._pennylane_words[i]]))
+                                )
+                    return pnp.stack(tuple(expval_list))
+                else:
                     if len(obs_param_list) > 0:
                         coeff_list = []
-                        for coeff in self._pennylane_obs_param_function[i]:
+                        for coeff in self._pennylane_obs_param_function:
                             if callable(coeff):
                                 evaluated_param = coeff(*obs_param_list)
                                 coeff_list.append(evaluated_param)
                             else:
                                 coeff_list.append(coeff)
-                        expval_list.append(qml.expval(qml.Hamiltonian(coeff_list, obs)))
+                        return qml.expval(qml.Hamiltonian(coeff_list, self._pennylane_words))
                     else:
                         # In case no parameters are present in the observable
-                        # Calculate the expectation value of the single observables
+                        # Calculate the expectation value of sum of the observables
                         # since this is more compatible with hardware backends
-                        expval_list.append(
-                            pnp.sum([qml.expval(obs) for obs in self._pennylane_words[i]])
-                        )
-                return pnp.stack(tuple(expval_list))
-            else:
-                if len(obs_param_list) > 0:
-                    coeff_list = []
-                    for coeff in self._pennylane_obs_param_function:
-                        if callable(coeff):
-                            evaluated_param = coeff(*obs_param_list)
-                            coeff_list.append(evaluated_param)
+                        if len(self._pennylane_words) == 0:
+                            return 0.0
                         else:
-                            coeff_list.append(coeff)
-                    return qml.expval(qml.Hamiltonian(coeff_list, self._pennylane_words))
+                            return qml.expval(sum([obs for obs in self._pennylane_words]))
+            else:
+                if isinstance(self._qiskit_observable, list):
+                    return pnp.stack(tuple([qml.expval(obs) for obs in self._qiskit_observable]))
                 else:
-                    # In case no parameters are present in the observable
-                    # Calculate the expectation value of the single observables
-                    # since this is more compatible with hardware backends
-                    return pnp.sum([qml.expval(obs) for obs in self._pennylane_words])
+                    return qml.expval(self._qiskit_observable)
 
         return pennylane_circuit
```

### Comparing `squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_gates.py` & `squlearn-0.7.2/src/squlearn/util/pennylane/pennylane_gates.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/encoding_circuit/test_layered_encoding_circuit.py` & `squlearn-0.7.2/tests/encoding_circuit/test_layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/kernel/ml/test_qgpc.py` & `squlearn-0.7.2/tests/kernel/ml/test_qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/kernel/ml/test_qgpr.py` & `squlearn-0.7.2/tests/kernel/ml/test_qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/kernel/ml/test_qkrr.py` & `squlearn-0.7.2/tests/kernel/ml/test_qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/kernel/ml/test_qsvc.py` & `squlearn-0.7.2/tests/kernel/ml/test_qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/kernel/ml/test_qsvr.py` & `squlearn-0.7.2/tests/kernel/ml/test_qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/qnn/test_base_qnn.py` & `squlearn-0.7.2/tests/qnn/test_base_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/qnn/test_qnnc.py` & `squlearn-0.7.2/tests/qnn/test_qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/qnn/test_qnnr.py` & `squlearn-0.7.2/tests/qnn/test_qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/qnn/test_training.py` & `squlearn-0.7.2/tests/qnn/test_training.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/util/optree/test_optree_derivative.py` & `squlearn-0.7.2/tests/util/optree/test_optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/util/optree/test_optree_evaluate.py` & `squlearn-0.7.2/tests/util/optree/test_optree_evaluate.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/tests/util/test_executor.py` & `squlearn-0.7.2/tests/util/test_executor.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.1/PKG-INFO` & `squlearn-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squlearn
-Version: 0.7.1
+Version: 0.7.2
 Summary: A library for quantum machine learning following the scikit-learnstandard.
 Keywords: quantum,machine learning,qml
 Author-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Frederic Rapp <frederic.rapp@ipa.fraunhofer.de>, Marco Roth <marco.roth@ipa.fraunhofer.de>, Jan Schnabel <jan.schnabel@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
 Maintainer-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,26 +16,28 @@
 Requires-Dist: qiskit-aer>=0.12.0
 Requires-Dist: qiskit-algorithms>=0.3.0
 Requires-Dist: qiskit-ibm-runtime>=0.15.1
 Requires-Dist: qiskit-machine-learning>=0.6.1
 Requires-Dist: pennylane>=0.34.0
 Requires-Dist: scipy>=1.5
 Requires-Dist: scikit-learn>=1.0
+Requires-Dist: scikit-optimize>=0.8
 Requires-Dist: tqdm>=4.0
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: myst-parser ; extra == "dev"
 Requires-Dist: nbmake ; extra == "dev"
 Requires-Dist: nbsphinx ; extra == "dev"
 Requires-Dist: nbsphinx_link ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: sphinx ; extra == "dev"
 Requires-Dist: sphinxcontrib-spelling ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme ; extra == "dev"
+Requires-Dist: sphinx-sitemap ; extra == "dev"
 Requires-Dist: jupyter-sphinx ; extra == "dev"
 Requires-Dist: jupyter ; extra == "examples"
 Requires-Dist: matplotlib>=3.5 ; extra == "examples"
 Requires-Dist: mlflow ; extra == "examples"
 Requires-Dist: pandas ; extra == "examples"
 Requires-Dist: pylatexenc>=2.10 ; extra == "examples"
 Requires-Dist: seaborn ; extra == "examples"
```

