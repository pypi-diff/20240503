# Comparing `tmp/runhelper-0.2.2.tar.gz` & `tmp/runhelper-0.2.3.tar.gz`

## Comparing `runhelper-0.2.2.tar` & `runhelper-0.2.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 runhelper-0.2.2/Cargo.lock
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 runhelper-0.2.2/Cargo.toml
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 runhelper-0.2.2/runhelper/__init__.py
--rwxr-xr-x   0        0        0     3530 2020-02-02 00:00:00.000000 runhelper-0.2.2/runhelper/log.py
--rwxr-xr-x   0        0        0     5808 2020-02-02 00:00:00.000000 runhelper-0.2.2/runhelper/run.py
--rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 runhelper-0.2.2/src/hashany.rs
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 runhelper-0.2.2/src/lib.rs
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 runhelper-0.2.2/src/log.rs
--rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/.rustc_info.json
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/CACHEDIR.TAG
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.cargo-lock
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/dep-lib-deranged
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/lib-deranged
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/lib-deranged.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/lib-deranged
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/lib-deranged.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-bee969585c26d931/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-bee969585c26d931/lib-itoa
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-bee969585c26d931/lib-itoa.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-d42e34ac651202b6/dep-lib-itoa
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-d42e34ac651202b6/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-d42e34ac651202b6/lib-itoa
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/itoa-d42e34ac651202b6/lib-itoa.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/lib-lazy_static
--rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/lib-lazy_static.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/dep-lib-lazy_static
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/lib-lazy_static
--rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/lib-lazy_static.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0b8f11d4e6b07352/dep-lib-log
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0b8f11d4e6b07352/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0b8f11d4e6b07352/lib-log
--rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0b8f11d4e6b07352/lib-log.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/lib-log
--rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/lib-log.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-228412733cf151d6/dep-lib-log
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-228412733cf151d6/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-228412733cf151d6/lib-log
--rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-228412733cf151d6/lib-log.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-93eb299558ddc7c9/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-93eb299558ddc7c9/lib-log
--rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/log-93eb299558ddc7c9/lib-log.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/dep-lib-num-conv
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/lib-num-conv
--rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/lib-num-conv.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-3d14c87ded27d719/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-3d14c87ded27d719/lib-num-conv
--rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-3d14c87ded27d719/lib-num-conv.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/dep-lib-num-conv
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/lib-num-conv
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/lib-num-conv.json
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/dep-lib-powerfmt
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/lib-powerfmt
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/lib-powerfmt.json
--rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/invoked.timestamp
--rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/lib-powerfmt
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/lib-powerfmt.json
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 runhelper-0.2.2/target/debug/.fingerprint/runhelper-05d804ff06814ff8/dep-test-lib-runhelper
--rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 runhelper-0.2.2/.gitignore
--rwxr-xr-x   0        0        0    35821 2020-02-02 00:00:00.000000 runhelper-0.2.2/LICENSE
--rwxr-xr-x   0        0        0     2933 2020-02-02 00:00:00.000000 runhelper-0.2.2/README.md
--rwxr-xr-x   0        0        0      610 2020-02-02 00:00:00.000000 runhelper-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    43802 2020-02-02 00:00:00.000000 runhelper-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 runhelper-0.2.3/Cargo.lock
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 runhelper-0.2.3/Cargo.toml
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 runhelper-0.2.3/runhelper/__init__.py
+-rwxr-xr-x   0        0        0     3530 2020-02-02 00:00:00.000000 runhelper-0.2.3/runhelper/log.py
+-rwxr-xr-x   0        0        0     5808 2020-02-02 00:00:00.000000 runhelper-0.2.3/runhelper/run.py
+-rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 runhelper-0.2.3/src/hashany.rs
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 runhelper-0.2.3/src/lib.rs
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 runhelper-0.2.3/src/log.rs
+-rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/.rustc_info.json
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.cargo-lock
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/dep-lib-deranged
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/lib-deranged
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-18559f2d1aa2f84b/lib-deranged.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/lib-deranged
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/deranged-bc6ce09c37ec6c58/lib-deranged.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-bee969585c26d931/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-bee969585c26d931/lib-itoa
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-bee969585c26d931/lib-itoa.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-d42e34ac651202b6/dep-lib-itoa
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-d42e34ac651202b6/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-d42e34ac651202b6/lib-itoa
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/itoa-d42e34ac651202b6/lib-itoa.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/lib-lazy_static
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-02ca1d3ff1a3af92/lib-lazy_static.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/dep-lib-lazy_static
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/lib-lazy_static
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/lazy_static-a74cec1b63bee500/lib-lazy_static.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0b8f11d4e6b07352/dep-lib-log
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0b8f11d4e6b07352/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0b8f11d4e6b07352/lib-log
+-rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0b8f11d4e6b07352/lib-log.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/lib-log
+-rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-0bfdd8ec9e3b7f29/lib-log.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-228412733cf151d6/dep-lib-log
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-228412733cf151d6/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-228412733cf151d6/lib-log
+-rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-228412733cf151d6/lib-log.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-93eb299558ddc7c9/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-93eb299558ddc7c9/lib-log
+-rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/log-93eb299558ddc7c9/lib-log.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/dep-lib-num-conv
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/lib-num-conv
+-rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-0ed052656ef43d3e/lib-num-conv.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-3d14c87ded27d719/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-3d14c87ded27d719/lib-num-conv
+-rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-3d14c87ded27d719/lib-num-conv.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/dep-lib-num-conv
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/lib-num-conv
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/num-conv-f19cfc73cc0280c4/lib-num-conv.json
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/dep-lib-powerfmt
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/lib-powerfmt
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-82d0abc0664de4d6/lib-powerfmt.json
+-rwxr-xr-x   0        0        0       48 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/invoked.timestamp
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/lib-powerfmt
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/powerfmt-f8a07c1db2a93596/lib-powerfmt.json
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 runhelper-0.2.3/target/debug/.fingerprint/runhelper-05d804ff06814ff8/dep-test-lib-runhelper
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 runhelper-0.2.3/.gitignore
+-rwxr-xr-x   0        0        0    35821 2020-02-02 00:00:00.000000 runhelper-0.2.3/LICENSE
+-rwxr-xr-x   0        0        0     2933 2020-02-02 00:00:00.000000 runhelper-0.2.3/README.md
+-rwxr-xr-x   0        0        0      610 2020-02-02 00:00:00.000000 runhelper-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    43802 2020-02-02 00:00:00.000000 runhelper-0.2.3/PKG-INFO
```

### Comparing `runhelper-0.2.2/Cargo.lock` & `runhelper-0.2.3/Cargo.lock`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/runhelper/log.py` & `runhelper-0.2.3/runhelper/log.py`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/runhelper/run.py` & `runhelper-0.2.3/runhelper/run.py`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/src/hashany.rs` & `runhelper-0.2.3/src/hashany.rs`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/src/log.rs` & `runhelper-0.2.3/src/log.rs`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/target/.rustc_info.json` & `runhelper-0.2.3/target/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/LICENSE` & `runhelper-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/README.md` & `runhelper-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `runhelper-0.2.2/pyproject.toml` & `runhelper-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 exclude = [
     "/venv",
     "/.idea"
 ]
 
 [project]
 name = "runhelper"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     { name = "Ricardo Brancas", email = "ricardo.brancas@tecnico.ulisboa.pt" },
 ]
 description = "A small library to help running and logging the behaviour of research tools"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `runhelper-0.2.2/PKG-INFO` & `runhelper-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: runhelper
-Version: 0.2.2
+Version: 0.2.3
 Summary: A small library to help running and logging the behaviour of research tools
 Project-URL: repository, https://github.com/RicardoBrancas/runhelper
 Author-email: Ricardo Brancas <ricardo.brancas@tecnico.ulisboa.pt>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

