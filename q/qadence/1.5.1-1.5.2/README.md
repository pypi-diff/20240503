# Comparing `tmp/qadence-1.5.1.tar.gz` & `tmp/qadence-1.5.2.tar.gz`

## Comparing `qadence-1.5.1.tar` & `qadence-1.5.2.tar`

### file list

```diff
@@ -1,154 +1,155 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.5.1/.coveragerc
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.5.1/MANIFEST.in
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 qadence-1.5.1/mkdocs.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qadence-1.5.1/renovate.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.5.1/setup.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_all.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_examples.yml
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_fast.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/__init__.py
--rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backend.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/circuit.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/decompose.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/divergences.py
--rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/execution.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/extensions.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/finitediff.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/libs.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/logger.py
--rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/overlap.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/parameters.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/py.typed
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/qubit_support.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/register.py
--rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/serialization.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/states.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/types.py
--rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/utils.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/__init__.py
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/addressing.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/constants.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/device.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/hamiltonian_terms.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/parse_analog.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/__init__.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/adjoint.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/api.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/gpsr.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/jax_utils.py
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/__init__.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/backend.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/config.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/convert_ops.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/__init__.py
--rw-r--r--   0        0        0     9329 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/backend.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/config.py
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/convert_ops.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/__init__.py
--rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/backend.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/channels.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/cloud.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/config.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/convert_ops.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/devices.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/pulses.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/waveforms.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/__init__.py
--rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/backend.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/config.py
--rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/convert_ops.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/__init__.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/abstract.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/analog.py
--rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/block_to_tensor.py
--rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/composite.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/embedding.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/manipulate.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/matrix.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/primitive.py
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/utils.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/__init__.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/ansatze.py
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/feature_maps.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/hamiltonians.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/iia.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/qft.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/rydberg_feature_maps.py
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/rydberg_hea.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/__init__.py
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/daqc.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/gen_parser.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/utils.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/__init__.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/themes.py
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/utils.py
--rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/vizbackend.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/dark/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/dark/measurement.svg
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/light/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/light/measurement.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/__init__.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/differentiable_backend.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/differentiable_backend.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/differentiable_expectation.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/__init__.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/differentiable_backend.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/differentiable_expectation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/exceptions/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/exceptions/exceptions.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/protocols.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/samples.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/shadow.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/tomography.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/__init__.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/analog_zne.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/protocols.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/readout.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/__init__.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/config.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/data.py
--rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/models.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/optimize_step.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/parameters.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/printing.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/saveload.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/tensors.py
--rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/train_grad.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/train_no_grad.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/utils.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/__init__.py
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/qnn.py
--rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/quantum_model.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/protocols.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/readout.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/analog.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/control_ops.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/ham_evo.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/parametric.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/primitive.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/apply_fn.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/block.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/circuit.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/digitalize.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/flatten.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/invert.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/transpile.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.5.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.5.1/LICENSE
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 qadence-1.5.1/README.md
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 qadence-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 qadence-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.5.2/.coveragerc
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.5.2/MANIFEST.in
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 qadence-1.5.2/mkdocs.yml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qadence-1.5.2/renovate.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.5.2/setup.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/dependabot.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/test_all.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/test_examples.yml
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.5.2/.github/workflows/test_fast.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/__init__.py
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backend.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/circuit.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/decompose.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/divergences.py
+-rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/execution.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/extensions.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/finitediff.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/libs.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/logger.py
+-rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/overlap.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/parameters.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/py.typed
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/qubit_support.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/register.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/serial_expr_grammar.peg
+-rw-r--r--   0        0        0    15695 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/serialization.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/states.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/types.py
+-rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/utils.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/__init__.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/addressing.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/constants.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/device.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/hamiltonian_terms.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/analog/parse_analog.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/__init__.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/adjoint.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/api.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/gpsr.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/jax_utils.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/braket/__init__.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/braket/backend.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/braket/config.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/braket/convert_ops.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/horqrux/__init__.py
+-rw-r--r--   0        0        0     9329 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/horqrux/backend.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/horqrux/config.py
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/horqrux/convert_ops.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/__init__.py
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/backend.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/channels.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/cloud.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/config.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/convert_ops.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/devices.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/pulses.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pulser/waveforms.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pyqtorch/backend.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pyqtorch/config.py
+-rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/backends/pyqtorch/convert_ops.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/__init__.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/abstract.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/analog.py
+-rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/block_to_tensor.py
+-rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/composite.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/embedding.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/manipulate.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/matrix.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/primitive.py
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/blocks/utils.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/__init__.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/ansatze.py
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/feature_maps.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/hamiltonians.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/iia.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/qft.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/rydberg_feature_maps.py
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/rydberg_hea.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/daqc/__init__.py
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/daqc/daqc.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/daqc/gen_parser.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/constructors/daqc/utils.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/__init__.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/themes.py
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/utils.py
+-rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/vizbackend.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/assets/dark/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/assets/dark/measurement.svg
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/assets/light/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/draw/assets/light/measurement.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/__init__.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/differentiable_backend.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/jax/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/jax/differentiable_backend.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/jax/differentiable_expectation.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/torch/__init__.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/torch/differentiable_backend.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/engines/torch/differentiable_expectation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/exceptions/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/exceptions/exceptions.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/protocols.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/samples.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/shadow.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/tomography.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/measurements/utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/mitigations/__init__.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/mitigations/analog_zne.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/mitigations/protocols.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/mitigations/readout.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/__init__.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/config.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/data.py
+-rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/models.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/optimize_step.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/parameters.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/printing.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/saveload.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/tensors.py
+-rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/train_grad.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/train_no_grad.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/ml_tools/utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/models/__init__.py
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/models/qnn.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/models/quantum_model.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/noise/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/noise/protocols.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/noise/readout.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/analog.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/control_ops.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/ham_evo.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/parametric.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/operations/primitive.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/apply_fn.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/block.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/circuit.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/digitalize.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/flatten.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/invert.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.5.2/qadence/transpile/transpile.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.5.2/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.5.2/LICENSE
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 qadence-1.5.2/README.md
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 qadence-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 qadence-1.5.2/PKG-INFO
```

### Comparing `qadence-1.5.1/.pre-commit-config.yaml` & `qadence-1.5.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 -   repo: https://github.com/ambv/black
     rev: 23.11.0
     hooks:
       - id: black
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         exclude: examples|docs
 
 -   repo: https://github.com/DanielNoord/pydocstringformatter
     rev: v0.7.3
     hooks:
```

### Comparing `qadence-1.5.1/mkdocs.yml` & `qadence-1.5.2/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,122 @@
 site_name: Qadence
 repo_url: "https://github.com/pasqal-io/qadence/"
 site_url: "https://pasqal-io.github.io/qadence/"
 repo_name: "qadence"
 
 nav:
+  - Home: index.md
 
