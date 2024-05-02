# Comparing `tmp/ansible_dev_tools-24.4.5.tar.gz` & `tmp/ansible_dev_tools-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_dev_tools-24.4.5.tar", last modified: Wed May  1 18:08:29 2024, max compression
+gzip compressed data, was "ansible_dev_tools-24.5.0.tar", last modified: Thu May  2 22:22:11 2024, max compression
```

## Comparing `ansible_dev_tools-24.4.5.tar` & `ansible_dev_tools-24.5.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.119852 ansible_dev_tools-24.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.107852 ansible_dev_tools-24.4.5/.config/
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/requirements-docs.in
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/requirements-server.in
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/requirements-test.in
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.config/requirements.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.107852 ansible_dev_tools-24.4.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.107852 ansible_dev_tools-24.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.107852 ansible_dev_tools-24.4.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-01 18:08:29.119852 ansible_dev_tools-24.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.107852 ansible_dev_tools-24.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/contributor-guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.111852 ansible_dev_tools-24.4.5/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/media/ansible-lint.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/media/ansible-navigator-run.mp4
--rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/media/compress.sh
--rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/media/create-collection.mp4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.111852 ansible_dev_tools-24.4.5/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/building-collection.md
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/ci-setup.md
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/content-best-practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/content-release.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.111852 ansible_dev_tools-24.4.5/docs/user-guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/images/ci.png
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/images/release.png
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/docs/user-guide/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:08:29.119852 ansible_dev_tools-24.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.103852 ansible_dev_tools-24.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/src/ansible_dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.103852 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/data/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/data/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/server_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/src/ansible_dev_tools/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/subcommands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools/version_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 18:08:29.000000 ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:08:29.115852 ansible_dev_tools-24.4.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tests/integration/test_server_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-01 18:08:16.000000 ansible_dev_tools-24.4.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.760176 ansible_dev_tools-24.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.748176 ansible_dev_tools-24.5.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/requirements-docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/requirements-server.in
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/requirements-test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.config/requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.748176 ansible_dev_tools-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.748176 ansible_dev_tools-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.748176 ansible_dev_tools-24.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-02 22:22:11.760176 ansible_dev_tools-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.748176 ansible_dev_tools-24.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/contributor-guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.752176 ansible_dev_tools-24.5.0/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   351712 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/media/ansible-lint.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   185365 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/media/ansible-navigator-run.mp4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      136 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/media/compress.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   325589 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/media/create-collection.mp4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.752176 ansible_dev_tools-24.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/building-collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/ci-setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/content-best-practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/content-release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.752176 ansible_dev_tools-24.5.0/docs/user-guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    75270 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/images/ci.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/images/release.png
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/docs/user-guide/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:22:11.760176 ansible_dev_tools-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.744176 ansible_dev_tools-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/src/ansible_dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.744176 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/data/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/server_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/src/ansible_dev_tools/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/subcommands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools/version_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.760176 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 22:22:11.000000 ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:22:11.756176 ansible_dev_tools-24.5.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tests/integration/test_server_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-02 22:21:58.000000 ansible_dev_tools-24.5.0/tox.ini
```

### Comparing `ansible_dev_tools-24.4.5/.config/constraints.txt` & `ansible_dev_tools-24.5.0/.config/constraints.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # by the following command:
 #
 #    pip-compile --all-extras --no-annotate --output-file=.config/constraints.txt --strip-extras pyproject.toml
 #
 ansible-builder==3.0.1
 ansible-compat==4.1.11
 ansible-core==2.16.6
-ansible-creator==24.4.6
+ansible-creator==24.5.0
 ansible-dev-environment==24.4.3
 ansible-lint==24.2.3
 ansible-navigator==24.3.2
 ansible-runner==2.3.6
 ansible-sign==0.1.1
 asgiref==3.8.1
 attrs==23.2.0
```

### Comparing `ansible_dev_tools-24.4.5/.github/dependabot.yml` & `ansible_dev_tools-24.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/.github/workflows/release.yml` & `ansible_dev_tools-24.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/.github/workflows/tox.yml` & `ansible_dev_tools-24.5.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/.gitignore` & `ansible_dev_tools-24.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/.pre-commit-config.yaml` & `ansible_dev_tools-24.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/LICENSE` & `ansible_dev_tools-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/PKG-INFO` & `ansible_dev_tools-24.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.5
+Version: 24.5.0
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
```

### Comparing `ansible_dev_tools-24.4.5/README.md` & `ansible_dev_tools-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/cspell.config.yaml` & `ansible_dev_tools-24.5.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/contributor-guide.md` & `ansible_dev_tools-24.5.0/docs/contributor-guide.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/index.md` & `ansible_dev_tools-24.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/installation.md` & `ansible_dev_tools-24.5.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/media/ansible-lint.mp4` & `ansible_dev_tools-24.5.0/docs/media/ansible-lint.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/media/ansible-navigator-run.mp4` & `ansible_dev_tools-24.5.0/docs/media/ansible-navigator-run.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/media/create-collection.mp4` & `ansible_dev_tools-24.5.0/docs/media/create-collection.mp4`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/building-collection.md` & `ansible_dev_tools-24.5.0/docs/user-guide/building-collection.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/ci-setup.md` & `ansible_dev_tools-24.5.0/docs/user-guide/ci-setup.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/content-best-practices.md` & `ansible_dev_tools-24.5.0/docs/user-guide/content-best-practices.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/content-release.md` & `ansible_dev_tools-24.5.0/docs/user-guide/content-release.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/images/ci.png` & `ansible_dev_tools-24.5.0/docs/user-guide/images/ci.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/images/release.png` & `ansible_dev_tools-24.5.0/docs/user-guide/images/release.png`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/index.md` & `ansible_dev_tools-24.5.0/docs/user-guide/index.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/docs/user-guide/testing.md` & `ansible_dev_tools-24.5.0/docs/user-guide/testing.md`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/mkdocs.yml` & `ansible_dev_tools-24.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/pyproject.toml` & `ansible_dev_tools-24.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/arg_parser.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/arg_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/cli.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/creator.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/creator.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/resources/server/data/openapi.yaml` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/resources/server/data/openapi.yaml`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/server_utils.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/server_utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/subcommands/server.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/subcommands/server.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/utils.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools/version_builder.py` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools/version_builder.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/PKG-INFO` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-dev-tools
-Version: 24.4.5
+Version: 24.5.0
 Summary: Ansible Developtment Tools kit bundles all tools needed for content creation and testing.
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: GPL-3.0-only
 Project-URL: changelog, https://github.com/ansible/ansible-dev-tools/releases
 Project-URL: documentation, https://ansible.readthedocs.io/projects/dev-tools/
 Project-URL: homepage, https://github.com/ansible/ansible-dev-tools
```

### Comparing `ansible_dev_tools-24.4.5/src/ansible_dev_tools.egg-info/SOURCES.txt` & `ansible_dev_tools-24.5.0/src/ansible_dev_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/tests/integration/conftest.py` & `ansible_dev_tools-24.5.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/tests/integration/test_cli.py` & `ansible_dev_tools-24.5.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/tests/integration/test_server_creator.py` & `ansible_dev_tools-24.5.0/tests/integration/test_server_creator.py`

 * *Files identical despite different names*

### Comparing `ansible_dev_tools-24.4.5/tox.ini` & `ansible_dev_tools-24.5.0/tox.ini`

 * *Files identical despite different names*

