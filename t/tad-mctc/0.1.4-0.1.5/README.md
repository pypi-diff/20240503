# Comparing `tmp/tad_mctc-0.1.4.tar.gz` & `tmp/tad_mctc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_mctc-0.1.4.tar", last modified: Mon Apr 22 07:21:00 2024, max compression
+gzip compressed data, was "tad_mctc-0.1.5.tar", last modified: Fri May  3 11:35:51 2024, max compression
```

## Comparing `tad_mctc-0.1.4.tar` & `tad_mctc-0.1.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    11358 2024-03-29 08:44:28.000000 tad_mctc-0.1.4/LICENSE
--rw-r--r--   0 marvin    (1000) marvin    (1000)    10999 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/PKG-INFO
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     8946 2024-04-20 21:35:38.000000 tad_mctc-0.1.4/README.md
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1648 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/pyproject.toml
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1597 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/setup.cfg
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      714 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/setup.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:20:59.994948 tad_mctc-0.1.4/src/
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:20:59.998948 tad_mctc-0.1.4/src/tad_mctc/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4375 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1590 2024-04-20 21:35:38.000000 tad_mctc-0.1.4/src/tad_mctc/_version.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/autograd/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      921 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1455 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/batched.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4489 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/compat.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4188 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/gradcheck.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2691 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/hessian.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2087 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/internals.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2578 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/nonfunctorch.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/batch/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      817 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/batch/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1911 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/batch/agnostic.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/batch/mask/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      923 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1291 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/atoms.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2861 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/jit.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2667 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/pairs.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2103 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/triples.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5722 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/pack.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5898 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/unpack.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.006948 tad_mctc-0.1.4/src/tad_mctc/convert/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      903 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3963 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/convert/numpy.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1692 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/pse.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3952 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/convert/pytorch.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2733 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/tensor.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.006948 tad_mctc-0.1.4/src/tad_mctc/data/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1041 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1890 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/en.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3320 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/getters.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2421 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/mass.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    69463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/molecules.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4440 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/pse.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4312 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/radii.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3607 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/zeff.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/exceptions/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      803 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1143 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/io.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      994 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/molecule.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      944 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/pytorch.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/io/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      750 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/__init__.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/io/checks/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      782 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     7839 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/molecule.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2281 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/shape.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/io/read/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1144 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/dotfiles.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     6759 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/frompath.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2834 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/orca.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3169 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/qcschema.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5446 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/reader.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2416 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/tblite.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5433 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/turbomole.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5472 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/xyz.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/io/write/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      770 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2240 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/turbomole.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2817 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/writer.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2446 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/xyz.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/math/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      746 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/math/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2305 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/math/einsum.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/molecule/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      838 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    13256 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/bond.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5706 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/container.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4014 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/geometry.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4546 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/property.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/ncoord/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2871 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5967 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/count.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     5623 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/d3.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3731 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/d4.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1593 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/defaults.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4385 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/eeq.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)        0 2024-01-10 18:46:05.000000 tad_mctc-0.1.4/src/tad_mctc/py.typed
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/storch/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1113 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/storch/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4532 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/storch/distance.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4289 2024-04-14 16:23:38.000000 tad_mctc-0.1.4/src/tad_mctc/storch/elemental.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)    30570 2024-04-17 05:57:02.000000 tad_mctc-0.1.4/src/tad_mctc/storch/linalg.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1343 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/storch/utils.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/tools/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      755 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/tools/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     6412 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/tools/caching.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3188 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/tools/memory.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc/typing/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      920 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/typing/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1107 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/typing/builtin.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     4777 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/typing/compat.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     8809 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/typing/pytorch.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc/units/
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      841 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/__init__.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2025 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/codata.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     3517 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/energy.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/length.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1682 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/mass.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      873 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/math.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2490 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/spectroscopy.py
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     1047 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/time.py
-drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc.egg-info/
--rw-r--r--   0 marvin    (1000) marvin    (1000)    10999 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/PKG-INFO
--rw-rw-r--   0 marvin    (1000) marvin    (1000)     2883 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/SOURCES.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)        1 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/dependency_links.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)      245 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/requires.txt
--rw-rw-r--   0 marvin    (1000) marvin    (1000)        9 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.203700 tad_mctc-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.207700 tad_mctc-0.1.5/src/tad_mctc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.211700 tad_mctc-0.1.5/src/tad_mctc/autograd/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/gradcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/autograd/nonfunctorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.211700 tad_mctc-0.1.5/src/tad_mctc/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/agnostic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.211700 tad_mctc-0.1.5/src/tad_mctc/batch/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/mask/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/mask/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/mask/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/mask/triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/batch/unpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.211700 tad_mctc-0.1.5/src/tad_mctc/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/convert/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/convert/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/convert/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/convert/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.215700 tad_mctc-0.1.5/src/tad_mctc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69463 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/radii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/data/zeff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.215700 tad_mctc-0.1.5/src/tad_mctc/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/exceptions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/exceptions/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/exceptions/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.215700 tad_mctc-0.1.5/src/tad_mctc/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.215700 tad_mctc-0.1.5/src/tad_mctc/io/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/checks/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/checks/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.215700 tad_mctc-0.1.5/src/tad_mctc/io/read/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/dotfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/frompath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/orca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/qcschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/tblite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/read/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/io/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/write/turbomole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/write/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/io/write/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/math/einsum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/molecule/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/molecule/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/molecule/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/molecule/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/molecule/property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/ncoord/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/d3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/d4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/ncoord/eeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/storch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/storch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/storch/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/storch/elemental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30570 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/storch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/storch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.219700 tad_mctc-0.1.5/src/tad_mctc/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/tools/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/tools/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/src/tad_mctc/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/typing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/typing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/typing/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/src/tad_mctc/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/codata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-03 11:35:48.000000 tad_mctc-0.1.5/src/tad_mctc/units/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:35:51.223700 tad_mctc-0.1.5/src/tad_mctc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-03 11:35:51.000000 tad_mctc-0.1.5/src/tad_mctc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-03 11:35:51.000000 tad_mctc-0.1.5/src/tad_mctc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:35:51.000000 tad_mctc-0.1.5/src/tad_mctc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 11:35:51.000000 tad_mctc-0.1.5/src/tad_mctc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 11:35:51.000000 tad_mctc-0.1.5/src/tad_mctc.egg-info/top_level.txt
```

### Comparing `tad_mctc-0.1.4/LICENSE` & `tad_mctc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/PKG-INFO` & `tad_mctc-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_mctc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Torch Autodiff Utility
 Home-page: https://github.com/tad-mctc/tad-mctc
 Author: "Marvin Friede"
 License: Apache-2.0
 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc
 Project-URL: Tracker, https://github.com/tad-mctc/tad-mctc/issues