-  - Qadence:
-    - Qadence: index.md
-    - Code of conduct: CODE_OF_CONDUCT.md
-    - Getting started: tutorials/getting_started.md
-    - Quantum models: tutorials/quantummodels.md
-    - Parametric programs: tutorials/parameters.md
-    - Quantum registers: tutorials/register.md
-    - State conventions: tutorials/state_conventions.md
-    - State initialization: tutorials/state_init.md
-    - Arbitrary Hamiltonians: tutorials/hamiltonians.md
-    - Wavefunction overlaps: tutorials/overlap.md
-    - Serialization: tutorials/serializ_and_prep.md
-    - Backends: tutorials/backends.md
-
-  - Digital-analog quantum computing:
-    - digital_analog_qc/index.md
-    - Basic operations on neutral-atoms: digital_analog_qc/analog-basics.md
-    - Fitting a simple function: digital_analog_qc/analog-qcl.md
-    - Restricted local addressability: digital_analog_qc/semi-local-addressing.md
-    - Pulse-level programming with Pulser: digital_analog_qc/pulser-basic.md
-    - Solve a QUBO problem: digital_analog_qc/analog-qubo.md
-    - CNOT with interacting qubits: digital_analog_qc/daqc-cnot.md
-
-  - Variational quantum algorithms:
-    - qml/index.md
-    - Constructors: qml/qml_constructors.md
-    - Training tools: qml/ml_tools.md
-    - Quantum circuit learning: qml/qcl.md
-    - Solving MaxCut with QAOA: qml/qaoa.md
-
-  - Advanced Tutorials:
-    - advanced_tutorials/index.md
-    - Quantum circuits differentiation: advanced_tutorials/differentiability.md
-    - Custom quantum models: advanced_tutorials/custom-models.md
-    - Projector blocks: advanced_tutorials/projectors.md
-
-  - Realistic simulations:
-    - realistic_sims/index.md
-    - Measurement protocols: realistic_sims/measurements.md
-    - Simulated errors: realistic_sims/noise.md
-    - Error mitigation: realistic_sims/mitigation.md
+  - Getting started:
+    - Installation: getting_started/installation.md
+    - Development & Info:
+      - Contributing: getting_started/CONTRIBUTING.md
+      - Code of conduct: getting_started/CODE_OF_CONDUCT.md
+      - License: getting_started/LICENSE.md
+
+  - Contents:
+    - Block system: content/block_system.md
+    - Parametric programs: content/parameters.md
+    - Quantum models: content/quantummodels.md
+    - Quantum registers: content/register.md
+    - State initialization: content/state_init.md
+    - Arbitrary Hamiltonians: content/hamiltonians.md
+    - QML Constructors: content/qml_constructors.md
+    - Wavefunction overlaps: content/overlap.md
+    - Backends: content/backends.md
+    - Useful info:
+      - State conventions: content/state_conventions.md
+      - Serialization: content/serializ_and_prep.md
+
+  - Tutorials:
+    - tutorials/index.md
+    - Digital-analog quantum computing:
+      - tutorials/digital_analog_qc/index.md
+      - Basic operations on neutral-atoms: tutorials/digital_analog_qc/analog-basics.md
+      - Fitting a simple function: tutorials/digital_analog_qc/analog-qcl.md
+      - Restricted local addressability: tutorials/digital_analog_qc/semi-local-addressing.md
+      - Pulse-level programming with Pulser: tutorials/digital_analog_qc/pulser-basic.md
+      - Solve a QUBO problem: tutorials/digital_analog_qc/analog-qubo.md
+      - CNOT with interacting qubits: tutorials/digital_analog_qc/daqc-cnot.md
+
+    - Variational quantum algorithms:
+      - tutorials/qml/index.md
+      - Training tools: tutorials/qml/ml_tools.md
+      - Quantum circuit learning: tutorials/qml/qcl.md
+      - Solving MaxCut with QAOA: tutorials/qml/qaoa.md
+      - Solving a 1D ODE: tutorials/qml/dqc_1d.md
+
+    - Advanced Tutorials:
+      - tutorials/advanced_tutorials/index.md
+      - Quantum circuits differentiation: tutorials/advanced_tutorials/differentiability.md
+      - Custom quantum models: tutorials/advanced_tutorials/custom-models.md
+      - Projector blocks: tutorials/advanced_tutorials/projectors.md
+
+    - Realistic simulations:
+      - tutorials/realistic_sims/index.md
+      - Measurement protocols: tutorials/realistic_sims/measurements.md
+      - Simulated errors: tutorials/realistic_sims/noise.md
+      - Error mitigation: tutorials/realistic_sims/mitigation.md
+
+    - Development:
+      - Architecture and sharp bits: tutorials/development/architecture.md
+      - Drawing: tutorials/development/draw.md
 
   - API:
-    - Block system: qadence/blocks.md
-    - Operations: qadence/operations.md
-    - Register: qadence/register.md
-    - QuantumCircuit: qadence/quantumcircuit.md
-    - Parameters: qadence/parameters.md
-    - State preparation: qadence/states.md
-    - Constructors: qadence/constructors.md
-    - Transpilation: qadence/transpile.md
-    - Execution: qadence/execution.md
-    - Quantum models: models.md
-    - QML tools: qadence/ml_tools.md
-    - Serialization: qadence/serialization.md
-    - Types: qadence/types.md
-    - Drawing: qadence/draw.md
+    - Block system: api/blocks.md
+    - Operations: api/operations.md
+    - Register: api/register.md
+    - QuantumCircuit: api/quantumcircuit.md
+    - Parameters: api/parameters.md
+    - State preparation: api/states.md
+    - Constructors: api/constructors.md
+    - Transpilation: api/transpile.md
+    - Execution: api/execution.md
+    - Quantum models: api/models.md
+    - QML tools: api/ml_tools.md
+    - Serialization: api/serialization.md
+    - Types: api/types.md
+    - Drawing: api/draw.md
 
     - Backends:
-      - Abstract backend: backends/backend.md
-      - PyQTorch: backends/pyqtorch.md
-      - Amazon Braket: backends/braket.md
-      - Pulser: backends/pulser.md
-      - DifferentiableBackend: backends/differentiable.md
-
-  - Development:
-    - Architecture and sharp bits: development/architecture.md
-    - Drawing: development/draw.md
-    - Contributing: CONTRIBUTING.md
+      - Abstract backend: api/backends/backend.md
+      - PyQTorch: api/backends/pyqtorch.md
+      - Amazon Braket: api/backends/braket.md
+      - Pulser: api/backends/pulser.md
+      - DifferentiableBackend: api/backends/differentiable.md
 
 edit_uri: edit/main/docs/
 
 theme:
   name: material
-  logo: assets/logo/qadence_logo_small_white.svg
+  custom_dir: docs/extras/overrides/
+  logo: extras/assets/logo/qadence_logo_small_white.svg
   features:
   - content.code.annotate
-  - content.action.view
-  - content.action.edit
   - navigation.tabs
   - navigation.indexes
   - navigation.sections
   - content.code.copy
   - content.code.annotate
 
   palette:
   - media: "(prefers-color-scheme: light)"
     scheme: default
     primary: custom
     accent: custom
     toggle:
