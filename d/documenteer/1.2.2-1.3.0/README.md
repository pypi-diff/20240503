# Comparing `tmp/documenteer-1.2.2.tar.gz` & `tmp/documenteer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-1.2.2.tar", last modified: Thu Apr 11 19:23:41 2024, max compression
+gzip compressed data, was "documenteer-1.3.0.tar", last modified: Fri May  3 16:02:47 2024, max compression
```

## Comparing `documenteer-1.2.2.tar` & `documenteer-1.3.0.tar`

### file list

```diff
@@ -1,314 +1,319 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.972368 documenteer-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 19:23:26.000000 documenteer-1.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-11 19:23:26.000000 documenteer-1.2.2/.github/workflows/dependencies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-11 19:23:26.000000 documenteer-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 19:23:26.000000 documenteer-1.2.2/.npmrc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 19:23:26.000000 documenteer-1.2.2/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 19:23:26.000000 documenteer-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 19:23:26.000000 documenteer-1.2.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 19:23:26.000000 documenteer-1.2.2/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 19:23:26.000000 documenteer-1.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-11 19:23:26.000000 documenteer-1.2.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)    39095 2024-04-11 19:23:26.000000 documenteer-1.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-11 19:23:26.000000 documenteer-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 19:23:26.000000 documenteer-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-11 19:23:26.000000 documenteer-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-11 19:23:41.972368 documenteer-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-11 19:23:26.000000 documenteer-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 19:23:26.000000 documenteer-1.2.2/changelog.d/_template.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.924368 documenteer-1.2.2/demo/ipynb-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/ipynb-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/demo/md-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/md-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    39095 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.928368 documenteer-1.2.2/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.932368 documenteer-1.2.2/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.932368 documenteer-1.2.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/including-notebooks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/markdown-primer.md
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.936368 documenteer-1.2.2/docs/guides/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pipelines/stack-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.936368 documenteer-1.2.2/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/githubbibcache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/openapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/docs/technotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/docs/technotes/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/_templates/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/author-metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/document-status.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/edit-locally.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/edit-on-github.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/how-your-technote-gets-published.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-11 19:23:26.000000 documenteer-1.2.2/docs/technotes/start-a-technote.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-11 19:23:26.000000 documenteer-1.2.2/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-04-11 19:23:34.000000 documenteer-1.2.2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-11 19:23:26.000000 documenteer-1.2.2/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 19:23:26.000000 documenteer-1.2.2/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-11 19:23:26.000000 documenteer-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:23:41.972368 documenteer-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.940368 documenteer-1.2.2/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_article-header.scss
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_authors.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_sidebar-section.scss
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.944368 documenteer-1.2.2/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/731c8feefe13e72a8691.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/rubin-technote.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-11 19:23:36.000000 documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.948368 documenteer-1.2.2/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/conf/technote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/githubbibcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/ext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.952368 documenteer-1.2.2/src/documenteer/services/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/technoteauthor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/services/technotemigration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.956368 documenteer-1.2.2/src/documenteer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/authordb.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.916368 documenteer-1.2.2/src/documenteer/storage/localtemplates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/localtemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/storage/technotetoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/components/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/components/sidebar-source.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.960368 documenteer-1.2.2/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-11 19:23:26.000000 documenteer-1.2.2/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 19:23:41.000000 documenteer-1.2.2/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/authordb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.964368 documenteer-1.2.2/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/autocppapi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/jira_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lsstdocushare_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/ext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/lssttasks/taskutils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/mockcoderefs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/packagetoctree_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/ext/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/packagemetadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.920368 documenteer-1.2.2/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/roots/test-autocppapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/services/technotemigration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:41.968368 documenteer-1.2.2/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/authordb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/storage/technotetoml_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-11 19:23:26.000000 documenteer-1.2.2/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-11 19:23:26.000000 documenteer-1.2.2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 19:23:26.000000 documenteer-1.2.2/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.019647 documenteer-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 16:02:31.000000 documenteer-1.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.967647 documenteer-1.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.967647 documenteer-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 16:02:31.000000 documenteer-1.3.0/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-03 16:02:31.000000 documenteer-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 16:02:31.000000 documenteer-1.3.0/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 16:02:31.000000 documenteer-1.3.0/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 16:02:31.000000 documenteer-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 16:02:31.000000 documenteer-1.3.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 16:02:31.000000 documenteer-1.3.0/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.967647 documenteer-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 16:02:31.000000 documenteer-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-03 16:02:31.000000 documenteer-1.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41327 2024-05-03 16:02:31.000000 documenteer-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-03 16:02:31.000000 documenteer-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 16:02:31.000000 documenteer-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 16:02:31.000000 documenteer-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-03 16:02:47.015647 documenteer-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-03 16:02:31.000000 documenteer-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.967647 documenteer-1.3.0/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 16:02:31.000000 documenteer-1.3.0/changelog.d/_template.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.959647 documenteer-1.3.0/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.971647 documenteer-1.3.0/demo/ipynb-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/extra-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.971647 documenteer-1.3.0/demo/ipynb-technote/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/subdir/subdir-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/ipynb-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.971647 documenteer-1.3.0/demo/md-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/md-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.971647 documenteer-1.3.0/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 16:02:31.000000 documenteer-1.3.0/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.971647 documenteer-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    41327 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.975647 documenteer-1.3.0/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.975647 documenteer-1.3.0/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.979647 documenteer-1.3.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/including-notebooks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/markdown-primer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/page-redirects.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.979647 documenteer-1.3.0/docs/guides/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pipelines/stack-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/guides/video-embeds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.979647 documenteer-1.3.0/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/githubbibcache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.983647 documenteer-1.3.0/docs/technotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.983647 documenteer-1.3.0/docs/technotes/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/_templates/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/author-metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/document-status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/edit-locally.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/edit-on-github.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/how-your-technote-gets-published.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-03 16:02:31.000000 documenteer-1.3.0/docs/technotes/start-a-technote.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.983647 documenteer-1.3.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 16:02:31.000000 documenteer-1.3.0/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-03 16:02:31.000000 documenteer-1.3.0/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-03 16:02:31.000000 documenteer-1.3.0/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-05-03 16:02:31.000000 documenteer-1.3.0/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   212497 2024-05-03 16:02:40.000000 documenteer-1.3.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-03 16:02:31.000000 documenteer-1.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 16:02:31.000000 documenteer-1.3.0/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-03 16:02:31.000000 documenteer-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:02:47.019647 documenteer-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.959647 documenteer-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.959647 documenteer-1.3.0/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.959647 documenteer-1.3.0/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.983647 documenteer-1.3.0/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.987647 documenteer-1.3.0/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_article-header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_authors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_sidebar-section.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.987647 documenteer-1.3.0/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.991647 documenteer-1.3.0/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   137996 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/731c8feefe13e72a8691.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   170188 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/b8bc3440ba2145e132f5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.991647 documenteer-1.3.0/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11494 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/rubin-technote.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.991647 documenteer-1.3.0/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-03 16:02:41.000000 documenteer-1.3.0/src/documenteer/assets/scripts/rubin-technote.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.991647 documenteer-1.3.0/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17998 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/conf/technote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.995647 documenteer-1.3.0/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/githubbibcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.995647 documenteer-1.3.0/src/documenteer/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39797 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/ext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.995647 documenteer-1.3.0/src/documenteer/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/services/technoteauthor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/services/technotemigration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.999647 documenteer-1.3.0/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.999647 documenteer-1.3.0/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1063166 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   105749 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (127)    23844 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.999647 documenteer-1.3.0/src/documenteer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/authordb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/src/documenteer/storage/localtemplates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.003647 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/localtemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/storage/technotetoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.003647 documenteer-1.3.0/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.003647 documenteer-1.3.0/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.003647 documenteer-1.3.0/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/components/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/components/sidebar-source.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.003647 documenteer-1.3.0/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 16:02:31.000000 documenteer-1.3.0/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.011647 documenteer-1.3.0/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 16:02:46.000000 documenteer-1.3.0/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    82475 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/authordb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.007647 documenteer-1.3.0/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/autocppapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/jira_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/lsstdocushare_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.011647 documenteer-1.3.0/tests/ext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/lssttasks/taskutils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/mockcoderefs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/packagetoctree_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/ext/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/packagemetadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:46.963647 documenteer-1.3.0/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.011647 documenteer-1.3.0/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199942 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/roots/test-autocppapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.011647 documenteer-1.3.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/services/technotemigration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:47.011647 documenteer-1.3.0/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/storage/authordb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/storage/technotetoml_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-03 16:02:31.000000 documenteer-1.3.0/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-03 16:02:31.000000 documenteer-1.3.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 16:02:31.000000 documenteer-1.3.0/webpack.config.js
```

### Comparing `documenteer-1.2.2/.github/workflows/ci-cron.yaml` & `documenteer-1.3.0/.github/workflows/ci-cron.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/.github/workflows/ci.yaml` & `documenteer-1.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/.github/workflows/dependencies.yaml` & `documenteer-1.3.0/.github/workflows/dependencies.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/.gitignore` & `documenteer-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/.pre-commit-config.yaml` & `documenteer-1.3.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-yaml
         exclude: ^src/documenteer/storage/localtemplates/technote/ci\.yaml
       - id: check-toml
       - id: check-json
       - id: trailing-whitespace
 