@@ -66,24 +66,33 @@
     <td>
       <a href="https://github.com/tad-mctc/tad-mctc/releases/latest">
         <img src="https://img.shields.io/github/v/release/tad-mctc/tad-mctc?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-mctc/">
         <img src="https://img.shields.io/pypi/v/tad-mctc?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-mctc">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-mctc.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml">
-        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml">
         <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-mctc.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-mctc/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -95,25 +104,24 @@
       </a>
     </td>
   </tr>
 </table>
 
 <br>
 
-
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
-In particular, the *tad-mctc* library provides:
+In particular, the _tad-mctc_ library provides:
 
 - autograd functions (Jacobian, Hessian)
 
 - atomic data (radii, EN, example molecules, ...)
 
 - batch utility (packing, masks, ...)
 
-- conversion functions (numpy, atmoic symbols/numbers, ...)
+- conversion functions (numpy, atomic symbols/numbers, ...)
 
 - coordination numbers (DFT-D3, DFT-D4, EEQ)
 
 - io (reading/writing coordinate files)
 
 - molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
@@ -121,25 +129,31 @@
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
 The name is inspired by the Fortran pendant "modular computation tool chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)).
 
-
 ## Installation
 
 ### pip
 
-*tad-mctc* can easily be installed with ``pip``.
+_tad-mctc_ can easily be installed with `pip`.
 
 ```sh
 pip install tad-mctc
 ```
 
+### conda
+
+_tad-mctc_ is also available from `conda`.
+
+```sh
+conda install tad-mctc
+```
 
 ### From source
 
 This project is hosted on GitHub at [tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/).
 Obtain the source by cloning the repository with
 
 ```sh
@@ -152,15 +166,15 @@
 Install the required dependencies from the conda-forge channel.
 
 ```sh
 mamba env create -n torch -f environment.yaml
 mamba activate torch
 ```
 
-Install this project with ``pip`` in the environment
+Install this project with `pip` in the environment
 
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
@@ -175,15 +189,15 @@
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
 pip install pytest-random-order
 ```
 
-With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
+With pip, add the option `-e` for installing in development mode, and add `[dev]` for the development dependencies
 
 ```sh
 pip install -e .[dev]
 ```
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -193,15 +207,15 @@
 
 For testing all Python environments, simply run `tox`.
 
 ```sh
 tox
 ```
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
 
 ```sh
 tox -- test
 ```
 
 ## Examples
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.4 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.5 Summary: Torch Autodiff
 Utility Home-page: https://github.com/tad-mctc/tad-mctc Author: "Marvin Friede"
 License: Apache-2.0 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc Project-URL: Tracker,
 https://github.com/tad-mctc/tad-mctc/issues Keywords:
 pytorch,autograd,computational chemistry,quantum chemistry Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
