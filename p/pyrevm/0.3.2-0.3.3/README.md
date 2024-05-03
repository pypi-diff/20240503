# Comparing `tmp/pyrevm-0.3.2.tar.gz` & `tmp/pyrevm-0.3.3.tar.gz`

## Comparing `pyrevm-0.3.2.tar` & `pyrevm-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pyrevm-0.3.2/Cargo.toml
--rw-r--r--   0     1001      127      612 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/py.yml
--rw-r--r--   0     1001      127     3522 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1537 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.github/workflows/rust.yml
--rw-r--r--   0     1001      127       30 2024-05-01 13:03:54.000000 pyrevm-0.3.2/.gitignore
--rw-r--r--   0     1001      127      205 2024-05-01 13:03:54.000000 pyrevm-0.3.2/Makefile
--rw-r--r--   0     1001      127     2265 2024-05-01 13:03:54.000000 pyrevm-0.3.2/README.md
--rw-r--r--   0     1001      127    35461 2024-05-01 13:03:54.000000 pyrevm-0.3.2/bench/snailtracer/snailtracer.evm
--rw-r--r--   0     1001      127     1715 2024-05-01 13:03:54.000000 pyrevm-0.3.2/bench/snailtracer/snailtracer.py
--rw-r--r--   0     1001      127    16997 2024-05-01 13:03:54.000000 pyrevm-0.3.2/poetry.lock
--rw-r--r--   0     1001      127    10135 2024-05-01 13:03:54.000000 pyrevm-0.3.2/pyrevm.pyi
--rw-r--r--   0     1001      127     4400 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/database.rs
--rw-r--r--   0     1001      127     1202 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/empty_db_wrapper.rs
--rw-r--r--   0     1001      127    12521 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/evm.rs
--rw-r--r--   0     1001      127     6226 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/executor.rs
--rw-r--r--   0     1001      127      894 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/lib.rs
--rw-r--r--   0     1001      127      786 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/pystdout.rs
--rw-r--r--   0     1001      127      193 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/checkpoint.rs
--rw-r--r--   0     1001      127     8830 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/evm_env.rs
--rw-r--r--   0     1001      127     2431 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/execution_result.rs
--rw-r--r--   0     1001      127     1898 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/info.rs
--rw-r--r--   0     1001      127      321 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/types/mod.rs
--rw-r--r--   0     1001      127      991 2024-05-01 13:03:54.000000 pyrevm-0.3.2/src/utils.rs
--rw-r--r--   0     1001      127        0 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/__init__.py
--rw-r--r--   0     1001      127      320 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blob_base_fee.bin
--rw-r--r--   0     1001      127      492 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blob_hash.bin
--rw-r--r--   0     1001      127      265 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/blueprint.bin
--rw-r--r--   0     1001      127     1194 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/full_math.bin
--rw-r--r--   0     1001      127     6248 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/fixtures/weth_9.bin
--rw-r--r--   0     1001      127     7995 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/test_evm.py
--rw-r--r--   0     1001      127      511 2024-05-01 13:03:54.000000 pyrevm-0.3.2/tests/utils.py
--rw-r--r--   0     1001      127    82487 2024-05-01 13:03:54.000000 pyrevm-0.3.2/Cargo.lock
--rw-r--r--   0     1001      127      711 2024-05-01 13:03:54.000000 pyrevm-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 pyrevm-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pyrevm-0.3.3/Cargo.toml
+-rw-r--r--   0     1001      127      612 2024-05-03 14:55:32.000000 pyrevm-0.3.3/.github/workflows/py.yml
+-rw-r--r--   0     1001      127     3522 2024-05-03 14:55:32.000000 pyrevm-0.3.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1537 2024-05-03 14:55:32.000000 pyrevm-0.3.3/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       30 2024-05-03 14:55:32.000000 pyrevm-0.3.3/.gitignore
+-rw-r--r--   0     1001      127      284 2024-05-03 14:55:32.000000 pyrevm-0.3.3/Makefile
+-rw-r--r--   0     1001      127     2265 2024-05-03 14:55:32.000000 pyrevm-0.3.3/README.md
+-rw-r--r--   0     1001      127    35461 2024-05-03 14:55:32.000000 pyrevm-0.3.3/bench/snailtracer/snailtracer.evm
+-rw-r--r--   0     1001      127     1715 2024-05-03 14:55:32.000000 pyrevm-0.3.3/bench/snailtracer/snailtracer.py
+-rw-r--r--   0     1001      127    16997 2024-05-03 14:55:32.000000 pyrevm-0.3.3/poetry.lock
+-rw-r--r--   0     1001      127    10135 2024-05-03 14:55:32.000000 pyrevm-0.3.3/pyrevm.pyi
+-rw-r--r--   0     1001      127     4400 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/database.rs
+-rw-r--r--   0     1001      127     1202 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/empty_db_wrapper.rs
+-rw-r--r--   0     1001      127    12525 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/evm.rs
+-rw-r--r--   0     1001      127     6232 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/executor.rs
+-rw-r--r--   0     1001      127      894 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/lib.rs
+-rw-r--r--   0     1001      127      786 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/pystdout.rs
+-rw-r--r--   0     1001      127      193 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/types/checkpoint.rs
+-rw-r--r--   0     1001      127     8830 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/types/evm_env.rs
+-rw-r--r--   0     1001      127     2431 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/types/execution_result.rs
+-rw-r--r--   0     1001      127     1898 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/types/info.rs
+-rw-r--r--   0     1001      127      321 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/types/mod.rs
+-rw-r--r--   0     1001      127      991 2024-05-03 14:55:32.000000 pyrevm-0.3.3/src/utils.rs
+-rw-r--r--   0     1001      127        0 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/__init__.py
+-rw-r--r--   0     1001      127      320 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/blob_base_fee.bin
+-rw-r--r--   0     1001      127      492 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/blob_hash.bin
+-rw-r--r--   0     1001      127      265 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/blueprint.bin
+-rw-r--r--   0     1001      127     1194 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/full_math.bin
+-rw-r--r--   0     1001      127      268 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/min.bin
+-rw-r--r--   0     1001      127     6248 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/fixtures/weth_9.bin
+-rw-r--r--   0     1001      127     8507 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/test_evm.py
+-rw-r--r--   0     1001      127      511 2024-05-03 14:55:32.000000 pyrevm-0.3.3/tests/utils.py
+-rw-r--r--   0     1001      127    82487 2024-05-03 14:55:32.000000 pyrevm-0.3.3/Cargo.lock
+-rw-r--r--   0     1001      127      711 2024-05-03 14:55:32.000000 pyrevm-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 pyrevm-0.3.3/PKG-INFO
```

### Comparing `pyrevm-0.3.2/.github/workflows/py.yml` & `pyrevm-0.3.3/.github/workflows/py.yml`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/.github/workflows/release.yml` & `pyrevm-0.3.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/.github/workflows/rust.yml` & `pyrevm-0.3.3/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/README.md` & `pyrevm-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/bench/snailtracer/snailtracer.evm` & `pyrevm-0.3.3/bench/snailtracer/snailtracer.evm`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/bench/snailtracer/snailtracer.py` & `pyrevm-0.3.3/bench/snailtracer/snailtracer.py`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/poetry.lock` & `pyrevm-0.3.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/pyrevm.pyi` & `pyrevm-0.3.3/pyrevm.pyi`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/database.rs` & `pyrevm-0.3.3/src/database.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/empty_db_wrapper.rs` & `pyrevm-0.3.3/src/empty_db_wrapper.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/evm.rs` & `pyrevm-0.3.3/src/evm.rs`

 * *Files 1% similar despite different names*

```diff
@@ -369,13 +369,13 @@
     }
 
     fn run_env(&mut self, env: RevmEnv, is_static: bool) -> PyResult<RevmExecutionResult> {
         self.context.env = Box::new(env);
         let evm_context: EvmContext<DB> =
             replace(&mut self.context, EvmContext::new(DB::new_memory()));
         let (result, evm_context) =
-            call_evm(evm_context, self.handler_cfg, self.tracing, is_static)?;
+            call_evm(evm_context, self.handler_cfg, self.tracing, is_static);
         self.context = evm_context;
-        self.result = Some(result.clone());
-        Ok(result)
+        self.result = result.as_ref().ok().cloned();
+        result
     }
 }
