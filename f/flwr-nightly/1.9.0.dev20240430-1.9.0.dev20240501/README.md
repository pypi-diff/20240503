# Comparing `tmp/flwr_nightly-1.9.0.dev20240430.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240430.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240501.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240430.tar` & `flwr_nightly-1.9.0.dev20240501.tar`

### file list

```diff
@@ -1,216 +1,218 @@
--rw-r--r--   0        0        0    11358 2024-04-30 23:05:21.507832 flwr_nightly-1.9.0.dev20240430/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-30 23:05:21.507832 flwr_nightly-1.9.0.dev20240430/README.md
--rw-r--r--   0        0        0     5776 2024-04-30 23:05:34.051937 flwr_nightly-1.9.0.dev20240430/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     4899 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5989 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      667 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1911 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      371 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      521 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      590 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      570 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      569 2024-04-30 23:05:21.919835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2334 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4903 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9052 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6920 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12686 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-30 23:05:21.923835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4533 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4707 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    28282 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5287 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-30 23:05:21.927835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4796 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     5902 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    11651 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    27167 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7709 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-30 23:05:21.931836 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    14380 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15896 2024-04-30 23:05:21.935835 flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240430/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-01 23:06:01.706781 flwr_nightly-1.9.0.dev20240501/LICENSE
+-rw-r--r--   0        0        0    12916 2024-05-01 23:06:01.706781 flwr_nightly-1.9.0.dev20240501/README.md
+-rw-r--r--   0        0        0     5812 2024-05-01 23:06:14.202758 flwr_nightly-1.9.0.dev20240501/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-05-01 23:06:02.118780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-01 23:06:02.118780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5106 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/build.py
+-rw-r--r--   0        0        0     4899 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     6035 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1280 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      579 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0     1044 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
+-rw-r--r--   0        0        0      523 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      592 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      572 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      571 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     5012 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9052 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-01 23:06:02.122780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6920 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12686 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4533 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4707 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    28282 2024-05-01 23:06:02.126780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5287 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17502 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12949 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4796 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     5902 2024-05-01 23:06:02.130780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    11651 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    27167 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7709 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1348 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15896 2024-05-01 23:06:02.134780 flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15303 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240501/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240430/LICENSE` & `flwr_nightly-1.9.0.dev20240501/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/README.md` & `flwr_nightly-1.9.0.dev20240501/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/pyproject.toml` & `flwr_nightly-1.9.0.dev20240501/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240430"
+version = "1.9.0.dev20240501"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
@@ -55,27 +55,28 @@
 flwr = "flwr.cli.app:app"
 flower-driver-api = "flwr.server:run_driver_api"
 flower-fleet-api = "flwr.server:run_fleet_api"
 flower-superlink = "flwr.server:run_superlink"
 flower-supernode = "flwr.client:run_supernode"
 flower-client-app = "flwr.client:run_client_app"
 flower-server-app = "flwr.server:run_server_app"
-flower-simulation = "flwr.simulation:run_simulation_from_cli"
+flower-simulation = "flwr.simulation.run_simulation:run_simulation_from_cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # Mandatory dependencies
 numpy = "^1.21.0"
 grpcio = "^1.60.0"
 protobuf = "^4.25.2"
 cryptography = "^42.0.4"
 pycryptodome = "^3.18.0"
 iterators = "^0.0.2"
 typer = { version = "^0.9.0", extras=["all"] }
 tomli = "^2.0.1"
+pathspec = "^0.12.1"
 # Optional dependencies (Simulation Engine)
 ray = { version = "==2.6.3", optional = true, python = ">=3.8,<3.12" }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.31.0", optional = true }
 starlette = { version = "^0.31.0", optional = true }
 uvicorn = { version = "^0.23.0", extras = ["standard"], optional = true }
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower command line interface."""
 
 import typer
 
+from .build import build
 from .example import example
 from .new import new
 from .run import run
 
 app = typer.Typer(
     help=typer.style(
         "flwr is the Flower command line interface.",
@@ -28,10 +29,11 @@
     ),
     no_args_is_help=True,
 )
 
 app.command()(new)
 app.command()(example)
 app.command()(run)
+app.command()(build)
 
 if __name__ == "__main__":
     app()
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
             "template": f"app/code/client.{framework_str}.py.tpl"
         },
     }
 
     # Depending on the framework, generate task.py file
     frameworks_with_tasks = [
         MlFramework.PYTORCH.value.lower(),
+        MlFramework.TENSORFLOW.value.lower(),
     ]
     if framework_str in frameworks_with_tasks:
         files[f"{import_name}/task.py"] = {
             "template": f"app/code/task.{framework_str}.py.tpl"
         }
 
     context = {
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ```bash
 pip install .
 ```
 
 ## Run (Simulation Engine)
 
-In the `$import_name` directory, use `flwr run` to run a local simulation:
+In the `$project_name` directory, use `flwr run` to run a local simulation:
 
 ```bash
 flwr run
 ```
 
 ## Run (Deployment Engine)
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
-license = {text = "Apache License (2.0)"}
+license = { text = "Apache License (2.0)" }
 dependencies = [
     "flwr[simulation]>=1.8.0,<2.0",
     "numpy>=1.21.0",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["."]
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
-license = {text = "Apache License (2.0)"}
+license = { text = "Apache License (2.0)" }
 dependencies = [
     "flwr[simulation]>=1.8.0,<2.0",
     "flwr-datasets[vision]>=0.0.2,<1.0.0",
     "torch==2.2.1",
     "torchvision==0.17.1",
 ]
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
-license = {text = "Apache License (2.0)"}
+license = { text = "Apache License (2.0)" }
 dependencies = [
     "flwr[simulation]>=1.8.0,<2.0",
     "flwr-datasets[vision]>=0.0.2,<1.0.0",
     "scikit-learn>=1.1.1",
 ]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "$package_name"
 version = "1.0.0"
 description = ""
 authors = [
     { name = "The Flower Authors", email = "hello@flower.ai" },
 ]
-license = {text = "Apache License (2.0)"}
+license = { text = "Apache License (2.0)" }
 dependencies = [
     "flwr[simulation]>=1.8.0,<2.0",
     "flwr-datasets[vision]>=0.0.2,<1.0.0",
     "tensorflow>=2.11.1",
 ]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,17 @@
     # Clip the client update
     compute_clip_model_update(
         client_to_server_params,
         server_to_client_params,
         clipping_norm,
     )
 
-    log(INFO, "fixedclipping_mod: parameters are clipped by value: %s.", clipping_norm)
+    log(
+        INFO, "fixedclipping_mod: parameters are clipped by value: %.4f.", clipping_norm
+    )
 
     fit_res.parameters = ndarrays_to_parameters(client_to_server_params)
     out_msg.content = compat.fitres_to_recordset(fit_res, keep_input=True)
     return out_msg
 
 
 def adaptiveclipping_mod(
@@ -142,15 +144,15 @@
     norm_bit = compute_adaptive_clip_model_update(
         client_to_server_params,
         server_to_client_params,
         clipping_norm,
     )
     log(
         INFO,
-        "adaptiveclipping_mod: parameters are clipped by value: %s.",
+        "adaptiveclipping_mod: parameters are clipped by value: %.4f.",
         clipping_norm,
     )
 
     fit_res.parameters = ndarrays_to_parameters(client_to_server_params)
 
     fit_res.metrics[KEY_NORM_BIT] = norm_bit
     out_msg.content = compat.fitres_to_recordset(fit_res, keep_input=True)
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/localdp_mod.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,25 +124,31 @@
         # Clip the client update
         compute_clip_model_update(
             client_to_server_params,
             server_to_client_params,
             self.clipping_norm,
         )
         log(
-            INFO, "LocalDpMod: parameters are clipped by value: %s.", self.clipping_norm
+            INFO,
+            "LocalDpMod: parameters are clipped by value: %.4f.",
+            self.clipping_norm,
         )
 
         fit_res.parameters = ndarrays_to_parameters(client_to_server_params)
 
         # Add noise to model params
         add_localdp_gaussian_noise_to_params(
             fit_res.parameters, self.sensitivity, self.epsilon, self.delta
         )
+
+        noise_value_sd = (
+            self.sensitivity * np.sqrt(2 * np.log(1.25 / self.delta)) / self.epsilon
+        )
         log(
             INFO,
             "LocalDpMod: local DP noise with "
-            "standard deviation: %s added to parameters.",
-            self.sensitivity * np.sqrt(2 * np.log(1.25 / self.delta)) / self.epsilon,
+            "standard deviation: %.4f added to parameters.",
+            noise_value_sd,
         )
 
         out_msg.content = compat.fitres_to_recordset(fit_res, keep_input=True)
         return out_msg
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             ]
 
             norm_bit = adaptive_clip_inputs_inplace(model_update, self.clipping_norm)
             norm_bit_set_count += norm_bit
 
             log(
                 INFO,
-                "aggregate_fit: parameters are clipped by value: %s.",
+                "aggregate_fit: parameters are clipped by value: %.4f.",
                 self.clipping_norm,
             )
 
             for i, _ in enumerate(self.current_round_params):
                 param[i] = self.current_round_params[i] + model_update[i]
             # Convert back to parameters
             res.parameters = ndarrays_to_parameters(param)
@@ -230,15 +230,16 @@
                 aggregated_params,
                 self.noise_multiplier,
                 self.clipping_norm,
                 self.num_sampled_clients,
             )
             log(
                 INFO,
-                "aggregate_fit: central DP noise with standard deviation: %s added to parameters.",
+                "aggregate_fit: central DP noise with "
+                "standard deviation: %.4f added to parameters.",
                 compute_stdv(
                     self.noise_multiplier, self.clipping_norm, self.num_sampled_clients
                 ),
             )
 
         return aggregated_params, metrics
 
@@ -420,15 +421,16 @@
                 aggregated_params,
                 self.noise_multiplier,
                 self.clipping_norm,
                 self.num_sampled_clients,
             )
             log(
                 INFO,
-                "aggregate_fit: central DP noise with standard deviation: %s added to parameters.",
+                "aggregate_fit: central DP noise with "
+                "standard deviation: %.4f added to parameters.",
                 compute_stdv(
                     self.noise_multiplier, self.clipping_norm, self.num_sampled_clients
                 ),
             )
 
         return aggregated_params, metrics
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             param = parameters_to_ndarrays(res.parameters)
             # Compute and clip update
             compute_clip_model_update(
                 param, self.current_round_params, self.clipping_norm
             )
             log(
                 INFO,
-                "aggregate_fit: parameters are clipped by value: %s.",
+                "aggregate_fit: parameters are clipped by value: %.4f.",
                 self.clipping_norm,
             )
             # Convert back to parameters
             res.parameters = ndarrays_to_parameters(param)
 
         # Pass the new parameters for aggregation
         aggregated_params, metrics = self.strategy.aggregate_fit(
@@ -176,15 +176,16 @@
                 self.noise_multiplier,
                 self.clipping_norm,
                 self.num_sampled_clients,
             )
 
             log(
                 INFO,
-                "aggregate_fit: central DP noise with standard deviation: %s added to parameters.",
+                "aggregate_fit: central DP noise with "
+                "standard deviation: %.4f added to parameters.",
                 compute_stdv(
                     self.noise_multiplier, self.clipping_norm, self.num_sampled_clients
                 ),
             )
 
         return aggregated_params, metrics
 
@@ -333,19 +334,21 @@
                 aggregated_params,
                 self.noise_multiplier,
                 self.clipping_norm,
                 self.num_sampled_clients,
             )
             log(
                 INFO,
-                "aggregate_fit: central DP noise with standard deviation: %s added to parameters.",
+                "aggregate_fit: central DP noise with "
+                "standard deviation: %.4f added to parameters.",
                 compute_stdv(
                     self.noise_multiplier, self.clipping_norm, self.num_sampled_clients
                 ),
             )
+
         return aggregated_params, metrics
 
     def aggregate_evaluate(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, EvaluateRes]],
         failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Flower simulation."""
 
 
 import importlib
 
-from flwr.simulation.run_simulation import run_simulation, run_simulation_from_cli
+from flwr.simulation.run_simulation import run_simulation
 
 is_ray_installed = importlib.util.find_spec("ray") is not None
 
 if is_ray_installed:
     from flwr.simulation.app import start_simulation
 else:
     RAY_IMPORT_ERROR: str = """Unable to import module `ray`.
@@ -32,8 +32,8 @@
 """
 
     def start_simulation(*args, **kwargs):  # type: ignore
         """Log error stating that module `ray` could not be imported."""
         raise ImportError(RAY_IMPORT_ERROR)
 
 
-__all__ = ["start_simulation", "run_simulation_from_cli", "run_simulation"]
+__all__ = ["start_simulation", "run_simulation"]
```

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240501/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240430/PKG-INFO` & `flwr_nightly-1.9.0.dev20240501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240430
+Version: 1.9.0.dev20240501
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
@@ -32,14 +32,15 @@
 Classifier: Typing :: Typed
 Provides-Extra: rest
 Provides-Extra: simulation
 Requires-Dist: cryptography (>=42.0.4,<43.0.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: pathspec (>=0.12.1,<0.13.0)
 Requires-Dist: protobuf (>=4.25.2,<5.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: ray (==2.6.3) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "simulation")
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "rest"
 Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest"
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240430 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240501 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
@@ -17,23 +17,24 @@
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Mathematics Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
 Provides-Extra: rest Provides-Extra: simulation Requires-Dist: cryptography
 (>=42.0.4,<43.0.0) Requires-Dist: grpcio (>=1.60.0,<2.0.0) Requires-Dist:
 iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
-Dist: protobuf (>=4.25.2,<5.0.0) Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
-Requires-Dist: ray (==2.6.3) ; (python_version >= "3.8" and python_version <
-"3.12") and (extra == "simulation") Requires-Dist: requests (>=2.31.0,<3.0.0) ;
-extra == "rest" Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest"
-Requires-Dist: tomli (>=2.0.1,<3.0.0) Requires-Dist: typer[all]
-(>=0.9.0,<0.10.0) Requires-Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra
-== "rest" Project-URL: Documentation, https://flower.ai Project-URL:
-Repository, https://github.com/adap/flower Description-Content-Type: text/
-markdown # Flower: A Friendly Federated Learning Framework
+Dist: pathspec (>=0.12.1,<0.13.0) Requires-Dist: protobuf (>=4.25.2,<5.0.0)
+Requires-Dist: pycryptodome (>=3.18.0,<4.0.0) Requires-Dist: ray (==2.6.3) ;
+(python_version >= "3.8" and python_version < "3.12") and (extra ==
+"simulation") Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "rest"
+Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest" Requires-Dist:
+tomli (>=2.0.1,<3.0.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Requires-
+Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra == "rest" Project-URL:
+Documentation, https://flower.ai Project-URL: Repository, https://github.com/
+adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
+Federated Learning Framework
                                _[_F_l_o_w_e_r_ _W_e_b_s_i_t_e_]
                   _W_e_b_s_i_t_e | _B_l_o_g | _D_o_c_s | _C_o_n_f_e_r_e_n_c_e | _S_l_a_c_k
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
```