@@ -18,20 +18,20 @@
     rev: 5.13.2
     hooks:
       - id: isort
         additional_dependencies:
           - toml
 
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.14.0
+    rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.12.0]
         args: [-l, '79', -t, py38]
 
   - repo: https://github.com/pycqa/flake8
     rev: 7.0.0
```

### Comparing `documenteer-1.2.2/.vscode/tasks.json` & `documenteer-1.3.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/CHANGELOG.md` & `documenteer-1.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.3.0'></a>
+## 1.3.0 (2024-05-03)
+
+### New features
+
+- Added a `[sphinx.redirects]` table to `documenteer.toml`. This provides support for configuring page redirects from the TOML configuratin. Redirects are useful if pages move because of a content re-organization. This feature is based on [sphinx-rediraffe](https://github.com/wpilibsuite/sphinxext-rediraffe).
+
+- Added the [sphinxcontrib-youtube](https://sphinxcontrib-youtube.readthedocs.io/en/latest/index.html) for embedded YouTube and Vimeo videos into documentation pages. This extension is available for both user guides (`documenteer.conf.guide`) and technotes (`documenteer.conf.technotes`).
+
+### Bug fixes
+
+- Technotes ignore files in the repository with `.md`, `.rst`, and `.ipynb` extensions if they aren't the index file. Since technotes are single-page documents, only the index file should be used as a source file. This change lets authors include auxiliary notebooks with their technotes without having to explicitly exclude them from the technote build process. This is implemented with `technote.conf.extend_excludes_for_non_index_source`.
+
+- In `documenteer.ext.lssttasks`, attempt to import `_pseudo_parse_arglist` from `sphinx.domains.python._annotations` before falling back to the `sphinx.domains.python` module. Ultimately this is a workaround.
+
+- Fix setting the rebuild condition for the `documenteer.ext.githubbibcache` extension.
+
+- Fixed the monospace text baseline alignment issue in Safari for technotes by updating to technote 0.8.0. In this version, the font size of the code is set to be 0.9em so that the browser doesn't push the text below the baseline in case its larger than the Source Sans body text. This version also changes the font size on the html element to 100% and instead increases the baseline body text size to 1.1rem on the body element. This change should help technotes respect the user's browser font size settings while also making the rem unit work as expected.
+
+### Other changes
+
+- Added `defusedxml` as a dev dependency. This is used by Sphinx's `sphinx.testing.fixtures`, but isn't included as a dependency by Sphinx itself. This change ensures that `defusedxml` is installed when running the tests.
+
 <a id='changelog-1.2.2'></a>
 ## 1.2.2 (2024-04-11)
 
 ### Bug fixes
 
 - Update `jira_uri_template` configuration default to `https://rubinobs.atlassian.net/browse/{issue}`. This will make all :jira:, :jirab:, and :jirap: roles point to the new Jira instance for Rubin Observatory.
 - Drop `jira.lsstcorp.org` from the linkcheck ignore list defaults for `documenteer.config.guide` since that instance is no longer being used.
```

### Comparing `documenteer-1.2.2/LICENSE` & `documenteer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/PKG-INFO` & `documenteer-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.2
+Version: 1.3.0
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -57,14 +57,15 @@
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: lxml; extra == "dev"
 Requires-Dist: cssselect; extra == "dev"
+Requires-Dist: defusedxml; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinxcontrib-autoprogram; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-docutils; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
@@ -80,14 +81,15 @@
 Requires-Dist: myst-nb; extra == "guide"
 Requires-Dist: markdown-it-py[linkify]; extra == "guide"
 Requires-Dist: sphinxcontrib-mermaid; extra == "guide"
 Requires-Dist: sphinxext-opengraph; extra == "guide"
 Requires-Dist: sphinxcontrib-redoc; extra == "guide"
 Requires-Dist: sphinxcontrib-jquery; extra == "guide"
 Requires-Dist: sphinxext-rediraffe; extra == "guide"
+Requires-Dist: sphinxcontrib-youtube; extra == "guide"
 Provides-Extra: pipelines
 Requires-Dist: sphinx_design; extra == "pipelines"
 Requires-Dist: pydata-sphinx-theme<0.13.0,>=0.10.0; extra == "pipelines"
 Requires-Dist: sphinx-autodoc-typehints; extra == "pipelines"
 Requires-Dist: sphinx-automodapi; extra == "pipelines"
 Requires-Dist: sphinx-copybutton; extra == "pipelines"
 Requires-Dist: sphinx-prompt; extra == "pipelines"
@@ -98,20 +100,21 @@
 Requires-Dist: sphinxext-opengraph; extra == "pipelines"
 Requires-Dist: sphinxcontrib-redoc; extra == "pipelines"
 Requires-Dist: sphinxcontrib-jquery; extra == "pipelines"
 Requires-Dist: sphinxcontrib-autoprogram; extra == "pipelines"
 Requires-Dist: sphinxcontrib-doxylink; extra == "pipelines"
 Requires-Dist: sphinx-click; extra == "pipelines"
 Provides-Extra: technote
-Requires-Dist: technote<0.8.0,>=0.7.0; extra == "technote"
+Requires-Dist: technote<0.9.0,>=0.8.0; extra == "technote"
 Requires-Dist: sphinx-prompt; extra == "technote"
 Requires-Dist: sphinxcontrib-mermaid; extra == "technote"
 Requires-Dist: sphinx-diagrams; extra == "technote"
 Requires-Dist: sphinx_design; extra == "technote"
 Requires-Dist: myst-nb; extra == "technote"
+Requires-Dist: sphinxcontrib-youtube; extra == "technote"
 
 [![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
```

### Comparing `documenteer-1.2.2/README.md` & `documenteer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/demo/ipynb-technote/index.ipynb` & `documenteer-1.3.0/demo/ipynb-technote/extra-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/demo/ipynb-technote/technote.toml` & `documenteer-1.3.0/demo/ipynb-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/demo/md-technote/index.md` & `documenteer-1.3.0/demo/md-technote/index.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/demo/md-technote/technote.toml` & `documenteer-1.3.0/demo/md-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/demo/rst-technote/index.rst` & `documenteer-1.3.0/demo/rst-technote/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Introduction
 ============
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
-A parenthetical citation :cite:p:`SQR-083`. And a textual citation :cite:t:`SQR-083`.
+A parenthetical citation :cite:p:`SQR-083`. And a textual citation :cite:t:`SQR-083`. Some ``source code`` embedded in text.
 
 Method
 ======
 
 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. Proin semper mollis enim eget interdum. Mauris eleifend eget diam vitae bibendum. Praesent ut aliquet odio, sodales imperdiet nisi. Nam interdum imperdiet tortor sed fringilla. Maecenas efficitur mi sodales nulla commodo rutrum. Ut ornare diam quam, sed commodo turpis aliquam et. In nec enim consequat, suscipit tortor sit amet, luctus ante. Integer dictum augue diam, non pulvinar massa euismod in. Morbi viverra condimentum auctor. Nullam et metus mauris. Cras risus ex, porta sit amet nibh et, dapibus auctor leo.
 
 A list:
```

### Comparing `documenteer-1.2.2/demo/rst-technote/technote.toml` & `documenteer-1.3.0/demo/rst-technote/technote.toml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/Makefile` & `documenteer-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/_rst_epilog.rst` & `documenteer-1.3.0/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/changelog.md` & `documenteer-1.3.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # Change Log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-1.3.0'></a>
+## 1.3.0 (2024-05-03)
+
+### New features
+
+- Added a `[sphinx.redirects]` table to `documenteer.toml`. This provides support for configuring page redirects from the TOML configuratin. Redirects are useful if pages move because of a content re-organization. This feature is based on [sphinx-rediraffe](https://github.com/wpilibsuite/sphinxext-rediraffe).
+
+- Added the [sphinxcontrib-youtube](https://sphinxcontrib-youtube.readthedocs.io/en/latest/index.html) for embedded YouTube and Vimeo videos into documentation pages. This extension is available for both user guides (`documenteer.conf.guide`) and technotes (`documenteer.conf.technotes`).
+
+### Bug fixes
+
+- Technotes ignore files in the repository with `.md`, `.rst`, and `.ipynb` extensions if they aren't the index file. Since technotes are single-page documents, only the index file should be used as a source file. This change lets authors include auxiliary notebooks with their technotes without having to explicitly exclude them from the technote build process. This is implemented with `technote.conf.extend_excludes_for_non_index_source`.
+
+- In `documenteer.ext.lssttasks`, attempt to import `_pseudo_parse_arglist` from `sphinx.domains.python._annotations` before falling back to the `sphinx.domains.python` module. Ultimately this is a workaround.
+
+- Fix setting the rebuild condition for the `documenteer.ext.githubbibcache` extension.
+
+- Fixed the monospace text baseline alignment issue in Safari for technotes by updating to technote 0.8.0. In this version, the font size of the code is set to be 0.9em so that the browser doesn't push the text below the baseline in case its larger than the Source Sans body text. This version also changes the font size on the html element to 100% and instead increases the baseline body text size to 1.1rem on the body element. This change should help technotes respect the user's browser font size settings while also making the rem unit work as expected.
+
+### Other changes
+
+- Added `defusedxml` as a dev dependency. This is used by Sphinx's `sphinx.testing.fixtures`, but isn't included as a dependency by Sphinx itself. This change ensures that `defusedxml` is installed when running the tests.
+
 <a id='changelog-1.2.2'></a>
 ## 1.2.2 (2024-04-11)
 
 ### Bug fixes
 
 - Update `jira_uri_template` configuration default to `https://rubinobs.atlassian.net/browse/{issue}`. This will make all :jira:, :jirab:, and :jirap: roles point to the new Jira instance for Rubin Observatory.
 - Drop `jira.lsstcorp.org` from the linkcheck ignore list defaults for `documenteer.config.guide` since that instance is no longer being used.
```

### Comparing `documenteer-1.2.2/docs/dev/api/documenteer.ext.rst` & `documenteer-1.3.0/docs/dev/api/documenteer.ext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.3.0/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/dev/development.rst` & `documenteer-1.3.0/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/dev/html-templates.rst` & `documenteer-1.3.0/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/dev/release.rst` & `documenteer-1.3.0/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/dev/theme-assets.rst` & `documenteer-1.3.0/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/documenteer.toml` & `documenteer-1.3.0/docs/documenteer.toml`

 * *Files 24% similar despite different names*

```diff
@@ -40,7 +40,16 @@
 sphinxcontrib-bibtex = "https://sphinxcontrib-bibtex.readthedocs.io/en/latest/"
 technote = "https://technote.lsst.io/"
 
 [sphinx.linkcheck]
 ignore = [
     "https://mermaid-js.github.io"
 ]
+
+[sphinx.redirects]
+"pipelines/build-overview.rst" = "guides/pipelines/build-overview.rst"
+"pipelines/configuration.rst" = "guides/pipelines/configuration.rst"
+"pipelines/cpp-api-linking.rst" = "guides/pipelines/cpp-api-linking.rst"
+"pipelines/index.rst" = "guides/pipelines/index.rst"
+"pipelines/install.rst" = "guides/pipelines/install.rst"
+"pipelines/package-docs-cli.rst" = "guides/pipelines/package-docs-cli.rst"
+"pipelines/stack-docs-cli.rst" = "guides/pipelines/stack-docs-cli.rst"
```

### Comparing `documenteer-1.2.2/docs/guides/badges.rst` & `documenteer-1.3.0/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/configuration.rst` & `documenteer-1.3.0/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/diagrams.rst` & `documenteer-1.3.0/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/extend-conf-py.rst` & `documenteer-1.3.0/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/including-notebooks.ipynb` & `documenteer-1.3.0/docs/guides/including-notebooks.ipynb`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/index.rst` & `documenteer-1.3.0/docs/guides/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -22,24 +22,26 @@
    :maxdepth: 2
    :caption: Advanced configuration
    :name: toc-guides-advanced-config
 
    pyproject-configuration
    openapi
    rst-epilog
+   page-redirects
    extend-conf-py
 
 .. toctree::
    :maxdepth: 2
    :caption: Design features
    :name: toc-guides-design
 
    diagrams
    badges
    tabsets
+   video-embeds
 
 .. toctree::
    :maxdepth: 2
    :caption: Markdown & Jupyter Notebooks
    :name: toc-guides-md-ipynb
 
    markdown-primer
```

### Comparing `documenteer-1.2.2/docs/guides/markdown-primer.md` & `documenteer-1.3.0/docs/guides/markdown-primer.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/openapi.rst` & `documenteer-1.3.0/docs/guides/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/organization.rst` & `documenteer-1.3.0/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/overview.rst` & `documenteer-1.3.0/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/build-overview.rst` & `documenteer-1.3.0/docs/guides/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/configuration.rst` & `documenteer-1.3.0/docs/guides/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/cpp-api-linking.rst` & `documenteer-1.3.0/docs/guides/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/index.rst` & `documenteer-1.3.0/docs/guides/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/install.rst` & `documenteer-1.3.0/docs/guides/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/package-docs-cli.rst` & `documenteer-1.3.0/docs/guides/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pipelines/stack-docs-cli.rst` & `documenteer-1.3.0/docs/guides/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/pyproject-configuration.rst` & `documenteer-1.3.0/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/rst-epilog.rst` & `documenteer-1.3.0/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/tabsets.rst` & `documenteer-1.3.0/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/guides/toml-reference.rst` & `documenteer-1.3.0/docs/guides/toml-reference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -368,18 +368,35 @@
 
 Set this to the directory where Python API documentation is generated, through automodapi_.
 The default value is ``api``, which is a good standard for Python projects with a public API.
 
 If the Python API is oriented towards contributors, such as in an application or service, you can change the default:
 
 .. code-block:: toml
+   :caption: documenteer.toml
 
    [sphinx]
    python_api_dir = "dev/api/contents"
 
+.. _guide-sphinx-redirects:
+
+[sphinx.redirects]
+==================
+
+|optional|
+
+A table of paths to redirect to other paths. Use this setting to redirect old page locations to the new locations when a documentation site is reorganized.
+
+.. code-block:: toml
+   :caption: documenteer.toml
+
+   [sphinx.redirects]
+   "old/path" = "new/path"
+   "old/path2" = "new/path2"
+
 [sphinx.theme]
 ==============
 
 |optional|
 
 Configurations related to the Sphinx HTML theme.
```

### Comparing `documenteer-1.2.2/docs/index.rst` & `documenteer-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.3.0/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.3.0/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.3.0/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/githubbibcache.rst` & `documenteer-1.3.0/docs/sphinx-extensions/githubbibcache.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.3.0/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.3.0/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.3.0/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/openapi.rst` & `documenteer-1.3.0/docs/sphinx-extensions/openapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.3.0/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.3.0/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/_templates/README.md` & `documenteer-1.3.0/docs/technotes/_templates/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/_templates/README.rst` & `documenteer-1.3.0/docs/technotes/_templates/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/author-metadata.rst` & `documenteer-1.3.0/docs/technotes/author-metadata.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/configuration.rst` & `documenteer-1.3.0/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/document-status.rst` & `documenteer-1.3.0/docs/technotes/document-status.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/edit-locally.rst` & `documenteer-1.3.0/docs/technotes/edit-locally.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/edit-on-github.rst` & `documenteer-1.3.0/docs/technotes/edit-on-github.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/extensions.rst` & `documenteer-1.3.0/docs/technotes/extensions.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/how-your-technote-gets-published.rst` & `documenteer-1.3.0/docs/technotes/how-your-technote-gets-published.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/index.rst` & `documenteer-1.3.0/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/migrate.rst` & `documenteer-1.3.0/docs/technotes/migrate.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/docs/technotes/start-a-technote.rst` & `documenteer-1.3.0/docs/technotes/start-a-technote.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/licenses/astropy-helpers.txt` & `documenteer-1.3.0/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/licenses/sphinx-issue.txt` & `documenteer-1.3.0/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/licenses/sphinx.txt` & `documenteer-1.3.0/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/package-lock.json` & `documenteer-1.3.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/package.json` & `documenteer-1.3.0/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/pyproject.toml` & `documenteer-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -43,23 +43,25 @@
     # Documenteer's testing and deployment deps
     "coverage[toml]",
     "pytest",
     "pytest-mock",
     # Test depedendencies for analyzing HTML output
     "lxml",
     "cssselect",
+    "defusedxml",  # used by Sphinx but not declared as a dependency
     # Extensions for documenteer's own docs
     "sphinx-click",
     "sphinxcontrib-autoprogram",
     # Type stubs
     "types-setuptools",
     "types-requests",
     "types-PyYAML",
     "types-docutils",
     "types-mock",
+    # Testing dependencies
 ]
 guide = [
     # Theme and extensions for Rubin user guide projects
     "sphinx_design",
     "pydata-sphinx-theme>=0.10.0,<0.13.0",
     "sphinx-autodoc-typehints",
     "sphinx-automodapi",
@@ -70,14 +72,15 @@
     "myst-nb",
     "markdown-it-py[linkify]",
     "sphinxcontrib-mermaid",
     "sphinxext-opengraph",
     "sphinxcontrib-redoc",
     "sphinxcontrib-jquery",
     "sphinxext-rediraffe",
+    "sphinxcontrib-youtube"
 ]
 pipelines = [
     # Theme and extensions for pipelines.lsst.io
     # Include all dependencies fof guide, and add additional dependencies
     # specifically for pipelines.lsst.io
     "sphinx_design",
     "pydata-sphinx-theme>=0.10.0,<0.13.0",
@@ -96,20 +99,21 @@
     # Additional extensions for Pipelines
     "sphinxcontrib-autoprogram",
     "sphinxcontrib-doxylink",
     "sphinx-click",
 ]
 technote = [
     # Theme and extensions for technotes
-    "technote>=0.7.0,<0.8.0",
+    "technote>=0.8.0,<0.9.0",
     "sphinx-prompt",
     "sphinxcontrib-mermaid",
     "sphinx-diagrams",
     "sphinx_design",
-    "myst-nb"
+    "myst-nb",
+    "sphinxcontrib-youtube"
 ]
 
 [project.urls]
 Homepage = "https://documenteer.lsst.io"
 Source = "https://github.com/lsst-sqre/documenteer"
 
 [project.scripts]
```

### Comparing `documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2` & `documenteer-1.3.0/src/assets/rubin-technote/styles/SourceSans3VF-Italic.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2` & `documenteer-1.3.0/src/assets/rubin-technote/styles/SourceSans3VF-Upright.ttf.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/assets/rubin-technote/styles/_hacks.scss` & `documenteer-1.3.0/src/assets/rubin-technote/styles/_hacks.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/assets/rubin-technote/styles/_properties.scss` & `documenteer-1.3.0/src/assets/rubin-technote/styles/_properties.scss`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/731c8feefe13e72a8691.woff2` & `documenteer-1.3.0/src/documenteer/assets/731c8feefe13e72a8691.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/b8bc3440ba2145e132f5.woff2` & `documenteer-1.3.0/src/documenteer/assets/b8bc3440ba2145e132f5.woff2`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/favicon.ico` & `documenteer-1.3.0/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-1.3.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-1.3.0/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.3.0/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.3.0/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.3.0/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-technote.css` & `documenteer-1.3.0/src/documenteer/assets/rubin-technote.css`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     --tn-component-h6-size: 1rem;
   }
 }
 /*
  * Custom styles for the author listing.
  */
 .technote-inline-authors {
-  font-size: 1.1rem;
+  font-size: 1.1em;
   font-weight: 425;
 }
 
 .rubin-technote-global-breadcrumbs {
   list-style: none;
   margin-left: 0;
   padding-left: 0;
@@ -186,20 +186,20 @@
 .mobile-rubin-technote-logo {
   display: block;
   margin: 0 auto 2rem auto;
   width: 100%;
   max-width: 12rem;
 }
 
-@media (max-width: 76rem) {
+@media (max-width: 76em) {
   .sb-container {
     margin-top: 0;
   }
 }
-@media (min-width: 76rem) {
+@media (min-width: 76em) {
   .mobile-rubin-technote-logo {
     display: none;
     margin: 0;
   }
 }
 /*
  * Styles that are applied at the end of the selector stack to override
```

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-technote.css.map` & `documenteer-1.3.0/src/documenteer/assets/rubin-technote.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974025974025974%*

 * *Differences: {"'sourcesContent'": "{insert: [(3, '/*\\n * Custom styles for the author listing.\\n "*

 * *                     '*/\\n\\n.technote-inline-authors {\\n  font-size: 1.1em;\\n  font-weight: '*

 * *                     "425;\\n}\\n'), (7, '.mobile-rubin-technote-logo {\\n  display: block;\\n  "*

 * *                     'margin: 0 auto 2rem auto;\\n  width: 100%;\\n  max-width: '*

 * *                     '12rem;\\n}\\n\\n@media (max-width: 76em) {\\n  // When the primary sidebar '*

 * *                     'is hidden, remove extra t […]*

```diff
@@ -14,16 +14,16 @@
         "webpack:///./src/assets/rubin-technote/styles/components/_article-header.scss",
         "webpack:///./src/assets/rubin-technote/styles/_hacks.scss"
     ],
     "sourcesContent": [
         "/**\n * Do not edit directly\n * Generated on Thu, 01 Dec 2022 19:33:46 GMT\n */\n\n:root {\n  --rsd-asset-image-favicon-svg: \"assets/favicon/rubin-favicon.svg\";\n  --rsd-asset-image-favicon-png-32-px: \"assets/favicon/rubin-favicon-transparent-32px.png\";\n  --rsd-asset-image-favicon-png-49-px: \"assets/favicon/rubin-favicon-transparent-49px.png\";\n  --rsd-asset-image-construction-agencies-png: \"assets/partner-logos/construction-agencies.png\"; /* Construction funding agency logo lineup (black on transparent). */\n  --rsd-asset-image-operations-agencies-png: \"assets/partner-logos/operations-lineup-black.png\"; /* Operations funding agency logo lineup (black on transparent). */\n  --rsd-asset-image-rubin-imagotype-color-on-black-png: \"assets/rubin-imagotype/rubin-imagotype-color-on-black.png\";\n  --rsd-asset-image-rubin-imagotype-color-on-black-svg: \"assets/rubin-imagotype/rubin-imagotype-color-on-black.svg\";\n  --rsd-asset-image-rubin-imagotype-color-on-white-png: \"assets/rubin-imagotype/rubin-imagotype-color-on-white.png\";\n  --rsd-asset-image-rubin-imagotype-color-on-white-svg: \"assets/rubin-imagotype/rubin-imagotype-color-on-white.svg\";\n  --rsd-asset-image-rubin-imagotype-gray-on-black-png: \"assets/rubin-imagotype/rubin-imagotype-gray-on-black.png\";\n  --rsd-asset-image-rubin-imagotype-gray-on-black-svg: \"assets/rubin-imagotype/rubin-imagotype-gray-on-black.svg\";\n  --rsd-asset-image-rubin-imagotype-gray-on-white-png: \"assets/rubin-imagotype/rubin-imagotype-gray-on-white.png\";\n  --rsd-asset-image-rubin-imagotype-gray-on-white-svg: \"assets/rubin-imagotype/rubin-imagotype-gray-on-white.svg\";\n  --rsd-asset-image-rubin-imagotype-color-on-black-crop-png: \"assets/rubin-imagotype/rubin-imagotype-color-on-black-crop.png\";\n  --rsd-asset-image-rubin-imagotype-color-on-black-crop-svg: \"assets/rubin-imagotype/rubin-imagotype-color-on-black-crop.svg\";\n  --rsd-asset-image-rubin-imagotype-color-on-white-crop-png: \"assets/rubin-imagotype/rubin-imagotype-color-on-white-crop.png\";\n  --rsd-asset-image-rubin-imagotype-color-on-white-crop-svg: \"assets/rubin-imagotype/rubin-imagotype-color-on-white-crop.svg\";\n  --rsd-asset-image-rubin-imagotype-gray-on-black-crop-png: \"assets/rubin-imagotype/rubin-imagotype-gray-on-black-crop.png\";\n  --rsd-asset-image-rubin-imagotype-gray-on-black-crop-svg: \"assets/rubin-imagotype/rubin-imagotype-gray-on-black-crop.svg\";\n  --rsd-asset-image-rubin-imagotype-gray-on-white-crop-png: \"assets/rubin-imagotype/rubin-imagotype-gray-on-white-crop.png\";\n  --rsd-asset-image-rubin-imagotype-gray-on-white-crop-svg: \"assets/rubin-imagotype/rubin-imagotype-gray-on-white-crop.svg\";\n  --rsd-asset-image-rubin-imagotype-email-png: \"assets/rubin-imagotype/rubin-imagotype-email.png\";\n  --rsd-asset-image-rubin-watermark-watermark-png: \"assets/rubin-watermarks/rubin-watermark.png\";\n  --rsd-asset-image-rubin-watermark-letterhead-watermark-png: \"assets/rubin-watermarks/rubin-letterhead-watermark.png\";\n  --rsd-asset-image-rubin-watermark-letterhead-watermark-2-png: \"assets/rubin-watermarks/rubin-letterhead-watermark-2.png\";\n  --rsd-color-blue-500: #1c81a4;\n  --rsd-color-gray-100: #dce0e3;\n  --rsd-color-gray-500: #6a6e6e;\n  --rsd-color-gray-800: #1f2121;\n  --rsd-color-gray-900: #000000; /* Pure black. */\n  --rsd-color-gray-000: #ffffff; /* Pure white. */\n  --rsd-color-green-500: #3cae3f;\n  --rsd-color-imagotype-light: #00babc; /* Light teal in imagotype (graphic element). */\n  --rsd-color-imagotype-dark: #058b8c; /* Dark teal in imagotype (for Observatory wordmark). */\n  --rsd-color-imagotype-black: #313333; /* Dark gray in imagotype. */\n  --rsd-color-imagotype-white: #f5f5f5; /* Imagotype white for dark backgrounds. */\n  --rsd-color-orange-500: #ed4c4c;\n  --rsd-color-primary-100: #f5f5f5;\n  --rsd-color-primary-200: #d9f7f6;\n  --rsd-color-primary-300: #b1f2ef;\n  --rsd-color-primary-400: #00babc;\n  --rsd-color-primary-500: #009fa1;\n  --rsd-color-primary-600: #058b8c;\n  --rsd-color-primary-700: #0c4a47;\n  --rsd-color-primary-800: #313333;\n  --rsd-color-purple-500: #583671;\n  --rsd-color-red-500: #ed4c4c;\n  --rsd-color-yellow-500: #ffe266;\n  --rsd-component-footer-background-color: #f5f5f5;\n  --rsd-component-header-background-color: #1f2121; /* Header background color. */\n  --rsd-component-header-nav-text-color: #ffffff;\n  --rsd-component-header-nav-text-hover-color: #00babc;\n  --rsd-component-header-nav-menulist-text-color: #1f2121;\n  --rsd-component-header-nav-menulist-background-color: #ffffff;\n  --rsd-component-header-nav-menulist-selected-background-color: #058b8c;\n  --rsd-component-page-background-color: #ffffff; /* Page background color */\n  --rsd-component-service-card-background-color: #ffffff;\n  --rsd-component-service-card-text-color: #1f2121;\n  --rsd-component-text-color: #1f2121; /* Body text color */\n  --rsd-component-text-reverse-color: #dce0e3; /* Body text color in reversed (light on dark) contexts. */\n  --rsd-component-text-link-color: #146685;\n  --rsd-component-text-link-hover-color: #1c81a4;\n  --rsd-component-text-link-reverse-color: #1c81a4; /* Link color in reversed (light on dark) contexts. */\n  --rsd-component-text-headline-color: #058b8c;\n}\n",
         "/*\n * Styles for Rubin technotes (documenteer.conf.technotebeta config).\n * These are intended to cascade *after* the base skeleton.css and\n * technote.css from https://technote.lsst.io.\n */\n\n@use '../../../../node_modules/@lsst-sqre/rubin-style-dictionary/dist/tokens.css';\n\n@use 'properties';\n@use 'components';\n@use 'hacks';\n",
         "/*\n * Override technote CSS properties with Rubin Style Dictionary.\n */\n\n@font-face {\n  font-family: 'Source Sans 3 VF';\n  font-weight: 200 900;\n  font-style: normal;\n  font-stretch: normal;\n  src: url('./SourceSans3VF-Upright.ttf.woff2') format('woff2');\n}\n\n@font-face {\n  font-family: 'Source Sans 3 VF';\n  font-weight: 200 900;\n  font-style: italic;\n  font-stretch: normal;\n  src: url('./SourceSans3VF-Italic.ttf.woff2') format('woff2');\n}\n\n:root {\n  --tn-component-text-font-family: 'Source Sans 3 VF', -apple-system,\n    BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans,\n    Droid Sans, Helvetica Neue, sans-serif;\n  --tn-component-text-color: var(--rsd-component-text-color);\n  --tn-component-toc-header-color: var(--rsd-color-primary-600);\n  --tn-component-sidebar-header-color: var(--rsd-color-primary-600);\n  --tn-component-toc-level-border-color: var(--rsd-color-primary-600);\n}\n\n@supports (font-variation-settings: 'wdth' 222) {\n  :root {\n    --tn-component-h1-weight: 600;\n    --tn-component-h2-weight: 500;\n    --tn-component-h3-weight: 600;\n    --tn-component-h4-weight: 700;\n    --tn-component-h5-weight: 800;\n    --tn-component-h6-weight: 800;\n  }\n}\n\n@media (max-width: 76rem) {\n  :root {\n    --tn-component-h1-size: 2.4rem;\n    --tn-component-h2-size: 1.8rem;\n    --tn-component-h3-size: 1.2rem;\n    --tn-component-h4-size: 1rem;\n    --tn-component-h5-size: 1rem;\n    --tn-component-h6-size: 1rem;\n  }\n}\n",
-        "/*\n * Custom styles for the author listing.\n */\n\n.technote-inline-authors {\n  font-size: 1.1rem;\n  font-weight: 425;\n}\n",
+        "/*\n * Custom styles for the author listing.\n */\n\n.technote-inline-authors {\n  font-size: 1.1em;\n  font-weight: 425;\n}\n",
         ".rubin-technote-global-breadcrumbs {\n  list-style: none;\n  margin-left: 0;\n  padding-left: 0;\n  margin: 0;\n}\n\n.rubin-technote-global-breadcrumbs li {\n  display: inline;\n}\n\n.rubin-technote-global-breadcrumbs li::after {\n  content: ' / ';\n}\n\n.rubin-technote-global-breadcrumbs li:last-child::after {\n  content: '';\n}\n\n.technote-article-header-id {\n  margin: var(--tn-space-xs) 0 var(--tn-space-xs);\n}\n",
         "/*\n * The version info in the header-article section (located below the\n * technote ID)\n */\n\n.rubin-technote-version-info {\n  display: flex;\n  flex-direction: row;\n}\n\n.rubin-technote-version-info > p {\n  margin: 0 0 var(--tn-space-sm);\n}\n\n.rubin-technote-version-info > p {\n  margin-right: var(--tn-space-xl);\n}\n\n.rubin-technote-version-info > p:last-child {\n  margin-right: 0;\n}\n\n@supports (font-variation-settings: 'wdth' 222) {\n  .rubin-technote-version-info a {\n    font-weight: 500;\n  }\n}\n",
         "@supports (font-variation-settings: 'wdth' 222) {\n  .technote-sidebar-section__heading {\n    font-weight: 600;\n    text-transform: uppercase;\n    letter-spacing: 0.01em; // goes well with upper case\n  }\n}\n",
-        ".mobile-rubin-technote-logo {\n  display: block;\n  margin: 0 auto 2rem auto;\n  width: 100%;\n  max-width: 12rem;\n}\n\n@media (max-width: 76rem) {\n  // When the primary sidebar is hidden, remove extra top margin from the\n  // container so the logo is closer to the top.\n  .sb-container {\n    margin-top: 0;\n  }\n}\n\n@media (min-width: 76rem) {\n  // Hide the mobile logo when the primary sidebar is visible.\n  .mobile-rubin-technote-logo {\n    display: none;\n    margin: 0;\n  }\n}\n",
+        ".mobile-rubin-technote-logo {\n  display: block;\n  margin: 0 auto 2rem auto;\n  width: 100%;\n  max-width: 12rem;\n}\n\n@media (max-width: 76em) {\n  // When the primary sidebar is hidden, remove extra top margin from the\n  // container so the logo is closer to the top.\n  .sb-container {\n    margin-top: 0;\n  }\n}\n\n@media (min-width: 76em) {\n  // Hide the mobile logo when the primary sidebar is visible.\n  .mobile-rubin-technote-logo {\n    display: none;\n    margin: 0;\n  }\n}\n",
         "/*\n * Styles that are applied at the end of the selector stack to override\n * other selectors. These selectors should eventually be refactored into\n * their proper module either in documenteer or in the parent technote theme.\n */\n\n@media (max-width: 76rem) {\n  // Reduce the margin-bottom on headings in mobile views\n  h1,\n  h2,\n  h3,\n  h4,\n  h5,\n  h6 {\n    margin-bottom: 0.5em;\n  }\n}\n\n/*\n * Border specififcally for prompts, which act differently than code blocks.\n */\n.highlight-default .highlight {\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n.highlight-default .highlight pre {\n  margin: 1em;\n}\n"
     ],
     "version": 3
 }
```

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.3.0/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.3.0/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-1.3.0/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-1.3.0/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/cli.py` & `documenteer-1.3.0/src/documenteer/cli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/conf/_toml.py` & `documenteer-1.3.0/src/documenteer/conf/_toml.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,22 @@
 
     intersphinx: IntersphinxModel = Field(
         default_factory=lambda: IntersphinxModel()
     )
 
     linkcheck: LinkCheckModel = Field(default_factory=lambda: LinkCheckModel())
 
+    redirects: Dict[str, str] = Field(
+        description=(
+            "Mapping of paths to redirect to other paths. These redirects "
+            "are implemented with sphinx-rediraffe."
+        ),
+        default_factory=dict,
+    )
+
 
 class ConfigRoot(BaseModel):
     """The root model for a documenteer.toml configuration file."""
 
     project: ProjectModel
 
     sphinx: Optional[SphinxModel] = None
@@ -405,14 +413,22 @@
         if not set.
         """
         if self.rst_epilog_path is None:
             return ""
         else:
             return self.rst_epilog_path.read_text()
 
+    @property
+    def redirects(self) -> Dict[str, str]:
+        """Redirects defined in the [sphinx.redirects] TOML configuration."""
+        if self.conf.sphinx:
+            return self.conf.sphinx.redirects
+        else:
+            return dict()
+
     def _get_pyproject_metadata(self, package_name: str) -> Message:
         if sys.version_info >= (3, 10) or sys.version_info < (3, 8):
             pkg_metadata = cast(Message, metadata(package_name))
         else:
             pkg_metadata = metadata(package_name)
         return pkg_metadata
```

### Comparing `documenteer-1.2.2/src/documenteer/conf/guide.py` & `documenteer-1.3.0/src/documenteer/conf/guide.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.ifconfig",
     "sphinx-prompt",
     "sphinx_jinja",
     "sphinxcontrib.redoc",
+    "sphinxcontrib.youtube",
     "sphinxext.rediraffe",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "sphinx_automodapi.automodapi",
     "sphinx_automodapi.smart_resolver",
     "documenteer.ext.jira",
     "documenteer.ext.lsstdocushare",
@@ -452,8 +453,8 @@
 # ============================================================================
 jinja_contexts: dict[str, Any] = {}
 
 # ============================================================================
 # #REDIRECTS Sphinx-rediraffe support
 # https://sphinxext-rediraffe.readthedocs.io/en/latest/
 # ============================================================================
-rediraffe_redirects: dict[str, str] = {}
+rediraffe_redirects: dict[str, str] = _conf.redirects
```

### Comparing `documenteer-1.2.2/src/documenteer/conf/pipelines.py` & `documenteer-1.3.0/src/documenteer/conf/pipelines.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.3.0/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/conf/technote.py` & `documenteer-1.3.0/src/documenteer/conf/technote.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Sphinx configuration for Rubin technotes."""
 
 from pathlib import Path
 
 from technote.sphinxconf import *  # noqa: F401 F403
 
 from documenteer.conf import (
+    extend_excludes_for_non_index_source,
     extend_static_paths_with_asset_extension,
     get_asset_path,
     get_template_dir,
 )
 
 try:
     # Remove the sphinxcontrib-bibtex extension so that we can add it back
@@ -36,14 +37,15 @@
         "documenteer.ext.bibtex",
         "documenteer.ext.githubbibcache",
         "sphinxcontrib.bibtex",
         "sphinx_diagrams",
         "sphinxcontrib.mermaid",
         "sphinx_prompt",
         "sphinx_design",
+        "sphinxcontrib.youtube",
     ]
 )
 
 # The source file suffixes for .md and .ipynb are automatically managed by
 # myst-nb.
 source_suffix = {
     ".rst": "restructuredtext",
@@ -70,14 +72,19 @@
 html_theme_options = {
     "light_logo": "rubin-imagotype-color-on-white-crop.svg",
     "dark_logo": "rubin-imagotype-color-on-black-crop.svg",
     "logo_link_url": "https://www.lsst.io",
     "logo_alt_text": "Rubin Observatory logo",
 }
 
+# Exclude non-index.ipynb Jupyter Notebooks
+extend_excludes_for_non_index_source(exclude_patterns, "ipynb")  # noqa: F405
+extend_excludes_for_non_index_source(exclude_patterns, "md")  # noqa: F405
+extend_excludes_for_non_index_source(exclude_patterns, "rst")  # noqa: F405
+
 # Configure bibliography with the bib cache
 documenteer_bibfile_cache_dir = ".technote/bibfiles"
 documenteer_bibfile_github_repos = [
     {
         "repo": "lsst/lsst-texmf",
         "ref": "main",
         "bibfiles": [
```

### Comparing `documenteer-1.2.2/src/documenteer/ext/_utils.py` & `documenteer-1.3.0/src/documenteer/ext/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/autocppapi.py` & `documenteer-1.3.0/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/autodocreset.py` & `documenteer-1.3.0/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/bibtex.py` & `documenteer-1.3.0/src/documenteer/ext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/githubbibcache.py` & `documenteer-1.3.0/src/documenteer/ext/githubbibcache.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,19 +112,19 @@
             if cached_path not in config["bibtex_bibfiles"]:
                 config["bibtex_bibfiles"].append(str(cached_path))
 
 
 def setup(app: Sphinx) -> dict[str, Any]:
     """Set up the ``documenteer.ext.autocppapi`` Sphinx extensions."""
     # Configuration values
-    app.add_config_value("documenteer_bibfile_github_repos", "", True, [list])
+    app.add_config_value("documenteer_bibfile_github_repos", "", "env", [list])
     app.add_config_value(
         "documenteer_bibfile_cache_dir",
         Path("_build/bibfile-cache"),
-        True,
+        "env",
         [str, Path],
     )
     app.connect("config-inited", cache_bibfiles)
 
     return {
         "version": __version__,
         "parallel_read_safe": True,
```

### Comparing `documenteer-1.2.2/src/documenteer/ext/jira.py` & `documenteer-1.3.0/src/documenteer/ext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lsstdocushare.py` & `documenteer-1.3.0/src/documenteer/ext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/__init__.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/configfieldlists.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/crossrefs.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/pyapisummary.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/pyapisummary.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,20 @@
     desc,
     desc_addname,
     desc_annotation,
     desc_content,
     desc_signature,
     seealso,
 )
-from sphinx.domains.python import PyXRefRole, _pseudo_parse_arglist
+
+try:
+    from sphinx.domains.python._annotations import _pseudo_parse_arglist
+except ImportError:
+    from sphinx.domains.python import _pseudo_parse_arglist  # type: ignore
+from sphinx.domains.python import PyXRefRole
 from sphinx.errors import SphinxError
 from sphinx.util.inspect import signature as make_signature
 from sphinx.util.inspect import stringify_signature
 from sphinx.util.logging import getLogger
 
 from .taskutils import extract_docstring_summary, get_docstring, get_type
```

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/taskutils.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/topiclists.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/lssttasks/topics.py` & `documenteer-1.3.0/src/documenteer/ext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/mockcoderefs.py` & `documenteer-1.3.0/src/documenteer/ext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/openapi.py` & `documenteer-1.3.0/src/documenteer/ext/openapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/packagetoctree.py` & `documenteer-1.3.0/src/documenteer/ext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/ext/remotecodeblock.py` & `documenteer-1.3.0/src/documenteer/ext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/packagemetadata.py` & `documenteer-1.3.0/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/requestsutils.py` & `documenteer-1.3.0/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/services/technoteauthor.py` & `documenteer-1.3.0/src/documenteer/services/technoteauthor.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/services/technotemigration.py` & `documenteer-1.3.0/src/documenteer/services/technotemigration.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/sphinxrunner.py` & `documenteer-1.3.0/src/documenteer/sphinxrunner.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/build.py` & `documenteer-1.3.0/src/documenteer/stackdocs/build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.3.0/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.3.0/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.3.0/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.3.0/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.3.0/src/documenteer/stackdocs/packagecli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.3.0/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.3.0/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.3.0/src/documenteer/stackdocs/stackcli.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/authordb.py` & `documenteer-1.3.0/src/documenteer/storage/authordb.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/latex.py` & `documenteer-1.3.0/src/documenteer/storage/latex.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/README.rst` & `documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/README.rst`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/localtemplates/technote/tox.ini` & `documenteer-1.3.0/src/documenteer/storage/localtemplates/technote/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/localtemplates.py` & `documenteer-1.3.0/src/documenteer/storage/localtemplates.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/storage/technotetoml.py` & `documenteer-1.3.0/src/documenteer/storage/technotetoml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/templates/technote/components/sidebar-source.html` & `documenteer-1.3.0/src/documenteer/templates/technote/components/sidebar-source.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-1.3.0/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer/utils.py` & `documenteer-1.3.0/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.3.0/src/documenteer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 1.2.2
+Version: 1.3.0
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -57,14 +57,15 @@
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: coverage[toml]; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: lxml; extra == "dev"
 Requires-Dist: cssselect; extra == "dev"
+Requires-Dist: defusedxml; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinxcontrib-autoprogram; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-docutils; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
@@ -80,14 +81,15 @@
 Requires-Dist: myst-nb; extra == "guide"
 Requires-Dist: markdown-it-py[linkify]; extra == "guide"
 Requires-Dist: sphinxcontrib-mermaid; extra == "guide"
 Requires-Dist: sphinxext-opengraph; extra == "guide"
 Requires-Dist: sphinxcontrib-redoc; extra == "guide"
 Requires-Dist: sphinxcontrib-jquery; extra == "guide"
 Requires-Dist: sphinxext-rediraffe; extra == "guide"
+Requires-Dist: sphinxcontrib-youtube; extra == "guide"
 Provides-Extra: pipelines
 Requires-Dist: sphinx_design; extra == "pipelines"
 Requires-Dist: pydata-sphinx-theme<0.13.0,>=0.10.0; extra == "pipelines"
 Requires-Dist: sphinx-autodoc-typehints; extra == "pipelines"
 Requires-Dist: sphinx-automodapi; extra == "pipelines"
 Requires-Dist: sphinx-copybutton; extra == "pipelines"
 Requires-Dist: sphinx-prompt; extra == "pipelines"
@@ -98,20 +100,21 @@
 Requires-Dist: sphinxext-opengraph; extra == "pipelines"
 Requires-Dist: sphinxcontrib-redoc; extra == "pipelines"
 Requires-Dist: sphinxcontrib-jquery; extra == "pipelines"
 Requires-Dist: sphinxcontrib-autoprogram; extra == "pipelines"
 Requires-Dist: sphinxcontrib-doxylink; extra == "pipelines"
 Requires-Dist: sphinx-click; extra == "pipelines"
 Provides-Extra: technote
-Requires-Dist: technote<0.8.0,>=0.7.0; extra == "technote"
+Requires-Dist: technote<0.9.0,>=0.8.0; extra == "technote"
 Requires-Dist: sphinx-prompt; extra == "technote"
 Requires-Dist: sphinxcontrib-mermaid; extra == "technote"
 Requires-Dist: sphinx-diagrams; extra == "technote"
 Requires-Dist: sphinx_design; extra == "technote"
 Requires-Dist: myst-nb; extra == "technote"
+Requires-Dist: sphinxcontrib-youtube; extra == "technote"
 
 [![Documentation](https://img.shields.io/badge/documenteer-lsst.io-brightgreen.svg)](https://documenteer.lsst.io)
 [![PyPI](https://img.shields.io/pypi/v/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![For Python 3.7+](https://img.shields.io/pypi/pyversions/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![MIT license](https://img.shields.io/pypi/l/documenteer.svg?style=flat-square)](https://pypi.python.org/pypi/documenteer)
 [![CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci.yaml)
 [![Weekly CI](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml/badge.svg)](https://github.com/lsst-sqre/documenteer/actions/workflows/ci-cron.yaml)
```

### Comparing `documenteer-1.2.2/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.3.0/src/documenteer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 .vscode/settings.json
 .vscode/tasks.json
 changelog.d/_template.md.jinja
 demo/ipynb-technote/.gitignore
 demo/ipynb-technote/Makefile
 demo/ipynb-technote/conf.py
 demo/ipynb-technote/diagram.py
+demo/ipynb-technote/extra-notebook.ipynb
 demo/ipynb-technote/index.ipynb
 demo/ipynb-technote/technote.toml
+demo/ipynb-technote/subdir/subdir-notebook.ipynb
 demo/md-technote/.gitignore
 demo/md-technote/Makefile
 demo/md-technote/conf.py
 demo/md-technote/diagram.py
 demo/md-technote/index.md
 demo/md-technote/technote.toml
 demo/rst-technote/.gitignore
@@ -70,18 +72,20 @@
 docs/guides/extend-conf-py.rst
 docs/guides/including-notebooks.ipynb
 docs/guides/index.rst
 docs/guides/markdown-primer.md
 docs/guides/openapi.rst
 docs/guides/organization.rst
 docs/guides/overview.rst
+docs/guides/page-redirects.rst
 docs/guides/pyproject-configuration.rst
 docs/guides/rst-epilog.rst
 docs/guides/tabsets.rst
 docs/guides/toml-reference.rst
+docs/guides/video-embeds.rst
 docs/guides/pipelines/build-overview.rst
 docs/guides/pipelines/configuration.rst
 docs/guides/pipelines/cpp-api-linking.rst
 docs/guides/pipelines/index.rst
 docs/guides/pipelines/install.rst
 docs/guides/pipelines/package-docs-cli.rst
 docs/guides/pipelines/stack-docs-cli.rst
```

### Comparing `documenteer-1.2.2/src/documenteer.egg-info/requires.txt` & `documenteer-1.3.0/src/documenteer.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 [dev]
 twine
 coverage[toml]
 pytest
 pytest-mock
 lxml
 cssselect
+defusedxml
 sphinx-click
 sphinxcontrib-autoprogram
 types-setuptools
 types-requests
 types-PyYAML
 types-docutils
 types-mock
@@ -38,14 +39,15 @@
 myst-nb
 markdown-it-py[linkify]
 sphinxcontrib-mermaid
 sphinxext-opengraph
 sphinxcontrib-redoc
 sphinxcontrib-jquery
 sphinxext-rediraffe
+sphinxcontrib-youtube
 
 [pipelines]
 sphinx_design
 pydata-sphinx-theme<0.13.0,>=0.10.0
 sphinx-autodoc-typehints
 sphinx-automodapi
 sphinx-copybutton
@@ -58,13 +60,14 @@
 sphinxcontrib-redoc
 sphinxcontrib-jquery
 sphinxcontrib-autoprogram
 sphinxcontrib-doxylink
 sphinx-click
 
 [technote]
-technote<0.8.0,>=0.7.0
+technote<0.9.0,>=0.8.0
 sphinx-prompt
 sphinxcontrib-mermaid
 sphinx-diagrams
 sphinx_design
 myst-nb
+sphinxcontrib-youtube
```

### Comparing `documenteer-1.2.2/tests/conftest.py` & `documenteer-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/data/afw.doxygen.conf` & `documenteer-1.3.0/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/data/authordb.yaml` & `documenteer-1.3.0/tests/data/authordb.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/data/doxygen.tag.zip` & `documenteer-1.3.0/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/autocppapi_test.py` & `documenteer-1.3.0/tests/ext/autocppapi_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/jira_test.py` & `documenteer-1.3.0/tests/ext/jira_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/lsstdocushare_test.py` & `documenteer-1.3.0/tests/ext/lsstdocushare_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/lssttasks/taskutils_test.py` & `documenteer-1.3.0/tests/ext/lssttasks/taskutils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/mockcoderefs_test.py` & `documenteer-1.3.0/tests/ext/mockcoderefs_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/packagetoctree_test.py` & `documenteer-1.3.0/tests/ext/packagetoctree_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/ext/utils_test.py` & `documenteer-1.3.0/tests/ext/utils_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/packagemetadata_test.py` & `documenteer-1.3.0/tests/packagemetadata_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/roots/test-autocppapi/conf.py` & `documenteer-1.3.0/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.3.0/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/services/technotemigration_test.py` & `documenteer-1.3.0/tests/services/technotemigration_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/storage/authordb_test.py` & `documenteer-1.3.0/tests/storage/authordb_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/storage/technotetoml_test.py` & `documenteer-1.3.0/tests/storage/technotetoml_test.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_conf_toml.py` & `documenteer-1.3.0/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_stackdocs_build.py` & `documenteer-1.3.0/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_stackdocs_doxygen.py` & `documenteer-1.3.0/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_stackdocs_doxygentag.py` & `documenteer-1.3.0/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.3.0/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.3.0/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/tox.ini` & `documenteer-1.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-1.2.2/webpack.config.js` & `documenteer-1.3.0/webpack.config.js`

 * *Files identical despite different names*