```

### Comparing `pyrevm-0.3.2/src/executor.rs` & `pyrevm-0.3.3/src/executor.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-use crate::database::DB;
-use crate::utils::pyerr;
+use std::mem::replace;
+
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::PyResult;
 use revm::inspectors::TracerEip3155;
 use revm::precompile::Log;
 use revm::primitives::TransactTo;
 use revm::primitives::{ExecutionResult, ShanghaiSpec};
 use revm::{
     inspector_handle_register, Context, ContextWithHandlerCfg, Evm, EvmContext, FrameOrResult,
     FrameResult,
 };
 use revm_interpreter::primitives::HandlerCfg;
 use revm_interpreter::{gas, CallInputs, CreateInputs, SuccessOrHalt};
-use std::mem::replace;
+
+use crate::database::DB;
+use crate::utils::pyerr;
 
 /// Calls the EVM with the given context and handler configuration.
 pub(crate) fn call_evm(
     evm_context: EvmContext<DB>,
     handler_cfg: HandlerCfg,
     tracing: bool,
     is_static: bool,
-) -> PyResult<(ExecutionResult, EvmContext<DB>)> {
+) -> (PyResult<ExecutionResult>, EvmContext<DB>) {
     if tracing {
         let tracer = TracerEip3155::new(Box::new(crate::pystdout::PySysStdout {}));
-        let evm = Evm::builder()
+        let mut evm = Evm::builder()
             .with_context_with_handler_cfg(ContextWithHandlerCfg {
                 cfg: handler_cfg,
                 context: Context {
                     evm: evm_context,
                     external: tracer,
                 },
             })
             .append_handler_register(inspector_handle_register)
             .build();
-        run_evm(evm, is_static)
+        (run_evm(&mut evm, is_static), evm.context.evm)
     } else {
-        let evm = Evm::builder()
+        let mut evm = Evm::builder()
             .with_context_with_handler_cfg(ContextWithHandlerCfg {
                 cfg: handler_cfg,
                 context: Context {
                     evm: evm_context,
                     external: (),
                 },
             })
             .build();
-        run_evm(evm, is_static)
+        (run_evm(&mut evm, is_static), evm.context.evm)
     }
 }
 
 /// Calls the given evm. This is originally a copy of revm::Evm::transact, but it calls our own output function
