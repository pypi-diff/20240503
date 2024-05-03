# Comparing `tmp/malevich-0.2.6.tar.gz` & `tmp/malevich-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malevich-0.2.6.tar", last modified: Wed Mar 20 19:04:27 2024, max compression
+gzip compressed data, was "malevich-0.4.0.tar", last modified: Fri May  3 18:33:58 2024, max compression
```

## Comparing `malevich-0.2.6.tar` & `malevich-0.4.0.tar`

### file list

```diff
@@ -1,200 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.217194 malevich-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.181194 malevich-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.189194 malevich-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-20 19:04:18.000000 malevich-0.2.6/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-20 19:04:18.000000 malevich-0.2.6/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-20 19:04:18.000000 malevich-0.2.6/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-20 19:04:18.000000 malevich-0.2.6/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-20 19:04:18.000000 malevich-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 19:04:18.000000 malevich-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 19:04:18.000000 malevich-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-20 19:04:27.217194 malevich-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-20 19:04:18.000000 malevich-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 19:04:25.000000 malevich-0.2.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.189194 malevich-0.2.6/malevich/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.193194 malevich-0.2.6/malevich/_autoflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_autoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_autoflow/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_autoflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_autoflow/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_autoflow/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.193194 malevich-0.2.6/malevich/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_cli/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/core/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_cli/dev/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/dev/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_cli/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/misc/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/misc/manifest_to_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/prefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_cli/space/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/space/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/space/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_cli/use.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_core/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_core/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.197194 malevich-0.2.6/malevich/_db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_db/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.201194 malevich-0.2.6/malevich/_meta/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/decor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_meta/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.201194 malevich-0.2.6/malevich/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_templates/Dockerfile.app
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_templates/README.app.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_templates/flow.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_templates/processor.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_templates/space.yaml.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.201194 malevich-0.2.6/malevich/_utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.201194 malevich-0.2.6/malevich/_utility/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/cache/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/_utility/ci/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/_utility/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/templates/malevich-ci-manual.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/ci/templates/malevich-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/_utility/git/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/letterhash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/_utility/space/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/space/get_core_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/space/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/_utility/summary/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/summary/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/summary/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/_utility/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/install/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/install/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/install/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/install/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.205194 malevich-0.2.6/malevich/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/interpreter/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/interpreter/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/interpreter/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.209194 malevich-0.2.6/malevich/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/flow_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/in_app_core_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/injections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.209194 malevich-0.2.6/malevich/models/installers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/installers/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/installers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/installers/space.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/nodes/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/registry/core_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/results/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/results/core/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/core/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/results/space/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/results/space/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/state/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/state/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/state/space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/task/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/models/task/interpreted/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/interpreted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23035 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/interpreted/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/interpreted/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task/promised.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/models/verdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.213194 malevich-0.2.6/malevich/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/runners/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.217194 malevich-0.2.6/malevich/square/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/square/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/square/df.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/square/jls.py
--rw-r--r--   0 runner    (1001) docker     (127)    42193 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/square/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.217194 malevich-0.2.6/malevich/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/testing/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-03-20 19:04:18.000000 malevich-0.2.6/malevich/testing/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:27.217194 malevich-0.2.6/malevich.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 19:04:27.000000 malevich-0.2.6/malevich.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 19:04:18.000000 malevich-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-20 19:04:18.000000 malevich-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:04:27.217194 malevich-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-20 19:04:18.000000 malevich-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.812160 malevich-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.820160 malevich-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 18:33:49.000000 malevich-0.4.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 18:33:49.000000 malevich-0.4.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-03 18:33:49.000000 malevich-0.4.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-03 18:33:49.000000 malevich-0.4.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 18:33:49.000000 malevich-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 18:33:49.000000 malevich-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 18:33:49.000000 malevich-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-03 18:33:58.848160 malevich-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-03 18:33:49.000000 malevich-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 18:33:56.000000 malevich-0.4.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.824160 malevich-0.4.0/malevich/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.824160 malevich-0.4.0/malevich/_autoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_autoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_autoflow/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_autoflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_autoflow/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_autoflow/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_cli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/core/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/core/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/core/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_cli/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/dev/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_cli/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/misc/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/misc/manifest_to_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/prefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_cli/space/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/space/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/space/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/space/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_cli/use.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_core/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.828160 malevich-0.4.0/malevich/_db/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/functions/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/functions/get_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.832160 malevich-0.4.0/malevich/_db/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/schema/core_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_db/schema/creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.832160 malevich-0.4.0/malevich/_export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_export/space_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.832160 malevich-0.4.0/malevich/_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_meta/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.832160 malevich-0.4.0/malevich/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_templates/Dockerfile.app
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_templates/README.app.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_templates/flow.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_templates/processor.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_templates/space.yaml.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/_try.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/cache/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/templates/malevich-ci-manual.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/ci/templates/malevich-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/space/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/space/get_core_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.836160 malevich-0.4.0/malevich/_utility/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/summary/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/summary/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/_utility/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.840160 malevich-0.4.0/malevich/install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/install/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.840160 malevich-0.4.0/malevich/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/interpreter/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/interpreter/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/interpreter/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.840160 malevich-0.4.0/malevich/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/flow_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/in_app_core_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/injections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/installers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/installers/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/installers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/installers/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/nodes/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/registry/core_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/results/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/core/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/results/space/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/results/space/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/state/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/state/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/state/space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.844160 malevich-0.4.0/malevich/models/task/interpreted/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/interpreted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23766 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/interpreted/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/interpreted/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task/promised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/models/verdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/malevich/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/runners/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/malevich/square/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/square/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/square/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/square/jls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42188 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/square/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/malevich/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/malevich/testing/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/malevich/testing/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:58.848160 malevich-0.4.0/malevich.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 18:33:58.000000 malevich-0.4.0/malevich.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:33:49.000000 malevich-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 18:33:49.000000 malevich-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:33:58.848160 malevich-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 18:33:49.000000 malevich-0.4.0/setup.py
```

### Comparing `malevich-0.2.6/.github/workflows/docs.yaml` & `malevich-0.4.0/.github/workflows/docs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -18,14 +18,17 @@
           python-version: '3.11'
       - name: Install dependencies
         run: |
           pip install -r requirements.dev.txt
       - name: Sphinx build
         run: |
           sphinx-build docs build-docs
+      - name: Add CNAME
+        run: |
+          echo "docs.malevich.ai" > build-docs/CNAME
       - name: Deploy to GitHub Pages
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/docs' }}
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.DOCS_GITHUB_TOKEN }}
           publish_dir: build-docs
```

### Comparing `malevich-0.2.6/.github/workflows/pypi.yaml` & `malevich-0.4.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/.github/workflows/pytest.yaml` & `malevich-0.4.0/.github/workflows/pytest.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -43,17 +43,24 @@
     - name: Install Python
       uses: actions/setup-python@v4
       with:
          python-version: '3.11'
 
     - name: Install Malevich
       run: |
-        pip install ./malevich
         pip install -r ./malevich/requirements.dev.txt
-        malevich space login --username=${{secrets.TESTS_SPACE_USER}} --password=${{secrets.TESTS_SPACE_PASSWORD}} --api-url=${{secrets.API_URL}}
+        pip install ./malevich
+        malevich init
+        malevich space login --username=${{secrets.TESTS_SPACE_USER}} --password=${{secrets.TESTS_SPACE_PASSWORD}} --api-url=${{secrets.TESTS_API_URL}} --no-input
+        mkdir -p ~/.malevich/testing
+        cp malevich.yaml ~/.malevich/testing
+        cp malevich.secrets.yaml ~/.malevich/testing
 
     - name: Testing
-      run: cd ./malevich && pytest -s ./tests/
+      run: |
+        cp -rf ./malevich/tests ./tests && rm -rf ./malevich
+        pytest -s ./tests/
       env:
         TESTS_SPACE_PASSWORD: ${{ secrets.TESTS_SPACE_PASSWORD }}
         TESTS_SPACE_USER: ${{ secrets.TESTS_SPACE_USER }}
         TEST_GHCR_PACKAGE_PASSWORD: ${{ secrets.TEST_GHCR_PACKAGE_PASSWORD }}
+        MALEVICH_TEST_DIR: ${{ secrets.MALEVICH_TEST_DIR }}
```

### Comparing `malevich-0.2.6/LICENSE` & `malevich-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/PKG-INFO` & `malevich-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: malevich
-Version: 0.2.6
+Version: 0.4.0
 Summary: ('A user-friendly interface to communicate with Malevich AI (malevich.ai)',)
 License-File: LICENSE
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: pydantic>=2.0.0
-Requires-Dist: malevich-coretools>=0.3.8
-Requires-Dist: malevich-space>=0.4.10
+Requires-Dist: malevich-coretools>=0.3.11
+Requires-Dist: malevich-space>=0.4.24
 Requires-Dist: pandas
 Requires-Dist: pydantic-yaml
 Requires-Dist: PyGithub
 Requires-Dist: GitPython
 Requires-Dist: randomname
 Requires-Dist: botocore
 Requires-Dist: boto3
@@ -19,7 +19,9 @@
 Requires-Dist: jsonpickle
 Requires-Dist: python-dotenv
 Requires-Dist: kafka-python
 Requires-Dist: deprecated
 Requires-Dist: datamodel-code-generator
 Requires-Dist: ruff
 Requires-Dist: duckdb
+Requires-Dist: duckdb-engine
+Requires-Dist: humanfriendly
```

### Comparing `malevich-0.2.6/README.md` & `malevich-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/__init__.py` & `malevich-0.4.0/malevich/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,12 +33,15 @@
 from .interpreter.core import CoreInterpreter
 from .interpreter.space import SpaceInterpreter
 
 # Malevich Core
 import malevich_coretools as core_api
 from malevich_space.schema import VersionMode
 
+# For simple deployment
+from ._deploy import Core, Space
+
 manf = ManifestManager()
 
 __logger = logging.getLogger("log")
 __logger.setLevel(logging.CRITICAL)
 core.set_logger(__logger)
```

### Comparing `malevich-0.2.6/malevich/_autoflow/flow.py` & `malevich-0.4.0/malevich/_autoflow/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_autoflow/function.py` & `malevich-0.4.0/malevich/_autoflow/function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import functools
+import inspect
 import warnings
+from itertools import islice
 from typing import Callable, ParamSpec, TypeVar
 
 from ..models.argument import ArgumentLink
 from . import tracer as gn
 
 C = ParamSpec("C")
 R = TypeVar("R")