-      icon: material/weather-sunny
-      name: Switch to dark mode
+        icon: material/weather-sunny
+        name: Switch to dark mode
   - media: "(prefers-color-scheme: dark)"
     scheme: slate
-    primary: custom
+    primary: black
     accent: custom
     toggle:
-      icon: material/weather-night
-      name: Switch to light mode
+        icon: material/weather-night
+        name: Switch to light mode
 
 markdown_extensions:
 - admonition  # for notes
 - footnotes
 - pymdownx.arithmatex: # for mathjax
     generic: true
 - pymdownx.highlight:
@@ -145,17 +153,19 @@
 
 extra:
  version:
    provider: mike
 
 # To get nice tabs
 extra_css:
-- css/mkdocstrings.css
+- extras/css/mkdocstrings.css
+- extras/css/colors.css
+- extras/css/home.css
 
 # For mathjax
 extra_javascript:
-  - javascripts/mathjax.js
+  - extras/javascripts/mathjax.js
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
 
 watch:
 - qadence
```

### Comparing `qadence-1.5.1/.github/workflows/build_docs.yml` & `qadence-1.5.2/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/.github/workflows/test_all.yml` & `qadence-1.5.2/.github/workflows/test_all.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/.github/workflows/test_examples.yml` & `qadence-1.5.2/.github/workflows/test_examples.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/.github/workflows/test_fast.yml` & `qadence-1.5.2/.github/workflows/test_fast.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/__init__.py` & `qadence-1.5.2/qadence/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backend.py` & `qadence-1.5.2/qadence/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/circuit.py` & `qadence-1.5.2/qadence/circuit.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/decompose.py` & `qadence-1.5.2/qadence/decompose.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/divergences.py` & `qadence-1.5.2/qadence/divergences.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/execution.py` & `qadence-1.5.2/qadence/execution.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/extensions.py` & `qadence-1.5.2/qadence/extensions.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/finitediff.py` & `qadence-1.5.2/qadence/finitediff.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/logger.py` & `qadence-1.5.2/qadence/logger.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/overlap.py` & `qadence-1.5.2/qadence/overlap.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/parameters.py` & `qadence-1.5.2/qadence/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/qubit_support.py` & `qadence-1.5.2/qadence/qubit_support.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/register.py` & `qadence-1.5.2/qadence/register.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/serialization.py` & `qadence-1.5.2/qadence/serialization.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 
 import json
 import os
+import sys
+from dataclasses import dataclass
+from dataclasses import field as dataclass_field
+from functools import lru_cache
 from pathlib import Path
-from typing import Any, get_args
+from typing import Any, Callable, get_args
 from typing import Union as TypingUnion
 
 import torch
+from arpeggio import NoMatch
+from arpeggio.cleanpeg import ParserPEG
 from sympy import *
-from sympy import Basic, Expr, srepr
+from sympy import core, srepr
 
-from qadence import QuantumCircuit, operations
+from qadence import QuantumCircuit, operations, parameters
 from qadence import blocks as qadenceblocks
 from qadence.blocks import AbstractBlock
 from qadence.blocks.utils import tag
 from qadence.logger import get_logger
-from qadence.ml_tools.models import TransformedModule
-from qadence.models import QNN, QuantumModel
+from qadence.models import QuantumModel
 from qadence.parameters import Parameter
 from qadence.register import Register
 from qadence.types import SerializationFormat
 
 # Modules to be automatically added to the qadence namespace
 __all__ = ["deserialize", "load", "save", "serialize"]
 
@@ -39,35 +44,180 @@
     return FORMAT
 
 
 SUPPORTED_OBJECTS = [
     AbstractBlock,
     QuantumCircuit,
     QuantumModel,
-    QNN,
-    TransformedModule,
     Register,
-    Basic,
+    core.Basic,
     torch.nn.Module,
 ]
 SUPPORTED_TYPES = TypingUnion[
     AbstractBlock,
     QuantumCircuit,
     QuantumModel,
-    QNN,
-    TransformedModule,
     Register,
-    Basic,
+    core.Basic,
     torch.nn.Module,
 ]
 
-
 ALL_BLOCK_NAMES = [
     n for n in dir(qadenceblocks) if not (n.startswith("__") and n.endswith("__"))
 ] + [n for n in dir(operations) if not (n.startswith("__") and n.endswith("__"))]
+SYMPY_EXPRS = [n for n in dir(core) if not (n.startswith("__") and n.endswith("__"))]
+QADENCE_PARAMETERS = [n for n in dir(parameters) if not (n.startswith("__") and n.endswith("__"))]
+
+
+THIS_PATH = Path(__file__).parent
+GRAMMAR_FILE = THIS_PATH / "serial_expr_grammar.peg"
+
+
+@lru_cache
+def _parser_fn() -> ParserPEG:
+    with open(GRAMMAR_FILE, "r") as f:
+        grammar = f.read()
+    return ParserPEG(grammar, "Program")
+
+
+_parsing_serialize_expr = _parser_fn()
+
+
+def parse_expr_fn(code: str) -> bool:
+    """
+    A parsing expressions function that checks whether a given code is valid on.
+
+    the parsing grammar. The grammar is defined to be compatible with `sympy`
+    expressions, such as `Float('-0.33261030434342942', precision=53)`, while
+    avoiding code injection such as `2*3` or `__import__('os').system('ls -la')`.
+
+    Args:
+        code (str): code to be parsed and checked.
+
+    Returns:
+        Boolean indicating whether the code matches the defined grammar or not.
+    """
+
+    parser = _parsing_serialize_expr
+    try:
+        parser.parse(code)
+    except NoMatch:
+        return False
+    else:
+        return True
+
+
+@dataclass
+class SerializationModel:
+    """
+    A serialization model class to serialize data from `QuantumModel`s,.
+
+    `torch.nn.Module` and similar structures. The data included in the
+    serialization logic includes: the `AbstractBlock` and its children
+    classes, `QuantumCircuit`, `Register`, and `sympy` expressions
+    (including `Parameter` class from `qadence.parameters`).
+
+    A children class must define the `value` attribute type and how to
+    handle it, since it is the main property for the class to be used
+    by the serialization process. For instance:
+
+    ```python
+    @dataclass
+    class QuantumCircuitSerialization(SerializationModel):
+        value: QuantumCircuit = dataclass_field(init=False)
+
+        def __post_init__(self) -> None:
+            self.value = (
+                QuantumCircuit._from_dict(self.d)
+                if isinstance(self.d, dict)
+                else self.d
+            )
+    ```
+    """
+
+    d: dict = dataclass_field(default_factory=dict)
+    value: Any = dataclass_field(init=False)
+
+
+@dataclass
+class BlockTypeSerialization(SerializationModel):
+    value: AbstractBlock = dataclass_field(init=False)
+
+    def __post_init__(self) -> None:
+        block = (
+            getattr(operations, self.d["type"])
+            if hasattr(operations, self.d["type"])
+            else getattr(qadenceblocks, self.d["type"])
+        )._from_dict(self.d)
+        if self.d["tag"] is not None:
+            block = tag(block, self.d["tag"])
+        self.value = block
+
+
+@dataclass
+class QuantumCircuitSerialization(SerializationModel):
+    value: QuantumCircuit = dataclass_field(init=False)
+
+    def __post_init__(self) -> None:
+        self.value = QuantumCircuit._from_dict(self.d) if isinstance(self.d, dict) else self.d
+
+
+@dataclass
+class RegisterSerialization(SerializationModel):
+    value: Register = dataclass_field(init=False)
+
+    def __post_init__(self) -> None:
+        self.value = Register._from_dict(self.d)
+
+
+@dataclass
+class ModelSerialization(SerializationModel):
+    as_torch: bool = False
+    value: torch.nn.Module = dataclass_field(init=False)
+
+    def __post_init__(self) -> None:
+        module_name = list(self.d.keys())[0]
+        obj = globals().get(module_name, None)
+        if obj is None:
+            obj = self._resolve_module(module_name)
+        if hasattr(obj, "_from_dict"):
+            self.value = obj._from_dict(self.d, self.as_torch)
+        elif hasattr(obj, "load_state_dict"):
+            self.value = obj.load_state_dict(self.d[module_name])
+        else:
+            msg = (
+                f"Unable to deserialize object '{module_name}'. "
+                f"Supported types are {SUPPORTED_OBJECTS}."
+            )
+            logger.error(TypeError(msg))
+            raise TypeError(msg)
+
+    @staticmethod
+    def _resolve_module(module: str) -> Any:
+        for loaded_module in sys.modules.keys():
+            if "qadence" in loaded_module:
+                obj = getattr(sys.modules[loaded_module], module, None)
+                if obj:
+                    return obj
+        raise ValueError(f"Couldn't resolve module '{module}'.")
+
+
+@dataclass
+class ExpressionSerialization(SerializationModel):
+    value: str | core.Expr | float = dataclass_field(init=False)
+
+    def __post_init__(self) -> None:
+        if parse_expr_fn(self.d["expression"]):
+            expr = eval(self.d["expression"])
+            if hasattr(expr, "free_symbols"):
+                for s in expr.free_symbols:
+                    s.value = float(self.d["symbols"][s.name]["value"])
+            self.value = expr
+        else:
+            raise ValueError(f"Invalid expression: {self.d['expression']}")
 
 
 def save_pt(d: dict, file_path: str | Path) -> None:
     torch.save(d, file_path)
 
 
 def save_json(d: dict, file_path: str | Path) -> None:
