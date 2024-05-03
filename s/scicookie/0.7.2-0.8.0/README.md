# Comparing `tmp/scicookie-0.7.2.tar.gz` & `tmp/scicookie-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.7.2.tar", max compression
+gzip compressed data, was "scicookie-0.8.0.tar", max compression
```

## Comparing `scicookie-0.7.2.tar` & `scicookie-0.8.0.tar`

### file list

```diff
@@ -1,85 +1,88 @@
--rw-r--r--   0        0        0     1508 2024-03-25 01:03:17.510717 scicookie-0.7.2/LICENSE
--rw-r--r--   0        0        0     4802 2024-03-25 01:03:17.514717 scicookie-0.7.2/docs/description.md
--rw-r--r--   0        0        0     2071 2024-03-25 01:04:35.118971 scicookie-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       80 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/__init__.py
--rw-r--r--   0        0        0      116 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/__main__.py
--rw-r--r--   0        0        0     5066 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/cli.py
--rw-r--r--   0        0        0     1835 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0    11921 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      971 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/logs.py
--rw-r--r--   0        0        0     1607 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/profile.py
--rw-r--r--   0        0        0     6422 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0     1380 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0     3754 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/ui.py
--rw-r--r--   0        0        0      336 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     5119 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1208 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2051 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2939 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1392 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1755 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     3254 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2812 2024-03-25 01:03:17.522717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     3918 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
--rw-r--r--   0        0        0     3354 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
--rw-r--r--   0        0        0      108 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
--rw-r--r--   0        0        0     2229 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     5996 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     3358 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0      432 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0      608 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/CMakeLists.txt
--rw-r--r--   0        0        0      618 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml
--rw-r--r--   0        0        0     1847 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
--rw-r--r--   0        0        0     4243 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
--rw-r--r--   0        0        0     4254 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch-pyproject.toml
--rw-r--r--   0        0        0      589 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs
--rw-r--r--   0        0        0      632 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp
--rw-r--r--   0        0        0     4212 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin-pyproject.toml
--rw-r--r--   0        0        0      400 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
--rw-r--r--   0        0        0     4170 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
--rw-r--r--   0        0        0     4164 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
--rw-r--r--   0        0        0     3269 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
--rw-r--r--   0        0        0     4190 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11-pyproject.toml
--rw-r--r--   0        0        0     4286 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core-pyproject.toml
--rw-r--r--   0        0        0      497 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setup.py
--rw-r--r--   0        0        0     3851 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
--rw-r--r--   0        0        0      171 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/skcdemo.cpp
--rw-r--r--   0        0        0     6436 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6436 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0    19228 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
--rw-r--r--   0        0        0     5593 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
--rw-r--r--   0        0        0     1998 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       54 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
--rw-r--r--   0        0        0      182 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
--rw-r--r--   0        0        0       20 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0    12824 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1116 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3382 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0     1123 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      141 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4571 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rwxr-xr-x   0        0        0     5275 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      374 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       30 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
--rw-r--r--   0        0        0    16405 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6840 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     1554 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0     1009 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
--rw-r--r--   0        0        0      892 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
--rw-r--r--   0        0        0      927 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      562 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0     2151 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
--rw-r--r--   0        0        0        0 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
--rw-r--r--   0        0        0       19 2024-03-25 01:03:17.526717 scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 scicookie-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1508 2024-05-03 05:03:41.865371 scicookie-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4874 2024-05-03 05:03:41.865371 scicookie-0.8.0/docs/description.md
+-rw-r--r--   0        0        0     2065 2024-05-03 05:04:57.929756 scicookie-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     5066 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1860 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0    12770 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      971 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1607 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/profile.py
+-rw-r--r--   0        0        0     6460 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0     1380 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0     4153 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/ui.py
+-rw-r--r--   0        0        0      336 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     5119 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1208 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2051 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2939 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1392 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1790 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     3254 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2812 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     4404 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
+-rw-r--r--   0        0        0     3354 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
+-rw-r--r--   0        0        0      108 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
+-rw-r--r--   0        0        0     2229 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     5996 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     3563 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0      432 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0      608 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/CMakeLists.txt
+-rw-r--r--   0        0        0      618 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml
+-rw-r--r--   0        0        0     1884 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml
+-rw-r--r--   0        0        0     4824 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/deps-pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch-pyproject.toml
+-rw-r--r--   0        0        0      589 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs
+-rw-r--r--   0        0        0      632 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp
+-rw-r--r--   0        0        0      264 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin-pyproject.toml
+-rw-r--r--   0        0        0      400 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/meson.build
+-rw-r--r--   0        0        0      223 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy-pyproject.toml
+-rw-r--r--   0        0        0      217 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm-pyproject.toml
+-rw-r--r--   0        0        0     3632 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml
+-rw-r--r--   0        0        0      275 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11-pyproject.toml
+-rw-r--r--   0        0        0      247 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core-pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setup.py
+-rw-r--r--   0        0        0      226 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools-pyproject.toml
+-rw-r--r--   0        0        0      171 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/skcdemo.cpp
+-rw-r--r--   0        0        0     6436 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6436 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0    19228 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
+-rw-r--r--   0        0        0     5593 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
+-rw-r--r--   0        0        0     1998 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0    14485 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3382 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0     1123 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      141 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4571 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rw-r--r--   0        0        0      719 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml
+-rw-r--r--   0        0        0       17 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/styles.css
+-rwxr-xr-x   0        0        0     5275 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2024-05-03 05:03:41.877371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16405 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6840 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     1554 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py
+-rw-r--r--   0        0        0     1009 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
+-rw-r--r--   0        0        0      892 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
+-rw-r--r--   0        0        0      831 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0     2151 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
+-rw-r--r--   0        0        0        0 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
+-rw-r--r--   0        0        0       19 2024-05-03 05:03:41.881371 scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0     5600 1970-01-01 00:00:00.000000 scicookie-0.8.0/PKG-INFO
```

### Comparing `scicookie-0.7.2/LICENSE` & `scicookie-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/docs/description.md` & `scicookie-0.8.0/docs/description.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![CI](https://img.shields.io/github/actions/workflow/status/osl-incubator/scicookie/main.yaml?logo=github&label=CI)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scicookie)](https://pypi.org/project/scicookie/)
 [![Package Version](https://img.shields.io/pypi/v/scicookie?color=blue)](https://pypi.org/project/scicookie/)
 ![License](https://img.shields.io/pypi/l/scicookie?color=blue)
 ![Discord](https://img.shields.io/discord/796786891798085652?logo=discord&color=blue)
 
-![logo_scicookie.png](images%2Flogo_scicookie.png)
+![logo_scicookie.png](https://github.com/osl-incubator/scicookie/blob/main/docs/images/logo_scicookie.png?raw=true)
 
 **SciCookie** is a project template designed to simplify scientific Python
 project creation. It provides an initial structure with recommended tools,
 workflows, and industry best practices, saving developers time and effort. Built
 upon the PyOpenSci recommendations, it offers a foundation that adheres to
 scientific Python standards while remaining customizable to specific project
 needs.
@@ -28,15 +28,15 @@
 - **Testing & Linting:** Integrates with pytest, hypothesis, black
   (auto-formatting), bandit (security), pydocstyle (documentation style),
   vulture (unused code detection), and McCabe (cyclomatic complexity analysis)
   for a robust development environment.
 - **Version Control & Automation:** Includes initial git integration, conda
   (base environment) support, pre-commit hooks, continuous integration with
   GitHub Actions, and release workflows with semantic-release.
-- **Documentation:** Offers options for mkdocs, sphinx, or jupyter-book
+- **Documentation:** Offers options for mkdocs, sphinx, jupyter-book or quarto
   documentation generation.
 - **Containerization:** Provides the ability to add initial files for running
   and managing containers using Docker or Podman.
 
 ### Benefits:
 
 - **Reduces boilerplate code:** SciCookie eliminates the need to write
```

### Comparing `scicookie-0.7.2/pyproject.toml` & `scicookie-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.7.2"  # semantic-release
+version = "0.8.0"  # semantic-release
 description = "Cookiecutter template for a Python package"
 readme = "docs/description.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD-3-Clause"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
@@ -29,20 +29,20 @@
 ruff = ">=0.2.0"
 mypy = ">=1.5"
 pytest-cov = ">=3"
 pytest-cookies = ">=0.6.1"
 markdown-callouts = ">=0.2"
 mkdocs = ">=1.3.1"
 mkdocs-include-exclude-files = ">=0.0.1"
-mkdocs-jupyter = ">=0.21"
+mkdocs-jupyter = ">=0.24.7"
 mkdocs-material = ">=8.3.9"
 mkdocstrings-python = ">=0.7.1"
 mkdocstrings-python-legacy = ">=0.2.3"
 pymdown-extensions = ">=9.5"
-makim = ">=1.14.0,<1.15"
+makim = "1.15.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 no_strict_optional = false
```

### Comparing `scicookie-0.7.2/src/scicookie/cli.py` & `scicookie-0.8.0/src/scicookie/cli.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/cookiecutter.json` & `scicookie-0.8.0/src/scicookie/cookiecutter.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899390243902439%*

 * *Differences: {"'documentation_engine'": "{insert: [(3, 'quarto')]}",*

 * * "'use_black'": "'no'",*

 * * "'use_conda'": "'no'",*

 * * "'use_makim'": "'no'",*

 * * "'use_pre_commit'": "'no'",*

 * * "'use_pyenv'": "'no'",*

 * * "'use_pytest'": "'no'",*

 * * "'use_ruff'": "'no'"}*

```diff
@@ -23,15 +23,16 @@
         "None",
         "Click",
         "Argparse"
     ],
     "documentation_engine": [
         "mkdocs",
         "sphinx",
-        "jupyter-book"
+        "jupyter-book",
+        "quarto"
     ],
     "documentation_url": "{{ cookiecutter.project_url }}",
     "git_https_origin": "",
     "git_https_upstream": "",
     "git_main_branch": "main",
     "git_username": "zoro_roronoa",
     "governance_document": [
@@ -58,30 +59,31 @@
     "project_url": "https://{{ cookiecutter.project_slug }}.com",
     "project_version": "0.1.0",
     "roadmap_document": [
         "None",
         "pytorch-ignite-roadmap"
     ],
     "use_bandit": "no",
-    "use_black": "yes",
-    "use_conda": "yes",
+    "use_black": "no",
+    "use_conda": "no",
     "use_containers": [
         "None",
         "Docker",
         "Podman"
     ],
     "use_coverage": "no",
     "use_flake8": "no",
     "use_hypothesis": "no",
     "use_isort": "no",
     "use_make": "no",
-    "use_makim": "yes",
+    "use_makim": "no",
     "use_mccabe": "no",
     "use_mypy": "no",
-    "use_pre_commit": "yes",
+    "use_pre_commit": "no",
     "use_prettier": "no",
     "use_pydocstyle": "no",
-    "use_pytest": "yes",
-    "use_ruff": "yes",
+    "use_pyenv": "no",
+    "use_pytest": "no",
+    "use_ruff": "no",
     "use_shellcheck": "no",
     "use_vulture": "no"
 }
```

### Comparing `scicookie-0.7.2/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.8.0/src/scicookie/hooks/post_gen_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pathlib import Path
 
 PROJECT_DIRECTORY = Path(os.path.abspath(os.path.curdir)).resolve()
 
 UNUSED_DOCS_DIRS = [
     PROJECT_DIRECTORY / 'docs-mkdocs',
     PROJECT_DIRECTORY / 'docs-sphinx',
-    PROJECT_DIRECTORY / 'docs-jupyter-book'
+    PROJECT_DIRECTORY / 'docs-jupyter-book',
+    PROJECT_DIRECTORY / 'docs-quarto',
 ]
 
 DOCUMENTATION_ENGINE = "{{ cookiecutter.documentation_engine }}"
 DOCS_SPEC_DIR = UNUSED_DOCS_DIRS.pop(
     UNUSED_DOCS_DIRS.index(
         PROJECT_DIRECTORY / f'docs-{DOCUMENTATION_ENGINE}'
     )
@@ -32,14 +33,17 @@
 USE_CONTAINERS = {{ cookiecutter.use_containers in ['Docker', 'Podman'] }}
 USE_CLI = {{ cookiecutter.command_line_interface != "None" }}
 USE_CONDA = {{ cookiecutter.use_conda == "yes" }}
 USE_MAKE = {{ cookiecutter.use_make == "yes" }}
 USE_MAKIM = {{ cookiecutter.use_makim == "yes" }}
 USE_MYPY = {{ cookiecutter.use_mypy == "yes" }}
 USE_PRETTIER = {{ cookiecutter.use_prettier == "yes" }}
+USE_PRE_COMMIT = {{ cookiecutter.use_pre_commit == "yes" }}
+USE_PYTEST = {{ cookiecutter.use_pytest == "yes" }}
+USE_HYPOTHESIS = {{ cookiecutter.use_hypothesis == "yes" }}
 {% if cookiecutter.code_of_conduct == "contributor-covenant" -%}
 COC_PATH = PROJECT_DIRECTORY / 'coc' / 'CONTRIBUTOR_COVENANT.md'
 {%- elif cookiecutter.code_of_conduct == "citizen-code-of-conduct" -%}
 COC_PATH = PROJECT_DIRECTORY / 'coc' / 'CITIZEN.md'
 {%- elif cookiecutter.code_of_conduct == "numfocus-adapted-coc" -%}
 COC_PATH = PROJECT_DIRECTORY / 'coc' / 'NUMFOCUS_adapted_coc.md'
 {%- elif cookiecutter.code_of_conduct == "python-adapted-coc" -%}
@@ -108,18 +112,25 @@
         docs_target_dir = PROJECT_DIRECTORY / "docs"
     for file_name in os.listdir(DOCS_SPEC_DIR):
         shutil.move(DOCS_SPEC_DIR / file_name, docs_target_dir)
 
     if DOCUMENTATION_ENGINE == "sphinx":
         remove_project_file(Path("docs") / "index.md")
         remove_project_file(Path("docs/api") / "references.md")
-
+    if DOCUMENTATION_ENGINE == "quarto":
+        remove_project_file(Path("docs/api") / "references.md")
+        remove_project_file(Path("docs/api") / "references.rst")
     shutil.rmtree(DOCS_SPEC_DIR)
 
 
+def clean_up_tests():
+    if not USE_PYTEST and not USE_HYPOTHESIS:
+        remove_project_file("tests/test_main.py")
+
+
 def clean_up_automation():
     if not USE_MAKE:
         remove_project_file("Makefile")
 
     if not USE_MAKIM:
         remove_project_file(".makim.yaml")
 
@@ -178,19 +189,14 @@
 
 def clean_up_cli():
     if not USE_CLI:
         remove_package_file("__main__.py")
         remove_package_file("cli.py")
 
 
-def clean_up_prettier():
-    if not USE_PRETTIER:
-        remove_project_file(".prettierrc.yaml")
-        remove_project_file(".prettierignore")
-
 def clean_up_build_system():
     build_system_dir = PROJECT_DIRECTORY / "build-system"
 
     if BUILD_SYSTEM == "poetry":
         shutil.move(
             build_system_dir / "poetry-pyproject.toml",
             PROJECT_DIRECTORY / 'pyproject.toml'
@@ -267,14 +273,36 @@
     remove_dir("build-system")
 
 
 def http2ssh(url):
     url = url.replace("https://", "git@")
     return url.replace("/", ":", 1)
 
+def clean_up_linter():
+    if not USE_MYPY:
+        remove_package_file("py.typed")
+
+    if not USE_PRE_COMMIT:
+        remove_project_file(".pre-commit-config.yaml")
+
+    if not USE_PRETTIER:
+        remove_project_file(".prettierrc.yaml")
+        remove_project_file(".prettierignore")
+
+    # keep this one at the end
+    if USE_PRETTIER:
+        subprocess.call([
+            "npx",
+            "--yes",
+            "prettier",
+            "--write",
+            "--ignore-unknown",
+            PROJECT_DIRECTORY
+        ])
+
 
 def prepare_git() -> None:
     git_https_origin = http2ssh("{{cookiecutter.git_https_origin}}")
     git_https_upstream = http2ssh("{{cookiecutter.git_https_upstream}}")
     git_main_branch = http2ssh("{{cookiecutter.git_main_branch}}")
     unique_id = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
     git_new_branch = f"initial-from-scicookie-{unique_id}"
@@ -355,35 +383,31 @@
         else:
             os.makedir(src_system_dir)
             shutil.move(build_system_dir / "main.cpp", src_system_dir)
     else:
         pass
 
 
-def clean_up_mypy():
-    if not USE_MYPY:
-        remove_package_file("py.typed")
-
-
 def post_gen():
-
     # keep this one first, because it changes the package folder
     clean_up_project_layout()
     add_binding_source_files()
     clean_up_automation()
     clean_up_cli()
-    clean_up_mypy()
     clean_up_code_of_conduct()
     clean_up_conda()
     clean_up_containers()
     clean_up_docs()
     clean_up_governance()
     clean_up_roadmap()
     clean_up_build_system()
-    clean_up_prettier()
+    clean_up_tests()
+
+    # keep it before the prepare_git function call
+    clean_up_linter()
 
     # keep it at the end, because it will create a new git commit
     prepare_git()
 
 
 if __name__ == "__main__":
     post_gen()
```

### Comparing `scicookie-0.7.2/src/scicookie/logs.py` & `scicookie-0.8.0/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/profile.py` & `scicookie-0.8.0/src/scicookie/profile.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/profiles/base.yaml` & `scicookie-0.8.0/src/scicookie/profiles/base.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   default: "{{ project_name.replace(' ', '-').lower() }}"
   visible: true
 
 package_slug:
   message: Type the code name for your package (the name used to import your package)
   help: https://osl-incubator.github.io/scicookie/guide/#information-about-the-project
   type: text
-  default: "{{project_slug.replace('-', '_')}}"
+  default: "{{project_slug.replace('-', '_') | sanitize_package_slug}} "
   visible: true
 
 project_version:
   message: Type the project version
   help: https://osl-incubator.github.io/scicookie/guide/#information-about-the-project
   type: text
   default: 0.1.0
@@ -116,14 +116,15 @@
   type: single-choice
   default: mkdocs
   # first choice is the default for the UI
   choices:
     - mkdocs
     - sphinx
     - jupyter-book
+    - quarto
   visible: true
 
 documentation_url:
   message: Type the documentation URL
   help: The URL for the documentation page.
   type: text
   default: "{{ project_url }}"
```

### Comparing `scicookie-0.7.2/src/scicookie/profiles/osl.yaml` & `scicookie-0.8.0/src/scicookie/profiles/osl.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/ui.py` & `scicookie-0.8.0/src/scicookie/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Define functions for the interface with the user."""
 
 from __future__ import annotations
 
 import os
+import re
 
 from typing import Any, Optional, Type
 
 import inquirer
 
 from colorama import Fore, Style, init
-from jinja2 import Template
+from jinja2 import Environment
 
 from scicookie.logs import SciCookieErrorType, SciCookieLogs
 
 # Initialize Colorama
 init()
 
 
@@ -72,14 +73,21 @@
     Check if dependencies are satisfied.
 
     Note: Not implemented yet.
     """
     return True
 
 
+def sanitize_package_slug(package_slug: str) -> str:
+    """Filter to sanitize the package slug."""
+    return re.sub(
+        r"^\s+|\s+$", "", re.sub(r"[^a-zA-Z0-9_]+", "", package_slug)
+    )
+
+
 def make_questions(questions: dict[str, Any]) -> dict[str, str]:
     """Generate all the visible questions."""
     answers: dict[str, str] = {}
 
     # Get the size of the terminal window
     columns, _ = os.get_terminal_size()
 
@@ -92,19 +100,25 @@
         + "For questions with single or multiple choices, use the ARROW "
         + "keys to navigate through the options. Use the SPACE BAR to "
         + "select or deselect an option. Confirm your selection with "
         + "the ENTER key."
     )
     print("." * columns)
 
+    # Create a Jinja2 environment and add the custom filter
+    env = Environment()
+    env.filters["sanitize_package_slug"] = sanitize_package_slug
+
     for question_id, question in questions.items():
         question_obj = _create_question(question_id, question)
 
         default_answer = question.get("default", "")
-        default_answer = Template(default_answer).render(answers)
+        default_answer = (
+            env.from_string(default_answer).render(answers).strip()
+        )
 
         # note: if question_object is None, that means that the question is
         #       not visible
         if not (
             check_dependencies_satisfied(question, answers) and question_obj
         ):
             answers[question_id] = default_answer
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
           {%- if cookiecutter.use_makim == "yes" %}
           makim tests.unit
           {%- else %}
           make test
           {%- endif %}
 
       - name: Run style checks
+        if: success() || failure()
         run: |
           pre-commit install
           {%- if cookiecutter.use_makim == "yes" %}
           makim tests.linter
           {%- else %}
           make lint
           {%- endif %}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {%- set package_path = "src/" + cookiecutter.package_slug -%}
 {%- else -%}
 {%- set package_path = cookiecutter.package_slug -%}
 {%- endif -%}
 version: 1.0
 groups:
   clean:
-    targets:
+    tasks:
       all:
         help: Clean unnecessary temporary files
         run: |
           rm -fr build/
           rm -fr dist/
           rm -fr .eggs/
           rm -f .coverage
@@ -22,42 +22,49 @@
           find . -name '*.egg' -exec rm -f {} +
           find . -name '*.pyc' -exec rm -f {} +
           find . -name '__pycache__' -exec rm -fr {} +
           find . -name '*.pyo' -exec rm -f {} +
           find . -name '*~' -exec rm -f {} +
 
   docs:
-    targets:
+    tasks:
       build:
         help: Build documentation
         run: |
           {%- if cookiecutter.documentation_engine == "jupyter-book" %}
           rm -rf docs/_build
           jupyter-book build docs
           {%- elif cookiecutter.documentation_engine == "mkdocs" %}
           mkdocs build --config-file mkdocs.yaml
           {%- elif cookiecutter.documentation_engine == "sphinx" %}
           sphinx-apidoc -o docs/_build {{ package_path }}
+          {%- elif cookiecutter.documentation_engine == "quarto" %}
+          cd docs
+          quartodoc build
+          quarto render
+          cd ..
           {%- endif %}
 
       preview:
         help: Preview documentation page locally
         dependencies:
-          - target: docs.build
+          - task: docs.build
         run: |
           {%- if cookiecutter.documentation_engine == "jupyter-book" %}
           cd docs/_build/html/ && python -m http.server
           {%- elif cookiecutter.documentation_engine == "mkdocs" %}
-          mkdocs build --config-file mkdocs.yaml
+          mkdocs serve --watch docs --config-file mkdocs.yaml
           {%- elif cookiecutter.documentation_engine == "sphinx" %}
           cd docs/_build && python -m http.server
+          {%- elif cookiecutter.documentation_engine == "quarto" %}
+          quarto preview docs
           {%- endif %}
 
   tests:
-    targets:
+    tasks:
       linter:
         help: Run linter tools
         run: |
           pre-commit install
           pre-commit run --all-files --verbose
 
       unit:
@@ -68,24 +75,30 @@
             type: string
             default: ""
           params:
             help: Specify parameters to be used for tests
             type: string
             default: "-vv"
         run: |
+          {%- if cookiecutter.use_pytest == "yes" %}
           pytest {{ "${{ args.path }} ${{ args.params }}" }}
+          {%- elif cookiecutter.use_hypothesis == "yes" %}
+          python -m unittest discover
+          {%- else %}
+          echo "No test library installed."
+          {%- endif %}
 
       ci:
         help: run the sames tests executed on CI
         dependencies:
-          - target: tests.unit
-          - target: tests.linter
+          - task: tests.unit
+          - task: tests.linter
 
   package:
-    targets:
+    tasks:
       build:
         help: "Build the package"
         run: |
           {%- if cookiecutter.build_system == "poetry" %}
           poetry build
           {%- elif cookiecutter.build_system == "flit" %}
           flit build
@@ -113,15 +126,15 @@
         -p "@semantic-release/changelog" \
         -p "@semantic-release/exec" \
         -p "@semantic-release/github" \
         -p "@semantic-release/git" \
         -p "@google/semantic-release-replace-plugin" \
         semantic-release
 
-    targets:
+    tasks:
       ci:
         help: run semantic release on CI
         run: {{ "${{ vars.app }} --ci" }}
 
       dry:
         help: run semantic release in dry-run mode
         run: {{ "${{ vars.app }} --dry-run" }}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 .PHONY: test
 test: ## run tests quickly with the default Python
 	{%- if cookiecutter.use_pytest == "yes" %}
 	pytest
 	{%- elif cookiecutter.use_hypothesis == "yes" %}
 	python -m unittest discover
 	{%- else %}
-	@echo "No test library selected."
+	@echo "No test library installed."
 	{%- endif %}
 
 {% if cookiecutter.documentation_engine == 'mkdocs' -%}
 .PHONY:docs-build
 docs-build:
 	mkdocs build --config-file mkdocs.yaml
 
@@ -96,14 +96,23 @@
 .PHONY:docs-build
 docs-build:
 	jupyter-book build --all docs/
 
 .PHONY: docs-preview
 docs-preview: docs-build
 	cd docs/_build/html/ && python -m http.server
+
+{%- elif cookiecutter.documentation_engine == 'quarto' -%}
+.PHONY:docs-build
+docs-build:
+	cd docs/ && quartodoc build && quarto render
+
+.PHONY: docs-preview
+docs-preview: docs-build
+	quarto preview docs
 {%- endif +%}
 
 .PHONY:build
 build:
 	{%- if cookiecutter.build_system == "poetry" %}
 	poetry build
 	{%- elif cookiecutter.build_system == "flit" %}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/CMakeLists.txt` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/base-pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 {% if cookiecutter.project_layout == "src" -%}
 {% set package_path = "src/" + cookiecutter.package_slug -%}
 {% else -%}
 {% set package_path = cookiecutter.package_slug -%}
 {% endif -%}
 
-{%- if cookiecutter.use_pytest == "yes" %}
+{%- if cookiecutter.use_pytest == "yes" -%}
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_black == "yes" %}
 [tool.black]
 line-length = 79
 target-version = ["py38"]
 force-exclude = '''(?x)(
     docs/*
   | .*\\.egg-info
 )'''  # TOML's single-quoted strings do not require escaping backslashes
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_isort == "yes" %}
 [tool.isort]
 ensure_newline_before_comments = true
 line_length = 79
 multi_line_output = 3
 include_trailing_comma = true
 skip_glob = ["docs/*", "*.egg-info"]
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_bandit == "yes" %}
 [tool.bandit]
 exclude_dirs = ["tests"]
 targets = "./"
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_vulture == "yes" %}
 [tool.vulture]
 exclude = ["tests"]
 ignore_decorators = []
 ignore_names = []
 make_whitelist = true
 min_confidence = 80
 paths = ["./"]
 sort_by_size = true
 verbose = false
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_ruff == "yes" %}
 [tool.ruff]
 line-length = 79
 force-exclude = true
 src = ["./"]
 exclude = [
@@ -70,20 +70,21 @@
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.ruff.lint.isort]
 # Use a single line between direct and from import
 lines-between-types = 1
-{% endif %}
+{% endif -%}
 
 {%- if cookiecutter.use_mypy == "yes" %}
 [tool.mypy]
 python_version = "3.8"
 check_untyped_defs = true
 strict = true
 ignore_missing_imports = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
-{% endif %}
-{#- keep this line at the end of the file -#}
+{% endif -%}
+{# keep this line at the end of the file #}
+# Add more configuration here!
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit-pyproject.toml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/deps-pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,151 @@
-[build-system]
-requires = ["flit_core >=3.4"]
-build-backend = "flit_core.buildapi"
-
-
 [project]
 name = "{{ cookiecutter.project_slug }}"
 authors = [
   { name = "{{ cookiecutter.author_full_name }}", email = "{{ cookiecutter.author_email }}" },
 ]
 description = "{{ cookiecutter.project_short_description }}"
+{% if cookiecutter.build_system not in ["setuptools", "pybind11"]%}
 {% if cookiecutter.project_layout == "src" -%}
 packages = [
   {include = "{{ cookiecutter.package_slug }}", from="src"},
 ]
 {% else -%}
 packages = [
   {include = "{{ cookiecutter.package_slug }}"},
 ]
 {% endif -%}
+{% endif -%}
 readme = "README.md"
 classifiers = [
   "Development Status :: 1 - Planning",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
 {%- if cookiecutter.project_license == "MIT" %}
   "License :: OSI Approved :: MIT License",
 {%- elif cookiecutter.project_license == "BSD 3 Clause" %}
   "License :: OSI Approved :: BSD License",
 {%- elif cookiecutter.project_license == "Apache Software License 2.0" %}
   "License :: OSI Approved :: Apache Software License",
 {%- elif cookiecutter.project_license == "GNU General Public License v3" %}
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-{%- endif %}
+{% endif %}
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
-{%- if cookiecutter.use_mypy == "yes" -%}
+{%- if cookiecutter.use_mypy == "yes" %}
   "Typing :: Typed",
-{% endif %}
+{% endif -%}
 ]
+{% if cookiecutter.build_system == "scikit-build-core" %}
+version = "{{ cookiecutter.project_version }}"
+{% else %}
 dynamic = ["version"]
+{% endif -%}
 requires-python = ">=3.8.1,<4"
 dependencies = [
+  # note: add your dependencies here
+]
 {# keep this line here #}
-{%- if cookiecutter.use_pytest == "yes" -%}
-    "pytest >= 7.3.2",
-{% if cookiecutter.use_coverage == "yes" -%}
-    "pytest-cov >= 4.1.0",
-{% endif %}
+{%- if cookiecutter.build_system == "pdm" %}
+[tool.pdm.dev-dependencies]
+{%- else %}
+# NOTE: it is not actually optional, instead it is development dependencies
+[project.optional-dependencies]
+{%- endif %}
+dev = [
+{#- keep this line here -#}
+{%- if cookiecutter.build_system in ["setuptools", "pybind11"] %}
+  "build>=0.10.0",
+{%- endif -%}
+{%- if cookiecutter.use_pytest == "yes" %}
+  "pytest >= 7.3.2",
+{%- if cookiecutter.use_coverage == "yes" %}
+  "pytest-cov >= 4.1.0",
+{%- endif -%}
 {%- endif -%}{#- end of use_pytest -#}
-{%- if cookiecutter.use_hypothesis == "yes" -%}
-    "hypothesis >= 6.0",
-{% endif %}
-{%- if cookiecutter.use_coverage == "yes" -%}
-    "coverage >= 7.2.7",
-{% endif %}
-{%- if cookiecutter.use_black == "yes" -%}
-    "black >= 23.3.0,<23.10",
-{% endif %}
-{%- if cookiecutter.use_isort == "yes" -%}
-    "isort >= 5.12.0",
-{% endif %}
-{%- if cookiecutter.use_pre_commit -%}
-    "pre-commit >= 3.3.2",
-{% endif %}
-{%- if cookiecutter.use_flake8 == "yes" -%}
-    "flake8 >= 4.0.1, < 7",
-{% endif %}
-{%- if cookiecutter.use_ruff == "yes" -%}
-    "ruff >= 0.2.0",
-{% endif %}
-{%- if cookiecutter.use_mypy == "yes" -%}
-    "mypy >= 1.5.0",
-{% endif %}
-{%- if cookiecutter.use_bandit == "yes" -%}
-    "bandit >= 1.7.5",
-{% endif %}
-{%- if cookiecutter.use_pydocstyle == "yes" -%}
-    "pydocstyle >= 6.3.0",
-{% endif %}
-{%- if cookiecutter.use_vulture == "yes" -%}
-    "vulture >= 2.7",
-{% endif %}
-{%- if cookiecutter.use_mccabe == "yes" -%}
-    "mccabe >= 0.6.1",
-{% endif %}
-{%- if cookiecutter.use_containers in ['Docker', 'Podman'] -%}
+{%- if cookiecutter.use_hypothesis == "yes" %}
+  "hypothesis >= 6.0",
+{%- endif -%}
+{%- if cookiecutter.use_coverage == "yes" %}
+  "coverage >= 7.2.7",
+{%- endif -%}
+{%- if cookiecutter.use_black == "yes" %}
+  "black >= 23.3.0,<23.10",
+{%- endif -%}
+{%- if cookiecutter.use_isort == "yes" %}
+  "isort >= 5.12.0",
+{%- endif -%}
+{%- if cookiecutter.use_pre_commit %}
+  "pre-commit >= 3.3.2",
+{%- endif -%}
+{%- if cookiecutter.use_flake8 == "yes" %}
+  "flake8 >= 4.0.1, < 7",
+{%- endif -%}
+{%- if cookiecutter.use_ruff == "yes" %}
+  "ruff >= 0.2.0",
+{%- endif -%}
+{%- if cookiecutter.use_mypy == "yes" %}
+  "mypy >= 1.5.0",
+{%- endif -%}
+{%- if cookiecutter.use_bandit == "yes" %}
+  "bandit >= 1.7.5",
+{%- endif -%}
+{%- if cookiecutter.use_pydocstyle == "yes" %}
+  "pydocstyle >= 6.3.0",
+{%- endif -%}
+{%- if cookiecutter.use_makim == "yes" %}
+  "makim == 1.15.1",
+{%- endif -%}
+{%- if cookiecutter.use_vulture == "yes" %}
+  "vulture >= 2.7",
+{%- endif -%}
+{%- if cookiecutter.use_mccabe == "yes" %}
+  "mccabe >= 0.6.1",
+{%- endif -%}
+{%- if cookiecutter.use_containers in ['Docker', 'Podman'] %}
 # if you want to use docker-compose from your system, remove compose-go here
-    "compose-go >= 2.18.1",
-{% endif %}
-    "ipython < 8",
-    "ipykernel >=6.0.0",
+  "compose-go >= 2.18.1",
+{%- endif %}
+  "ipython < 8",
+  "ipykernel >=6.0.0",
 {%- if cookiecutter.documentation_engine == 'mkdocs' %}
-    "Jinja2 >= 3.1.2",
-    "mkdocs >= 1.4.3",
-    "mkdocs-exclude >= 1.0.2",
-    "mkdocs-jupyter >= 0.24.1",
-    "mkdocs-literate-nav >= 0.6.0",
-    "mkdocs-macros-plugin >= 0.7.0, < 1",
-    "mkdocs-material >= 9.1.15",
-    "mkdocstrings >= 0.21.2",
-    "mkdocstrings-python >= 1.1.2",
-{% elif cookiecutter.documentation_engine == 'sphinx' -%}
-    "Sphinx >= 6.2.1",
-    "sphinx-rtd-theme >= 1.2.2",
-    "importlib-metadata >= 6.5.1",
-    "myst-parser >= 0.19.2",
-    "nbsphinx >= 0.9.2",
-    "pandoc >= 2.3",
-{% elif cookiecutter.documentation_engine == 'jupyter-book' -%}
-    "jupyter-book >= 0.15.1",
-    "myst-parser >= 0.18.1",
-{% endif %}
-{%- if cookiecutter.use_makim == "yes" %}
-    "makim>=1.14.0,<1.15",
-{% endif %}
+  "Jinja2 >= 3.1.2",
+  "mkdocs >= 1.4.3",
+  "mkdocs-exclude >= 1.0.2",
+  "mkdocs-jupyter >= 0.24.1",
+  "mkdocs-literate-nav >= 0.6.0",
+  "mkdocs-macros-plugin >= 0.7.0, < 1",
+  "mkdocs-material >= 9.1.15",
+  "mkdocstrings >= 0.21.2",
+  "mkdocstrings-python >= 1.1.2",
+{%- elif cookiecutter.documentation_engine == 'sphinx' %}
+  "Sphinx >= 6.2.1",
+  "sphinx-rtd-theme >= 1.2.2",
+  "importlib-metadata >= 6.5.1",
+  "myst-parser >= 0.19.2",
+  "nbsphinx >= 0.9.2",
+  "pandoc >= 2.3",
+{%- elif cookiecutter.documentation_engine == 'jupyter-book' %}
+  "jupyter-book >= 0.15.1",
+  "myst-parser >= 0.18.1",
+{%- elif cookiecutter.documentation_engine == 'quarto' %}
+  "quarto-cli >= 1.4.550",
+  "quartodoc >= 0.7.2",
+{%- endif %}
+  # 'PosixPath' object has no attribute 'endswith'
+  "virtualenv<=20.25.1",
 ]
 
 [project.urls]
 Homepage = "{{ cookiecutter.project_url }}"
 "Bug Tracker" = "{{ cookiecutter.project_url }}/issues"
 Discussions = "{{ cookiecutter.project_url }}/discussions"
 Changelog = "{{ cookiecutter.project_url }}/releases"
-
-{% include "build-system/base-pyproject.toml" %}
 {#- keep this line at the end of the file -#}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/lib.rs`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/main.cpp`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry-pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,88 +2,89 @@
 {% set package_path = "src/" + cookiecutter.package_slug -%}
 {% else -%}
 {% set package_path = cookiecutter.package_slug -%}
 {% endif -%}
 
 [tool.poetry]
 name = "{{ cookiecutter.project_slug }}"
-version = "{{ cookiecutter.project_version }}"  # semantic-release
+version = "{{ cookiecutter.project_version }}" #semantic-release
 description = "{{ cookiecutter.project_short_description }}"
 readme = "README.md"
 authors = ["{{ cookiecutter.author_full_name }} <{{ cookiecutter.author_email }}>"]
 {% if cookiecutter.project_layout == "src" -%}
 packages = [
   {include = "{{ cookiecutter.package_slug }}", from="src"},
 ]
-{% else -%}
+{%- else -%}
 packages = [
   {include = "{{ cookiecutter.package_slug }}"},
 ]
-{% endif -%}
+{% endif %}
 license = "{{ cookiecutter.project_license }}"
 exclude = [
   ".git/*",
   ".env*",
 ]
 {%- if cookiecutter.use_mypy == "yes" %}
 include = ["{{ package_path }}/py.typed"]
-{%- endif %}
-
+{% endif %}
 {% if cookiecutter.command_line_interface != "None" -%}
 [tool.poetry.scripts]
 "{{ cookiecutter.project_slug }}" = "{{ cookiecutter.package_slug }}.__main__:app"
-{%- endif %}
-
+{% endif -%}
+{# keep this line here #}
 [tool.poetry.dependencies]
+{%- if cookiecutter.documentation_engine == 'quarto' %}
+python = ">=3.9,<4"
+{% else %}
 python = ">=3.8.1,<4"
-
-[tool.poetry.dev-dependencies]
-{# keep this line here #}
-{%- if cookiecutter.use_pytest == "yes" -%}
+{% endif %}
+[tool.poetry.group.dev.dependencies]
+{% if cookiecutter.use_pytest == "yes" -%}
 pytest = ">=7.3.2"
 {% if cookiecutter.use_coverage == "yes" -%}
 pytest-cov = ">=4.1.0"
-{% endif %}
+{% endif -%}
 {%- endif -%}{#- end of use_pytest -#}
 {%- if cookiecutter.use_hypothesis == "yes" -%}
 hypothesis = ">=6.0"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_coverage == "yes" -%}
 coverage = ">=7.2.7"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_black == "yes" -%}
 black = ">=23.3.0,<23.10"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_isort == "yes" -%}
 isort = ">=5.12.0"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_pre_commit -%}
 pre-commit = ">=3.3.2"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_flake8 == "yes" -%}
 flake8 = ">=4.0.1, <7"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_ruff == "yes" -%}
 ruff = ">=0.2.0"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_mypy == "yes" -%}
 mypy = ">=1.5.0"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_bandit == "yes" -%}
 bandit = ">=1.7.5"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_pydocstyle == "yes" -%}
 pydocstyle = ">=6.3.0"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_vulture == "yes" -%}
 vulture = ">=2.7"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_mccabe == "yes" -%}
 mccabe = ">=0.6.1"
-{% endif %}
+{% endif -%}
 {%- if cookiecutter.use_containers in ['Docker', 'Podman'] -%}
 # if you want to use docker-compose from your system, remove compose-go here
 compose-go = ">=2.18.1"
 {% endif -%}
 ipython = "<8"
 ipykernel = ">=6.0.0"
 {%- if cookiecutter.documentation_engine == 'mkdocs' %}
@@ -92,24 +93,32 @@
 mkdocs-exclude = ">=1.0.2"
 mkdocs-jupyter = ">=0.24.1"
 mkdocs-literate-nav = ">=0.6.0"
 mkdocs-macros-plugin = ">=0.7.0,<1"
 mkdocs-material = ">=9.1.15"
 mkdocstrings = ">=0.21.2"
 mkdocstrings-python = ">=1.1.2"
+{# keep this line here #}
 {%- elif cookiecutter.documentation_engine == 'sphinx' %}
 Sphinx = ">=6.2.1"
 sphinx-rtd-theme = ">=1.2.2"
 importlib-metadata = ">=6.5.1"
 myst-parser = ">=0.19.2"
 nbsphinx = ">=0.9.2"
 pandoc = ">=2.3"
+{# keep this line here #}
 {%- elif cookiecutter.documentation_engine == 'jupyter-book' %}
 jupyter-book = ">=0.15.1"
 myst-parser = ">=0.18.1"
-{% endif %}
-{%- if cookiecutter.use_makim == "yes" %}
-makim = ">=1.14.0,<1.15"
-{% endif %}
+{# keep this line here #}
+{%- elif cookiecutter.documentation_engine == 'quarto' %}
+quarto-cli = ">=1.4.550"
+quartodoc = ">=0.7.2"
+{% endif -%}
+{%- if cookiecutter.use_makim == "yes" -%}
+makim = "1.15.1"
+{% endif -%}
+# 'PosixPath' object has no attribute 'endswith'
+virtualenv = "<=20.25.1"
 
 {% include "build-system/base-pyproject.toml" %}
 {#- keep this line at the end of the file -#}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files 18% similar despite different names*

```diff
@@ -108,134 +108,156 @@
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
   welcome :)
 
 ## Get Started!
 
-Ready to contribute? Here’s how to set up `{{ cookiecutter.project_slug}}` for local
+Ready to contribute? Here’s how to set up `{{ cookiecutter.project_slug }}` for local
 development.
 
 1.  Fork the `{{ cookiecutter.project_slug }}` repo on GitHub.
-
-2.  Clone your fork locally:
-
-    ```
-    git clone git@github.com:your_name_here/{{ cookiecutter.project_slug }}.git
-    ```
-
-3.  Install your local copy into a virtualenv. This is how you set up your fork
-    for local development:
-
-    ```
-    cd {{cookiecutter.project_slug }}/
-    python -m venv env
-    ```
-
-    Using poetry:
-
-    ```
-    poetry install --with dev
-    ```
-
-    To get poetry, just pip install it into your virtualenv.
-
-    Alternatively, using pip:
-
-    ```
-    pip install -e .
-    ```
-
-4.  Create a branch for local development:
-
-    ```
-    git checkout -b name-of-your-bugfix-or-feature
-    ```
-
-    Now you can make your changes locally.
-
-5.  `{{ cookiecutter.project_slug }}` uses a set of `pre-commit` hooks and the `pre-commit`
-    bot to format, type-check, and prettify the codebase. The hooks can be
-    installed locally using -
-
-    ```
-    pre-commit install
-    ```
-
-    This would run the checks every time a commit is created locally. The checks
-    will only run on the files modified by that commit, but the checks can be
-    triggered for all the files using -
-
-    ```
-    pre-commit run --all-files
-    ```
-
-    If you would like to skip the failing checks and push the code for further
-    discussion, use the `--no-verify` option with `git commit`.
-
-6.  `{{ cookiecutter.project_slug }}` is tested with `pytest`. `pytest` is responsible for
-    testing the code, whose configuration is available in pyproject.toml.
-    Additionally, `{{ cookiecutter.project_slug }}` also uses `pytest-cov` to calculate the
-    coverage of these unit tests.
-
-    #### Running tests locally
-
-    The tests can be executed using the `test` dependencies of
-    `{{ cookiecutter.project_slug }}` in the following way -
-
-    ```
-    python -m pytest
-    ```
-
-    #### Running tests with coverage locally
-
-    The coverage value can be obtained while running the tests using
-    `pytest-cov` in the following way -
-
-    ```
-    python -m pytest --cov={{ cookiecutter.project_slug }} tests/
-    ```
-
-    A much more detailed guide on testing with `pytest` is available
-    [here](https://docs.pytest.org/en/8.0.x/how-to/index.html).
-
-7.  Commit your changes and push your branch to GitHub::
-
-    ```
-    git add .
-    git commit -m “Your detailed description of your changes.”
-    git push origin name-of-your-bugfix-or-feature
-    ```
-
-8.  Submit a pull request through the GitHub website.
+1.  Clone your fork locally and change to the directory of your project:
+```bash
+$ git clone git@github.com:your_name_here/{{ cookiecutter.project_slug }}.git
+$ cd {{cookiecutter.project_slug }}/
+```
+{% if cookiecutter.git_https_upstream -%}
+Also, create a remote to the upstream repository, you will need that later:
+```bash
+$ git remote add upstream {{ cookiecutter.git_https_upstream }}
+$ git fetch --all
+```
+{% endif -%}
+1.  Prepare and use virtual environment:
+{%- if cookiecutter.use_conda == "yes" %}
+If you don't have yet conda installed in your machine, you can check the
+installation steps here:
+<https://github.com/conda-forge/miniforge?tab=readme-ov-file#download>
+After that, ensure that conda is already available in your terminal session and
+run:
+```bash
+$ conda env create env create --file conda/dev.yaml
+$ conda activate {{ cookiecutter.package_slug }}
+```
+Note: you can use `mamba env create` instead, if you have it already installed,
+in order to boost the installation step.
+{% elif cookiecutter.use_pyenv == "yes" -%}
+Create your environment using `virtualenv`:
+```bash
+$ virtualenv {{ cookiecutter.package_slug }}
+$ source {{ cookiecutter.package_slug }}/bin/activate
+```
+{% else -%}
+We highly recommend you to use `conda` for managing virtual environment, but
+you can use any other one of your preference.
+{% endif -%}
+1. Install the dependencies:
+Now, you can already install the dependencies for the project:
+{% if cookiecutter.build_system == "poetry" -%}
+```bash
+$ poetry install
+```
+{%- elif cookiecutter.build_system == "pdm" -%}
+```bash
+$ pdm install
+```
+{%- elif cookiecutter.build_system == "flit" -%}
+```bash
+$ flit install
+```
+{%- else -%}
+```bash
+$ pip install -e ".[dev]"
+```
+{%- endif -%}
+{% if cookiecutter.use_pre_commit == "yes" %}
+1.  `{{ cookiecutter.project_slug }}` uses a set of `pre-commit` hooks to
+improve code quality. The hooks can be installed locally using:
+```bash
+$ pre-commit install
+```
+This would run the checks every time a `git commit` is executed locally.
+Usually, the verification will only run on the files modified by that commit,
+but the verification can also be triggered for all the files using:
+```bash
+$ pre-commit run --all-files
+```
+If you would like to skip the failing checks and push the code for further
+discussion, use the `--no-verify` option with `git commit`.
+{% endif -%}
+{% if cookiecutter.use_pytest == "yes" %}
+1.  This project uses `pytest` as a testing tool. `pytest` is responsible for
+testing the code, whose configuration is available in pyproject.toml.
+Additionally, this project also uses `pytest-cov` to calculate the coverage of
+these unit tests. For more information, check the section about tests later in
+this document.
+{% elif cookiecutter.use_hypothesis == "yes" %}
+1.  This project uses `hypothesis` as a testing tool. For more information,
+please check its official documentation <https://hypothesis.readthedocs.io/>
+{% endif -%}
+1.  Commit your changes and push your branch to GitHub::
+```
+$ git add .
+$ git commit -m "Your detailed description of your changes.""
+$ git push origin name-of-your-bugfix-or-feature
+```
+1.  Submit a pull request through the GitHub website.
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1.  The pull request should include tests.
 2.  If the pull request adds functionality, the docs should be updated. Put your
     new functionality into a function with a docstring, and add the feature to
     the list in README.rst.
 3.  The pull request should work for Python >= 3.8.
 
-## Tips
+{% if cookiecutter.use_pytest == "yes" -%}
+## Running tests locally
 
-To run a subset of tests:
+The tests can be executed using the `test` dependencies of
+`{{ cookiecutter.project_slug }}` in the following way:
 
-{% if cookiecutter.use_pytest == "yes" -%}
+```bash
+$ python -m pytest
 ```
-pytest tests.test_{{ cookiecutter.package_slug }}
+
+{% if cookiecutter.use_coverage == "yes" -%}
+### Running tests with coverage locally
+
+The coverage value can be obtained while running the tests using
+`pytest-cov` in the following way:
+
+```bash
+$ python -m pytest --cov={{ cookiecutter.project_slug }} tests/
 ```
+
+A much more detailed guide on testing with `pytest` is available
+[here](https://docs.pytest.org/en/8.0.x/how-to/index.html).
 {%- endif %}
-{% if cookiecutter.use_hypothesis == "yes" -%}
-```
-python -m unittest discover
+{%- endif %}
+
+{% if cookiecutter.use_makim == "yes" -%}
+## Automation Tasks with Makim
+
+This project uses `makim` as  an automation tool. Please, check the
+`.makim.yaml` file to check all the tasks available or run:
+
+```bash
+$ makim --help
 ```
+{% elif cookiecutter.use_make == "yes" -%}
+## Automation Tasks with Make
+
+This project uses `make` as  an automation tool. Please, check the `Makefile`
+to check all the tasks (targets) available.
 {%- endif %}
+
 ## Release
 
 This project uses semantic-release in order to cut a new release based on the
 commit-message.
 
 ### Commit message format
 
@@ -262,14 +284,16 @@
 `semantic-release` runs (using the default configuration):
 
 | Commit message                                                 | Release type     |
 | -------------------------------------------------------------- | ---------------- |
 | `fix(pencil): stop graphite breaking when pressure is applied` | Fix Release      |
 | `feat(pencil): add 'graphiteWidth' option`                     | Feature Release  |
 | `perf(pencil): remove graphiteWidth option`                    | Chore            |
-| `BREAKING CHANGE: The graphiteWidth option has been removed`   | Breaking Release |
+| `feat(pencil)!: The graphiteWidth option has been removed`     | Breaking Release |
+
+Note: For a breaking change release, uses `!` at the end of the message prefix.
 
 source:
 <https://github.com/semantic-release/semantic-release/blob/master/README.md#commit-message-format>
 
 As this project uses the `squash and merge` strategy, ensure to apply the commit
 message format to the PR's title.
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.package_slug}}.py` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """{{ cookiecutter.project_name }}."""
-{%- if cookiecutter.use_mypy == "yes" %}
-# mypy: disable-error-code="attr-defined"
-{%- endif %}
 {%- if cookiecutter.use_black == "yes" %}
   {%- set QUOTE = '"' -%}
 {%- else %}
   {%- set QUOTE = "'" -%}
 {%- endif %}
 {% if cookiecutter.build_system == "hatch" -%}
 __version__ = {{ QUOTE }}{{ cookiecutter.project_version }}{{ QUOTE }}
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 """
 {%- if cookiecutter.use_black == "yes" %}
   {%- set QUOTE = '"' -%}
 {%- else %}
   {%- set QUOTE = "'" -%}
 {%- endif %}
 
-from {{cookiecutter.package_slug}}.cli import main  # type: ignore
+from {{cookiecutter.package_slug}}.cli import main
 
 if __name__ == {{ QUOTE }}__main__{{ QUOTE }}:
     main()
```

### Comparing `scicookie-0.7.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py` & `scicookie-0.8.0/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.7.2/PKG-INFO` & `scicookie-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.7.2
+Version: 0.8.0
 Summary: Cookiecutter template for a Python package
 License: BSD-3-Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 ![CI](https://img.shields.io/github/actions/workflow/status/osl-incubator/scicookie/main.yaml?logo=github&label=CI)
 [![Python Versions](https://img.shields.io/pypi/pyversions/scicookie)](https://pypi.org/project/scicookie/)
 [![Package Version](https://img.shields.io/pypi/v/scicookie?color=blue)](https://pypi.org/project/scicookie/)
 ![License](https://img.shields.io/pypi/l/scicookie?color=blue)
 ![Discord](https://img.shields.io/discord/796786891798085652?logo=discord&color=blue)
 
-![logo_scicookie.png](images%2Flogo_scicookie.png)
+![logo_scicookie.png](https://github.com/osl-incubator/scicookie/blob/main/docs/images/logo_scicookie.png?raw=true)
 
 **SciCookie** is a project template designed to simplify scientific Python
 project creation. It provides an initial structure with recommended tools,
 workflows, and industry best practices, saving developers time and effort. Built
 upon the PyOpenSci recommendations, it offers a foundation that adheres to
 scientific Python standards while remaining customizable to specific project
 needs.
@@ -49,15 +49,15 @@
 - **Testing & Linting:** Integrates with pytest, hypothesis, black
   (auto-formatting), bandit (security), pydocstyle (documentation style),
   vulture (unused code detection), and McCabe (cyclomatic complexity analysis)
   for a robust development environment.
 - **Version Control & Automation:** Includes initial git integration, conda
   (base environment) support, pre-commit hooks, continuous integration with
   GitHub Actions, and release workflows with semantic-release.
-- **Documentation:** Offers options for mkdocs, sphinx, or jupyter-book
+- **Documentation:** Offers options for mkdocs, sphinx, jupyter-book or quarto
   documentation generation.
 - **Containerization:** Provides the ability to add initial files for running
   and managing containers using Docker or Podman.
 
 ### Benefits:
 
 - **Reduces boilerplate code:** SciCookie eliminates the need to write
```