@@ -22,62 +24,65 @@
     The link produced is :class:`ArgumentLink <malevich.models.argument.ArgumentLink`
     with ``index`` set to the argument position and ``name`` set to the argument name.
     If the argument is passed as a keyword argument,
     and the function accepts the argument as
     **kwargs, raises a warning and does not link the argument.
     """
     @functools.wraps(func)
-    def wrapper(*args, **kwargs):  # noqa: ANN202
+    def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
         result = gn.traced(result) if not isinstance(
-            result, gn.traced) else result
-
-        varnames = func.__code__.co_varnames
-        for i, arg in enumerate(args):
-            argument_name = varnames[min(i, len(varnames) - 1)]
+            result, gn.traced
+        ) else result
+        parameters = list(inspect.signature(func).parameters.values())
+        varnames = [
+            p.name for p in parameters
+            if p.kind == inspect.Parameter.POSITIONAL_ONLY
+
+        ]
+        for i, arg in enumerate(islice(args, 0, len(varnames))):
+            argument_name = varnames[i]
             if isinstance(arg, gn.traced):
                 arg._autoflow.calledby(
                     result,
                     ArgumentLink(index=i, name=argument_name)
                 )
-        for key in kwargs:
-            if isinstance(kwargs[key], gn.traced):
-                if key in varnames:
-                    kwargs[key]._autoflow.calledby(
-                        result, ArgumentLink(index=varnames.index(key), name=key)
-                    )
-                else:
-                    warnings.warn(
-                        "Passing a keyword argument to a traced function that is not"
-                        " a formal argument of the function is not supported."
-                    )
+
 
         return result
     return wrapper
 
 
 def sinktrace(func: Callable[C, R]) -> Callable[C, R]:
     """A special form of autotrace to trace functions with *args
 
     This decorator is applied to processors that contains
     """
     @functools.wraps(func)
-    def wrapper(*args, **kwargs):  # noqa: ANN202
-        from ..models.nodes.collection import CollectionNode
-        for arg in args:
-            if isinstance(arg, CollectionNode):
-                # NOTE: That should be addressed
-                raise ValueError(
-                    "App with unrestricted number of arguments cannot be "
-                    "run with collections")
+    def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
         result = gn.traced(result) if not isinstance(result, gn.traced) else result
+        parameters = list(inspect.signature(func).parameters.values())
+        names = [
+            p.name for p in parameters
+            if p.kind in (
+                inspect.Parameter.VAR_POSITIONAL,
+                inspect.Parameter.POSITIONAL_ONLY
+            )
+        ]
+
         for i, arg in enumerate(args):
+            real_index = min(i, len(names) - 1)
+            argument_name = names[real_index]
             if isinstance(arg, gn.traced):
-                arg._autoflow.calledby(result, ArgumentLink(index=i, name=''))
+                arg._autoflow.calledby(result, ArgumentLink(
+                        index=real_index,
+                        name=argument_name
+                    )
+                )
             else:
                 warnings.warn(
                     "Ignoring non-traced argument in sinktrace function"
                     f" (argument index= {i})"
                 )
         return result
```

### Comparing `malevich-0.2.6/malevich/_autoflow/tracer.py` & `malevich-0.4.0/malevich/_autoflow/tracer.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_autoflow/tree.py` & `malevich-0.4.0/malevich/_autoflow/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import deque
+from collections import defaultdict, deque
 from typing import Any, Generic, Iterable, Iterator, Optional, TypeVar
 
 T = TypeVar("T")
 LinkType = TypeVar("LinkType", bound=Any)
 
 
 class BadEdgeError(Exception):
@@ -81,40 +81,42 @@
         ]
 
         self.nodes_ = set([
             x for x in self.nodes_
             if x not in outer_nodes
         ])
 
+    def roots(self) -> Iterable[tuple[int, T]]:
+        return [
+            (i, x) for i, x in enumerate(self.tree)
+            if not any(y[1] == x[0] for y in self.tree)
+        ]
+
     def edges_from(self, node: T) -> None:
         """Returns all edges starting from the specified node"""
         return [n for n in self.tree if n[0] == node]
 
     def traverse(self) -> Iterator[tuple[T, T, LinkType]]:
         """Traverse the execution tree
 
         The traversal is performed in a multi-source
         breadth-first manner.
 
         Returns:
             Generator[T]: Generator of nodes
         """
-        graph = self.tree
 
         # Mark visited nodes
-        visited = [False] * len(graph)
+        visited = [False] * len(self.tree)
 
         # Find roots
-        roots = [
-            (i, x) for i, x in enumerate(graph)
-            if not any(y[1] == x[0] for y in graph)
-        ]
+        roots = self.roots()
 
         # Traverse
-        q = deque(maxlen=len(graph))
+        q = deque(maxlen=len(self.tree))
         for i, r in roots:
             # BFS
             q.append((i, r,))
 
         while q:
             j, edge = q.popleft()
 
@@ -123,18 +125,42 @@
 
             yield edge
             visited[j] = True
 
             q.extend(
                 filter(
                     lambda x: x[1][0] == edge[1] and not visited[x[0]],
-                    enumerate(graph)
+                    enumerate(self.tree)
                 )
             )
 
+    def topsort(self) -> Iterator[tuple[T, T, LinkType]]:
+        sort_ = []
+        s = [r[0] for _, r in self.roots()]
+        edges = list(enumerate(self.tree))
+        mask = [False] * len(edges)
+        while s:
+            n = s.pop()
+            if n not in sort_:
+                sort_.append(n)
+            for i, (_, to, _) in filter(
+                lambda x: x[1][0] == n and not mask[x[0]], edges
+            ):
+                mask[i] = True
+                in_ = list(filter(lambda x: x[1][1] == to and not mask[x[0]], edges))
+                add = True
+                for j, (m, _, _) in in_:
+                    if m != n and not mask[j]:
+                        add = False
+                if add:
+                    s = [to, *s]
+
+        return sort_
+
+
     def leaves(self) -> Iterable[T]:
         """Returns all leaves of the execution tree"""
         return (
             x[1] for x in self.traverse()
             if not any(y[0] == x[1] for y in self.tree)
         )
```

### Comparing `malevich-0.2.6/malevich/_cli/ci.py` & `malevich-0.4.0/malevich/_cli/ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..constants import IMAGE_BASE
 from ..constants import SPACE_API_URL as DEFAULT_SPACE_HOST
 
 github = typer.Typer()
 
 
 @github.command(help="Initialize the Github CI/CD pipeline")
-def init(  # noqa: ANN201
+def init(
     interactive: bool = typer.Option(
         False,
         help="Run the initialization wizard",
         show_default=False,
     ),
     repo_name: str = typer.Option(
         None,
```

### Comparing `malevich-0.2.6/malevich/_cli/core/endpoints.py` & `malevich-0.4.0/malevich/_cli/core/endpoints.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/dev/dev.py` & `malevich-0.4.0/malevich/_cli/dev/dev.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import ast
 import json
 import os
 import re
+import shutil
+import site
 import sys
 from pathlib import Path
 from subprocess import CalledProcessError, call
 from typing import Union
 
+import rich
 import typer
 from datamodel_code_generator import InputFileType, generate
 from typing_extensions import Annotated
 
 dev = typer.Typer(help="Document operations")
 
 SECTIONS = ["heading", "input", "output", "config", "example"]
 
 
-def error_exit(msg: str = ""):  # noqa: ANN201
-    print(msg, file=sys.stderr)
+def error_exit(msg: str = "") -> None:
+    rich.print(f"[bold red]{msg}[/bold red]", file=sys.stderr)
     exit(1)
 
 
 TYPES = {
     "str": "string",
     "int": "integer",
     "float": "number",
@@ -111,29 +114,29 @@
                 "description": column[4],
             }
         )
     return result
 
 
 @dev.command("list-procs", help="List all processors and paths to their files")
-def list_procs(  # noqa: ANN201
+def list_procs(
     path=typer.Argument(
         ".", help="Directory to extract processors from", show_default=False
     ),
     out: Annotated[
         Union[str, None],
         typer.Option("--out", help="File to save results in", show_default=False),
     ] = None,
     verbose: Annotated[
         bool,
         typer.Option(
             "--verbose", "-v", help="If enabled, will print result JSON to stdout"
         ),
     ] = False,
-):
+) -> str:
     data = []
 
     for root, _, files in os.walk(path):
         for file in files:
             # Parsing python files
             if file.endswith(".py"):
                 with open(os.path.join(root, file)) as f:
@@ -159,20 +162,20 @@
                                     }
                                 )
 
     if out is not None:
         with open(out, "w") as f:
             f.write(json.dumps(data))
     if verbose:
-        print(json.dumps(data))
+        rich.print(json.dumps(data))
     return json.dumps(data)
 
 
 @dev.command("get-doc", help="Get process docstring")
-def get_processor_docstring(  # noqa: ANN201
+def get_processor_docstring(
     name=typer.Argument(
         ...,
         help="Processor name",
     ),
     path=typer.Argument(
         ...,
         help="Path to the file",
@@ -183,41 +186,41 @@
     ] = None,
     verbose: Annotated[
         bool,
         typer.Option(
             "--verbose", "-v", help="If enabled, will print result docstring to stdout"
         ),
     ] = False,
-):
+) -> str:
     if not os.path.exists(path):
         error_exit(f"Can not open {path}. No such file exists")
 
     with open(path) as f:
         tree = ast.parse(f.read())
         for node in ast.walk(tree):
             if (
                 isinstance(node, ast.FunctionDef)
                 or isinstance(node, ast.AsyncFunctionDef)
             ) and node.name == name:
                 doc = ast.get_docstring(node)
                 if out is not None:
                     open(out, "w").write(doc)
                 if verbose:
-                    print(doc)
+                    rich.print(doc)
                 return doc
 
-    print(
+    rich.print(
         "Could not find processor inside a file. "
         "Make sure you have provided correct arguments"
     )
     exit(1)
 
 
 @dev.command("parse-doc", help="Parse processor docstring")
-def parse_docstring(  # noqa: ANN201
+def parse_docstring(
     doc=typer.Argument(..., help="docstring"),
     file: Annotated[
         bool,
         typer.Option("--file", "-f", help="If enabled, will read from argument string"),
     ] = False,
     out: Annotated[
         Union[str, None],
@@ -225,15 +228,15 @@
     ] = None,
     verbose: Annotated[
         bool,
         typer.Option(
             "--verbose", "-v", help="If enabled, will print result JSON to stdout"
         ),
     ] = False,
-):
+) -> str:
     idx = 0
     if file:
         doc = open(doc).read()
 
     doc = doc.replace("\n", "\\n ")
     try:
         user = re.search(r"(?P<USER>[\S\s]+)-----(?P<DEV>[\S\s]*)", doc).group("USER")
@@ -284,64 +287,63 @@
             result["example"] = example
     except Exception:
         error_exit(f"Docstring doesn't suit the rules in {SECTIONS[idx]} section")
 
     if out:
         open(out, "w").write(json.dumps(result))
     if verbose:
-        print(json.dumps(result))
+        rich.print(json.dumps(result))
     return json.dumps(result)
 
 
 @dev.command("install-lib-hook", help="Configure git hooks path")
-def intstall_hook(  # noqa: ANN201
+def intstall_hook(
     path=typer.Option(
         ".githooks/",
         help="Folder with hooks",
         show_default=False,
     ),
-):
+) -> None:
     if not os.path.exists(path):
         error_exit(
             f"Cannot find {path}. "
             "Make sure you've provided a valid path, and run from the right directory",
         )
 
     try:
         call(["git", "config", "core.hooksPath", path])
     except CalledProcessError:
         error_exit("Failed to execute the process")
 
 
 @dev.command("make-configs", help="Create Context configurations for processors")
-def make_config(  # noqa: ANN201
+def make_config(
     path=typer.Argument(..., help="Path to start directory"),
     verbose: Annotated[
         bool,
         typer.Option(
             "--verbose", "-v", help="If enabled, will print result JSON to stdout"
         ),
     ] = False,
-):
+) -> None:
     data = json.loads(list_procs(path))
     by_path = {}
     for d in data:
         names: list = by_path.get(d["path"], [])
         names.append(d["name"])
         by_path[d["path"]] = names
 
     for path_ in by_path.keys():
         modules = []
         models_path = None
-        print(f"Processing {path_}...")
+        rich.print(f"Processing {path_}...")
         for name_ in by_path[path_]:
             doc = get_processor_docstring(name_, path_)
             schema = json.loads(parse_docstring(doc))
-            if "configuration" in schema.keys() and len(schema['configuration']) > 0:
-                print(schema['configuration'])
+            if "configuration" in schema.keys() and len(schema["configuration"]) > 0:
                 schema_path = os.path.join(
                     os.path.dirname(path_), "models", f"{name_}_model.json"
                 )
                 schema_model = os.path.join(
                     os.path.dirname(path_), "models", f"{name_}_model.py"
                 )
                 models_path = os.path.dirname(schema_model)
@@ -369,18 +371,19 @@
                     f.write(schema)
 
                 generate(
                     Path(schema_path),
                     output=Path(schema_model),
                     class_name=name_,
                     input_file_type=InputFileType.JsonSchema,
+                    disable_timestamp=True
                 )
                 model = open(schema_model).read()
                 model = re.sub(
-                    r"^class", "scheme()\nclass", model, flags=re.MULTILINE
+                    r"^class", "@scheme()\nclass", model, flags=re.MULTILINE
                 ).replace(
                     "from __future__ import annotations",
                     "from __future__ import annotations\n"
                     "from malevich.square import scheme",
                 )
 
                 with open(schema_model, "w") as f:
@@ -405,23 +408,26 @@
                 search_import = re.search(
                     rf"^from .{module['module']} import {module['classname']}",
                     file,
                     flags=re.MULTILINE,
                 )
                 if search_import is None:
                     if verbose:
-                        print(f"Added {module['classname']} to __init__.py")
+                        rich.print(f"Added {module['classname']} to __init__.py")
                     file += f"from .{module['module']} import {module['classname']}\n"
-                if re.search(
-                    rf"^from .models import {module['classname']}$",
-                    procs,
-                    flags=re.MULTILINE
-                ) is None:
+                if (
+                    re.search(
+                        rf"^from .models import {module['classname']}$",
+                        procs,
+                        flags=re.MULTILINE,
+                    )
+                    is None
+                ):
                     if verbose:
-                        print(f"Added{module['classname']} to {path_}")
+                        rich.print(f"Added{module['classname']} to {path_}")
                     procs = f"from .models import {module['classname']}\n" + procs
 
                 search_proc = re.search(
                     rf"(?P<DEF>^(async )?def {module['name']}"
                     r"\([\s\S]*? Context)(\[\w+\])?",
                     procs,
                     flags=re.MULTILINE,
@@ -430,13 +436,66 @@
                     "Context", f"Context[{module['classname']}]"
                 )
                 procs = re.sub(
                     rf"(?P<DEF>^(async )?def {module['name']}"
                     r"\([\s\S]*? Context(\[\w+\])?)",
                     group,
                     procs,
-                    flags=re.MULTILINE
+                    flags=re.MULTILINE,
                 )
-            with open(init_file, 'w') as f:
+            with open(init_file, "w") as f:
                 f.write(file)
-            with open(path_, 'w') as f:
+            with open(path_, "w") as f:
                 f.write(procs)
+
+
+@dev.command("procs-info", help="Get processors info in JSON format")
+def procs_info(
+    path=typer.Argument("./", show_default=False),
+    out: Annotated[
+        Union[str, None],
+        typer.Option("--out", help="File to save results in", show_default=False),
+    ] = None,
+    verbose: Annotated[
+        bool,
+        typer.Option(
+            ...,
+            "--verbose",
+            "-v",
+            help="Verbose mode",
+        ),
+    ] = False,
+) -> str | None:
+    procs = json.loads(list_procs(path))
+    if len(procs) == 0:
+        rich.print("No procs found.")
+        return
+    info = []
+    for p in procs:
+        if verbose:
+            rich.print(
+                f"Processing [bold]{p['name']}[/bold] "
+                f"from [italic]{p['path']}[/italic]"
+            )
+        doc = get_processor_docstring(p["name"], p["path"])
+        info.append(json.loads(parse_docstring(doc)))
+
+    if verbose:
+        rich.print(info)
+    if out is not None:
+        with open(out, "w") as f:
+            f.write(json.dumps(info))
+    return json.dumps(info)
+
+
+@dev.command("in-app-install", help="Install malevich inside the app")
+def in_app_install() -> None:
+    if os.getcwd() == "/julius":
+        pkg_ = site.getsitepackages()[0]
+        shutil.rmtree(os.path.join(pkg_, "malevich", "square"))
+        shutil.copytree(
+            "/julius/malevich/square", os.path.join(pkg_, "malevich", "square")
+        )
+        shutil.rmtree("/julius/malevich")
+        shutil.move(os.path.join(pkg_, "malevich"), "/julius/malevich")
+    else:
+        error_exit("You are running command outside of the app")
```

### Comparing `malevich-0.2.6/malevich/_cli/flow.py` & `malevich-0.4.0/malevich/_cli/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/install.py` & `malevich-0.4.0/malevich/_cli/install.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from typing import Annotated
 
 import rich
 import typer
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
-from .._utility.args import parse_kv_args
 from .._cli.prefs import prefs as prefs
 from .._cli.use import _install_from_image, _install_from_space
+from .._utility.args import parse_kv_args
 
 logging.getLogger("gql.transport.requests").setLevel(logging.ERROR)
 
 
 __With_Args_Help = (
     "Arguments to pass to the installer. "
     "Must be in the format [b]key1=value1,key2=value2[/b] "
```

### Comparing `malevich-0.2.6/malevich/_cli/list.py` & `malevich-0.4.0/malevich/_cli/list.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/manifest.py` & `malevich-0.4.0/malevich/_cli/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,10 +100,11 @@
         rich.print("[red]Not found[/red]")
     else:
         rich.print(__q)
 
 @app.command("show", help="Show manifest file")
 def show() -> None:
     manf = ManifestManager()
+    rich.print(manf.path)
     rich.print(manf.as_dict())
 
 app.add_typer(secrets, name="secrets")
```

### Comparing `malevich-0.2.6/malevich/_cli/misc/manifest_to_env.py` & `malevich-0.4.0/malevich/_cli/misc/manifest_to_env.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/new.py` & `malevich-0.4.0/malevich/_cli/new.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/prefs.py` & `malevich-0.4.0/malevich/_cli/prefs.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/remove.py` & `malevich-0.4.0/malevich/_cli/remove.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/restore.py` & `malevich-0.4.0/malevich/_cli/restore.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/space/init.py` & `malevich-0.4.0/malevich/_cli/space/init.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_cli/space/login.py` & `malevich-0.4.0/malevich/_cli/space/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Annotated, Optional
+from typing import Optional
 
 import rich
 import typer
 from malevich_space.ops import SpaceOps
 from malevich_space.schema import HostSchema, SpaceSetup
 from rich.prompt import Prompt
 
@@ -17,32 +17,34 @@
     api_url: str = PROD_SPACE_API_URL,
     core_url: str = DEFAULT_CORE_HOST,
     space_url: Optional[str] = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     org_id: Optional[str] = None,
 ) -> None:
-    if not space_url:
-        domain = re.search(r"\/\/(.*)api\.(.+)\/?", api_url)
-        left = domain.group(1) if domain.group(1) else ''
-        right = '.' + domain.group(2) if domain.group(2) else ''
-        space_url = f'https://{left}space{right}/'
-        base_space_url = f'{left}space{right}'.rstrip('/')
-    else:
-        domain = re.search(r"\/\/(.*)space\.(.+)\/?", space_url)
-        left = domain.group(1) if domain.group(1) else ''
-        right = '.' + domain.group(2) if domain.group(2) else ''
-        base_space_url = f'{left}space{right}'.rstrip('/')
-        api_url = f'https://{left}api{right}/'
-
+    try:
+        if not space_url:
+            domain = re.search(r"\/\/(.*)api\.(.+)\/?", api_url)
+            left = domain.group(1) if domain.group(1) else ''
+            right = '.' + domain.group(2) if domain.group(2) else ''
+            space_url = f'https://{left}space{right}/'
+            base_space_url = f'{left}space{right}'.rstrip('/')
+        else:
+            domain = re.search(r"\/\/(.*)space\.(.+)\/?", space_url)
+            left = domain.group(1) if domain.group(1) else ''
+            right = '.' + domain.group(2) if domain.group(2) else ''
+            base_space_url = f'{left}space{right}'.rstrip('/')
+            api_url = f'https://{left}api{right}/'
+    except Exception:
+        base_space_url = api_url
 
     if no_input and (username is None or password is None):
         rich.print("[red]You have to set --username and --password parameters, "
                    "if --no-input is used[/red]")
-        exit(-1)
+        return False
 
     manf = ManifestManager()
     rich.print(
         "[b]Welcome to [purple]Malevich Space[/purple]![/b]"
         " The command allows you to connect your account "
         f"to [bright_cyan]{space_url}[/bright_cyan]"
         "[bright_black]\nIf you don't have an account, "
@@ -57,17 +59,18 @@
         password = Prompt.ask(
             "Password",
             password=True
         )
 
     if not org_id and not no_input:
         org_id = Prompt.ask(
-            "Organization Slug (leave blank to use personal account)",
+            "Organization slug (leave blank to use personal account)",
             default=None,
         )
+
     setup = SpaceSetup(
         api_url=api_url,
         username=username,
         password=password,
         org=org_id,
         host=HostSchema(
             conn_url=core_url,
@@ -77,14 +80,16 @@
     try:
         SpaceOps(space_setup=setup)
     except Exception:
         rich.print(
             f"\n\n[red]Failed to connect to {space_url}. "
             "Please check your credentials and try again.[/red]"
         )
-        exit(-1)
+        return False
 
     space_password = manf.put_secret("space_password", setup.password)
     setup.password = space_password
     manf.put("space", value=setup)
     rich.print("\nMalevich Space configuration [green]successfully[/green]"
                " added to the manifest\n")
+
+    return True
```

### Comparing `malevich-0.2.6/malevich/_cli/use.py` & `malevich-0.4.0/malevich/_cli/use.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_core/ops.py` & `malevich-0.4.0/malevich/_core/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import os
 from concurrent.futures import Future, ProcessPoolExecutor
 from multiprocessing import cpu_count
 from typing import Optional
 
 import malevich_coretools as core
+from malevich_coretools import FilesDirs
 
 from ..constants import DEFAULT_CORE_HOST
 from ..models.collection import Collection
 from ..models.nodes.asset import AssetNode
 
 executor = ProcessPoolExecutor(max_workers=cpu_count())
 
@@ -247,28 +248,28 @@
 def _assure_asset(
     asset: AssetNode,
     auth: core.AUTH = None,
     conn_url: Optional[str] = None,
 ) -> None:
     try:
         if not asset.is_composite:
-            objs = [
-                core.get_collection_object(
-                    asset.core_path,
-                    auth=auth,
-                    conn_url=conn_url,
-                )
-            ]
+            core.get_collection_object(
+                asset.core_path,
+                auth=auth,
+                conn_url=conn_url,
+            )
+            objs = FilesDirs(files={asset.core_path: 0}, directories=[])
         else:
             objs = core.get_collection_objects(
                 asset.core_path,
                 auth=auth,
                 conn_url=conn_url,
             )
     except Exception as e:
+        print(e)
         if asset.real_path is not None:
             _upload_asset(asset, auth, conn_url)
             return
         else:
             raise Exception(
                 f"Asset {asset.core_path} is not found in Core. Cannot "
                 "upload it because real_path is not specified."
```

### Comparing `malevich-0.2.6/malevich/_core/scan.py` & `malevich-0.4.0/malevich/_core/scan.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_meta/asset.py` & `malevich-0.4.0/malevich/_meta/asset.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_meta/collection.py` & `malevich-0.4.0/malevich/_meta/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_meta/decor.py` & `malevich-0.4.0/malevich/_meta/decor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Generic, ParamSpec, Type, TypeVar
 
 from pydantic import BaseModel
 
 from .._autoflow.function import autotrace, sinktrace
 from ..constants import reserved_config_fields
+from ..models.type_annotations import ConfigArgument
 
 FnArgs = ParamSpec("FnArgs")
 FnReturn = TypeVar("FnReturn")
 Config = TypeVar("Config", bound=BaseModel)
 ProcConfig = TypeVar("ProcConfig", bound=BaseModel)
 
 ProcFunArgs = ParamSpec("ProcFunArgs")
@@ -23,14 +24,22 @@
         self.base_fn = fn
         if use_sinktrace:
             self.__fn = sinktrace(fn)
         else:
             self.__fn = autotrace(fn)
         self.__config_model = config_model
         self.__call__ = self._fn_call
+        self.__required_fields = [
+            key
+            for key, value in self.__fn.__annotations__.items()
+            if hasattr(value, '__metadata__')
+            and (metadata := getattr(value, '__metadata__'))
+            and isinstance(metadata[0], ConfigArgument)
+            and metadata[0].required
+        ]
 
     def _fn_call(self, *args: FnArgs.args, **kwargs: FnArgs.kwargs) -> FnReturn:
         # FIXME: literal 'config' is overused. Should be replaced with constant.
         if kwargs.get('config', None) is None:
             kwargs['config'] = {}
 
         if isinstance(kwargs['config'], BaseModel):
@@ -38,25 +47,42 @@
                 f"You have set config={kwargs['config']}, "
                 f"but it should be of type {self.__config_model}."
             )
 
             kwargs['config'] = kwargs['config'].model_dump()
         else:
             assert isinstance(kwargs, dict)
-
+        reserved_keys = {
+            x[0] for x in reserved_config_fields
+        }
         extra_fields = {**kwargs}
         extra_fields.pop('config')
-        for reserved, _ in reserved_config_fields:
-            extra_fields.pop(reserved, None)
+        for reserved_keys, _ in reserved_config_fields:
+            extra_fields.pop(reserved_keys, None)
 
         kwargs['config'] = {
             **kwargs['config'],
             **extra_fields,
         }
 
+        kwargs = {
+            'config': kwargs['config'],
+            **{
+                k: v for k, v in kwargs.items()
+                if k in reserved_keys
+            }
+        }
+
+        if (diff_ := set.difference(set(self.__required_fields), kwargs['config'].keys())) != set():  # noqa: E501
+            fields_ = ', '.join([f"`{x}`" for x in diff_])
+            raise Exception(
+                f"Missing required fields {fields_}"
+                f" in configuration of the processor `{self.__fn.__name__}`"
+            )
+
         return self.__fn(*args, **kwargs)
 
     __call__: Callable[ProcFunArgs, ProcFunReturn] = _fn_call
 
     @property
     def config(self) -> Type[Config]:
         return self.__config_model
```

### Comparing `malevich-0.2.6/malevich/_meta/flow.py` & `malevich-0.4.0/malevich/_meta/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_meta/run.py` & `malevich-0.4.0/malevich/_meta/run.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_templates/Dockerfile.app` & `malevich-0.4.0/malevich/_templates/Dockerfile.app`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Malevich App image. You may edit this file to add
 # additional dependencies to your app or set more
 # specific enironment.
 
 # Keep in mind, that source code containing
 # Malevich-specific code (declaration of processors, inits, etc.)
 # should be placed into ./apps directory
-FROM pogrebnoijak/julius_export_python:0.1
+FROM malevichai/app:python_v0.1
 
 # Copying requirements.txt and installing dependencies
 COPY requirements.txt requirements.txt
 RUN if test -e requirements.txt; then pip install --no-cache-dir -r requirements.txt; fi
 
 # Placing source code into the image
 # DO NOT change this line
```

### Comparing `malevich-0.2.6/malevich/_templates/README.app.md` & `malevich-0.4.0/malevich/_templates/README.app.md`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_templates/flow.py.txt` & `malevich-0.4.0/malevich/_templates/flow.py.txt`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_templates/processor.py.txt` & `malevich-0.4.0/malevich/_templates/processor.py.txt`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/args.py` & `malevich-0.4.0/malevich/_utility/args.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/cache/manager.py` & `malevich-0.4.0/malevich/_utility/cache/manager.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/ci/functions.py` & `malevich-0.4.0/malevich/_utility/ci/functions.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/ci/github.py` & `malevich-0.4.0/malevich/_utility/ci/github.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/ci/templates/malevich-ci-manual.yml` & `malevich-0.4.0/malevich/_utility/ci/templates/malevich-ci-manual.yml`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/ci/templates/malevich-ci.yml` & `malevich-0.4.0/malevich/_utility/ci/templates/malevich-ci.yml`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/dicts.py` & `malevich-0.4.0/malevich/_utility/dicts.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/git/clone.py` & `malevich-0.4.0/malevich/_utility/git/clone.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/logging.py` & `malevich-0.4.0/malevich/_utility/logging.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/package.py` & `malevich-0.4.0/malevich/_utility/package.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/registry.py` & `malevich-0.4.0/malevich/_utility/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from typing import TypeVar
 
-from .._utility.singleton import SingletonMeta
+from .singleton import SingletonMeta
 
 T = TypeVar('T')
 
 class Registry(metaclass=SingletonMeta):
     _registry = {}
 
     @property
```

### Comparing `malevich-0.2.6/malevich/_utility/scan.py` & `malevich-0.4.0/malevich/_utility/scan.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/stub.py` & `malevich-0.4.0/malevich/_utility/stub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import json
 import os
 import re
 import tempfile
+import typing
 from contextlib import chdir
 from hashlib import sha256
 from pathlib import Path
 from typing import Type
 
 import pydantic_yaml as pydml
 from datamodel_code_generator import generate
@@ -36,17 +37,18 @@
 Third-party Malevich app. Use it in flow by importing any processor
 from this module and calling it within @flow decorated function.
 \"\"\"
 """
 
     imports = """
 import typing
-from typing import Any, Optional
+from typing import *
 
 import malevich.annotations
+from malevich.models.type_annotations import ConfigArgument
 from malevich._meta.decor import proc
 from malevich._utility.registry import Registry
 from malevich.models.nodes import OperationNode
 from .scheme import *
 """
 
     registry = """
@@ -140,51 +142,56 @@
             #    argX: typeX,
             def_ += f'\n\t{arg[0]}: {arg[1] or "Any"}' + ","
         # def processor_name(
         #    ...
         #    argX: typeX,
         #    *,
         if self.sink:
-            def_ += f'\n\t*{self.sink[0]}: Any,'
+            if len(self.args) > 0:
+                def_ += f'\n\t/,\n\t*{self.sink[0]}: Any, '
+            else:
+                def_ += f'\n\t*{self.sink[0]}: Any, '
         else:
-            def_ += "\n\t*, "
+            def_ += "\n\t/, "
         if self.config_schema is not None:
             config_fields = self.config_schema.model_fields
             for field in config_fields:
                 if field == "config":
                     raise ValueError(
                         "Trying to generate a definition for "
                         "a function with a config field named 'config'"
                     )
-
-                if 'typing' in str(config_fields[field].annotation):
-                    # typing.Union, typing.Optional
-                    annotation = str(config_fields[field].annotation)
-                elif hasattr(config_fields[field].annotation, "__name__"):
+                is_required = config_fields[field].is_required()
+                annotation = config_fields[field].annotation
+                if (
+                    hasattr(annotation, "__name__")
+                    and annotation.__module__ != typing.__name__
+                ):
                     # class
                     annotation = config_fields[field].annotation.__name__
                 else:
                     # etc.
                     annotation = str(config_fields[field].annotation)
+                # if not config_fields[field].is_required() and 'Optional' not in str(annotation):  # noqa: E501
+                #     def_ += f'\n\t{field}: Optional["{annotation}"]' + " = None,"
+                # elif not config_fields[field].is_required():
+                #     def_ += f'\n\t{field}: "{annotation}"' + " = None,"
+                # else:
+                #     def_ += f'\n\t{field}: "{annotation}"' + ","
 
-                if not config_fields[field].is_required() and 'Optional' not in str(annotation):  # noqa: E501
-                    def_ += f'\n\t{field}: Optional["{annotation}"]' + " = None,"
-                elif not config_fields[field].is_required():
-                    def_ += f'\n\t{field}: "{annotation}"' + " = None,"
-                else:
-                    def_ += f'\n\t{field}: "{annotation}"' + ","
+                def_ += f'\n\t{field}: Annotated["{annotation}", ConfigArgument(required={is_required})] = None,'  # noqa: E501
 
         for rkey, rtype in reserved_config_fields:
             def_ += f'\n\t{rkey}: Optional["{rtype}"]' + " = None,"
 
         if config_model:
             def_ += f'\n\tconfig: Optional["{config_model}"] = None, '
         else:
             def_ += '\n\tconfig: Optional[dict] = None, '
-        def_ += '\n\t**extra_config_fields: dict[str, str], '
+        def_ += '\n\t**extra_config_fields: dict[str, Any], '
         def_ = def_[:-2] + ") -> malevich.annotations.OpResult:"
         def_ += f'\n\t"""{self.docstrings}"""\n'
         return def_.replace('\t', ' ' * 4)
 
 
 class StubSchema(BaseModel):
     name: str
@@ -200,25 +207,27 @@
     schemes_index: dict[str, tuple[int, int]]
 
 
 class Stub:
     class Utils:
         @staticmethod
         def generate_context_schema(json_schema: str) -> tuple[str, str]:
+
             with (
                 tempfile.NamedTemporaryFile(mode='w+', suffix='.json') as f,
                 tempfile.NamedTemporaryFile(mode='w+', suffix='.py') as out
             ):
                 f.write(json_schema)
                 f.seek(0)
                 generate(
                     Path(f.name),
                     output=Path(out.name),
                     use_annotated=False,
-                    input_file_type='jsonschema'
+                    input_file_type='jsonschema',
+                    base_class='malevich.models._model._Model', # cool
                 )
                 out_script =  open(out.name).read().replace(
                     'from __future__ import annotations',
                     '\n'
                 )
                 return (
                     re.search(
```

### Comparing `malevich-0.2.6/malevich/_utility/summary/abstract.py` & `malevich-0.4.0/malevich/_utility/summary/abstract.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/_utility/summary/time.py` & `malevich-0.4.0/malevich/_utility/summary/time.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 
 import pandas as pd
 import rich
 from malevich_coretools import logs_clickhouse
 from rich.table import Table
 
-from ..._utility.host import fix_host
-from ..._utility.summary.abstract import AbstractSummary
+from ..._utility import fix_host
 from ...interpreter.core import CoreInterpreterState
+from ..summary.abstract import AbstractSummary
 
 
 class CoreTimeSummary(AbstractSummary[CoreInterpreterState]):
     def __init__(self, interpreter_state: CoreInterpreterState) -> None:
         super().__init__(None, interpreter_state)
 
     def json(self) -> None:
```

### Comparing `malevich-0.2.6/malevich/_utility/tree.py` & `malevich-0.4.0/malevich/_utility/tree.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/annotations.py` & `malevich-0.4.0/malevich/annotations.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/cli.py` & `malevich-0.4.0/malevich/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 
 import typer
 import typer.core
 from malevich_space.cli.cli import app as space_app
 
+from ._cli.space.whoami import get_user_on_space
 import malevich.help as help
 
 from ._cli.ci import app as ci_app
 from ._cli.core.app import core_app
 from ._cli.dev.dev import dev as dev_app
 from ._cli.flow import flow as flow_app
+from ._cli.init import init as init_
 from ._cli.install import auto_use
 from ._cli.list import list_packages
 from ._cli.manifest import app as manifest_app
 from ._cli.new import new
 from ._cli.prefs import prefs as prefs
 from ._cli.remove import remove
 from ._cli.restore import restore
@@ -65,24 +67,34 @@
         name="list",
         help=help.list_["--help"],
         callback=list_packages,
         cls=typer.core.TyperCommand
     )
 )
 
-# malevich list
+# malevich new
 app.registered_commands.append(
     typer.models.CommandInfo(
         name="new",
-        help=help.list_["--help"],
+        help=help.new["--help"],
         callback=new,
         cls=typer.core.TyperCommand
     )
 )
 
+# malevich init
+app.registered_commands.append(
+    typer.models.CommandInfo(
+        name="init",
+        help="Initializes new Malevich project",
+        callback=init_,
+        cls=typer.core.TyperCommand
+    )
+)
+
 # _________________________________________________
 
 # Space Additional Commands
 # -------------------------------------------------
 
 # malevich space init
 space_app.registered_commands.append(
@@ -98,14 +110,22 @@
     typer.models.CommandInfo(
         help=help.space["login --help"],
         callback=login,
         cls=typer.core.TyperCommand
     )
 )
 
+space_app.registered_commands.append(
+    typer.models.CommandInfo(
+        "whoami",
+        help=help.space["whoami --help"],
+        callback=get_user_on_space,
+        cls=typer.core.TyperCommand
+    )
+)
 # __________________________________________________
 
 
 # =============== Register Groups ==================
 # --------------------------------------------------
 
 
@@ -127,15 +147,15 @@
 # malevich prefs
 app.add_typer(prefs, name="prefs")
 
 # malevich dev
 app.add_typer(dev_app, name='dev')
 
 #malevich core
-app.add_typer(core_app, name='core')
+app.add_typer(core_app, name='core', help=help.core['--help'])
 # _________________________________________________
 
 
 class CLIContext:
     global_ = False
 
 @app.callback()
```

### Comparing `malevich-0.2.6/malevich/help.py` & `malevich-0.4.0/malevich/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     '--help': """Restore all installed apps manifested in the current environment"""
 }
 
 space = {
     '--help': """Communicate with Malevich Space - a public provider of Malevich Core""",
     'init --help': """Imports Malevich Space configuration into the current environment""",
     'login --help': """Interactive login to Malevich Space""",
+    'whoami --help': """Get information about connected Space user"""
 }
 
 remove = {
     '--help': """Remove apps from the current environment""",
 }
 
 ci = {
@@ -84,7 +85,11 @@
 list_ = {
     '--help': """List all installed package stubs."""
 }
 
 new = {
     '--help': """Create a new app from a template""",
 }
+
+core = {
+    '--help': """Manage your Core account"""
+}
```

### Comparing `malevich-0.2.6/malevich/install/image.py` & `malevich-0.4.0/malevich/install/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 Provides functionality to install packages from plain Docker images
 using Malevich Core capabilities
 """
 
 import hashlib