@@ -23,53 +23,55 @@
 Dist: pytest-xdist; extra == "dev" Requires-Dist: scipy; extra == "dev"
 Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-Dist:
 covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox" Requires-
 Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order; extra ==
 "tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-Dist: scipy; extra
 == "tox" # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
-lab). In particular, the *tad-mctc* library provides: - autograd functions
+lab). In particular, the _tad-mctc_ library provides: - autograd functions
 (Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
-utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+utility (packing, masks, ...) - conversion functions (numpy, atomic symbols/
 numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
 writing coordinate files) - molecular properties (bond lengths/orders/angles,
 moment of inertia, ...) - safeops (autograd-safe implementations of common
 functions) - typing (base class for tensor-like behavior of arbitrary classes)
 - units The name is inspired by the Fortran pendant "modular computation tool
 chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
-Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
-install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
-cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+Installation ### pip _tad-mctc_ can easily be installed with `pip`. ```sh pip
+install tad-mctc ``` ### conda _tad-mctc_ is also available from `conda`. ```sh
+conda install tad-mctc ``` ### From source This project is hosted on GitHub at
+[tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source
+by cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
 mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
 ) environment to install the package. You can setup the environment manager
 using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
 Install the required dependencies from the conda-forge channel. ```sh mamba env
 create -n torch -f environment.yaml mamba activate torch ``` Install this
-project with ``pip`` in the environment ```sh pip install . ``` The following
+project with `pip` in the environment ```sh pip install . ``` The following
 dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
 optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
 psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
 only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
-tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
-installing in development mode, and add ``[dev]`` for the development
+tox pip install pytest-random-order ``` With pip, add the option `-e` for
+installing in development mode, and add `[dev]` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
 `tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
 "large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
+_posargs_. ```sh tox -- test ``` ## Examples The following example shows how to
 calculate the coordination number used in the EEQ model for a single structure.
 ```python import torch import tad_mctc as mctc numbers =
 mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
 coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
 0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
 0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
 [+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
```

### Comparing `tad_mctc-0.1.4/README.md` & `tad_mctc-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,33 @@
     <td>
       <a href="https://github.com/tad-mctc/tad-mctc/releases/latest">
         <img src="https://img.shields.io/github/v/release/tad-mctc/tad-mctc?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-mctc/">
         <img src="https://img.shields.io/pypi/v/tad-mctc?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-mctc">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-mctc.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml">
-        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml">
         <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-mctc.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-mctc/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -42,25 +51,24 @@
       </a>
     </td>
   </tr>
 </table>
 
 <br>
 
-
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
-In particular, the *tad-mctc* library provides:
+In particular, the _tad-mctc_ library provides:
 
 - autograd functions (Jacobian, Hessian)
 
 - atomic data (radii, EN, example molecules, ...)
 
 - batch utility (packing, masks, ...)
 
-- conversion functions (numpy, atmoic symbols/numbers, ...)
+- conversion functions (numpy, atomic symbols/numbers, ...)
 
 - coordination numbers (DFT-D3, DFT-D4, EEQ)
 
 - io (reading/writing coordinate files)
 
 - molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
@@ -68,25 +76,31 @@
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
 The name is inspired by the Fortran pendant "modular computation tool chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)).
 
-
 ## Installation
 
 ### pip
 
-*tad-mctc* can easily be installed with ``pip``.
+_tad-mctc_ can easily be installed with `pip`.
 
 ```sh
 pip install tad-mctc
 ```
 
+### conda
+
+_tad-mctc_ is also available from `conda`.
+
+```sh
+conda install tad-mctc
+```
 
 ### From source
 
 This project is hosted on GitHub at [tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/).
 Obtain the source by cloning the repository with
 
 ```sh
@@ -99,15 +113,15 @@
 Install the required dependencies from the conda-forge channel.
 
 ```sh
 mamba env create -n torch -f environment.yaml
 mamba activate torch
 ```
 
-Install this project with ``pip`` in the environment
+Install this project with `pip` in the environment
 
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
@@ -122,15 +136,15 @@
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
 pip install pytest-random-order
 ```
 
-With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
+With pip, add the option `-e` for installing in development mode, and add `[dev]` for the development dependencies
 
 ```sh
 pip install -e .[dev]
 ```
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -140,15 +154,15 @@
 
 For testing all Python environments, simply run `tox`.
 
 ```sh
 tox
 ```
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
 
 ```sh
 tox -- test
 ```
 
 ## Examples
```

#### html2text {}

```diff
@@ -1,48 +1,50 @@
 # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
-lab). In particular, the *tad-mctc* library provides: - autograd functions
+lab). In particular, the _tad-mctc_ library provides: - autograd functions
 (Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
-utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+utility (packing, masks, ...) - conversion functions (numpy, atomic symbols/
 numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
 writing coordinate files) - molecular properties (bond lengths/orders/angles,
 moment of inertia, ...) - safeops (autograd-safe implementations of common
 functions) - typing (base class for tensor-like behavior of arbitrary classes)
 - units The name is inspired by the Fortran pendant "modular computation tool
 chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
-Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
-install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
-cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+Installation ### pip _tad-mctc_ can easily be installed with `pip`. ```sh pip
+install tad-mctc ``` ### conda _tad-mctc_ is also available from `conda`. ```sh
+conda install tad-mctc ``` ### From source This project is hosted on GitHub at
+[tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source
+by cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
 mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
 ) environment to install the package. You can setup the environment manager
 using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
 Install the required dependencies from the conda-forge channel. ```sh mamba env
 create -n torch -f environment.yaml mamba activate torch ``` Install this
-project with ``pip`` in the environment ```sh pip install . ``` The following
+project with `pip` in the environment ```sh pip install . ``` The following
 dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
 optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
 psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
 only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
-tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
-installing in development mode, and add ``[dev]`` for the development
+tox pip install pytest-random-order ``` With pip, add the option `-e` for
+installing in development mode, and add `[dev]` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
 `tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
 "large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
+_posargs_. ```sh tox -- test ``` ## Examples The following example shows how to
 calculate the coordination number used in the EEQ model for a single structure.
 ```python import torch import tad_mctc as mctc numbers =
 mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
 coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
 0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
 0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
 [+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
```

### Comparing `tad_mctc-0.1.4/pyproject.toml` & `tad_mctc-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/setup.cfg` & `tad_mctc-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/setup.py` & `tad_mctc-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 - autograd functions (Jacobian, Hessian)
 
 - atomic data (radii, EN, example molecules, ...)
 
 - batch utility (packing, masks, ...)
 
-- conversion functions (numpy, atmoic symbols/numbers, ...)
+- conversion functions (numpy, atomic symbols/numbers, ...)
 
 - coordination numbers (DFT-D3, DFT-D4, EEQ)
 
 - io (reading/writing coordinate files)
 
 - molecular properties (bond lengths/orders/angles, moment of inertia, ...)
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/_version.py` & `tad_mctc-0.1.5/src/tad_mctc/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,9 +46,12 @@
             f"versioning scheme of MAJOR.MINOR.PATCH ({s})."
         )
 
     version_numbers = [int(part) for part in s[:3]]
     return tuple(version_numbers)
 
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
+"""Version of tad-mctc in semantic versioning."""
+
 __tversion__ = version_tuple(torch.__version__)
+"""Version of PyTorch reduced to semantic versioning."""
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/batched.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/batched.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/compat.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/gradcheck.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/gradcheck.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/hessian.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/hessian.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/internals.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/internals.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/autograd/nonfunctorch.py` & `tad_mctc-0.1.5/src/tad_mctc/autograd/nonfunctorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/agnostic.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/agnostic.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/mask/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/mask/atoms.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/mask/atoms.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/mask/jit.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/mask/jit.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/mask/pairs.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/mask/pairs.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/mask/triples.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/mask/triples.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/pack.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of dxtb, modified from tbmalt/tbmalt.
+# This file is part of tad-mctc, modified from tbmalt/tbmalt.
 #
 # SPDX-Identifier: Apache-2.0
 # Copyright (C) 2024 Grimme Group
 #
 # Original file licensed under the LGPL-3.0 License by tbmalt/tbmalt.
 # Modifications made by Grimme Group.
 #
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/batch/unpack.py` & `tad_mctc-0.1.5/src/tad_mctc/batch/unpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of dxtb, modified from tbmalt/tbmalt.
+# This file is part of tad-mctc, modified from tbmalt/tbmalt.
 #
 # SPDX-Identifier: Apache-2.0
 # Copyright (C) 2024 Grimme Group
 #
 # Original file licensed under the LGPL-3.0 License by tbmalt/tbmalt.
 # Modifications made by Grimme Group.
 #
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/convert/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/convert/numpy.py` & `tad_mctc-0.1.5/src/tad_mctc/convert/numpy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/convert/pse.py` & `tad_mctc-0.1.5/src/tad_mctc/convert/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/convert/pytorch.py` & `tad_mctc-0.1.5/src/tad_mctc/convert/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/convert/tensor.py` & `tad_mctc-0.1.5/src/tad_mctc/convert/tensor.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/en.py` & `tad_mctc-0.1.5/src/tad_mctc/data/en.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/getters.py` & `tad_mctc-0.1.5/src/tad_mctc/data/getters.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/mass.py` & `tad_mctc-0.1.5/src/tad_mctc/data/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/molecules.py` & `tad_mctc-0.1.5/src/tad_mctc/data/molecules.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/pse.py` & `tad_mctc-0.1.5/src/tad_mctc/data/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/radii.py` & `tad_mctc-0.1.5/src/tad_mctc/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/data/zeff.py` & `tad_mctc-0.1.5/src/tad_mctc/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/exceptions/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/exceptions/io.py` & `tad_mctc-0.1.5/src/tad_mctc/exceptions/io.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/exceptions/molecule.py` & `tad_mctc-0.1.5/src/tad_mctc/exceptions/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/exceptions/pytorch.py` & `tad_mctc-0.1.5/src/tad_mctc/exceptions/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/checks/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/io/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/checks/molecule.py` & `tad_mctc-0.1.5/src/tad_mctc/io/checks/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,45 +103,56 @@
     # Check if any distance below the threshold is found
     if torch.any((distances < threshold) & mask):
         raise MoleculeError("Too close interatomic distances found")
 
     return True
 
 
-def content_checks(numbers: Tensor, positions: Tensor) -> bool | NoReturn:
+def content_checks(
+    numbers: Tensor,
+    positions: Tensor,
+    max_element: int = pse.MAX_ELEMENT,
+    allow_batched: bool = True,
+) -> bool | NoReturn:
     """
     Check the content of the numbers and positions tensors.
 
     This function should be asserted as it returns `True` on success and raises
     an error on failure.
 
     Parameters
     ----------
     numbers : Tensor
-        A 1D tensor containing atomic numbers or symbols.
+        Atomic numbers for all atoms in the system of shape `(..., nat)`.
     positions : Tensor
-        A 2D tensor of shape (n_atoms, 3) containing atomic positions.
+        Cartesian coordinates of all atoms (shape: `(..., nat, 3)`).
+    max_element : int, optional
+        Maximum atomic number allowed. Defaults to `pse.MAX_ELEMENT`.
+    allow_batched : bool, optional
+        Allow batched tensors. Defaults to `True`.
 
     Returns
     -------
     bool
         True if content is correct.
 
     Raises
     ------
-    ValueError
+    MoleculeError
         Atomic number too large or too small.
     """
-    if numbers.max() > pse.MAX_ELEMENT:
-        raise MoleculeError(f"Atomic number larger than {pse.MAX_ELEMENT} found.")
-    if numbers.min() < 1:
-        raise MoleculeError(
-            "Atomic number smaller than 1 found. This may indicate residual "
-            "padding. Remove before writing to file."
-        )
+    if numbers.max() > max_element:
+        raise MoleculeError(f"Atomic number larger than {max_element} found.")
+
+    if allow_batched is False:
+        if numbers.min() < 1:
+            raise MoleculeError(
+                "Atomic number smaller than 1 found. This may indicate "
+                "residual padding. Remove before writing to file."
+            )
 
     assert coldfusion_check(numbers, positions)
 
     return True
 
 
 def deflatable_check(
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/checks/shape.py` & `tad_mctc-0.1.5/src/tad_mctc/io/checks/shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from __future__ import annotations
 
 from ...typing import Tensor
 
 __all__ = ["shape_checks"]
 
 
-def shape_checks(numbers: Tensor, positions: Tensor) -> bool:
+def shape_checks(
+    numbers: Tensor, positions: Tensor, allow_batched: bool = True
+) -> bool:
     """
     Check the shapes of the numbers and positions tensors. This explicitly
     checks for non-batched tensor shapes (batched tensors throw errors).
 
     Parameters
     ----------
     numbers : Tensor
@@ -61,11 +63,12 @@
     if positions.shape[-1] != 3:
         raise ValueError(
             "The last dimension of the position tensor must present the "
             "cartesian directions, i.e., it must be size 3 (but is "
             f"{positions.shape[-1]}"
         )
 
-    if len(numbers.shape) != 1 or len(positions.shape) != 2:
-        raise ValueError("Invalid shape for tensors (batched tensors not allowed).")
+    if allow_batched is False:
+        if len(numbers.shape) != 1 or len(positions.shape) != 2:
+            raise ValueError("Invalid shape for tensors (batched tensors not allowed).")
 
     return True
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/dotfiles.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/dotfiles.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/frompath.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/frompath.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/orca.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/orca.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/qcschema.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/qcschema.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     coords = []
     for i in range(0, len(geo), 3):
         coords.append([float(geo[i]), float(geo[i + 1]), float(geo[i + 2])])
 
     numbers = torch.tensor([pse.S2Z[s] for s in mol["symbols"]], **ddi)
     positions = torch.tensor(coords, **dd)
 
-    assert shape_checks(numbers, positions)
-    assert content_checks(numbers, positions)
+    assert shape_checks(numbers, positions, allow_batched=False)
+    assert content_checks(numbers, positions, allow_batched=False)
     assert deflatable_check(positions, fileobj, **kwargs)
 
     return numbers, positions
 
 
 read_qcschema_from_path = create_path_reader(read_qcschema)
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/reader.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/reader.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/tblite.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/tblite.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/turbomole.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/turbomole.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,16 @@
             symbols.append(symbol.title().replace("Q", "X"))
             coords.append([float(x), float(y), float(z)])
             i += 1
 
         numbers = torch.tensor([pse.S2Z[symbol] for symbol in symbols], **ddi)
         positions = torch.tensor(coords, **dd)
 
-        assert shape_checks(numbers, positions)
-        assert content_checks(numbers, positions)
+        assert shape_checks(numbers, positions, allow_batched=False)
+        assert content_checks(numbers, positions, allow_batched=False)
         assert deflatable_check(positions, fileobj, **kwargs)
 
     # Check if data was actually parsed
     if numbers is None or positions is None:
         raise EmptyFileError("No valid data found in the file.")
 
     return numbers, positions
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/read/xyz.py` & `tad_mctc-0.1.5/src/tad_mctc/io/read/xyz.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             symbol, x, y, z = line[:4]
             symbols.append(symbol.title())
             coords.append([float(x), float(y), float(z)])
 
         numbers = torch.tensor([pse.S2Z[symbol] for symbol in symbols], **ddi)
         positions = torch.tensor(coords, **dd) * length.AA2AU
 
-        assert shape_checks(numbers, positions)
-        assert content_checks(numbers, positions)
+        assert shape_checks(numbers, positions, allow_batched=False)
+        assert content_checks(numbers, positions, allow_batched=False)
         assert deflatable_check(positions, fileobj, **kwargs)
 
         numbers_images.append(numbers)
         positions_images.append(positions)
 
     # if only one image, return its tensors directly
     if len(numbers_images) == 1:
@@ -168,15 +168,15 @@
         line = fileobj.readline().split()
         symbols.append(line[0].title())
         coords.append([float(x.replace("*^", "e")) for x in line[1:4]])
 
     numbers = torch.tensor([pse.S2Z[symbol] for symbol in symbols], **ddi)
     positions = torch.tensor(coords, **dd) * length.AA2AU
 
-    assert shape_checks(numbers, positions)
-    assert content_checks(numbers, positions)
+    assert shape_checks(numbers, positions, allow_batched=False)
+    assert content_checks(numbers, positions, allow_batched=False)
     assert deflatable_check(positions, fileobj)
 
     return numbers, positions
 
 
 read_xyz_qm9_from_path = create_path_reader(read_xyz_qm9)
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/write/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/io/write/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/write/turbomole.py` & `tad_mctc-0.1.5/src/tad_mctc/io/write/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/io/write/writer.py` & `tad_mctc-0.1.5/src/tad_mctc/io/write/writer.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/math/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/math/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/math/einsum.py` & `tad_mctc-0.1.5/src/tad_mctc/math/einsum.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/molecule/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/molecule/bond.py` & `tad_mctc-0.1.5/src/tad_mctc/molecule/bond.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/molecule/container.py` & `tad_mctc-0.1.5/src/tad_mctc/molecule/container.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/molecule/geometry.py` & `tad_mctc-0.1.5/src/tad_mctc/molecule/geometry.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/molecule/property.py` & `tad_mctc-0.1.5/src/tad_mctc/molecule/property.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/count.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/count.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/d3.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/d3.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/d4.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/d4.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/defaults.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/ncoord/eeq.py` & `tad_mctc-0.1.5/src/tad_mctc/ncoord/eeq.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/storch/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/storch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/storch/distance.py` & `tad_mctc-0.1.5/src/tad_mctc/storch/distance.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/storch/elemental.py` & `tad_mctc-0.1.5/src/tad_mctc/storch/elemental.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/storch/linalg.py` & `tad_mctc-0.1.5/src/tad_mctc/storch/linalg.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/storch/utils.py` & `tad_mctc-0.1.5/src/tad_mctc/storch/utils.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/tools/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/tools/caching.py` & `tad_mctc-0.1.5/src/tad_mctc/tools/caching.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/tools/memory.py` & `tad_mctc-0.1.5/src/tad_mctc/tools/memory.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/typing/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/typing/builtin.py` & `tad_mctc-0.1.5/src/tad_mctc/typing/builtin.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/typing/compat.py` & `tad_mctc-0.1.5/src/tad_mctc/typing/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/typing/pytorch.py` & `tad_mctc-0.1.5/src/tad_mctc/typing/pytorch.py`

 * *Files 15% similar despite different names*

```diff
@@ -150,14 +150,33 @@
         Raises
         ------
         AttributeError
             Setter is called.
         """
         raise AttributeError("Move object to device using the `.to` method")
 
+    def override_device(self, device: torch.device) -> None:
+        """
+        Override the device of the class object.
+
+        .. warning::
+
+            This does not change the device of the underlying tensors. It only
+            changes the device of the class object. Use with caution.
+
+        Parameters
+        ----------
+        device : torch.device
+            Device to override the current device.
+
+        """
+        self.__device = device
+
+    ###########################################################################
+
     @property
     def dtype(self) -> torch.dtype:
         """Floating point dtype used by class object."""
         return self.__dtype
 
     @dtype.setter
     def dtype(self, *_: Any) -> NoReturn:
@@ -172,14 +191,32 @@
         Raises
         ------
         AttributeError
             Setter is called.
         """
         raise AttributeError("Change object to dtype using the `.type` method")
 
+    def override_dtype(self, dtype: torch.dtype) -> None:
+        """
+        Override the dtype of the class object.
+
+        .. warning::
+
+            This does not change the dtype of the underlying tensors. It only
+            changes the dtype of the class object. Use with caution.
+
+        Parameters
+        ----------
+        dtype : torch.dtype
+            Floating point dtype to override the current dtype.
+        """
+        self.__dtype = dtype
+
+    ###########################################################################
+
     @property
     def dd(self) -> DD:
         """Shortcut for device and dtype."""
         return {"device": self.device, "dtype": self.dtype}
 
     @dd.setter
     def dd(self, *_: Any) -> NoReturn:
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/__init__.py` & `tad_mctc-0.1.5/src/tad_mctc/units/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/codata.py` & `tad_mctc-0.1.5/src/tad_mctc/units/codata.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/energy.py` & `tad_mctc-0.1.5/src/tad_mctc/units/energy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/length.py` & `tad_mctc-0.1.5/src/tad_mctc/units/length.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/mass.py` & `tad_mctc-0.1.5/src/tad_mctc/units/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/math.py` & `tad_mctc-0.1.5/src/tad_mctc/units/math.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/spectroscopy.py` & `tad_mctc-0.1.5/src/tad_mctc/units/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc/units/time.py` & `tad_mctc-0.1.5/src/tad_mctc/units/time.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.4/src/tad_mctc.egg-info/PKG-INFO` & `tad_mctc-0.1.5/src/tad_mctc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_mctc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Torch Autodiff Utility
 Home-page: https://github.com/tad-mctc/tad-mctc
 Author: "Marvin Friede"
 License: Apache-2.0
 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc
 Project-URL: Tracker, https://github.com/tad-mctc/tad-mctc/issues
@@ -66,24 +66,33 @@
     <td>
       <a href="https://github.com/tad-mctc/tad-mctc/releases/latest">
         <img src="https://img.shields.io/github/v/release/tad-mctc/tad-mctc?color=orange" alt="Release"/>
       </a>
       <a href="https://pypi.org/project/tad-mctc/">
         <img src="https://img.shields.io/pypi/v/tad-mctc?color=orange" alt="PyPI"/>
       </a>
+      <a href="https://anaconda.org/conda-forge/tad-mctc">
+        <img src="https://img.shields.io/conda/vn/conda-forge/tad-mctc.svg" alt="Conda Version"/>
+      </a>
       <a href="http://www.apache.org/licenses/LICENSE-2.0">
         <img src="https://img.shields.io/badge/License-Apache%202.0-orange.svg" alt="Apache-2.0"/>
       </a>
     </td>
   </tr>
   <tr>
     <td>Status:</td>
     <td>
-      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml">
-        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/python.yaml/badge.svg" alt="Test Status"/>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/ubuntu.yaml/badge.svg" alt="Test Status Ubuntu"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/macos.yaml/badge.svg" alt="Test Status macOS"/>
+      </a>
+      <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml">
+        <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/windows.yaml/badge.svg" alt="Test Status Windows"/>
       </a>
       <a href="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml">
         <img src="https://github.com/tad-mctc/tad-mctc/actions/workflows/release.yaml/badge.svg" alt="Build Status"/>
       </a>
       <a href="https://tad-mctc.readthedocs.io">
         <img src="https://readthedocs.org/projects/tad-mctc/badge/?version=latest" alt="Documentation Status"/>
       </a>
@@ -95,25 +104,24 @@
       </a>
     </td>
   </tr>
 </table>
 
 <br>
 
-
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
-In particular, the *tad-mctc* library provides:
+In particular, the _tad-mctc_ library provides:
 
 - autograd functions (Jacobian, Hessian)
 
 - atomic data (radii, EN, example molecules, ...)
 
 - batch utility (packing, masks, ...)
 
-- conversion functions (numpy, atmoic symbols/numbers, ...)
+- conversion functions (numpy, atomic symbols/numbers, ...)
 
 - coordination numbers (DFT-D3, DFT-D4, EEQ)
 
 - io (reading/writing coordinate files)
 
 - molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
@@ -121,25 +129,31 @@
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
 The name is inspired by the Fortran pendant "modular computation tool chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)).
 
-
 ## Installation
 
 ### pip
 
-*tad-mctc* can easily be installed with ``pip``.
+_tad-mctc_ can easily be installed with `pip`.
 
 ```sh
 pip install tad-mctc
 ```
 
+### conda
+
+_tad-mctc_ is also available from `conda`.
+
+```sh
+conda install tad-mctc
+```
 
 ### From source
 
 This project is hosted on GitHub at [tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/).
 Obtain the source by cloning the repository with
 
 ```sh
@@ -152,15 +166,15 @@
 Install the required dependencies from the conda-forge channel.
 
 ```sh
 mamba env create -n torch -f environment.yaml
 mamba activate torch
 ```
 
-Install this project with ``pip`` in the environment
+Install this project with `pip` in the environment
 
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
@@ -175,15 +189,15 @@
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
 pip install pytest-random-order
 ```
 
-With pip, add the option ``-e`` for installing in development mode, and add ``[dev]`` for the development dependencies
+With pip, add the option `-e` for installing in development mode, and add `[dev]` for the development dependencies
 
 ```sh
 pip install -e .[dev]
 ```
 
 The pre-commit hooks are initialized by running the following command in the root of the repository.
 
@@ -193,15 +207,15 @@
 
 For testing all Python environments, simply run `tox`.
 
 ```sh
 tox
 ```
 
-Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional *posargs*.
+Note that this randomizes the order of tests but skips "large" tests. To modify this behavior, `tox` has to skip the optional _posargs_.
 
 ```sh
 tox -- test
 ```
 
 ## Examples
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.4 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.5 Summary: Torch Autodiff
 Utility Home-page: https://github.com/tad-mctc/tad-mctc Author: "Marvin Friede"
 License: Apache-2.0 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc Project-URL: Tracker,
 https://github.com/tad-mctc/tad-mctc/issues Keywords:
 pytorch,autograd,computational chemistry,quantum chemistry Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
@@ -23,53 +23,55 @@
 Dist: pytest-xdist; extra == "dev" Requires-Dist: scipy; extra == "dev"
 Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-Dist:
 covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox" Requires-
 Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order; extra ==
 "tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-Dist: scipy; extra
 == "tox" # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
-Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
-Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
-               _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
+Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_A_p_a_c_h_e_-_2_._0_]
+               _[_T_e_s_t_ _S_t_a_t_u_s_ _U_b_u_n_t_u_]_[_T_e_s_t_ _S_t_a_t_u_s_ _m_a_c_O_S_]_[_T_e_s_t_ _S_t_a_t_u_s_ _W_i_n_d_o_w_s_]
+Status:        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _S_t_a_t_u_s_]
+               _[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
-lab). In particular, the *tad-mctc* library provides: - autograd functions
+lab). In particular, the _tad-mctc_ library provides: - autograd functions
 (Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
-utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+utility (packing, masks, ...) - conversion functions (numpy, atomic symbols/
 numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
 writing coordinate files) - molecular properties (bond lengths/orders/angles,
 moment of inertia, ...) - safeops (autograd-safe implementations of common
 functions) - typing (base class for tensor-like behavior of arbitrary classes)
 - units The name is inspired by the Fortran pendant "modular computation tool
 chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
-Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
-install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
-cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+Installation ### pip _tad-mctc_ can easily be installed with `pip`. ```sh pip
+install tad-mctc ``` ### conda _tad-mctc_ is also available from `conda`. ```sh
+conda install tad-mctc ``` ### From source This project is hosted on GitHub at
+[tad-mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source
+by cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
 mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
 ) environment to install the package. You can setup the environment manager
 using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
 Install the required dependencies from the conda-forge channel. ```sh mamba env
 create -n torch -f environment.yaml mamba activate torch ``` Install this
-project with ``pip`` in the environment ```sh pip install . ``` The following
+project with `pip` in the environment ```sh pip install . ``` The following
 dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
 optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
 psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
 only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
-tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
-installing in development mode, and add ``[dev]`` for the development
+tox pip install pytest-random-order ``` With pip, add the option `-e` for
+installing in development mode, and add `[dev]` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
 `tox`. ```sh tox ``` Note that this randomizes the order of tests but skips
 "large" tests. To modify this behavior, `tox` has to skip the optional
-*posargs*. ```sh tox -- test ``` ## Examples The following example shows how to
+_posargs_. ```sh tox -- test ``` ## Examples The following example shows how to
 calculate the coordination number used in the EEQ model for a single structure.
 ```python import torch import tad_mctc as mctc numbers =
 mctc.convert.symbol_to_number(symbols="C C C C N C S H H H H H".split()) #
 coordinates in Bohr positions = torch.tensor( [ [-2.56745685564671, -
 0.02509985979910, 0.00000000000000], [-1.39177582455797, +2.27696188880014,
 0.00000000000000], [+1.27784995624894, +2.45107479759386, 0.00000000000000],
 [+2.62801937615793, +0.25927727028120, 0.00000000000000], [+1.41097033661123, -
```

### Comparing `tad_mctc-0.1.4/src/tad_mctc.egg-info/SOURCES.txt` & `tad_mctc-0.1.5/src/tad_mctc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

