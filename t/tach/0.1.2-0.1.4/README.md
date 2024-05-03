# Comparing `tmp/tach-0.1.2.tar.gz` & `tmp/tach-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.2.tar", last modified: Wed May  1 17:02:41 2024, max compression
+gzip compressed data, was "tach-0.1.4.tar", last modified: Fri May  3 01:18:31 2024, max compression
```

## Comparing `tach-0.1.2.tar` & `tach-0.1.4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.178931 tach-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.182931 tach-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 17:02:36.000000 tach-0.1.2/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-01 17:02:36.000000 tach-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 17:02:36.000000 tach-0.1.2/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 17:02:36.000000 tach-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-01 17:02:41.198931 tach-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-01 17:02:36.000000 tach-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 17:02:36.000000 tach-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-01 17:02:36.000000 tach-0.1.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 17:02:36.000000 tach-0.1.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-01 17:02:36.000000 tach-0.1.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 17:02:36.000000 tach-0.1.2/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 17:02:36.000000 tach-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-01 17:02:36.000000 tach-0.1.2/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 17:02:36.000000 tach-0.1.2/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-01 17:02:36.000000 tach-0.1.2/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-01 17:02:36.000000 tach-0.1.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-01 17:02:36.000000 tach-0.1.2/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-01 17:02:36.000000 tach-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-01 17:02:36.000000 tach-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:02:41.198931 tach-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-01 17:02:36.000000 tach-0.1.2/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-01 17:02:36.000000 tach-0.1.2/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-01 17:02:36.000000 tach-0.1.2/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 17:02:36.000000 tach-0.1.2/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.186931 tach-0.1.2/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 17:02:36.000000 tach-0.1.2/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:36.000000 tach-0.1.2/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 17:02:36.000000 tach-0.1.2/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 17:02:36.000000 tach-0.1.2/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-01 17:02:36.000000 tach-0.1.2/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-01 17:02:36.000000 tach-0.1.2/tach/hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-01 17:02:36.000000 tach-0.1.2/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 17:02:36.000000 tach-0.1.2/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 17:02:36.000000 tach-0.1.2/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.190930 tach-0.1.2/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-01 17:02:36.000000 tach-0.1.2/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 17:02:41.000000 tach-0.1.2/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-01 17:02:36.000000 tach-0.1.2/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.194930 tach-0.1.2/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:02:41.198931 tach-0.1.2/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 17:02:36.000000 tach-0.1.2/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:02:36.000000 tach-0.1.2/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.876860 tach-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.880860 tach-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-03 01:18:24.000000 tach-0.1.4/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-03 01:18:24.000000 tach-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 01:18:24.000000 tach-0.1.4/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-03 01:18:24.000000 tach-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-03 01:18:31.896860 tach-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-03 01:18:24.000000 tach-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 01:18:24.000000 tach-0.1.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-03 01:18:24.000000 tach-0.1.4/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-03 01:18:24.000000 tach-0.1.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-03 01:18:24.000000 tach-0.1.4/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 01:18:24.000000 tach-0.1.4/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 01:18:24.000000 tach-0.1.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-03 01:18:24.000000 tach-0.1.4/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-03 01:18:24.000000 tach-0.1.4/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-03 01:18:24.000000 tach-0.1.4/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-03 01:18:24.000000 tach-0.1.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 01:18:24.000000 tach-0.1.4/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-03 01:18:24.000000 tach-0.1.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-03 01:18:24.000000 tach-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 01:18:31.896860 tach-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-03 01:18:24.000000 tach-0.1.4/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-03 01:18:24.000000 tach-0.1.4/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-03 01:18:24.000000 tach-0.1.4/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.884860 tach-0.1.4/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 01:18:24.000000 tach-0.1.4/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 01:18:24.000000 tach-0.1.4/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 01:18:24.000000 tach-0.1.4/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 01:18:24.000000 tach-0.1.4/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:18:24.000000 tach-0.1.4/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-03 01:18:24.000000 tach-0.1.4/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.888860 tach-0.1.4/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-03 01:18:24.000000 tach-0.1.4/tach/hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-03 01:18:24.000000 tach-0.1.4/tach/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-03 01:18:24.000000 tach-0.1.4/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 01:18:24.000000 tach-0.1.4/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-03 01:18:24.000000 tach-0.1.4/tach/parsing/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 01:18:31.000000 tach-0.1.4/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 01:18:24.000000 tach-0.1.4/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.892860 tach-0.1.4/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:18:31.896860 tach-0.1.4/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-03 01:18:24.000000 tach-0.1.4/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_module_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:18:24.000000 tach-0.1.4/tests/test_show.py
```

### Comparing `tach-0.1.2/.github/workflows/ci.yml` & `tach-0.1.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,8 +47,8 @@
     - name: Check types with pyright
       run: |
         source .venv/bin/activate
         pyright .
     - name: Check tach
       run: |
         pip install .