@@ -90,19 +240,19 @@
 }
 
 
 def serialize(obj: SUPPORTED_TYPES, save_params: bool = False) -> dict:
     """
     Supported Types:
 
-    AbstractBlock | QuantumCircuit | QuantumModel | TransformedModule | Register | Module
+    AbstractBlock | QuantumCircuit | QuantumModel | torch.nn.Module | Register | Module
     Serializes a qadence object to a dictionary.
 
     Arguments:
-        obj (AbstractBlock | QuantumCircuit | QuantumModel | Register | Module):
+        obj (AbstractBlock | QuantumCircuit | QuantumModel | Register | torch.nn.Module):
     Returns:
         A dict.
 
     Examples:
     ```python exec="on" source="material-block" result="json"
     import torch
     from qadence import serialize, deserialize, hea, hamiltonian_factory, Z
@@ -128,45 +278,53 @@
     qm_deserialized = deserialize(qm_dict)
     # Lets check if the loaded QuantumModel returns the same expectation
     assert torch.isclose(qm.expectation({}), qm_deserialized.expectation({}))
     ```
     """
     if not isinstance(obj, get_args(SUPPORTED_TYPES)):
         logger.error(TypeError(f"Serialization of object type {type(obj)} not supported."))
-    d: dict = {}
+
+    d: dict = dict()
     try:
-        if isinstance(obj, Expr):
-            symb_dict = {}
+        if isinstance(obj, core.Expr):
+            symb_dict = dict()
             expr_dict = {"name": str(obj), "expression": srepr(obj)}
-            symbs: set[Parameter | Basic] = obj.free_symbols
+            symbs: set[Parameter | core.Basic] = obj.free_symbols
             if symbs:
                 symb_dict = {"symbols": {str(s): s._to_dict() for s in symbs}}
             d = {**expr_dict, **symb_dict}
-        elif isinstance(obj, (QuantumModel, QNN, TransformedModule)):
-            d = obj._to_dict(save_params)
-        elif isinstance(obj, torch.nn.Module):
-            d = {type(obj).__name__: obj.state_dict()}
         else:
-            d = obj._to_dict()
+            if hasattr(obj, "_to_dict"):
+                model_to_dict: Callable = obj._to_dict
+                d = (
+                    model_to_dict(save_params)
+                    if isinstance(obj, torch.nn.Module)
+                    else model_to_dict()
+                )
+            elif hasattr(obj, "state_dict"):
+                d = {type(obj).__name__: obj.state_dict()}
+            else:
+                raise ValueError(f"Cannot serialize object {obj}.")
     except Exception as e:
         logger.error(f"Serialization of object {obj} failed due to {e}")
     return d
 
 
 def deserialize(d: dict, as_torch: bool = False) -> SUPPORTED_TYPES:
     """
     Supported Types:
 
-    AbstractBlock | QuantumCircuit | QuantumModel | TransformedModule | Register | Module
+    AbstractBlock | QuantumCircuit | QuantumModel | Register | torch.nn.Module
     Deserializes a dict to one of the supported types.
 
     Arguments:
         d (dict): A dict containing a serialized object.
+        as_torch (bool): Whether to transform to torch for the deserialized object.
     Returns:
-        AbstractBlock, QuantumCircuit, QuantumModel, TransformedModule, Register, Module.
+        AbstractBlock, QuantumCircuit, QuantumModel, Register, torch.nn.Module.
 
     Examples:
     ```python exec="on" source="material-block" result="json"
     import torch
     from qadence import serialize, deserialize, hea, hamiltonian_factory, Z
     from qadence import QuantumCircuit, QuantumModel
 
@@ -188,59 +346,26 @@
 
     qm_dict = serialize(qm)
     qm_deserialized = deserialize(qm_dict)
     # Lets check if the loaded QuantumModel returns the same expectation
     assert torch.isclose(qm.expectation({}), qm_deserialized.expectation({}))
     ```
     """
-    obj: Any
+    obj: SerializationModel
     if d.get("expression"):
-        expr = eval(d["expression"])
-        if hasattr(expr, "free_symbols"):
-            for symb in expr.free_symbols:
-                symb.value = float(d["symbols"][symb.name]["value"])
-        obj = expr
-    elif d.get("QuantumModel"):
-        obj = QuantumModel._from_dict(d, as_torch)
-    elif d.get("QNN"):
-        obj = QNN._from_dict(d, as_torch)
-    elif d.get("TransformedModule"):
-        obj = TransformedModule._from_dict(d, as_torch)
+        obj = ExpressionSerialization(d)
     elif d.get("block") and d.get("register"):
-        obj = QuantumCircuit._from_dict(d)
+        obj = QuantumCircuitSerialization(d)
     elif d.get("graph"):
