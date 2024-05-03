# Comparing `tmp/OZI-1.2.2.tar.gz` & `tmp/OZI-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.2.2.tar", last modified: Tue Apr 30 20:32:23 2024, max compression
+gzip compressed data, was "OZI-1.3.0.tar", last modified: Fri May  3 04:58:29 2024, max compression
```

## Comparing `OZI-1.2.2.tar` & `OZI-1.3.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:32:23.695530 OZI-1.2.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-30 20:26:34.000000 OZI-1.2.2/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-30 20:26:34.000000 OZI-1.2.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   289498 2024-04-30 20:26:34.000000 OZI-1.2.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-30 20:26:34.000000 OZI-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-30 20:32:23.695530 OZI-1.2.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-30 20:26:34.000000 OZI-1.2.2/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-30 20:26:34.000000 OZI-1.2.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-30 20:26:34.000000 OZI-1.2.2/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-30 20:26:34.000000 OZI-1.2.2/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10755 2024-04-30 20:26:34.000000 OZI-1.2.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-04-30 20:26:34.000000 OZI-1.2.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-30 20:26:34.000000 OZI-1.2.2/subprojects/blastpipe.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-30 20:26:34.000000 OZI-1.2.2/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-30 20:26:34.000000 OZI-1.2.2/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.324882 OZI-1.3.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.300882 OZI-1.3.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.296882 OZI-1.3.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.300882 OZI-1.3.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-05-03 04:53:10.000000 OZI-1.3.0/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-03 04:53:10.000000 OZI-1.3.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   293780 2024-05-03 04:53:10.000000 OZI-1.3.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-03 04:53:10.000000 OZI-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-03 04:58:29.100881 OZI-1.3.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-03 04:53:10.000000 OZI-1.3.0/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-05-03 04:53:10.000000 OZI-1.3.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-03 04:53:10.000000 OZI-1.3.0/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.320882 OZI-1.3.0/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.308882 OZI-1.3.0/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.308882 OZI-1.3.0/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.308882 OZI-1.3.0/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.308882 OZI-1.3.0/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.312882 OZI-1.3.0/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.316882 OZI-1.3.0/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     4854 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.316882 OZI-1.3.0/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.320882 OZI-1.3.0/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6065 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.320882 OZI-1.3.0/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.320882 OZI-1.3.0/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.320882 OZI-1.3.0/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.324882 OZI-1.3.0/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.324882 OZI-1.3.0/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-03 04:53:10.000000 OZI-1.3.0/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10782 2024-05-03 04:53:10.000000 OZI-1.3.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      190 2024-05-03 04:53:10.000000 OZI-1.3.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.324882 OZI-1.3.0/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-05-03 04:53:10.000000 OZI-1.3.0/subprojects/blastpipe.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.324882 OZI-1.3.0/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-03 04:53:10.000000 OZI-1.3.0/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:58:29.328882 OZI-1.3.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-03 04:53:10.000000 OZI-1.3.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11072 2024-05-03 04:53:10.000000 OZI-1.3.0/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14164 2024-05-03 04:53:10.000000 OZI-1.3.0/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-03 04:53:10.000000 OZI-1.3.0/tests/test_tap.py
```

### Comparing `OZI-1.2.2/.github/CODEOWNERS` & `OZI-1.3.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/CODE_OF_CONDUCT.md` & `OZI-1.3.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/CONTRIBUTING.md` & `OZI-1.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/SECURITY.md` & `OZI-1.3.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/workflows/codeql.yml` & `OZI-1.3.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/workflows/dependency-review.yml` & `OZI-1.3.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/workflows/dev-workflow.yml` & `OZI-1.3.0/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.github/workflows/dist-workflow.yml` & `OZI-1.3.0/.github/workflows/dist-workflow.yml`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
             github.com:443
             pypi.org:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/release@7bbceab384cd0290577dec4b4fb04eed3c07b926
+      - uses: OZI-Project/release@26edb1dd060fbfe54494fb6c17aed8afc776a9f2
         id: release
         with:
           python-dist: ${{ matrix.py }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   generate-provenance:
     needs: [release, checkpoint]
```