-        tach check --exclude tests
+        tach check --exclude tests,build
```

### Comparing `tach-0.1.2/.github/workflows/publish.yml` & `tach-0.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/.github/workflows/publish_docs.yml` & `tach-0.1.4/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/.gitignore` & `tach-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/LICENSE` & `tach-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/PKG-INFO` & `tach-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,20 +73,23 @@
 # utils/package.yml
 tags: ["utils"]
 ```
 Next, specify the constraints for each tag in `tach.yml` in the root of your project:
 ```yaml
 # [root]/tach.yml
 constraints:
-  core:
-    depends_on: ["db", "utils"]
-  db:
-    depends_on: ["utils"]
-  utils:
-    depends_on: []
+- tag: core
+  depends_on:
+  - db
+  - utils
+- tag: db
+  depends_on:
+  - utils
+- tag: utils
+  depends_on: []
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
@@ -122,14 +125,19 @@
 
 If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
 ```bash
 tach add [file_or_path]
 ```
 This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
+
+### Pre-Commit Hook
+`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+
+
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
 ```
 This will stop `tach` from flagging this import as a boundary violation.
```

### Comparing `tach-0.1.2/README.md` & `tach-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,20 +44,23 @@
 # utils/package.yml
 tags: ["utils"]
 ```
 Next, specify the constraints for each tag in `tach.yml` in the root of your project:
 ```yaml
 # [root]/tach.yml
 constraints:
-  core:
-    depends_on: ["db", "utils"]
-  db:
-    depends_on: ["utils"]
-  utils:
-    depends_on: []
+- tag: core
+  depends_on:
+  - db
+  - utils
+- tag: db
+  depends_on:
+  - utils
+- tag: utils
+  depends_on: []
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
@@ -93,14 +96,19 @@
 
 If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
 ```bash
 tach add [file_or_path]
 ```
 This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
+
+### Pre-Commit Hook
+`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+
+
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
 ```
 This will stop `tach` from flagging this import as a boundary violation.
```

### Comparing `tach-0.1.2/docs/configuration.md` & `tach-0.1.4/docs/configuration.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,40 +7,47 @@
 ## `tach.yml`
 
 This is the project-level configuration file which should be in the root of your project.
 It accepts `exclude` and `constraints` as top-level keys.
 
 `exclude` accepts a list of directory patterns to exclude from checking.
 
-`constraints` defines the expected dependencies between tags in your project, and accepts dictionary of tags.
+`constraints` defines the expected dependencies between tags in your project, and accepts a list of constraints as shown below
 
 ```yaml
 constraints:
-  scope:filesystem:
-    depends_on:
-    - scope:utils
-  scope:parsing:
-    depends_on:
-    - scope:filesystem
-    - scope:utils
-  scope:root:
-    depends_on:
-    - scope:filesystem
-    - scope:parsing
-    - scope:utils
-ignore: ['tests', 'docs']
+- tag: scope:filesystem
+  depends_on:
+  - scope:utils
+- tag: scope:parsing
+  depends_on:
+  - scope:core
+  - scope:filesystem
+  - scope:utils
+- tag: scope:root
+  depends_on:
+  - scope:utils
+  - scope:core
+  - scope:filesystem
+  - scope:parsing
+exclude:
+- tests/
+- docs/
+- build/
+exclude_hidden_paths: true
+
 ```
 
 
 ## `package.yml`
 
 This is the package-level configuration file which should exist in each package in your project.
 It accepts `tags` and `strict` as top-level keys.
 