-import json
+import re
 from typing import Optional
 
-import malevich_coretools as core
-
 from .._core.scan import scan_core
 from .._utility.stub import Stub
 from ..constants import DEFAULT_CORE_HOST, IMAGE_BASE
 from ..install.installer import Installer
 from ..manifest import ManifestManager
 from ..models.installers.image import ImageDependency, ImageOptions
 from ..path import Paths
@@ -94,14 +92,15 @@
         self,
         package_name: str,
         image_ref: str,
         image_auth: tuple[str, str],
         core_host: str = DEFAULT_CORE_HOST,
         core_auth: Optional[tuple[str, str]] = None,
     ) -> ImageDependency:
+        package_name = re.sub(r'[\W\s]+', '_', package_name)
         app_info = scan_core(
             core_auth=core_auth,
             core_host=core_host,
             image_ref=image_ref,
             image_auth=image_auth,
         )
         checksum = hashlib.sha256(
@@ -143,15 +142,15 @@
             path=Paths.module(package_name),
             package_name=package_name,
             dependency=dependency,
             operation_ids=operation_ids,
             registry_records={
                 processor_id: {
                     "operation_id": operation_id,
-                    "image_ref": image_ref,
+                    "image_ref":  ('dependencies', package_name, 'options', 'image_ref'),
                     "image_auth_user": ('dependencies', package_name, 'options', 'image_auth_user'),  # noqa: E501
                     "image_auth_pass": ('dependencies', package_name, 'options', 'image_auth_pass'),  # noqa: E501
                     "processor_id": operation_names[processor_id],
                 }
                 for processor_id, operation_id in operation_ids.items()
             },
         )