-        obj = Register._from_dict(d)
+        obj = RegisterSerialization(d)
     elif d.get("type"):
-        if d["type"] in ALL_BLOCK_NAMES:
-            block: AbstractBlock = (
-                getattr(operations, d["type"])._from_dict(d)
-                if hasattr(operations, d["type"])
-                else getattr(qadenceblocks, d["type"])._from_dict(d)
-            )
-            if d["tag"] is not None:
-                block = tag(block, d["tag"])
-            obj = block
+        obj = BlockTypeSerialization(d)
     else:
-        import warnings
-
-        msg = warnings.warn(
-            "In order to load a custom torch.nn.Module, make sure its imported in the namespace."
-        )
-        try:
-            module_name = list(d.keys())[0]
-            obj = getattr(globals(), module_name)
-            obj.load_state_dict(d[module_name])
-        except Exception as e:
-            logger.error(
-                TypeError(
-                    f"{msg}. Unable to deserialize object due to {e}.\
-                    Supported objects are: {SUPPORTED_OBJECTS}"
-                )
-            )
-    return obj
+        obj = ModelSerialization(d, as_torch=as_torch)
+    return obj.value
 
 
 def save(
     obj: SUPPORTED_TYPES,
     folder: str | Path,
     file_name: str = "",
     format: SerializationFormat = SerializationFormat.JSON,
```

### Comparing `qadence-1.5.1/qadence/states.py` & `qadence-1.5.2/qadence/states.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/types.py` & `qadence-1.5.2/qadence/types.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/utils.py` & `qadence-1.5.2/qadence/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,19 +150,25 @@
             return f"{im}j"
         else:
             return "0"
     else:
         raise ValueError(f"Unknown number type: {type(x)}")
 
 
-def format_parameter(p: sympy.Basic) -> str:
+def format_parameter(p: sympy.Basic, num_digits: int = 3) -> str:
+    """Format numerical values within a sympy expression."""
+
     def round_expr(expr: sympy.Basic, num_digits: int) -> sympy.Basic:
         return expr.xreplace({n: round(n, num_digits) for n in expr.atoms(sympy.Number)})
 
-    return str(round_expr(p, 3))
+    expr = round_expr(p, num_digits)
+    conv_str = str(expr)
+    if expr.is_real and len(conv_str) > num_digits + 2:
+        conv_str = conv_str[0 : num_digits + 2]
+    return conv_str
 
 
 def print_sympy_expr(expr: sympy.Expr, num_digits: int = 3) -> str:
     """
     Converts numerical values in a sympy expression.
 
     The result is a numerical expression with fewer digits for better readability.
```

### Comparing `qadence-1.5.1/qadence/analog/addressing.py` & `qadence-1.5.2/qadence/analog/addressing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/analog/constants.py` & `qadence-1.5.2/qadence/analog/constants.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/analog/device.py` & `qadence-1.5.2/qadence/analog/device.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/analog/hamiltonian_terms.py` & `qadence-1.5.2/qadence/analog/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/analog/parse_analog.py` & `qadence-1.5.2/qadence/analog/parse_analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/adjoint.py` & `qadence-1.5.2/qadence/backends/adjoint.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/api.py` & `qadence-1.5.2/qadence/backends/api.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/gpsr.py` & `qadence-1.5.2/qadence/backends/gpsr.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/jax_utils.py` & `qadence-1.5.2/qadence/backends/jax_utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/utils.py` & `qadence-1.5.2/qadence/backends/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/braket/backend.py` & `qadence-1.5.2/qadence/backends/braket/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/braket/config.py` & `qadence-1.5.2/qadence/backends/braket/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/braket/convert_ops.py` & `qadence-1.5.2/qadence/backends/braket/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/horqrux/backend.py` & `qadence-1.5.2/qadence/backends/horqrux/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/horqrux/config.py` & `qadence-1.5.2/qadence/backends/horqrux/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/horqrux/convert_ops.py` & `qadence-1.5.2/qadence/backends/horqrux/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/backend.py` & `qadence-1.5.2/qadence/backends/pulser/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/cloud.py` & `qadence-1.5.2/qadence/backends/pulser/cloud.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/config.py` & `qadence-1.5.2/qadence/backends/pulser/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/convert_ops.py` & `qadence-1.5.2/qadence/backends/pulser/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/devices.py` & `qadence-1.5.2/qadence/backends/pulser/devices.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/pulses.py` & `qadence-1.5.2/qadence/backends/pulser/pulses.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pulser/waveforms.py` & `qadence-1.5.2/qadence/backends/pulser/waveforms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pyqtorch/backend.py` & `qadence-1.5.2/qadence/backends/pyqtorch/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pyqtorch/config.py` & `qadence-1.5.2/qadence/backends/pyqtorch/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/backends/pyqtorch/convert_ops.py` & `qadence-1.5.2/qadence/backends/pyqtorch/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/__init__.py` & `qadence-1.5.2/qadence/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/abstract.py` & `qadence-1.5.2/qadence/blocks/abstract.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/analog.py` & `qadence-1.5.2/qadence/blocks/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/block_to_tensor.py` & `qadence-1.5.2/qadence/blocks/block_to_tensor.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/composite.py` & `qadence-1.5.2/qadence/blocks/composite.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/embedding.py` & `qadence-1.5.2/qadence/blocks/embedding.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/manipulate.py` & `qadence-1.5.2/qadence/blocks/manipulate.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/matrix.py` & `qadence-1.5.2/qadence/blocks/matrix.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/primitive.py` & `qadence-1.5.2/qadence/blocks/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/blocks/utils.py` & `qadence-1.5.2/qadence/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/__init__.py` & `qadence-1.5.2/qadence/constructors/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/ansatze.py` & `qadence-1.5.2/qadence/constructors/ansatze.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/feature_maps.py` & `qadence-1.5.2/qadence/constructors/feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/hamiltonians.py` & `qadence-1.5.2/qadence/constructors/hamiltonians.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/iia.py` & `qadence-1.5.2/qadence/constructors/iia.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/qft.py` & `qadence-1.5.2/qadence/constructors/qft.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/rydberg_feature_maps.py` & `qadence-1.5.2/qadence/constructors/rydberg_feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/rydberg_hea.py` & `qadence-1.5.2/qadence/constructors/rydberg_hea.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/utils.py` & `qadence-1.5.2/qadence/constructors/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/daqc/daqc.py` & `qadence-1.5.2/qadence/constructors/daqc/daqc.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/daqc/gen_parser.py` & `qadence-1.5.2/qadence/constructors/daqc/gen_parser.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/constructors/daqc/utils.py` & `qadence-1.5.2/qadence/constructors/daqc/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/__init__.py` & `qadence-1.5.2/qadence/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/themes.py` & `qadence-1.5.2/qadence/draw/themes.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/utils.py` & `qadence-1.5.2/qadence/draw/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/vizbackend.py` & `qadence-1.5.2/qadence/draw/vizbackend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/assets/dark/measurement.svg` & `qadence-1.5.2/qadence/draw/assets/dark/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/draw/assets/light/measurement.svg` & `qadence-1.5.2/qadence/draw/assets/light/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/engines/differentiable_backend.py` & `qadence-1.5.2/qadence/engines/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/engines/jax/differentiable_backend.py` & `qadence-1.5.2/qadence/engines/jax/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/engines/jax/differentiable_expectation.py` & `qadence-1.5.2/qadence/engines/jax/differentiable_expectation.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/engines/torch/differentiable_backend.py` & `qadence-1.5.2/qadence/engines/torch/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/engines/torch/differentiable_expectation.py` & `qadence-1.5.2/qadence/engines/torch/differentiable_expectation.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/measurements/protocols.py` & `qadence-1.5.2/qadence/measurements/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/measurements/samples.py` & `qadence-1.5.2/qadence/measurements/samples.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/measurements/shadow.py` & `qadence-1.5.2/qadence/measurements/shadow.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/measurements/tomography.py` & `qadence-1.5.2/qadence/measurements/tomography.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/measurements/utils.py` & `qadence-1.5.2/qadence/measurements/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/mitigations/analog_zne.py` & `qadence-1.5.2/qadence/mitigations/analog_zne.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/mitigations/protocols.py` & `qadence-1.5.2/qadence/mitigations/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/mitigations/readout.py` & `qadence-1.5.2/qadence/mitigations/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/__init__.py` & `qadence-1.5.2/qadence/ml_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/config.py` & `qadence-1.5.2/qadence/ml_tools/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/data.py` & `qadence-1.5.2/qadence/ml_tools/data.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/models.py` & `qadence-1.5.2/qadence/ml_tools/models.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/optimize_step.py` & `qadence-1.5.2/qadence/ml_tools/optimize_step.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/parameters.py` & `qadence-1.5.2/qadence/ml_tools/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/printing.py` & `qadence-1.5.2/qadence/ml_tools/printing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/saveload.py` & `qadence-1.5.2/qadence/ml_tools/saveload.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/tensors.py` & `qadence-1.5.2/qadence/ml_tools/tensors.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/train_grad.py` & `qadence-1.5.2/qadence/ml_tools/train_grad.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/train_no_grad.py` & `qadence-1.5.2/qadence/ml_tools/train_no_grad.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/ml_tools/utils.py` & `qadence-1.5.2/qadence/ml_tools/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/models/qnn.py` & `qadence-1.5.2/qadence/models/qnn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/models/quantum_model.py` & `qadence-1.5.2/qadence/models/quantum_model.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/noise/protocols.py` & `qadence-1.5.2/qadence/noise/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/noise/readout.py` & `qadence-1.5.2/qadence/noise/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/__init__.py` & `qadence-1.5.2/qadence/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/analog.py` & `qadence-1.5.2/qadence/operations/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/control_ops.py` & `qadence-1.5.2/qadence/operations/control_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/ham_evo.py` & `qadence-1.5.2/qadence/operations/ham_evo.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/parametric.py` & `qadence-1.5.2/qadence/operations/parametric.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/operations/primitive.py` & `qadence-1.5.2/qadence/operations/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/apply_fn.py` & `qadence-1.5.2/qadence/transpile/apply_fn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/block.py` & `qadence-1.5.2/qadence/transpile/block.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/digitalize.py` & `qadence-1.5.2/qadence/transpile/digitalize.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/flatten.py` & `qadence-1.5.2/qadence/transpile/flatten.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/invert.py` & `qadence-1.5.2/qadence/transpile/invert.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/qadence/transpile/transpile.py` & `qadence-1.5.2/qadence/transpile/transpile.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/.gitignore` & `qadence-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/LICENSE` & `qadence-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qadence-1.5.1/README.md` & `qadence-1.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/logo/qadence_logo_white.svg">
-  <source media="(prefers-color-scheme: light)" srcset="./docs/assets/logo/qadence_logo.svg">
-  <img alt="Qadence logo" src="./docs/assets/logo/qadence_logo.svg">
-</picture>
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./docs/extras/assets/logo/qadence_logo_white.svg" width="75%">
+    <source media="(prefers-color-scheme: light)" srcset="./docs/extras/assets/logo/qadence_logo.svg" width="75%">
+    <img alt="Qadence logo" src="./docs/assets/logo/qadence_logo.svg" width="75%">
+  </picture>
+</p>
+
+**Qadence** is a Python package that provides a simple interface to build **digital-analog quantum
+programs** with tunable qubit interactions and arbitrary register topologies realizable on neutral atom devices.
 
 **For a high-level overview of Qadence features, [check out our white paper](https://arxiv.org/abs/2401.09915).**
 
 **For more detailed information, [check out the documentation](https://pasqal-io.github.io/qadence/latest/).**
 
-**Qadence** is a Python package that provides a simple interface to build _**digital-analog quantum
-programs**_ with tunable qubit interaction defined on _**arbitrary register topologies**_ realizable on neutral atom devices.
-
 [![Linting](https://github.com/pasqal-io/qadence/actions/workflows/lint.yml/badge.svg)](https://github.com/pasqal-io/qadence/actions/workflows/lint.yml)
 [![Tests](https://github.com/pasqal-io/qadence/actions/workflows/test_fast.yml/badge.svg)](https://github.com/pasqal-io/qadence/actions/workflows/test_fast.yml)
 [![Documentation](https://github.com/pasqal-io/qadence/actions/workflows/build_docs.yml/badge.svg)](https://pasqal-io.github.io/qadence/latest)
 [![Pypi](https://badge.fury.io/py/qadence.svg)](https://pypi.org/project/qadence/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Feature highlights
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/qadence_arch.svg">
-  <source media="(prefers-color-scheme: light)" srcset="./docs/assets/qadence_arch.svg">
-  <img alt="Qadence architecture" src="./docs/assets/qadence_arch.svg">
-</picture>
-
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./docs/extras/assets/qadence_arch.svg" width="75%">
+    <source media="(prefers-color-scheme: light)" srcset="./docs/extras/assets/qadence_arch.svg" width="75%">
+    <img alt="Qadence architecture" src="./docs/assets/qadence_arch.svg" width="75%">
+  </picture>
+<p align="center">
 
-* A [block-based system](docs/tutorials/getting_started.md) for composing _**complex digital-analog
+* A [block-based system](docs/content/block_system.md) for composing _**complex digital-analog
   programs**_ in a flexible and scalable manner, inspired by the Julia quantum SDK
   [Yao.jl](https://github.com/QuantumBFS/Yao.jl) and functional programming concepts.
 
-* A [simple interface](docs/digital_analog_qc/analog-basics.md) to work with _**interacting neutral-atom qubit systems**_
-  using [arbitrary registers topologies](docs/tutorials/register.md).
-
-* An intuitive [expression-based system](docs/tutorials/parameters.md) developed on top of the symbolic library [Sympy](https://www.sympy.org/en/index.html) to construct _**parametric quantum programs**_ easily.
-
-* [High-order generalized parameter shift rules](docs/advanced_tutorials/differentiability.md) for _**differentiating parametrized quantum operations**_.
+* An intuitive [expression-based system](docs/content/parameters.md) developed on top of the symbolic library [Sympy](https://www.sympy.org/en/index.html) to construct _**parametric quantum programs**_ easily.
 
 * Out-of-the-box _**automatic differentiability**_ of quantum programs with [PyTorch](https://pytorch.org/) integration.
 
-* _**Efficient execution**_ on a variety of different purpose backends: from state vector simulators to tensor network emulators and real devices.
+* [High-order generalized parameter shift rules](docs/tutorials/advanced_tutorials/differentiability.md) for _**differentiating parametrized quantum operations**_.
+
+* A [simple interface](docs/tutorials/digital_analog_qc/analog-basics.md) to work with _**interacting neutral-atom qubit systems**_
+  using [arbitrary registers topologies](docs/content/register.md).
 
 ## Installation guide
 
 Qadence is available on [PyPI](https://pypi.org/project/qadence/) and can be installed using `pip` as follows:
 
 ```bash
 pip install qadence
 ```
 
 The default, pre-installed backend for Qadence is [PyQTorch](https://github.com/pasqal-io/pyqtorch), a differentiable state vector simulator for digital-analog simulation based on `PyTorch`. It is possible to install additional, `PyTorch` -based backends and the circuit visualization library using the following extras:
 
-* `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices.
-* `braket`: The [Braket](https://github.com/amazon-braket/amazon-braket-sdk-python) backend, an open source library that provides a framework for interacting with quantum computing hardware devices through Amazon Braket.
 * `visualization`: A visualization library to display quantum circuit diagrams.
 * `protocols`: A collection of [protocols](https://github.com/pasqal-io/qadence-protocols) for error mitigation in Qadence.
 * `libs`: A collection of [functionalities](https://github.com/pasqal-io/qadence-libs) for graph machine learning problems build on top of Qadence.
+* `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices (experimental).
 
 Qadence also supports a `JAX` engine which is currently supporting the [Horqrux](https://github.com/pasqal-io/horqrux) backend. `horqrux` is currently only available via the [low-level API](examples/backends/low_level/horqrux_backend.py).
 
 
 To install individual extras, use the following syntax (**IMPORTANT** Make sure to use quotes):
 
 ```bash
-pip install "qadence[braket,pulser,visualization]"
+pip install "qadence[pulser,visualization]"
 ```
 
 To install all available extras, simply do:
 
 ```bash
 pip install "qadence[all]"
 ```
@@ -85,18 +85,18 @@
 
 # via conda
 conda install python-graphviz
 ```
 
 ## Contributing
 
-Before making a contribution, please review our [code of conduct](docs/CODE_OF_CONDUCT.md).
+Before making a contribution, please review our [code of conduct](docs/getting_started/CODE_OF_CONDUCT.md).
 
 - **Submitting Issues:** To submit bug reports or feature requests, please use our [issue tracker](https://github.com/pasqal-io/qadence/issues).
-- **Developing in qadence:** To learn more about how to develop within `qadence`, please refer to [contributing guidelines](docs/CONTRIBUTING.md).
+- **Developing in qadence:** To learn more about how to develop within `qadence`, please refer to [contributing guidelines](docs/getting_started/CONTRIBUTING.md).
 
 ### Setting up qadence in development mode
 
 We recommend to use the [`hatch`](https://hatch.pypa.io/latest/) environment manager to install `qadence` from source:
 
 ```bash
 python -m pip install hatch
```

### Comparing `qadence-1.5.1/pyproject.toml` & `qadence-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Vincent Elfving", email = "vincent.elfving@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Roland Guichard", email = "roland.guichard@pasqal.com" },
     { name = "Joao P. Moutinho", email = "joao.moutinho@pasqal.com"},
     { name = "Vytautas Abramavicius", email = "vytautas.abramavicius@pasqal.com" },
     { name = "Gergana Velikova", email = "gergana.velikova@pasqal.com" },
+    { name = "Eduardo Maschio", email = "eduardo.maschio@pasqal.com" },
 ]
 requires-python = ">=3.9,<3.13"
 license = {text = "Apache 2.0"}
-version = "1.5.1"
+version = "1.5.2"
 classifiers=[
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -40,14 +41,15 @@
     "tensorboard>=2.12.0",
     "deepdiff",
     "jsonschema",
     "nevergrad",
     "scipy",
     "pyqtorch==1.1.0",
     "matplotlib",
+    "Arpeggio==2.0.2",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
 
 [project.optional-dependencies]
@@ -67,15 +69,15 @@
     "jaxopt",
     "einops",
     "sympy2jax"]
 protocols = ["qadence-protocols"]
 libs = ["qadence-libs"]
 all = [
   "pulser>=0.15.2",
-  "amazon-braket-sdk",
+  "amazon-braket-sdk==1.71.0",
   "graphviz",
   "protocols",
   "libs",
   # FIXME: will be needed once we support latex labels
   # "latex2svg @ git+https://github.com/Moonbase59/latex2svg.git#egg=latex2svg",
   # "scour",
 ]
```

### Comparing `qadence-1.5.1/PKG-INFO` & `qadence-1.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.3
 Name: qadence
-Version: 1.5.1
+Version: 1.5.2
 Summary: Pasqal interface for circuit-based quantum computing SDKs
-Author-email: Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Gert-Jan Both <gert-jan.both@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Vincent Elfving <vincent.elfving@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>, Vytautas Abramavicius <vytautas.abramavicius@pasqal.com>, Gergana Velikova <gergana.velikova@pasqal.com>
+Author-email: Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Gert-Jan Both <gert-jan.both@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Vincent Elfving <vincent.elfving@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>, Vytautas Abramavicius <vytautas.abramavicius@pasqal.com>, Gergana Velikova <gergana.velikova@pasqal.com>, Eduardo Maschio <eduardo.maschio@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.13,>=3.9
+Requires-Dist: arpeggio==2.0.2
 Requires-Dist: deepdiff
 Requires-Dist: jsonschema
 Requires-Dist: matplotlib
 Requires-Dist: nevergrad
 Requires-Dist: numpy
 Requires-Dist: openfermion
 Requires-Dist: pyqtorch==1.1.0
 Requires-Dist: rich
 Requires-Dist: scipy
 Requires-Dist: sympytorch>=0.1.2
 Requires-Dist: tensorboard>=2.12.0
 Requires-Dist: torch
 Provides-Extra: all
-Requires-Dist: amazon-braket-sdk; extra == 'all'
+Requires-Dist: amazon-braket-sdk==1.71.0; extra == 'all'
 Requires-Dist: graphviz; extra == 'all'
 Requires-Dist: libs; extra == 'all'
 Requires-Dist: protocols; extra == 'all'
 Requires-Dist: pulser>=0.15.2; extra == 'all'
 Provides-Extra: braket
 Requires-Dist: amazon-braket-sdk==1.71.0; extra == 'braket'
 Provides-Extra: horqrux
@@ -49,80 +50,80 @@
 Provides-Extra: pulser
 Requires-Dist: pasqal-cloud>=0.3.5; extra == 'pulser'
 Requires-Dist: pulser>=v0.15.2; extra == 'pulser'
 Provides-Extra: visualization
 Requires-Dist: graphviz; extra == 'visualization'
 Description-Content-Type: text/markdown
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/logo/qadence_logo_white.svg">
-  <source media="(prefers-color-scheme: light)" srcset="./docs/assets/logo/qadence_logo.svg">
-  <img alt="Qadence logo" src="./docs/assets/logo/qadence_logo.svg">
-</picture>
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./docs/extras/assets/logo/qadence_logo_white.svg" width="75%">
+    <source media="(prefers-color-scheme: light)" srcset="./docs/extras/assets/logo/qadence_logo.svg" width="75%">
+    <img alt="Qadence logo" src="./docs/assets/logo/qadence_logo.svg" width="75%">
+  </picture>
+</p>
+
+**Qadence** is a Python package that provides a simple interface to build **digital-analog quantum
+programs** with tunable qubit interactions and arbitrary register topologies realizable on neutral atom devices.
 
 **For a high-level overview of Qadence features, [check out our white paper](https://arxiv.org/abs/2401.09915).**
 
 **For more detailed information, [check out the documentation](https://pasqal-io.github.io/qadence/latest/).**
 
-**Qadence** is a Python package that provides a simple interface to build _**digital-analog quantum
-programs**_ with tunable qubit interaction defined on _**arbitrary register topologies**_ realizable on neutral atom devices.
-
 [![Linting](https://github.com/pasqal-io/qadence/actions/workflows/lint.yml/badge.svg)](https://github.com/pasqal-io/qadence/actions/workflows/lint.yml)
 [![Tests](https://github.com/pasqal-io/qadence/actions/workflows/test_fast.yml/badge.svg)](https://github.com/pasqal-io/qadence/actions/workflows/test_fast.yml)
 [![Documentation](https://github.com/pasqal-io/qadence/actions/workflows/build_docs.yml/badge.svg)](https://pasqal-io.github.io/qadence/latest)
 [![Pypi](https://badge.fury.io/py/qadence.svg)](https://pypi.org/project/qadence/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Feature highlights
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/qadence_arch.svg">
-  <source media="(prefers-color-scheme: light)" srcset="./docs/assets/qadence_arch.svg">
-  <img alt="Qadence architecture" src="./docs/assets/qadence_arch.svg">
-</picture>
-
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./docs/extras/assets/qadence_arch.svg" width="75%">
+    <source media="(prefers-color-scheme: light)" srcset="./docs/extras/assets/qadence_arch.svg" width="75%">
+    <img alt="Qadence architecture" src="./docs/assets/qadence_arch.svg" width="75%">
+  </picture>
+<p align="center">
 
-* A [block-based system](docs/tutorials/getting_started.md) for composing _**complex digital-analog
+* A [block-based system](docs/content/block_system.md) for composing _**complex digital-analog
   programs**_ in a flexible and scalable manner, inspired by the Julia quantum SDK
   [Yao.jl](https://github.com/QuantumBFS/Yao.jl) and functional programming concepts.
 
-* A [simple interface](docs/digital_analog_qc/analog-basics.md) to work with _**interacting neutral-atom qubit systems**_
-  using [arbitrary registers topologies](docs/tutorials/register.md).
-
-* An intuitive [expression-based system](docs/tutorials/parameters.md) developed on top of the symbolic library [Sympy](https://www.sympy.org/en/index.html) to construct _**parametric quantum programs**_ easily.
-
-* [High-order generalized parameter shift rules](docs/advanced_tutorials/differentiability.md) for _**differentiating parametrized quantum operations**_.
+* An intuitive [expression-based system](docs/content/parameters.md) developed on top of the symbolic library [Sympy](https://www.sympy.org/en/index.html) to construct _**parametric quantum programs**_ easily.
 
 * Out-of-the-box _**automatic differentiability**_ of quantum programs with [PyTorch](https://pytorch.org/) integration.
 
-* _**Efficient execution**_ on a variety of different purpose backends: from state vector simulators to tensor network emulators and real devices.
+* [High-order generalized parameter shift rules](docs/tutorials/advanced_tutorials/differentiability.md) for _**differentiating parametrized quantum operations**_.
+
+* A [simple interface](docs/tutorials/digital_analog_qc/analog-basics.md) to work with _**interacting neutral-atom qubit systems**_
+  using [arbitrary registers topologies](docs/content/register.md).
 
 ## Installation guide
 
 Qadence is available on [PyPI](https://pypi.org/project/qadence/) and can be installed using `pip` as follows:
 
 ```bash
 pip install qadence
 ```
 
 The default, pre-installed backend for Qadence is [PyQTorch](https://github.com/pasqal-io/pyqtorch), a differentiable state vector simulator for digital-analog simulation based on `PyTorch`. It is possible to install additional, `PyTorch` -based backends and the circuit visualization library using the following extras:
 
-* `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices.
-* `braket`: The [Braket](https://github.com/amazon-braket/amazon-braket-sdk-python) backend, an open source library that provides a framework for interacting with quantum computing hardware devices through Amazon Braket.
 * `visualization`: A visualization library to display quantum circuit diagrams.
 * `protocols`: A collection of [protocols](https://github.com/pasqal-io/qadence-protocols) for error mitigation in Qadence.
 * `libs`: A collection of [functionalities](https://github.com/pasqal-io/qadence-libs) for graph machine learning problems build on top of Qadence.
+* `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices (experimental).
 
 Qadence also supports a `JAX` engine which is currently supporting the [Horqrux](https://github.com/pasqal-io/horqrux) backend. `horqrux` is currently only available via the [low-level API](examples/backends/low_level/horqrux_backend.py).
 
 
 To install individual extras, use the following syntax (**IMPORTANT** Make sure to use quotes):
 
 ```bash
-pip install "qadence[braket,pulser,visualization]"
+pip install "qadence[pulser,visualization]"
 ```
 
 To install all available extras, simply do:
 
 ```bash
 pip install "qadence[all]"
 ```
@@ -140,18 +141,18 @@
 
 # via conda
 conda install python-graphviz
 ```
 
 ## Contributing
 
-Before making a contribution, please review our [code of conduct](docs/CODE_OF_CONDUCT.md).
+Before making a contribution, please review our [code of conduct](docs/getting_started/CODE_OF_CONDUCT.md).
 
 - **Submitting Issues:** To submit bug reports or feature requests, please use our [issue tracker](https://github.com/pasqal-io/qadence/issues).
-- **Developing in qadence:** To learn more about how to develop within `qadence`, please refer to [contributing guidelines](docs/CONTRIBUTING.md).
+- **Developing in qadence:** To learn more about how to develop within `qadence`, please refer to [contributing guidelines](docs/getting_started/CONTRIBUTING.md).
 
 ### Setting up qadence in development mode
 
 We recommend to use the [`hatch`](https://hatch.pypa.io/latest/) environment manager to install `qadence` from source:
 
 ```bash
 python -m pip install hatch
```