-fn run_evm<EXT>(
-    mut evm: Evm<'_, EXT, DB>,
-    is_static: bool,
-) -> PyResult<(ExecutionResult, EvmContext<DB>)> {
+fn run_evm<EXT>(evm: &mut Evm<'_, EXT, DB>, is_static: bool) -> PyResult<ExecutionResult> {
     let logs_i = evm.context.evm.journaled_state.logs.len();
 
     evm.handler
         .validation()
         .env(&evm.context.evm.env)
         .map_err(pyerr)?;
     let initial_gas_spend = evm
@@ -133,15 +132,15 @@
     post_exec
         .reward_beneficiary(ctx, result.gas())
         .map_err(pyerr)?;
 
     let logs = ctx.evm.journaled_state.logs[logs_i..].to_vec();
 
     // Returns output of transaction.
-    Ok((output(ctx, result, logs)?, evm.context.evm))
+    output(ctx, result, logs)
 }
 
 fn call_inputs<EXT>(
     ctx: &&mut Context<EXT, DB>,
     gas_limit: u64,
     is_static: bool,
 ) -> Box<CallInputs> {
```

### Comparing `pyrevm-0.3.2/src/lib.rs` & `pyrevm-0.3.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/pystdout.rs` & `pyrevm-0.3.3/src/pystdout.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/types/evm_env.rs` & `pyrevm-0.3.3/src/types/evm_env.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/types/execution_result.rs` & `pyrevm-0.3.3/src/types/execution_result.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/types/info.rs` & `pyrevm-0.3.3/src/types/info.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/src/utils.rs` & `pyrevm-0.3.3/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/tests/fixtures/full_math.bin` & `pyrevm-0.3.3/tests/fixtures/full_math.bin`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/tests/fixtures/weth_9.bin` & `pyrevm-0.3.3/tests/fixtures/weth_9.bin`

 * *Files identical despite different names*

### Comparing `pyrevm-0.3.2/tests/test_evm.py` & `pyrevm-0.3.3/tests/test_evm.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,7 +276,24 @@
         to=deployer_address,
         calldata=bytes.fromhex("cc883ac4"),  # method_id("log_blobhashes()")
     )
     logged = [log.data[0][1] for log in evm.result.logs]
 
     # the contract logs 6 blob hashes, so pad with 0s
     assert logged == blob_hashes + [b"\0" * 32] * (6 - len(blob_hashes))
+
+
+@pytest.mark.parametrize("kwargs", KWARG_CASES)
+def test_call_reverting(kwargs):
+    evm = EVM()
+    code = load_contract_bin("min.bin")
+    deploy_address = evm.deploy(address, code)
+
+    with pytest.raises(RuntimeError) as err:
+        evm.message_call(
+            caller=address,
+            to=deploy_address,
+            value=10,
+        )
+
+    assert evm.get_code(deploy_address), "The code should still be deployed after revert"
+    assert str(err.value).startswith("Transaction(LackOfFundForMaxFee")
```

### Comparing `pyrevm-0.3.2/Cargo.lock` & `pyrevm-0.3.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1813,15 +1813,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyrevm"
-version = "0.3.2"
+version = "0.3.3"
 dependencies = [
  "ethers-core",
  "ethers-providers",
  "pyo3",
  "revm",
  "revm-interpreter",
  "ruint",
```

### Comparing `pyrevm-0.3.2/pyproject.toml` & `pyrevm-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [tool.poetry]
 name = "pyrevm"
-version = "0.3.2"  # Cargo.toml needs to be updated for releases
+version = "0.3.3"  # Cargo.toml needs to be updated for releases
 description = "Python bindings to rust evm (revm)"
 authors = ["Georgios Konstantopoulos <me@gakonst.com>", "Dani Popes", "Daniel Schiavini", "Charles Cooper"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 maturin = "1.5.1"
```

### Comparing `pyrevm-0.3.2/PKG-INFO` & `pyrevm-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrevm
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # <h1 align="center"> pyrevm </h1>
```