```

### Comparing `malevich-0.2.6/malevich/install/installer.py` & `malevich-0.4.0/malevich/install/installer.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/install/stub.py` & `malevich-0.4.0/malevich/install/stub.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/interpreter/abstract.py` & `malevich-0.4.0/malevich/interpreter/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 from abc import abstractmethod
 from copy import deepcopy
-from typing import Any, Generic, TypeVar
+from typing import Generic, TypeVar
 
 from malevich_space.schema import ComponentSchema
 
 from .._autoflow.tracer import traced
 from .._utility.tree import unwrap_tree
 from ..models.argument import ArgumentLink
 from ..models.nodes.base import BaseNode
```

### Comparing `malevich-0.2.6/malevich/interpreter/core.py` & `malevich-0.4.0/malevich/interpreter/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         state: CoreInterpreterState,
         callee: traced[BaseNode],
         caller: traced[BaseNode],
         link: ArgumentLink,
     ) -> CoreInterpreterState:
         state.depends[caller.owner.uuid].append((callee.owner, link))
         _log(
-            f"Dependency: {caller.owner.short_info()} -> {callee.owner.short_info()}, "
+            f"Dependency: {callee.owner.short_info()} -> {caller.owner.short_info()}, "
             f"Link: {link.name}", -1, 0, True
         )
         return state
 
     def before_interpret(self, state: CoreInterpreterState) -> CoreInterpreterState:
         _log("Connection to Core is established.", 0, 0, True)
         _log(f"Core host: {self.__core_host}", 0, 0, True)
@@ -321,15 +321,15 @@
                     continue
 
                 coll, uploaded_core_id = state.collections[node.uuid]
                 state.cfg.collections = {
                     **state.cfg.collections,
                     f"{coll}": uploaded_core_id,
                 }
-                state.extra_colls[op.uuid][link.name] = coll
+                state.extra_colls[op.uuid][link.name].append(coll)
 
             if not op.alias:
                 op.alias = extra["processor_id"] + '-' + str(_name(extra["processor_id"]))  # noqa: E501
 
             app_core_name = op.uuid + f"-{extra['processor_id']}-{op.alias}"
 
             state.task_aliases[op.alias] = app_core_name
```

### Comparing `malevich-0.2.6/malevich/interpreter/space.py` & `malevich-0.4.0/malevich/interpreter/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 from ..models.types import TracedNode
 
 manf = ManifestManager()
 reg = Registry()
 cache = CacheManager()
 
 _levels = [LogLevel.Info, LogLevel.Warning, LogLevel.Error, LogLevel.Debug]
-_actions = [Action.Interpretation,
-            Action.Preparation, Action.Run, Action.Results]
+_actions = [Action.Interpretation, Action.Preparation, Action.Run, Action.Results]
 
 
 def _log(
     message: str,
     level: int = 0,
     action: int = 0,
     step: bool = False,
@@ -115,60 +114,55 @@
     Results
     -------
 
     Results is represented as a list of
     :class:`malevich.results.space.SpaceCollectionResult`
     objects.
     """
+
     supports_subtrees = True
 
-    def prettify_collection_id(
-        self,
-        collection_id: str
-    ) -> str:
+    def prettify_collection_id(self, collection_id: str) -> str:
         # Replace spaces with dashes
-        _s = re.sub(r'\s+', '-', collection_id)
+        _s = re.sub(r"\s+", "-", collection_id)
         # Lowercase
         _s = _s.lower()
         # Replace underscores with dashes
         return _s
 
-    def prettify_collection_name(
-        self,
-        collection_name: str
-    ) -> str:
+    def prettify_collection_name(self, collection_name: str) -> str:
         # Replace multiple spaces with one
-        _s = re.sub(r'\s+', ' ', collection_name)
+        _s = re.sub(r"\s+", " ", collection_name)
         # Replace dashes and underscores with spaces
-        _s = re.sub(r'-', ' ', _s)
+        _s = re.sub(r"-", " ", _s)
         # Title case
         return _s.title()
 
     def prettify_schema_id(self, schema_name: str) -> str:
         # 'Schema Name - Some_Name' -> 'SchemaNameSome_Name"
-        _s = re.sub(r'[\s-]+', ' ', schema_name)
-        return _s.replace(' ', '').lower()
+        _s = re.sub(r"[\s-]+", " ", schema_name)
+        return _s.replace(" ", "").lower()
 
     def prettify_component_name(self, component_name: str) -> str:
-        _s = re.sub(r'[\s-]+', ' ', component_name)
+        _s = re.sub(r"[\s-]+", " ", component_name)
         return _s.title()
 
     def prettify_config_name(self, component_name: str) -> str:
-        _s = re.sub(r'[\s-]+', ' ', component_name)
-        return 'Meta Config for ' + _s.title()
+        _s = re.sub(r"[\s-]+", " ", component_name)
+        return "Meta Config for " + _s.title()
 
     def prettify_config_id(
         self,
         component_name: str,
-        rand: Optional[str] = None  # Random string
+        rand: Optional[str] = None,  # Random string
     ) -> str:
         rand = rand or uuid4().hex[:8]
-        __b = 'meta-config-for-' + re.sub(r'[\s|_|-]+', ' ', component_name)
+        __b = "meta-config-for-" + re.sub(r"[\s|_|-]+", " ", component_name)
         if rand:
-            __b += '-' + rand
+            __b += "-" + rand
         return __b
 
     def update_state(self, state: SpaceInterpreterState = None) -> None:
         """
         The state contains pydantic models, which are not deepcopyable.
         So, this method is used to update the state using custom `copy` method.
         """
@@ -193,82 +187,83 @@
             name (str): Name of the flow.
             reverse_id (str): Reverse id of the flow.
         """
         super().__init__()
         self._state = SpaceInterpreterState()
         if not setup and not ops:
             try:
-                setup = resolve_setup(manf.query(
-                    "space", resolve_secrets=True))
+                setup = resolve_setup(manf.query("space", resolve_secrets=True))
             except Exception as e:
+                from malevich._cli.space.login import login
+                if login():
+                    setup = resolve_setup(manf.query("space", resolve_secrets=True))
                 raise InterpretationError(
                     "Failed to resolve space setup. "
                     "Please check your manifest file.",
-                    self, self._state
+                    self,
+                    self._state,
                 ) from e
 
         space = ops or SpaceOps(setup)
 
         try:  # Local patch for space
             host_ = space.get_my_hosts(url=setup.host.conn_url)[0]
         except Exception:
             host_ = None
 
         if not host_:
             try:
                 host_ = space.create_host(
-                    alias=setup.host.alias or '',
-                    conn_url=setup.host.conn_url
+                    alias=setup.host.alias or "", conn_url=setup.host.conn_url
                 )
             except KeyError as ke:
-                if 'details' in ke.args[0]:
+                if "details" in ke.args[0]:
                     # Local patch for space
                     pass
 
         self._state.component_manager = ComponentManager(
-            host=host_,
-            space=space,
-            comp_dir='./'
+            host=host_, space=space, comp_dir="./"
         )
 
         self._state.host = host_
         self._state.space = space
         self._upload_collections = update_collections
         self._version_mode = version_mode
 
         self.update_state()
 
     @overload
     def _upload_schema(
         self,
         state: SpaceInterpreterState,
         node: CollectionNode,
-        skip_create: Literal[True]
+        skip_create: Literal[True],
     ) -> tuple[str | None, str]:
         pass
 
     @overload
     def _upload_schema(
         self,
         state: SpaceInterpreterState,
         node: CollectionNode,
-        skip_create: Literal[False]
+        skip_create: Literal[False],
     ) -> tuple[str, str]:
         pass
 
     def _upload_schema(
         self,
         state: SpaceInterpreterState,
         node: CollectionNode,
-        skip_create: bool = False
+        skip_create: bool = False,
     ) -> tuple[str | None, str]:
         if not node.scheme:
             raise InterpretationError(
                 "To be able to use collection, it should have an attached schema",
-                self, state
+                self,
+                state,
             )
 
         # Understanding scheme
         if isinstance(node.scheme, SchemaMetadata):
             # If scheme is already parsed
             core_id = node.scheme.core_id
 
@@ -280,28 +275,24 @@
             else:
                 schema_uid = s.uid
                 return schema_uid, core_id
 
         if isinstance(node.scheme, str):
             # If scheme is a string, then it should firstly
             # be uploaded
-            core_id = self.prettify_schema_id(
-                node.collection.collection_id
-            )
+            core_id = self.prettify_schema_id(node.collection.collection_id)
 
             if skip_create:
                 return None, core_id
 
             schema_uid = state.space.create_scheme(
                 # $core_id: String!, $raw: String!, $name: String
                 core_id=core_id,
                 raw=node.scheme,
-                name=self.prettify_schema_id(
-                    node.collection.collection_id
-                )
+                name=self.prettify_schema_id(node.collection.collection_id),
             )
             # RFC: Should I allow to upload collection without scheme?
             assert schema_uid, "Failed to upload the schema"
 
         return schema_uid, core_id
 
     def _upload_collection(
@@ -310,60 +301,50 @@
         node: CollectionNode,
         core_id: str | None = None,
     ) -> str:
         """Uploads collection (and underlying scheme) to the space."""
         if not core_id:
             core_id = node.collection.collection_id
 
-        _, schema_core_id = self._upload_schema(
-            state, node
-        )
+        _, schema_core_id = self._upload_schema(state, node)
         # Uploading collection
-        alias = self.prettify_collection_name(
-            node.collection.collection_id
-        )
+        alias = self.prettify_collection_name(node.collection.collection_id)
 
         # RFC!: Is it correct way to upload collection?
         uid = state.space.create_collection(
             host_id=state.host.uid,
             core_id=core_id,
             core_alias=alias,
             schema_core_id=schema_core_id,
             docs=[
-                row.to_json()
-                for _, row in node.collection.collection_data.iterrows()
-            ]
+                row.to_json() for _, row in node.collection.collection_data.iterrows()
+            ],
         )
 
         return uid
 
     def interpret(self, node: TreeNode, component: ComponentSchema) -> BaseTask:
         self._state.aux.tree = node
         if self._version_mode == VersionMode.DEFAULT:
             loaded = self.state.space.get_parsed_component_by_reverse_id(
                 reverse_id=component.reverse_id
             )
 