-`tags` accepts a list of string tags which map onto project-level `constraints`
+`tags` accepts a list of string tags which are checked against project-level `constraints`
 
 `strict` accepts a boolean which enables ['Strict Mode'](strict-mode.md) for the package.
 
 ```yaml
 tags: ['scope:utils']
 strict: true
 ```
```

### Comparing `tach-0.1.2/docs/faq.md` & `tach-0.1.4/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/favicon.ico` & `tach-0.1.4/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/getting-started.md` & `tach-0.1.4/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/index.md` & `tach-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/strict-mode.md` & `tach-0.1.4/docs/strict-mode.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 tags: ['parsing']
 ```
 
 
 ```yaml
 # tach.yml
 constraints:
-  parsing:
-    depends_on:
-    - core
+- tag: parsing
+  depends_on:
+  - core
 ```
 
 Then, in a file within the 'parsing' package, we may have:
 ```python
 from core.main import get_data  # This import fails
 
 get_data()
```

### Comparing `tach-0.1.2/docs/tach-ignore.md` & `tach-0.1.4/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/tach_demo.mp4` & `tach-0.1.4/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/usage.md` & `tach-0.1.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/docs/why-tach.md` & `tach-0.1.4/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/mkdocs.yml` & `tach-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/pyproject.toml` & `tach-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tach-0.1.2/tach/add.py` & `tach-0.1.4/tach/add.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 from datetime import datetime
 from typing import Iterable, Optional
 
-import yaml
 
 from tach import filesystem as fs
 from tach.check import check
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME, PACKAGE_FILE_NAME
-from tach.core import ScopeDependencyRules
 from tach.errors import TachError
 from tach.filesystem import canonical
-from tach.parsing import parse_project_config, parse_package_config
+from tach.parsing import (
+    parse_project_config,
+    parse_package_config,
+    dump_project_config_to_yaml,
+)
 
 init_content_template = """# Generated by tach on {timestamp}
 from .main import *
 """
 
 
 def build_init_content():
@@ -54,36 +56,31 @@
         fs.chdir(root)
         project_config = parse_project_config()
         check_errors = check(
             root,
             project_config=project_config,
             exclude_paths=project_config.exclude,
         )
-        # TODO: handle case where we pivoted a file in a strict package
         for error in check_errors:
             if error.is_tag_error:
                 invalid_tags = set(error.invalid_tags)
-                existing_dependencies = set(
-                    project_config.constraints.get(
-                        error.source_tag, ScopeDependencyRules(depends_on=[])
-                    ).depends_on
-                )
                 if error.source_tag in tags:
-                    # This is updating the config for a new tag
-                    project_config.constraints[error.source_tag] = ScopeDependencyRules(
-                        depends_on=list(existing_dependencies | invalid_tags)
+                    # A package with one of the added tags caused this error and should update its dependencies
+                    project_config.add_dependencies_to_tag(
+                        error.source_tag, error.invalid_tags
                     )
                 if invalid_tags & tags:
-                    # This is updating the config for an existing tag
-                    project_config.constraints[error.source_tag] = ScopeDependencyRules(
-                        depends_on=list(existing_dependencies | (invalid_tags & tags))
+                    # A package now depends on one of the added tags and should add the newly added tags
+                    # Note that we should leave pre-existing invalid tags
+                    project_config.add_dependencies_to_tag(
+                        error.source_tag, list(invalid_tags & tags)
                     )
 
         tach_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
-        tach_yml_content = yaml.dump(project_config.model_dump())
+        tach_yml_content = dump_project_config_to_yaml(project_config)
         fs.write_file(tach_yml_path, tach_yml_content)
 
         check_errors = check(
             root, project_config=project_config, exclude_paths=project_config.exclude
         )
         if check_errors:
             return (
```

### Comparing `tach-0.1.2/tach/check.py` & `tach-0.1.4/tach/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,15 @@
                 exception_message="Could not find config for packages."
             )
         )
     file_tags = file_nearest_package.config.tags
     import_tags = import_nearest_package.config.tags
 
     for file_tag in file_tags:
-        dependency_tags = (
-            project_config.constraints[file_tag].depends_on
-            if file_tag in project_config.constraints
-            else []
-        )
+        dependency_tags = project_config.dependencies_for_tag(file_tag)
         if any(
             any(
                 re.match(dependency_tag, import_tag)
                 for dependency_tag in dependency_tags
             )
             for import_tag in import_tags
         ):
```

### Comparing `tach-0.1.2/tach/cli.py` & `tach-0.1.4/tach/cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/core/package.py` & `tach-0.1.4/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/filesystem/__init__.py` & `tach-0.1.4/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/filesystem/install.py` & `tach-0.1.4/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/filesystem/project.py` & `tach-0.1.4/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/filesystem/service.py` & `tach-0.1.4/tach/filesystem/service.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/init.py` & `tach-0.1.4/tach/init.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from dataclasses import field, dataclass
 from typing import Optional
 
-import yaml
 
 from tach import errors
 from tach import filesystem as fs
 from tach.check import check
 from tach.colors import BCOLORS
 from tach.constants import PACKAGE_FILE_NAME, CONFIG_FILE_NAME
-from tach.core import ProjectConfig, ScopeDependencyRules
+from tach.core import ProjectConfig
+from tach.parsing import dump_project_config_to_yaml
 
 __package_yml_template = """tags: ['{dir_name}']\n"""
 
 
 @dataclass
 class PackageInitResult:
     package_paths: list[str] = field(default_factory=list)
@@ -57,25 +57,18 @@
 
     project_config = ProjectConfig()
     check_errors = check(
         root, project_config=project_config, exclude_paths=exclude_paths
     )
     for error in check_errors:
         if error.is_tag_error:
-            existing_dependencies = set(
-                project_config.constraints.get(
-                    error.source_tag, ScopeDependencyRules(depends_on=[])
-                ).depends_on
-            )
-            project_config.constraints[error.source_tag] = ScopeDependencyRules(
-                depends_on=list(existing_dependencies | set(error.invalid_tags))
-            )
+            project_config.add_dependencies_to_tag(error.source_tag, error.invalid_tags)
 
     tach_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
-    tach_yml_content = yaml.dump(project_config.model_dump())
+    tach_yml_content = dump_project_config_to_yaml(project_config)
     fs.write_file(tach_yml_path, tach_yml_content)
 
     check_errors = check(
         root, project_config=project_config, exclude_paths=exclude_paths
     )
     if check_errors:
         return InitRootResult(
```

### Comparing `tach-0.1.2/tach/loading.py` & `tach-0.1.4/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/parsing/imports.py` & `tach-0.1.4/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/parsing/interface.py` & `tach-0.1.4/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach/parsing/packages.py` & `tach-0.1.4/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tach.egg-info/PKG-INFO` & `tach-0.1.4/tach.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.2
+Version: 0.1.4
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -73,20 +73,23 @@
 # utils/package.yml
 tags: ["utils"]
 ```
 Next, specify the constraints for each tag in `tach.yml` in the root of your project:
 ```yaml
 # [root]/tach.yml
 constraints:
-  core:
-    depends_on: ["db", "utils"]
-  db:
-    depends_on: ["utils"]
-  utils:
-    depends_on: []
+- tag: core
+  depends_on:
+  - db
+  - utils
+- tag: db
+  depends_on:
+  - utils
+- tag: utils
+  depends_on: []
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
@@ -122,14 +125,19 @@
 
 If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
 ```bash
 tach add [file_or_path]
 ```
 This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
+
+### Pre-Commit Hook
+`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+
+
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
 ```
 This will stop `tach` from flagging this import as a boundary violation.
```

### Comparing `tach-0.1.2/tach.egg-info/SOURCES.txt` & `tach-0.1.4/tach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tests/test_add.py` & `tach-0.1.4/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tests/test_check.py` & `tach-0.1.4/tests/test_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pytest
 from tach.core import (
     PackageConfig,
     PackageTrie,
     PackageNode,
     ProjectConfig,
-    ScopeDependencyRules,
+    TagDependencyRules,
 )
 from tach.check import check_import
 
 
 @pytest.fixture
 def test_config() -> PackageConfig:
     return PackageConfig(tags=["test"], strict=False)
 
 
 @pytest.fixture
 def project_config() -> ProjectConfig:
     return ProjectConfig(
-        constraints={
-            "domain_one": ScopeDependencyRules(
-                depends_on=["domain_one", "domain_three"]
+        constraints=[
+            TagDependencyRules(
+                tag="domain_one", depends_on=["domain_one", "domain_three"]
             ),
-            "domain_two": ScopeDependencyRules(depends_on=["domain_one"]),
-            "domain_three": ScopeDependencyRules(depends_on=[]),
-        }
+            TagDependencyRules(tag="domain_two", depends_on=["domain_one"]),
+            TagDependencyRules(tag="domain_three", depends_on=[]),
+        ]
     )
 
 
 @pytest.fixture
 def package_trie() -> PackageTrie:
     return PackageTrie(
         root=PackageNode(
```

### Comparing `tach-0.1.2/tests/test_cli.py` & `tach-0.1.4/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import Mock
 import pytest
 
 from tach import cli
 from tach.check import ErrorInfo
 from tach.constants import CONFIG_FILE_NAME
-from tach.core import ProjectConfig, ScopeDependencyRules
+from tach.core import ProjectConfig, TagDependencyRules
 
 
 @pytest.fixture
 def mock_check(mocker) -> Mock:
     mock = Mock(return_value=[])  # default to a return with no errors
     mocker.patch("tach.cli.check", mock)
     return mock
@@ -36,15 +36,15 @@
     mocker.patch("tach.filesystem.project.os.path.exists", mock_path_exists)
 
 
 @pytest.fixture
 def mock_project_config(mocker) -> None:
     def mock_project_config() -> ProjectConfig:
         return ProjectConfig(
-            constraints={"mocked": ScopeDependencyRules(depends_on=["mocked"])}
+            constraints=[TagDependencyRules(tag="mocked", depends_on=["mocked"])]
         )
 
     mocker.patch("tach.cli.parse_project_config", mock_project_config)
 
 
 def test_execute_with_tach_yml(
     capfd, mock_path_exists, mock_check, mock_project_config
```

### Comparing `tach-0.1.2/tests/test_init.py` & `tach-0.1.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tests/test_module_trie.py` & `tach-0.1.4/tests/test_module_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.2/tests/test_parsing.py` & `tach-0.1.4/tests/test_parsing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 
 import pytest
 from pydantic import ValidationError
 
 from tach.check import check, ErrorInfo
-from tach.core.config import PackageConfig, ScopeDependencyRules, ProjectConfig
+from tach.core.config import PackageConfig, TagDependencyRules, ProjectConfig
 from tach.parsing.config import parse_project_config, parse_package_config
 from tach.filesystem import file_to_module_path
 from tach import filesystem as fs
 
 
 def test_file_to_mod_path():
     assert file_to_module_path("__init__.py") == ""
     assert file_to_module_path("domain_one/__init__.py") == "domain_one"
     assert file_to_module_path("domain_one/interface.py") == "domain_one.interface"
 
 
 def test_parse_valid_project_config():
     result = parse_project_config("example/valid/")
     assert result == ProjectConfig(
-        constraints={
-            "one": ScopeDependencyRules(depends_on=["two"]),
-            "two": ScopeDependencyRules(depends_on=["one"]),
-            "three": ScopeDependencyRules(depends_on=[]),
-        },
+        constraints=[
+            TagDependencyRules(tag="one", depends_on=["two"]),
+            TagDependencyRules(tag="two", depends_on=["one"]),
+            TagDependencyRules(tag="three", depends_on=[]),
+        ],
         exclude=["domain_thr.*"],
         exclude_hidden_paths=True,
     )
 
 
 def test_run_valid_project_config():
     current_dir = os.getcwd()
```