### Comparing `OZI-1.2.2/.github/workflows/scorecard.yml` & `OZI-1.3.0/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/.gitignore` & `OZI-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/CHANGELOG.md` & `OZI-1.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,116 @@
 # CHANGELOG
+## 1.3.0 (2024-05-03)
+
+### :arrow_up:
+
+* :arrow_up: OZI.build 0.0.9 for correct wheel names. (#457)
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`adde41a`](https://github.com/OZI-Project/OZI/commit/adde41a9dd0eadcea050905799dc0509b3fb7e24))
+
+* :arrow_up: OZI-Project/release 0.2.4
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`cefd702`](https://github.com/OZI-Project/OZI/commit/cefd702d81b1e0b9428d67b78c10a8cebcc1b3ef))
+
+* :arrow_up: OZI-Project/release 0.2.2
+
+* Update ci.py 
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt;
+
+* Update dist-workflow.yml
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt;
+
+---------
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`28a1e70`](https://github.com/OZI-Project/OZI/commit/28a1e70a41dfe62a94e124790ec34ba592c9d773))
+
+* :arrow_up: release 0.2.1
+
+* Update dist-workflow.yml - release 0.2.1
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt;
+
+* Update ci.py - release 0.2.1
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt;
+
+---------
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`eb56e91`](https://github.com/OZI-Project/OZI/commit/eb56e91c27c40b359674b29d744124c25eacf322))
+
+* :arrow_up: OZI.build 0.0.7 in spec
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`1e3a51d`](https://github.com/OZI-Project/OZI/commit/1e3a51dfd7fc140e122a999ae92e642a84cea822))
+
+* :arrow_up: OZI-Project/release 0.2.0 for OZI.build backend change.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`24e23ba`](https://github.com/OZI-Project/OZI/commit/24e23baf1d795ee265580c84c721d55b6d7f037f))
+
+* :arrow_up: OZI.build 0.0.7
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`817265b`](https://github.com/OZI-Project/OZI/commit/817265bd093260eda4e6ad1136fd87552a2657b5))
+
+* :arrow_up: OZI.build 0.0.6
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`958b39a`](https://github.com/OZI-Project/OZI/commit/958b39aad552d2bc91520c2320c9fa94a1df4c09))
+
+### :hammer:
+
+* :hammer: unlink extant PKG-INFO during dist.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`7b99c62`](https://github.com/OZI-Project/OZI/commit/7b99c62023ab54f2c6b9da017f1cbdcce5f2f949))
+
+* :hammer: remove monkey-patched setuptools_scm dist script. ([`0505516`](https://github.com/OZI-Project/OZI/commit/050551600633572a647e239ebcfcadd5904c1c7f))
+
+* :hammer: auto pkg-info
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`dc0ee47`](https://github.com/OZI-Project/OZI/commit/dc0ee47ef9789fabadbd63fee08ba62093bf719b))
+
+* :hammer: revert pkg-info move
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`ff8356f`](https://github.com/OZI-Project/OZI/commit/ff8356f4fab00fd9b632f4fae356c1c5632a94b7))
+
+* :hammer: change metadata pkg-info-file
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`84a6b13`](https://github.com/OZI-Project/OZI/commit/84a6b13c8d8b86b925c0c014b6d863caf5c5df2e))
+
+* :hammer: Implement OZI.build
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`7a25a87`](https://github.com/OZI-Project/OZI/commit/7a25a870cefee7ad5bf054c152bd81d59f177055))
+
+### :sparkles:
+
+* :sparkles: Add 1.3 release group!
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`fd418e4`](https://github.com/OZI-Project/OZI/commit/fd418e4b7ca008b63f62da106f9f7d5bf020d80d))
+
+* :sparkles: OZI 1.3
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`c957112`](https://github.com/OZI-Project/OZI/commit/c9571120ba6765801e8f0447f60af0b5cead88b3))
+
+### Other
+
+* OZI-Project/release 0.2.5
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`e3801f4`](https://github.com/OZI-Project/OZI/commit/e3801f4161facecbb31385c933bfd0e90dd7bb83))
+
+* Update dist-workflow.yml
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`65b7b67`](https://github.com/OZI-Project/OZI/commit/65b7b672b70a5791fbc76807b1dbcc3ed3036961))
+
+* Update ci.py
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`924cd7e`](https://github.com/OZI-Project/OZI/commit/924cd7ee3cbb700cb55d772b06a2a8752fb2abcd))
+
+* use pkg-info-file
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`1f09610`](https://github.com/OZI-Project/OZI/commit/1f096107ab8818f5e7d72c181a41cf29971573a5))
+
 ## 1.2.2 (2024-04-30)
 
 ### :arrow_up:
 
 * :arrow_up: Bump step-security/harden-runner from 2.7.0 to 2.7.1
 
 Bumps [step-security/harden-runner](https://github.com/step-security/harden-runner) from 2.7.0 to 2.7.1.
```

### Comparing `OZI-1.2.2/LICENSE.txt` & `OZI-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/PKG-INFO` & `OZI-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.2.2
+Version: 1.3.0
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.2.2.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.3.0.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.2.2/README.rst` & `OZI-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/meson.build` & `OZI-1.3.0/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/meson.options` & `OZI-1.3.0/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/__main__.py` & `OZI-1.3.0/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/actions.py` & `OZI-1.3.0/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/comment.py` & `OZI-1.3.0/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/__main__.py` & `OZI-1.3.0/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/build_definition.py` & `OZI-1.3.0/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/meson.build` & `OZI-1.3.0/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/missing.py` & `OZI-1.3.0/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/parser.py` & `OZI-1.3.0/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/fix/rewrite_command.py` & `OZI-1.3.0/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/lint/meson.build` & `OZI-1.3.0/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/lint/pyright/meson.build` & `OZI-1.3.0/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/meson.build` & `OZI-1.3.0/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/meson.py` & `OZI-1.3.0/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/new/__main__.py` & `OZI-1.3.0/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/new/meson.build` & `OZI-1.3.0/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/new/parser.py` & `OZI-1.3.0/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/new/validate.py` & `OZI-1.3.0/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/pkg_extra.py` & `OZI-1.3.0/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/render.py` & `OZI-1.3.0/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/core_metadata_template.py` & `OZI-1.3.0/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/meson.build` & `OZI-1.3.0/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.3.0/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,11 +54,13 @@
             '/',
         ),
     )
     with (source / 'pyproject.toml').open('rb') as project_file:
         pyproject_toml = toml.load(project_file)
     setuptools_scm = pyproject_toml.get('tool', {}).get('setuptools_scm', {})
     path = Path(dist / setuptools_scm.get('version_file')).resolve()
+    if path.exists():
+        path.unlink()
     if path.parent != Path(dist).resolve():
         raise RuntimeError('Invalid version_file path in pyproject.toml')
     else:
         path.write_text(setuptools_scm.get('version_file_template'))
```

### Comparing `OZI-1.2.2/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.3.0/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/render_requirements.py` & `OZI-1.3.0/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.3.0/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/scm_version_snip.py` & `OZI-1.3.0/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/to_distribution_template.py` & `OZI-1.3.0/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/scripts/version_metadata_template.py` & `OZI-1.3.0/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spdx.py` & `OZI-1.3.0/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/_license.py` & `OZI-1.3.0/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/_spec.py` & `OZI-1.3.0/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/base.py` & `OZI-1.3.0/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/ci.py` & `OZI-1.3.0/ozi/spec/ci.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     version: str = '0.1.0'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Release(Default):
     """Release patterns for packaged project."""
 
-    version: str = '0.1.18'
+    version: str = '0.2.5'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Checkpoint(Default):
     """Checkpoint suites to run."""
 
     suites: tuple[str, ...] = ('dist', 'lint', 'test')
@@ -167,18 +167,18 @@
     )
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Build(Default):
     """Build backend and required packages for OZI."""
 
-    backend: str = 'mesonpep517.buildapi'
+    backend: str = 'ozi_build.buildapi'
     requires: Mapping[str, str] = field(
         default_factory=lambda: {
-            'mesonpep517': 'mesonpep517==0.2',
+            'OZI.build': 'OZI.build==0.0.9',
             'meson': 'meson[ninja]>=1.1.0',
             'pip-tools': 'pip-tools>=7',
             'setuptools': 'setuptools>=64',
             'setuptools_scm': 'setuptools_scm>=8.0',
             'tomli': 'tomli>=2.0.0;python_version<"3.11"',
         },
     )
```

### Comparing `OZI-1.2.2/ozi/spec/meson.build` & `OZI-1.3.0/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/pkg.py` & `OZI-1.3.0/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/project.py` & `OZI-1.3.0/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/python.py` & `OZI-1.3.0/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/spec/src.py` & `OZI-1.3.0/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/tap.py` & `OZI-1.3.0/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/trove.py` & `OZI-1.3.0/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/__init__.py` & `OZI-1.3.0/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/__main__.py` & `OZI-1.3.0/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/deliverability.py` & `OZI-1.3.0/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.3.0/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/meson.build` & `OZI-1.3.0/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.3.0/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/syntax.py` & `OZI-1.3.0/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/email_validator/validate_email.py` & `OZI-1.3.0/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/ozi/vendor/meson.build` & `OZI-1.3.0/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/pyproject.toml` & `OZI-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # pyproject.toml
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 [build-system]
-build-backend = "mesonpep517.buildapi"
+build-backend = "ozi_build.buildapi"
 requires      = [
-    "mesonpep517==0.2",
+    "OZI.build==0.0.9",
     "meson[ninja]>=1.1.0",
     "pip-tools>=7",
     "setuptools>=64",
     "setuptools_scm>=8.0",
     'tomli>=2.0.0;python_version<"3.11"',
 ]
 
-[tool.mesonpep517.entry-points]
+[tool.ozi-build.entry-points]
 console_scripts = [
     "ozi = ozi.__main__:main",
     "ozi-new = ozi.new.__main__:main",
     "ozi-fix = ozi.fix.__main__:main",
 ]
 
-[tool.mesonpep517.metadata]
-pkg-info-file = 'build/PKG-INFO'
+[tool.ozi-build.metadata]
 summary = 'Packager for Python projects using Meson.'
+pkg-info-file = 'build/PKG-INFO'
 
 [tool.cibuildwheel]
 build-frontend = "build"
 before-build = [
      "pip install --upgrade pip",
      "pip install --upgrade build",
      "pip install --upgrade sigstore",
      "pip install --upgrade meson[ninja]>=1.1.0",
-     "pip install --upgrade mesonpep517",
+     "pip install --upgrade OZI.build",
      "pip install --upgrade setuptools_scm",
      "pip install --upgrade pip-tools",
      "meson setup build",
 ]
 
 [tool.setuptools_scm]
 version_file_template = """
@@ -70,15 +70,14 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Description-Content-Type: text/x-rst
 
 @README_TEXT@
 """
 version_file = "PKG-INFO"
-# meson writes during configuration so that meson dist can have a valid version.
 fallback_version = "@VCS_TAG@"
 parentdir_prefix_version = "OZI-"
 tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.in"] }
 
@@ -297,14 +296,19 @@
 prerelease = false
 
 [tool.semantic_release.branches."release/1.2"]
 match = "release/1.2"
 prerelease_token = "alpha"
 prerelease = false
 
+[tool.semantic_release.branches."release/1.3"]
+match = "release/1.3"
+prerelease_token = "alpha"
+prerelease = false
+
 [tool.semantic_release.commit_parser_options]
 major_tags = [":boom:"]
 minor_tags = [
     ":sparkles:",
 ]
 patch_tags = [
     ":adhesive_bandage:",
```

### Comparing `OZI-1.2.2/templates/CHANGELOG.md.j2` & `OZI-1.3.0/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/tests/meson.build` & `OZI-1.3.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/tests/test_ozi_fix.py` & `OZI-1.3.0/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/tests/test_ozi_new.py` & `OZI-1.3.0/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.2.2/tests/test_tap.py` & `OZI-1.3.0/tests/test_tap.py`

 * *Files identical despite different names*