-            task = SpaceTask(
-                state=self.state,
-                component=loaded
-            )
+            task = SpaceTask(state=self.state, component=loaded)
             all = {i.uid for i in loaded.flow.components}
             non_leaves = set().union(
                 *[{i.uid for i in c.prev} for c in loaded.flow.components]
             )
             leaves = all.difference(non_leaves)
             returned = [
                 gn.tracedLike(BaseNode(uuid=c.uid, alias=c.alias))
                 for c in loaded.flow.components
                 if c.uid in leaves
             ]
-            task.commit_returned(
-                returned
-            )
+            task.commit_returned(returned)
             return task
 
         return super().interpret(node, component)
 
     def before_interpret(self, state) -> SpaceInterpreterState:
         state.flow = FlowSchema()
         return state
@@ -377,30 +358,25 @@
             state (SpaceInterpreterState): Interpreter state.
             node (gn.traced[BaseNode]): Node to wrap.
 
         Returns:
             SpaceInterpreterState: Interpreter state.
         """
 
-
         if isinstance(node.owner, CollectionNode):  # If the node is a collection
             alias_base = node.owner.collection.collection_id
 
-            _, path = cache.space.probe_new_entry(
-                node.owner.collection.collection_id,
-                entry_group='collections/temp'
-            )
-
-            if not node.owner.collection.collection_data.empty:
-                node.owner.collection.collection_data.to_csv(
-                    path,
-                    index=False
-                )
-            else:
-                path = None
+            # _, path = cache.space.probe_new_entry(
+            #     node.owner.collection.collection_id, entry_group="collections/temp"
+            # )
+
+            # if not node.owner.collection.collection_data.empty:
+            #     node.owner.collection.collection_data.to_csv(path, index=False)
+            # else:
+            #     path = None
 
             state.node_type[node.owner.uuid] = NodeType.COLLECTION
             # Try to get the collection component from the space
             component = state.space.get_parsed_component_by_reverse_id(
                 # Using the collection id as the reverse id
                 reverse_id=node.owner.collection.collection_id
             )
@@ -411,103 +387,110 @@
                     node.owner.collection.collection_id
                 )
 
                 _, schema_core_id = self._upload_schema(
                     state=state, node=node.owner, skip_create=False
                 )
 
-                if not path:
+                if node.owner.collection.collection_data is None:
                     # NOTE: path is None is the only
                     # case for the exception. However,
                     # there may be some more, which should be
                     # checked as well
                     raise InterpretationError(
-                        'Cannot interpret collection '
+                        "Cannot interpret collection "
                         + node.owner.collection.collection_id
-                        + '. There is no such collection on Space and'
-                        + ' there is no data provided to upload. Either use'
-                        + ' existing collections, or provide `df` or `file` argument'
-                        + ' in collection(...) call'
+                        + ". There is no such collection on Space and"
+                        + " there is no data provided to upload. Either use"
+                        + " existing collections, or provide `df` or `file` argument"
+                        + " in collection(...) call"
                     )
 
                 comp = ComponentSchema(
                     name=name,
                     description=f"Meta collection {name}",
                     reverse_id=node.owner.collection.collection_id,
                     collection=CollectionAliasSchema(
                         core_alias=node.owner.collection.collection_id,
                         schema_core_id=schema_core_id,
-                        path=path
-                    )
+                        # NOTE: 0.4.18 patch: path -> docs
+                        # path=path,
+                        docs=[
+                            row.to_json() for _, row in
+                            node.owner.collection.collection_data.iterrows()
+                        ],
+                    ),
                 )
             else:
                 if self._upload_collections:
                     coll_id = self.prettify_collection_id(
                         node.owner.collection.collection_id
                     )
                     uid = self._upload_collection(
-                        state, node.owner,
-                        core_id=f'override-{coll_id}-{state.interpretation_id}'
+                        state,
+                        node.owner,
+                        core_id=f"override-{coll_id}-{state.interpretation_id}",
                     )
                     state.collection_overrides[component.collection.uid] = uid
 
                 comp = ComponentSchema(
                     reverse_id=component.reverse_id,
                     name=component.name,
                 )
 
-
         elif isinstance(node.owner, OperationNode):  # If the node is an operation
             state.node_type[node.owner.uuid] = NodeType.OPERATION
 
             # All the required information to interpret the node
             # should be in the registry
             extra = reg.get(node.owner.operation_id)
 
             # If no extra information is found, it means
             # local information is too old
             # (but it is user fault, not mine)
-            if 'reverse_id' not in extra:
+            if "reverse_id" not in extra:
                 raise InterpretationError(
-                "Could not find reverse_id for the operation. Most probably, "
-                "you are trying to use an operation installed by another installer.",
-                    self, state
+                    "Could not find reverse_id for the operation. "
+                    "Most probably, you are trying to use an operation "
+                    "installed by another installer.",
+                    self,
+                    state,
                 )
 
-            alias_base = extra['reverse_id']
+            alias_base = extra["reverse_id"]
 
             # Get the component from the space (it should be there)
-            component = state.component_manager.space.get_parsed_component_by_reverse_id(  # noqa: E501
-                reverse_id=extra['reverse_id']
+            component = (
+                state.component_manager.space.get_parsed_component_by_reverse_id(
+                    reverse_id=extra["reverse_id"]
+                )
             )
 
             if not component:
                 # How then you install it? Was it wiped? :(
                 raise InterpretationError(
                     "Trying to interpret an operation that is not installed "
                     "properly or extremely outdated. Try to reinstall "
                     "the operation with\n\t"
                     f"`malevich install {extra['reverse_id']} --using space`",
-                    self, state
+                    self,
+                    state,
                 )
 
             state.components_config[node.owner.uuid] = node.owner.config
             comp = ComponentSchema(
-                name=component.name,
-                reverse_id=component.reverse_id,
-                app=component.app
+                name=component.name, reverse_id=component.reverse_id, app=component.app
             )
             state.node_to_operation[node.owner.uuid] = node.owner.operation_id
 
         elif isinstance(node.owner, TreeNode):
             alias_base = node.owner.reverse_id
             if not state.children_states.get(node.owner.uuid, None):
                 child_interpreter = SpaceInterpreter(
-                    name=node.owner.name,
-                    reverse_id=node.owner.reverse_id
+                    name=node.owner.name, reverse_id=node.owner.reverse_id
                 )
 
                 child_interpreter.interpret(node.owner)
                 child_state: SpaceInterpreterState = child_interpreter.state
 
                 comp = ComponentSchema(
                     name=node.owner.name,
@@ -526,30 +509,34 @@
 
         if not comp:
             raise InterpretationError(
                 "Failed to interpret the node. This is a bug, please report it.",
             )
 
         state.components[node.owner.uuid] = comp
-        state.components_alias[node.owner.uuid] = node.owner.alias or f'{alias_base} {_name(alias_base)}'  # noqa: E501
+        state.components_alias[node.owner.uuid] = (
+            node.owner.alias or f"{alias_base} {_name(alias_base)}"
+        )
         node.owner.alias = state.components_alias[node.owner.uuid]
         return state
 
     def create_dependency(
         self,
         state: SpaceInterpreterState,
         caller: TracedNode,
         callee: traced[OperationNode],
-        link: ArgumentLink
+        link: ArgumentLink,
     ) -> SpaceInterpreterState:
         """Creates a dependency between two nodes."""
 
         # Case Collection / App -> Flow
 
-        if isinstance(callee.owner, TreeNode) and not isinstance(caller.owner, TreeNode):  # noqa: E501
+        if isinstance(callee.owner, TreeNode) and not isinstance(
+            caller.owner, TreeNode
+        ):
             child = state.children_states[callee.owner.uuid]
             caller_alias = state.components_alias[caller.owner.uuid]
             inter_flow_map = {}
 
             bridges = link.compressed_nodes
 
             for _, to in bridges:
@@ -558,49 +545,44 @@
             dependency = InFlowDependency(
                 from_op_id=(
                     # provided by space installer
                     caller.owner.operation_id
                     if isinstance(caller.owner, OperationNode)
                     else None
                 ),
-                to_op_id=callee.owner.underlying_node.operation_id if isinstance(
-                    callee.owner.underlying_node, OperationNode) else None,
+                to_op_id=callee.owner.underlying_node.operation_id
+                if isinstance(callee.owner.underlying_node, OperationNode)
+                else None,
                 alias=state.components_alias[caller.owner.uuid],
                 order=link.index,
                 terminals=[
-                    Terminal(
-                        src=x,
-                        target=y
-                    ) for x, y in inter_flow_map.items()
-                ]
+                    Terminal(src=x, target=y) for x, y in inter_flow_map.items()
+                ],
             )
-        elif isinstance(caller.owner, TreeNode) and not isinstance(callee.owner, TreeNode):  # noqa: E501
+        elif isinstance(caller.owner, TreeNode) and not isinstance(
+            callee.owner, TreeNode
+        ):
             child = state.children_states[caller.owner.uuid]
             callee_alias = state.components_alias[callee.owner.uuid]
             op: OperationNode = caller.owner.underlying_node
-            inter_flow_map = {
-                child.components_alias[op.uuid]: callee_alias
-            }
+            inter_flow_map = {child.components_alias[op.uuid]: callee_alias}
 
             dependency = InFlowDependency(
                 from_op_id=op.operation_id,
                 to_op_id=(
                     # provided by space installer
                     callee.owner.operation_id
                     if isinstance(callee.owner, OperationNode)
                     else None
                 ),
                 alias=state.components_alias[caller.owner.uuid],
                 order=link.index,
                 terminals=[
-                    Terminal(
-                        src=x,
-                        target=y
-                    ) for x, y in inter_flow_map.items()
-                ]
+                    Terminal(src=x, target=y) for x, y in inter_flow_map.items()
+                ],
             )
         elif isinstance(caller.owner, TreeNode) and isinstance(callee.owner, TreeNode):
             left_op = caller.owner.underlying_node
             right_edges = link.compressed_nodes
             for rel, right_node in right_edges:
                 state.dependencies[callee.owner.uuid].append(
                     InFlowDependency(
@@ -612,18 +594,24 @@
                         to_op_id=(
                             right_node.owner.operation_id
                             if isinstance(right_node.owner, OperationNode)
                             else None
                         ),
                         alias=state.components_alias[caller.owner.uuid],
                         order=rel.index,
-                        terminals=[Terminal(
-                            src=state.children_states[caller.owner.uuid].components_alias[left_op.uuid],
-                            target=state.children_states[callee.owner.uuid].components_alias[right_node.owner.uuid]
-                        )]
+                        terminals=[
+                            Terminal(
+                                src=state.children_states[
+                                    caller.owner.uuid
+                                ].components_alias[left_op.uuid],
+                                target=state.children_states[
+                                    callee.owner.uuid
+                                ].components_alias[right_node.owner.uuid],
+                            )
+                        ],
                     )
                 )
             return state
         else:
             dependency = InFlowDependency(
                 from_op_id=(
                     # provided by space installer
@@ -643,40 +631,41 @@
     def after_interpret(self, state: SpaceInterpreterState) -> SpaceInterpreterState:
         """Finishes the interpretation by adding components to the flow."""
         for uid, component in state.components.items():
             try:
                 # I don't know why, but sometimes
                 # it fails, so try/exc here
                 loaded_component = state.component_manager.component(
-                    component,
-                    VersionMode.DEFAULT
+                    component, VersionMode.DEFAULT
                 )
             except Exception as e:
                 # If it fails, try to get the component
                 # by reverse id
-                loaded_component = state.component_manager.space.get_component_by_reverse_id(  # noqa: E501
-                    component.reverse_id
+                loaded_component = (
+                    state.component_manager.space.get_component_by_reverse_id(
+                        component.reverse_id
+                    )
                 )
 
                 # No components?(
                 # Nothing to do here
                 if loaded_component is None:
                     raise InterpretationError(
                         f"Failed to interpret the flow: component {component.name} "
                         "failed to load. ",
-                        self, state
+                        self,
+                        state,
                     ) from e
 
             # If the component is an operation
             # and has config
             if uid in state.components_config:
                 # RFC: Is it correct way to update config?
                 space_config = CfgSchema(
-                    readable_name=self.prettify_config_name(
-                        component.reverse_id),
+                    readable_name=self.prettify_config_name(component.reverse_id),
                     cfg_json=state.components_config.get(uid),
                     core_name=self.prettify_config_id(component.reverse_id),
                 )
             else:
                 space_config = None
 
             if uid in state.node_to_operation:
@@ -686,150 +675,112 @@
 
             # Add the component to the flow
             state.flow.components = [
                 *state.flow.components,
                 InFlowComponentSchema(
                     reverse_id=component.reverse_id,
                     alias=state.components_alias[uid],
-                    depends={
-                        dep.alias: dep
-                        for dep in state.dependencies[uid]
-                    },
+                    depends={dep.alias: dep for dep in state.dependencies[uid]},
                     app=InFlowAppSchema(
                         active_op=[
-                            OpSchema(
-                                core_id=extra['processor_name'],
-                                type='processor'
-                            )
+                            OpSchema(core_id=extra["processor_name"], type="processor")
                         ]
-                    ) if component.app is not None else None,
+                    )
+                    if component.app is not None
+                    else None,
                     active_cfg=space_config,
                 ),
             ]
 
         return state
 
-    def get_task(
-        self,
-        state: SpaceInterpreterState
-    ) -> BaseTask[SpaceInterpreterState]:
+    def get_task(self, state: SpaceInterpreterState) -> BaseTask[SpaceInterpreterState]:
         if self._component is None:
             raise Exception("Expected _component to be not None")
 
         self._component.flow = state.flow
 
-        component = state.component_manager.component(
-            self._component,
-            self._version_mode,
-        )
+        def get_component():
+            component = state.component_manager.component(
+                self._component,
+                self._version_mode,
+            )
+            if self._version_mode != VersionMode.DEFAULT:
+                state.space.auto_layout(flow=component.flow.uid)
 
-        if self._version_mode != VersionMode.DEFAULT:
-            self.state.space.client.execute(
-                gql("""
-                query AutoLayout($flow: String!) {
-                    flow(uid: $flow) {
-                        autoLayout {
-                            pageInfo {
-                                totalLen
-                            }
-                        }
-                    }
-                }
-                """),
-                variable_values={'flow': component.flow.uid}
-            )
-
-        return SpaceTask(
-            state=self.state,
-            component=component
-        )
+            return component
+
+        return SpaceTask(state=self.state, get_component=get_component)
 
     def attach(
         self,
         reverse_id: str | None = None,
-        deployment_id: str | None = None
+        deployment_id: str | None = None,
+        attach_to_last: bool = False,
     ) -> SpaceTask:
-        assert reverse_id or deployment_id, (
-            'Either reverse_id or deployment_id should be set'
-        )
+        assert (
+            reverse_id or deployment_id
+        ), "Either reverse_id or deployment_id should be set"
 
         successful = False
         if deployment_id:
             try:
-                results = self._state.space.client.execute(
-                    gql("""
-                        query GetTaskCoreId($task_id: String!) {
-                            task(uid: $task_id) {
-                                details {
-                                    coreId
-                                }
-                                component {
-                                    details {
-                                        reverseId
-                                    }
-                                }
-                            }
-                        }
-                        """
-                    ), variable_values={'task_id': deployment_id}
-                )
-                self._state.aux.core_task_id = results['task']['details']['coreId']
-                reverse_id = results['task']['component']['details']['reverseId']
+                core_id, loaded_reverse_id = self._state.space.get_task_core_id(task_id=deployment_id)
+                self._state.aux.core_task_id = core_id
+                reverse_id = loaded_reverse_id
                 self._state.aux.task_id = deployment_id
                 successful |= True
             except Exception:
                 if reverse_id is None:
                     raise Exception(
-                        'Could not attach to the flow. '
-                        '`deployment_id` is not correct and '
-                        '`reverse_id` is either not correct or provided'
+                        "Could not attach to the flow. "
+                        "`deployment_id` is not correct and "
+                        "`reverse_id` is either not correct or provided"
                     )
 
-        component: LoadedComponentSchema | None = self._state.space.get_parsed_component_by_reverse_id(
-            reverse_id=reverse_id
+        elif attach_to_last:
+            deployments = self._state.space.get_deployments_by_reverse_id(reverse_id=reverse_id, status=["started"])
+            if len(deployments) == 0:
+                raise ValueError(
+                    "You have not supplied deployment ID "
+                    "and no deployments are available at the moment"
+                )
+            self._state.aux.task_id = deployments[0].uid
+
+        component: LoadedComponentSchema | None = (
+            self._state.space.get_parsed_component_by_reverse_id(reverse_id=reverse_id)
         )
 
         if component is not None and component.flow is not None:
             self._state.flow = component.flow
             self._state.aux.flow_id = component.flow.uid
             self._state.components_alias = {
-                x.uid: x.alias
-                for x in component.flow.components
+                x.uid: x.alias for x in component.flow.components
             }
             successful |= True
             all_components = {x.uid for x in component.flow.components}
             prev_components = set.union(
-                set(),
-                *[{x.uid for x in y.prev}
-                 for y in component.flow.components]
+                set(), *[{x.uid for x in y.prev} for y in component.flow.components]
             )
             leaves = all_components.difference(prev_components)
             # NOTE: there can be more leaves in future
             leave_aliasses = [
-                x.alias
-                for x in component.flow.components
-                if x.uid in (leaves)
+                x.alias for x in component.flow.components if x.uid in (leaves)
             ]
 
-            leaf_nodes = [
-                tracedLike(BaseNode(alias=x))
-                for x in leave_aliasses
-            ]
+            leaf_nodes = [tracedLike(BaseNode(alias=x)) for x in leave_aliasses]
 
         else:
             raise Exception(
-                'Could not attach to the flow. Component failed to be parsed.'
+                "Could not attach to the flow. Component failed to be parsed."
             )
 
         if not successful:
             raise Exception(
                 "Failed to attach to the task. Possible reasons are: "
                 "could not find neither component nor deployment."
             )
 
-        task = SpaceTask(
-            state=self._state,
-            component=component
-        )
+        task = SpaceTask(state=self._state, component=component)
 
         task.commit_returned(leaf_nodes)
         return task
```

### Comparing `malevich-0.2.6/malevich/manifest.py` & `malevich-0.4.0/malevich/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import deepcopy
 from typing import Any, Iterable, Optional
 
 import pydantic_yaml as pydml
 
 from ._utility.singleton import SingletonMeta
 from .models.manifest import Manifest, Secret, Secrets
+from .path import Paths
 
 
 class OverrideManifest:
     def __init__(self, path: str) -> None:
         self._path = path
         self._backup_path = getattr(ManifestManager(), "_ManifestManager__path")
         self._backup_secrets_path = getattr(
@@ -42,29 +43,51 @@
     def secret_pattern() -> str:
         return r"secret#[0-9]{1,6}"
 
     @staticmethod
     def is_secret(value: str) -> bool:
         return re.match(ManifestManager.secret_pattern(), str(value)) is not None
 
+    @staticmethod
+    def create_manifest() -> None:
+        pydml.to_yaml_file(Paths.pwd('malevich.yaml'), Manifest())
+        pydml.to_yaml_file(Paths.pwd('malevich.secrets.yaml'), Secrets())
+
+    @property
+    def path(self) -> str:
+        return '' + self.__path
+
     def __init__(self, workdir: str | None = None) -> None:
+        if os.path.exists(Paths.pwd('malevich.yaml')):
+            self.__path = Paths.pwd('malevich.yaml')
+            self.__secrets_path = Paths.pwd('malevich.secrets.yaml')
+            self.local = True
+        else:
+            self.__path = Paths.home('malevich.yaml', create=True)
+            self.__secrets_path = Paths.home('malevich.secrets.yaml', create=True)
+            self.local = False
+
         if workdir is None:
             workdir = os.getcwd()
 
-        self.__path = os.path.join(workdir, "malevich.yaml")
-        self.__secrets_path = os.path.join(workdir, "malevich.secrets.yaml")
-        if not os.path.exists(self.__path):
-            pydml.to_yaml_file(self.__path, Manifest())
-        if not os.path.exists(self.__secrets_path):
-            pydml.to_yaml_file(self.__secrets_path, Secrets())
-        with open(self.__path) as _file:
+        with open(self.__path, 'r+') as _file:
+            if os.path.getsize(self.__path) == 0:
+                _file.write('{}')
+                _file.seek(0)
             self.__manifest = pydml.parse_yaml_file_as(Manifest, _file)
             self.__backup = self.__manifest.model_dump()
+
+        with open(self.__secrets_path, 'r+') as _file:
+            if os.path.getsize(self.__secrets_path) == 0:
+                _file.write('{}')
+                _file.seek(0)
+
             self.__secrets = pydml.parse_yaml_file_as(
-                Secrets, self.__secrets_path)
+                Secrets, _file
+            )
 
     def cleanup_secrets(self) -> list[Secret]:
         secrets = re.findall(
             r"secret#[0-9]{1,6}", self.__manifest.model_dump_json(indent=4)
         )
         cleaned_secrets = Secrets(
             secrets={
@@ -304,9 +327,11 @@
                     break
         else:
             cursor.pop(key)
         self.__manifest = Manifest(**dump)
         self.save()
         return self.__manifest
 
-
-manf = ManifestManager()
+try:
+    manf = ManifestManager()
+except FileNotFoundError:
+    manf = None
```

### Comparing `malevich-0.2.6/malevich/models/argument.py` & `malevich-0.4.0/malevich/models/argument.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/collection.py` & `malevich-0.4.0/malevich/models/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/dependency.py` & `malevich-0.4.0/malevich/models/dependency.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/flow_function.py` & `malevich-0.4.0/malevich/models/flow_function.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/injections.py` & `malevich-0.4.0/malevich/models/injections.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/installers/compat.py` & `malevich-0.4.0/malevich/models/installers/compat.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/installers/image.py` & `malevich-0.4.0/malevich/models/installers/image.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/installers/space.py` & `malevich-0.4.0/malevich/models/installers/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/manifest.py` & `malevich-0.4.0/malevich/models/manifest.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/nodes/asset.py` & `malevich-0.4.0/malevich/models/nodes/asset.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/nodes/base.py` & `malevich-0.4.0/malevich/models/nodes/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/nodes/collection.py` & `malevich-0.4.0/malevich/models/nodes/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/nodes/operation.py` & `malevich-0.4.0/malevich/models/nodes/operation.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/nodes/tree.py` & `malevich-0.4.0/malevich/models/nodes/tree.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/preferences.py` & `malevich-0.4.0/malevich/models/preferences.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/registry/core_entry.py` & `malevich-0.4.0/malevich/models/registry/core_entry.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/results/base.py` & `malevich-0.4.0/malevich/models/results/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/results/core/result.py` & `malevich-0.4.0/malevich/models/results/core/result.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/results/space/collection.py` & `malevich-0.4.0/malevich/models/results/space/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/models/state/core.py` & `malevich-0.4.0/malevich/models/state/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,12 +60,14 @@
         # Results
         self.results: dict[str, str] = {}
         # Interpretation ID
         self.interpretation_id: str = uuid.uuid4().hex
         # App args
         self.app_args: dict[str, Any] = {}
         # Collections
-        self.extra_colls: dict[str, dict[str, str]] = defaultdict(dict)
+        self.extra_colls: dict[str, dict[str, list]] = defaultdict(
+            lambda: defaultdict(list)
+        )
         # Alias to task id
         self.task_aliases: dict[str, str] = {}
         # Component
         self.component: ComponentSchema | None = None
```

### Comparing `malevich-0.2.6/malevich/models/state/space.py` & `malevich-0.4.0/malevich/models/state/space.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,28 +24,15 @@
 class SpaceAuxParams:
     task_id: str | None
     run_id: str | None
     core_task_id: str | None
     flow_id: str | None
     tree: TreeNode | None
 
-    # operation_id: str
-    # task_id: str
-    # core_host: str
-    # core_auth: tuple[str, str]
-    # base_config: core.Cfg
-    # base_config_id: str
-
     def __init__(self, **kwargs) -> None:
-        # self.operation_id = kwargs.get('operation_id', None)
-        # self.task_id = kwargs.get('task_id', None)
-        # self.core_host = kwargs.get('core_host', None)
-        # self.core_auth = kwargs.get('core_auth', None)
-        # self.base_config = kwargs.get('base_config', None)
-        # self.base_config_id = kwargs.get('base_config_id', None)
         self.task_id = kwargs.get('task_id', None)
         self.run_id = kwargs.get('run_id', None)
         self.core_task_id = kwargs.get('core_task_id', None)
         self.flow_id = kwargs.get('flow_id', None)
         self.tree = kwargs.get('tree', None)
 
     def __getitem__(self, key: str) -> Any:  # noqa: ANN401
```

### Comparing `malevich-0.2.6/malevich/models/task/base.py` & `malevich-0.4.0/malevich/models/task/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import enum
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Generic, ParamSpec, TypeVar
+from typing import Any, Callable, Generic, Optional, ParamSpec, TypeVar
 
 from ..endpoint import MetaEndpoint
 
 # from ...interpreter.abstract import Interpreter
 from ..injections import BaseInjectable
 from ..nodes.tree import TreeNode
 from ..results import Result
@@ -147,15 +147,22 @@
 
     @abstractmethod
     def get_operations(self) -> list[str]:
         """Returns a operations within the task"""
         pass
 
     @abstractmethod
-    def configure(self, operation: str, **kwargs) -> None:
+    def configure(
+        self,
+        *operations: str,
+        # Configurable parameters
+        platform: str = 'base',
+        platform_settings: dict[str, Any] | None = None,
+        **kwargs
+    )-> None:
         """Configures a given operation within the task"""
         pass
 
     # Interpretation
     # ==============
     @abstractmethod
     def get_interpreted_task(self) -> BaseTask:
```

### Comparing `malevich-0.2.6/malevich/models/task/interpreted/core.py` & `malevich-0.4.0/malevich/models/task/interpreted/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,23 +131,48 @@
                 pass
 
         return CoreTaskStage.NO_TASK
 
     def get_stage_class(self) -> Type[CoreTaskStage]:
         pass
 
+    def _configure(
+        self,
+        operation: str,
+        # Configurable parameters
+        platform: str = 'base',
+        platform_settings: Optional[dict[str, Any]] = None,
+        # Rest of the parameters for compatibility
+        **kwargs
+    ) -> None:
+        """internal"""
+        assert platform in ['base', 'vast'], f"Platform {platform} is not supported. "
+        cout(
+            message=f"Configure {operation}: platform={platform}, platform_settings={platform_settings}",  # noqa: E501
+            action=Action.Interpretation,
+            verbosity=VerbosityLevel.OnlyStatus,
+        )
+        uuid_ = {
+            k.alias: k.uuid
+            for k in self.state.ops.values()
+        }[operation]
+
+        self.state.app_args[uuid_]['platform'] = platform
+        if platform_settings:
+            self.state.app_args[uuid_]['platform_settings'] = platform_settings
+
     def configure(
-            self,
-            operation: str,
-            # Configurable parameters
-            platform: str = 'base',
-            platform_settings: Optional[dict[str, Any]] = None,
-            # Rest of the parameters for compatibility
-            **kwargs
-        ) -> None:
+        self,
+        *operations: str,
+        # Configurable parameters
+        platform: str = 'base',
+        platform_settings: Optional[dict[str, Any]] = None,
+        # Rest of the parameters for compatibility
+        **kwargs
+    ) -> None:
         """Configures the operation on Malevich Core
 
         Available configurations
         ------------------------
 
         Platform
         ++++++++
@@ -157,25 +182,22 @@
         Malevich Core cluster. The `vast` platform is a on-demand GPU cluster that can
         be utilized for GPU-intensive operations.
 
         To configure the platform, use the `platform` parameter. The default value is
         `base`. To use the `vast` platform, set the value to `vast` and configure
         it with `malevich.core_api.vast_settings`.
         """
-        assert platform in [
-            'base', 'vast'], f"Platform {platform} is not supported. "
+        for o in operations:
+            self._configure(
+                o,
+                platform=platform,
+                platform_settings=platform_settings,
+                **kwargs
+            )
 
-        uuid_ = {
-            k.alias: k.uuid
-            for k in self.state.ops.values()
-        }[operation]
-
-        self.state.app_args[uuid_]['platform'] = platform
-        if platform_settings:
-            self.state.app_args[uuid_]['platform_settings'] = platform_settings
 
     def prepare(
         self,
         stage: PrepareStages = PrepareStages.ALL,
         *args,
         **kwargs
     ) -> None:
@@ -238,19 +260,19 @@
                     auth=self.state.params.core_auth,
                     conn_url=self.state.params.core_host,
                     *args,
                     **kwargs
                 ).operationId
             except (Exception, KeyboardInterrupt) as e:
                 # Cleanup
-                core.task_stop(
-                    self.state.params.task_id,
-                    auth=self.state.params.core_auth,
-                    conn_url=self.state.params.core_host,
-                )
+                # core.task_stop(
+                #     self.state.params.task_id,
+                #     auth=self.state.params.core_auth,
+                #     conn_url=self.state.params.core_host,
+                # )
                 raise e
 
         return self.state.params.task_id, self.state.params.operation_id
 
     def run(
         self,
         override: dict[str, pd.DataFrame] | None = None,
@@ -368,19 +390,19 @@
                     conn_url=self.state.params.core_host,
                     run_id=self.run_id,
                     wait=not detached,
                     **kwargs
                 )
         except (Exception, KeyboardInterrupt) as e:
             # Cleanup
-            core.task_stop(
-                self.state.params.operation_id,
-                auth=self.state.params.core_auth,
-                conn_url=self.state.params.core_host,
-            )
+            # core.task_stop(
+            #     self.state.params.operation_id,
+            #     auth=self.state.params.core_auth,
+            #     conn_url=self.state.params.core_host,
+            # )
             raise e
         return self.run_id
 
     def stop(
         self,
         *args,
         **kwargs
@@ -407,15 +429,15 @@
     def results(
         self,
         # returned: Iterable[traced[BaseNode]] | traced[BaseNode] | None,
         run_id: Optional[str] = None,
         # For compatibility with other interpreters
         *args,
         **kwargs
-    ) -> Iterable[CoreResult | CoreLocalDFResult]:
+    ) -> list[CoreResult | CoreLocalDFResult]:
         cout(message="Task results are being fetched from Core",
              action=Action.Results)
         if self.state.params.operation_id is None:
             raise Exception("Attempt to run a task which is not prepared. "
                             "Please, run `.prepare()` first.")
 
         returned = self._returned
@@ -595,15 +617,15 @@
         capture_results: list[str] | Literal['all'] | Literal['last'] = 'last',
         enable_not_auth: bool = True,
         hash: str | None = None,
         *args,
         **kwargs
     ) -> MetaEndpoint:
         from malevich_coretools import create_endpoint, update_endpoint
-        if self.get_stage() != CoreTaskStage.BUILT:
+        if self.get_stage() not in [CoreTaskStage.BUILT, CoreTaskStage.ONLINE]:
             self.prepare(stage=PrepareStages.BUILD)
 
         cfg = deepcopy(self.state.cfg)
         if capture_results == 'last':
             cfg.app_settings = [
                 x for x in cfg.app_settings
                 if x.taskId == self.state.params.task_id
```

### Comparing `malevich-0.2.6/malevich/models/task/interpreted/space.py` & `malevich-0.4.0/malevich/models/task/interpreted/space.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pickle
 import uuid
-import warnings
 from enum import Enum
 from functools import cache
-from typing import Iterable, Optional
+from typing import Callable, Iterable, Optional
 
 import pandas as pd
 from gql import gql
 from malevich_coretools.abstract.statuses import AppStatus, TaskStatus
 from malevich_space.schema import LoadedComponentSchema
 
 from malevich.models.injections import SpaceInjectable
@@ -16,14 +15,15 @@
 from ....interpreter.space import SpaceInterpreterState
 from ...nodes.base import BaseNode
 from ...nodes.tree import TreeNode
 from ...results.space.collection import SpaceCollectionResult
 from ...types import FlowOutput
 from ..base import BaseTask
 
+from malevich.core_api import BasePlatformSettings
 
 class SpaceTaskStage(Enum):
     INTERPRETED     = "interpreted"
     # from Space definition
     GENERATED       = "generated"
     STARTED         = "started"
     STOPPED         = "stopped"
@@ -35,22 +35,35 @@
     def load(object_bytes) -> 'SpaceTask':
         return pickle.loads(object_bytes)
 
     @property
     def tree(self) -> TreeNode:
         return self.state.aux.tree
 
+    @property
+    def component(self) -> LoadedComponentSchema:
+        self.upload()
+        return self._component
+
+    @property
+    def allow_configurations(self) -> bool:
+        return self._component is None
+
     def __init__(
         self,
         state: SpaceInterpreterState,
-        component: LoadedComponentSchema
+        component: LoadedComponentSchema | None = None,
+        get_component: Callable[..., LoadedComponentSchema] | None = None,
     ) -> None:
         super().__init__()
+        assert component is not None or get_component is not None
+
         self.state = state
-        self.component = component
+        self._component = component
+        self.__get_component = get_component
         self._returned = []
 
     def _deflate(
         self,
         returned: list[traced[BaseNode]],
         alias2infid: dict[str, str]
     ) -> tuple[list[str], list[str]]:
@@ -169,17 +182,34 @@
 
         self.state.aux.run_id = self.state.space.run_task(
             task_id=self.state.aux.task_id,
             ca_override=overrides
         )
         return self.state.aux.run_id
 
-    def configure(self, operation: str, **kwargs) -> None:
-        # NOTE: Nothing to tweak
-        return None
+    def configure(
+        self,
+        *operations: str,
+        # Configurable parameters
+        platform: str = 'base',
+        platform_settings: BasePlatformSettings | str = None,
+        # Rest of the parameters for compatibility
+        **kwargs
+    ) -> None:
+        if not self.allow_configurations:
+            raise Exception(
+                "Intepreter already uploaded a new component to Malevich Space, so "
+                "configurations are not available. To configure the task, use "
+                "`Space(configurable=True)` and call `upload()` afterwards to apply "
+                "custom configurations"
+            )
+        for operation in operations:
+            for component in self.state.flow.components:
+                if component.alias == operation:
+                    component.limits = platform_settings
 
     def get_interpreted_task(self) -> BaseTask:
         return self
 
     def get_stage(self) -> SpaceTaskStage:
         if not self.state.aux.task_id:
             return SpaceTaskStage.INTERPRETED
@@ -254,14 +284,15 @@
 
     def commit_returned(self, returned: FlowOutput) -> None:
         self._returned = returned
 
     async def __async_get_results(
         self,
         run_id: Optional[str] = None,
+        fetch_timeout: int = 150,
         *args,
         **kwargs
     ) -> Iterable[SpaceCollectionResult]:
         """internal"""
         returned = self._returned
         if returned is None:
             return None
@@ -294,15 +325,16 @@
         exc_message = None
         if rs_ != AppStatus.COMPLETE.value:
             finished_ = {
                 x.in_flow_comp_id for x in cs_ if x.status == AppStatus.COMPLETE.value
             }
             to_be_finished_ = set(infid_)
             async for update in self.state.space.subscribe_to_status(
-                run_id or self.state.aux.run_id
+                run_id or self.state.aux.run_id,
+                fetch_timeout
             ):
                 if isinstance(update, str):
                     if update == TaskStatus.COMPLETE.value:
                         break
                     if update == TaskStatus.FAIL.value:
                         exc_message = "Run failed. No results could be fetched..."
                         break
@@ -326,38 +358,41 @@
             SpaceCollectionResult(
                 run_id=run_id or self.state.aux.run_id,
                 in_flow_id=i,
                 space_ops=self.state.space
             ) for i in infid_
         ]
 
-
     def results(
         self,
         run_id: Optional[str] = None,
+        fetch_timeout: int = 150,
         *args,
         **kwargs
     ) -> list[SpaceCollectionResult]:
         import asyncio
-        import warnings
 
         try:
+            import warnings
             with warnings.catch_warnings():
                 warnings.filterwarnings(
                     "ignore", message="There is no current event loop"
                 )
                 loop = asyncio.get_event_loop()
         except RuntimeError:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
 
-        def raise_exc(e) -> None:
+        def raise_exc(e, *args) -> None:
             raise e
 
         loop.set_exception_handler(raise_exc)
         return loop.run_until_complete(self.__async_get_results(
             run_id,
             *args,
             **kwargs
         ))
 
+    def upload(self) -> None:
+        if not self._component:
+            self._component = self.__get_component()
```

### Comparing `malevich-0.2.6/malevich/models/task/promised.py` & `malevich-0.4.0/malevich/models/task/promised.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         tree: TreeNode,
         component: ComponentSchema
     ) -> None:
         self.__results = results
         self.__tree = tree
         self.__task = None
         self.__conf_memory = []
-        self.__component = component
+        self._component = component
 
     @property
     def tree(self) -> TreeNode:
         return self.__tree
 
     def _attach_task(self, _task: BaseTask) -> None:
         self.__task = _task
@@ -90,15 +90,15 @@
         Args:
             interpreter (:class:`malevich.interpreter.Interpreter`, optional):
                 Interpreter to use. :class:`malevich.interprete.SpaceInterpreter`
                 is used when not specified. Defaults to None.
         """
         __interpreter = interpreter or SpaceInterpreter()
         try:
-            task = __interpreter.interpret(self.__tree, self.__component)
+            task = __interpreter.interpret(self.__tree, self._component)
             if self.__results:
                 task.commit_returned(self.__results)
             self.__task = task
             # Apply the configuration that was stored in memory
             for operation, kwargs in self.__conf_memory:
                 self.__task.configure(operation, **kwargs)
             del self.__conf_memory
@@ -241,28 +241,28 @@
 
     def dump(self) -> bytes:
         """Serialize the task to bytes, which can be saved and used to load it again"""
         if self.__task:
             task_bytes_ = self.__task.dump()
         else:
             task_bytes_ = b""
-        tree_bytes_ = pickle.dumps(self.__tree)
+        tree_bytes_ = pickle.dumps(self.__tree.model_dump())
         results_bytes_ = pickle.dumps(self.__results)
-        component_bytes_ = pickle.dumps(self.__component)
+        component_bytes_ = pickle.dumps(self._component)
         return pickle.dumps(
             (task_bytes_, tree_bytes_, results_bytes_, component_bytes_)
         )
 
     @staticmethod
     def load(object_bytes: bytes) -> 'PromisedTask':
         """Static method. Deserialize bytes into task object"""
         task_bytes_, tree_bytes_, results_bytes_, component_bytes_ = pickle.loads(object_bytes)  # noqa: E501
         task = PromisedTask(
             results=pickle.loads(results_bytes_),
-            tree=pickle.loads(tree_bytes_),
+            tree=TreeNode(**pickle.loads(tree_bytes_)),
             component=pickle.loads(component_bytes_)
         )
         if len(task_bytes_) > 0:
             task._attach_task(pickle.loads(task_bytes_))
 
         return task
 
@@ -292,31 +292,32 @@
             raise Exception(
                 "Unable to get operations. "
                 "Please, use `.interpret` first to attach task to "
                 "a particular platform"
             )
         return self.__task.get_operations()
 
-    def configure(self, operation: str, **kwargs) -> None:
+    def configure(self, *operations: str, **kwargs) -> None:
         """Configures the task for a particular operation
 
         What is configurable and how it is configurable is defined by the
         interpreter used. See the documentation of the corresponding
         interpreter used before calling this method.
 
         Args:
             operation (str): Operation to configure (one from :meth:`get_operations`)
             **kwargs (Any): Arguments to configure the operation
         """
         if not self.__task:
+            for op in operations:
             # Remember the configuration to apply it later
-            self.__conf_memory.append((operation, kwargs))
+                self.__conf_memory.append((op, kwargs))
             return None
         # Otherwise proxy directly
-        return self.__task.configure(operation, **kwargs)
+        return self.__task.configure(*operations, **kwargs)
 
     def get_interpreted_task(self) -> BaseTask:
         """Retrieves the interpreted task that is produced when calling :meth:`interpret`
 
         Returns:
             :class:`BaseTask`: The interpreted task
         """  # noqa: E501
@@ -325,13 +326,23 @@
                 "Unable to get interpreted task. "
                 "Please, use `.interpret` first to attach task to "
                 "a particular platform"
             )
         return self.__task
 
     def publish(self, *args, **kwargs) -> MetaEndpoint:
+        """Creates a HTTP endpoint for the task
+
+        Accepts any arguments and keyword arguments and passes them to the
+        underlying callback created in the interpreter itself. For particular
+        arguments and keyword arguments, see the documentation of the interpreter
+        used before calling this method.
+
+        Returns:
+            :class:`malevich.models.endpoint.MetaEndpoint`: An endpoint object
+        """
         if not self.__task:
             raise Exception(
                 "Cannot publish uninterpreted task. "
                 "Use `.interpret()` first."
             )
         return self.__task.publish(*args, **kwargs)
```

### Comparing `malevich-0.2.6/malevich/models/task.py` & `malevich-0.4.0/malevich/models/task.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/path.py` & `malevich-0.4.0/malevich/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 import sys
+from pathlib import Path as _Path
 
 MALEVICH_HOME = os.getenv("MALEVICH_HOME", os.path.expanduser('~/.malevich/'))
 MALEVICH_CACHE =  os.path.expanduser(os.getenv("MALEVICH_CACHE", '~/.malevich/cache'))
 DB_PATH = '.db'
 
 class Paths:
     @staticmethod
     def home(*path, create: bool = False, create_dir: bool = False) -> str:
         path = list(path)
         if create:
             os.makedirs(os.path.join(MALEVICH_HOME, *path[:-1]), exist_ok=True)
+            _Path(os.path.join(MALEVICH_HOME, *path)).touch()
         if create_dir:
             os.makedirs(
-                os.path.dirname(os.path.join(MALEVICH_HOME, *path)),
+                os.path.join(MALEVICH_HOME, *path),
                 exist_ok=True
             )
         return os.path.join(MALEVICH_HOME, *path)
 
     @staticmethod
     def cache(*path) -> str:
         return os.path.join(MALEVICH_CACHE, *path)
@@ -28,9 +30,9 @@
 
     @staticmethod
     def module(*path) -> str:
         return os.path.join(os.path.dirname(sys.modules['malevich'].__file__), *path)
 
     @staticmethod
     def db() -> str:
-        return Paths.home(DB_PATH, create=True)
+        return Paths.home(DB_PATH)
```

### Comparing `malevich-0.2.6/malevich/runners/base.py` & `malevich-0.4.0/malevich/runners/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/square/df.py` & `malevich-0.4.0/malevich/square/df.py`

 * *Files identical despite different names*

### Comparing `malevich-0.2.6/malevich/square/jls.py` & `malevich-0.4.0/malevich/square/jls.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return wrapper
 
 
 def processor(id: Optional[str] = None, finish_msg: Optional[str] = None, drop_internal: bool = True, get_scale_part_all: bool = False):    # noqa: ANN201, E501
     """Denotes a processor of the app.
     
     Processors are core logical units of the app. To
-    understand processors more, see `What is Processor? <../Apps/What_is_Processor.html>`_
+    understand processors more, see :doc:`What is Processor? </SDK/Apps/Processors>`
     
     Args:
         id: The id of the processor. If not provided, the name of the function will be used.
         finish_msg: The message to be sent to e-mail (if configured) when the processor finishes.
         drop_internal: Whether to drop the internal collections after the processor finishes.
         get_scale_part_all: Whether to get the scale part of the input collection.
```

### Comparing `malevich-0.2.6/malevich/square/utils.py` & `malevich-0.4.0/malevich/square/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,15 +584,14 @@
         paths: List[str],
         all_runs: bool = False,
         path_prefix: str = APP_DIR,
         force: bool = False,
         synchronize: bool = True
     ) -> None:
         """Shares multiple files or directories.
-
         The same as :meth:`async_share`, but for multiple files or directories.
         Ignores paths that do not exist.
         """
 
     def get_share_path(
         self,
         path: str,
@@ -819,24 +818,22 @@
             OBJ: OBJ with created directory captured
         """ # noqa: E501
         pass
 
 
 def to_binary(smth: Any) -> bytes:  # noqa: ANN401
     """Converts object to binary
-
     Args:
         smth (Any): object to convert
     """
     return pickle.dumps(smth)
 
 
 def from_binary(smth: bytes) -> Any:
     """Converts binary to object
-
     Args:
         smth (bytes): binary to convert
     """
     return pickle.loads(smth)
 
 
 def load(url: str, path: str, path_prefix: str = APP_DIR) -> None:
@@ -924,15 +921,14 @@
         """  # noqa: E501
         pass
 
 
 class SmtpSender:
     """
     Ready-made auxiliary wrapper for interacting with SMTP
-
     Args:
         login (str): login
         password (str): password
         smtp_server (str, optional): smtp server. Defaults to "smtp.gmail.com".
         smtp_port (int, optional): smtp port. Defaults to 465.
     """
 
@@ -1108,15 +1104,14 @@
         _out.append(_t)
 
     return _out
 
 
 def to_df(x: Any, force: bool = False) -> pd.DataFrame:
     """Creates a data frame from an arbitrary object
-
     - `torch.Tensor`: Tensor is serialized using torch.save and then encoded using base112. Autograd information is preserved.
     - `numpy`, `list`, `tuple`, `range`, `bytearray`: Data is serialized using pickle and stored as is in `data` column.
     - `set`, `frozenset`: Data is converted to list and stored as is in `data` column.
     - `dict`: Data is serialized using json and stored as is in `data` column.
     - `int`, float, complex, str, bytes, bool: Data is stored as is in `data` column.
```

### Comparing `malevich-0.2.6/malevich/testing/env.py` & `malevich-0.4.0/malevich/testing/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 
 from malevich._utility.package import package_manager as pm
 from malevich._utility.singleton import SingletonMeta
+from malevich.constants import TEST_DIR
 from malevich.install.image import ImageInstaller
 from malevich.install.installer import Installer
 from malevich.install.space import SpaceInstaller
 from malevich.manifest import OverrideManifest, manf
 from malevich.models.dependency import Dependency
-from malevich.path import Paths
+from malevich.models.installers.compat import CompatabilityStrategy
+from malevich.models.preferences import (
+    Action,
+    LogFormat,
+    UserPreferences,
+    VerbosityLevel,
+)
 
-from ..models.installers.compat import CompatabilityStrategy
-from ..models.preferences import Action, LogFormat, UserPreferences, VerbosityLevel
-
-test_manifest = OverrideManifest(Paths.home("testing", create=True))
+test_manifest = OverrideManifest(TEST_DIR)
 
 class EnvManager(metaclass=SingletonMeta):
     """Efficient environment manager
 
     Provides optimized and flexible way for installing,
     tracking and removing environments for testing.
     """
@@ -113,15 +117,12 @@
                     manf.remove('dependencies', dependency.package_id)
                     restored = (
                         self.installers[dependency.installer].restore(dependency).model_dump()
                     )
 
                     manf.put(
                         'dependencies',
-                        value={
-                            dependency.package_id:
-                            restored
-                        },
-                        append=True
+                        dependency.package_id,
+                        value=restored,
                     )
 
         return self.get_current_env()
```

### Comparing `malevich-0.2.6/malevich/testing/suite.py` & `malevich-0.4.0/malevich/testing/suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import os
 import sys
 from typing import Any, Type
 
 from pydantic import BaseModel
 from pytest import fixture
 
-from ..interpreter.abstract import Interpreter
-from ..models.flow_function import FlowFunction
-from ..models.installers.image import ImageDependency
-from ..models.installers.space import SpaceDependency
-from ..models.results.base import BaseResult
-from ..models.task.promised import PromisedTask
-from .env import EnvManager, test_manifest
+from malevich.constants import TEST_DIR
+from malevich.interpreter.abstract import Interpreter
+from malevich.manifest import OverrideManifest
+from malevich.models.flow_function import FlowFunction
+from malevich.models.installers.image import ImageDependency
+from malevich.models.installers.space import SpaceDependency
+from malevich.models.results.base import BaseResult
+from malevich.models.task.interpreted.space import SpaceTask
+from malevich.models.task.promised import PromisedTask
+
+from .env import EnvManager
 
 env_manager = EnvManager()
+manifest_override = OverrideManifest(TEST_DIR)
 
 @fixture(autouse=True, scope='session')
 def clean_env() -> None:
     global env_manager
-    env_manager.clean_env()
+    # env_manager.clean_env()
 
 class FlowTestEnv(BaseModel):
     dependencies: dict[str, ImageDependency | SpaceDependency] = []
     env_vars: dict[str, str] = {}
 
 
 class FlowTestSuite:
@@ -33,15 +38,15 @@
     prepare_kwargs: dict[str, Any] = {}
     run_args: list[Any] = []
     run_kwargs: dict[str, Any] = {}
     result_kwargs: dict[str, Any] = {}
     interpreter: Interpreter = None
 
     @staticmethod
-    def __offload_modules(stubs):
+    def __offload_modules(stubs) -> None:
         packages = ['malevich.' + x[0] for x in stubs]
         for package in packages:
             for module in [*sys.modules.keys()]:
                 if package in module:
                     sys.modules.pop(module)
 
 
@@ -83,30 +88,35 @@
 
     @staticmethod
     def on_result_error(flow: FlowFunction, error: Exception) -> Exception | None:
         return error
 
     @classmethod
     def test_flow(cls: Type['FlowTestSuite']) -> None:
-        old_stubs, _ = env_manager.get_current_env()
+        old_stubs, _ = env_manager.current_env()
         cls.__offload_modules(old_stubs)
-        stubs, _ = env_manager.request_env([*cls.environment.dependencies.values()])
+        env_manager.request_env([*cls.environment.dependencies.values()])
+        stubs, _ = env_manager.current_env()
         for k, v in cls.environment.env_vars.items():
             os.environ[k] = v
         cls.__offload_modules(stubs)
-        with test_manifest:
-            for attr in dir(cls):
-                f = getattr(cls, attr)
-                if isinstance(f, FlowFunction):
+        for attr in dir(cls):
+            f = getattr(cls, attr)
+            if isinstance(f, FlowFunction):
+                with manifest_override:
                     task: PromisedTask = f(
                         *cls.func_args,
                         **cls.func_kwargs
                     )
                     try:
                         task.interpret(cls.interpreter)
+                        if isinstance(t := task.get_interpreted_task(), SpaceTask):
+                            # FIXME: local fix for upload, remove later
+                            print("UPLOADING")
+                            t.upload()
                         cls.on_interpretation(task)
                     except Exception as e:
                         if e_ := cls.on_interpretation_error(task, e):
                             raise e_
                     if not isinstance(task, PromisedTask):
                         raise TypeError(
                             f"FlowFunction {f} did not return a PromisedTask"
```

### Comparing `malevich-0.2.6/malevich.egg-info/PKG-INFO` & `malevich-0.4.0/malevich.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: malevich
-Version: 0.2.6
+Version: 0.4.0
 Summary: ('A user-friendly interface to communicate with Malevich AI (malevich.ai)',)
 License-File: LICENSE
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: pydantic>=2.0.0
-Requires-Dist: malevich-coretools>=0.3.8
-Requires-Dist: malevich-space>=0.4.10
+Requires-Dist: malevich-coretools>=0.3.11
+Requires-Dist: malevich-space>=0.4.24
 Requires-Dist: pandas
 Requires-Dist: pydantic-yaml
 Requires-Dist: PyGithub
 Requires-Dist: GitPython
 Requires-Dist: randomname
 Requires-Dist: botocore
 Requires-Dist: boto3
@@ -19,7 +19,9 @@
 Requires-Dist: jsonpickle
 Requires-Dist: python-dotenv
 Requires-Dist: kafka-python
 Requires-Dist: deprecated
 Requires-Dist: datamodel-code-generator
 Requires-Dist: ruff
 Requires-Dist: duckdb
+Requires-Dist: duckdb-engine
+Requires-Dist: humanfriendly
```

### Comparing `malevich-0.2.6/malevich.egg-info/SOURCES.txt` & `malevich-0.4.0/malevich.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 requirements.txt
 setup.py
 ./.pre-commit-config.yaml
 ./.github/workflows/docs.yaml
 ./.github/workflows/pypi.yaml
 ./.github/workflows/pytest.yaml
 ./.github/workflows/ruff.yaml
+./malevich/_templates/Dockerfile.app
+./malevich/_templates/README.app.md
+./malevich/_templates/flow.py.txt
+./malevich/_templates/processor.py.txt
+./malevich/_templates/space.yaml.txt
 ./malevich/_utility/ci/templates/malevich-ci-manual.yml
 ./malevich/_utility/ci/templates/malevich-ci.yml
 malevich/__init__.py
+malevich/_deploy.py
 malevich/annotations.py
 malevich/cli.py
 malevich/constants.py
 malevich/core_api.py
 malevich/help.py
 malevich/manifest.py
 malevich/path.py
@@ -30,57 +36,69 @@
 malevich/_autoflow/flow.py
 malevich/_autoflow/function.py
 malevich/_autoflow/tracer.py
 malevich/_autoflow/tree.py
 malevich/_cli/__init__.py
 malevich/_cli/ci.py
 malevich/_cli/flow.py
+malevich/_cli/init.py
 malevich/_cli/install.py
 malevich/_cli/list.py
 malevich/_cli/manifest.py
 malevich/_cli/new.py
 malevich/_cli/prefs.py
 malevich/_cli/remove.py
 malevich/_cli/restore.py
 malevich/_cli/use.py
 malevich/_cli/core/app.py
+malevich/_cli/core/assets.py
 malevich/_cli/core/endpoints.py
+malevich/_cli/core/limits.py
 malevich/_cli/dev/__init__.py
 malevich/_cli/dev/dev.py
 malevich/_cli/misc/__init__.py
 malevich/_cli/misc/make.py
 malevich/_cli/misc/manifest_to_env.py
 malevich/_cli/space/init.py
 malevich/_cli/space/login.py
+malevich/_cli/space/whoami.py
 malevich/_core/__init__.py
 malevich/_core/ops.py
 malevich/_core/scan.py
 malevich/_db/__init__.py
 malevich/_db/local.py
+malevich/_db/functions/__init__.py
+malevich/_db/functions/credentials.py
+malevich/_db/functions/get_db.py
+malevich/_db/schema/__init__.py
+malevich/_db/schema/base.py
+malevich/_db/schema/core_creds.py
+malevich/_db/schema/creds.py
+malevich/_export/__init__.py
+malevich/_export/space_flow.py
 malevich/_meta/__init__.py
 malevich/_meta/asset.py
 malevich/_meta/collection.py
 malevich/_meta/config.py
 malevich/_meta/decor.py
 malevich/_meta/flow.py
 malevich/_meta/run.py
 malevich/_meta/table.py
 malevich/_templates/Dockerfile.app
 malevich/_templates/README.app.md
 malevich/_templates/flow.py.txt
 malevich/_templates/processor.py.txt
 malevich/_templates/space.yaml.txt
 malevich/_utility/__init__.py
+malevich/_utility/_try.py
 malevich/_utility/args.py
 malevich/_utility/dicts.py
 malevich/_utility/host.py
-malevich/_utility/letterhash.py
 malevich/_utility/logging.py
 malevich/_utility/package.py
-malevich/_utility/print.py
 malevich/_utility/registry.py
 malevich/_utility/scan.py
 malevich/_utility/schema.py
 malevich/_utility/singleton.py
 malevich/_utility/stub.py
 malevich/_utility/tree.py
 malevich/_utility/cache/__init__.py
@@ -98,34 +116,37 @@
 malevich/_utility/space/space.py
 malevich/_utility/summary/__init__.py
 malevich/_utility/summary/abstract.py
 malevich/_utility/summary/time.py
 malevich/install/__init__.py
 malevich/install/image.py
 malevich/install/installer.py
+malevich/install/iso.py
 malevich/install/space.py
 malevich/install/stub.py
 malevich/interpreter/__init__.py
 malevich/interpreter/abstract.py
 malevich/interpreter/core.py
 malevich/interpreter/space.py
 malevich/models/__init__.py
+malevich/models/_model.py
 malevich/models/actions.py
 malevich/models/argument.py
 malevich/models/collection.py
 malevich/models/dependency.py
 malevich/models/endpoint.py
 malevich/models/exceptions.py
 malevich/models/flow_function.py
 malevich/models/in_app_core_info.py
 malevich/models/injections.py
 malevich/models/manifest.py
 malevich/models/platform.py
 malevich/models/preferences.py
 malevich/models/task.py
+malevich/models/type_annotations.py
 malevich/models/types.py
 malevich/models/verdict.py
 malevich/models/installers/__init__.py
 malevich/models/installers/compat.py
 malevich/models/installers/image.py
 malevich/models/installers/space.py
 malevich/models/nodes/__init__.py
@@ -156,8 +177,11 @@
 malevich/square/__init__.py
 malevich/square/defaults.py
 malevich/square/df.py
 malevich/square/jls.py
 malevich/square/utils.py
 malevich/testing/__init__.py
 malevich/testing/env.py
-malevich/testing/suite.py
+malevich/testing/fixtures.py
+malevich/testing/suite.py
+malevich/testing/testcase.py
+malevich/testing/env/__init__.py
```

