# Comparing `tmp/great-tables-0.5.0.tar.gz` & `tmp/great_tables-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great-tables-0.5.0.tar", last modified: Fri Apr 12 15:35:40 2024, max compression
+gzip compressed data, was "great_tables-0.5.1.tar", last modified: Fri May  3 19:41:20 2024, max compression
```

## Comparing `great-tables-0.5.0.tar` & `great_tables-0.5.1.tar`

### file list

```diff
@@ -1,256 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.443452 great-tables-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/scripts/no_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/workflows/ci-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-12 15:35:35.000000 great-tables-0.5.0/.github/workflows/code-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 15:35:35.000000 great-tables-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 15:35:35.000000 great-tables-0.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-12 15:35:35.000000 great-tables-0.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 15:35:35.000000 great-tables-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 15:35:35.000000 great-tables-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-12 15:35:35.000000 great-tables-0.5.0/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-04-12 15:35:35.000000 great-tables-0.5.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-04-12 15:35:35.000000 great-tables-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 15:35:35.000000 great-tables-0.5.0/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-04-12 15:35:35.000000 great-tables-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 15:35:35.000000 great-tables-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-12 15:35:35.000000 great-tables-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-04-12 15:35:40.443452 great-tables-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-12 15:35:35.000000 great-tables-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.387452 great-tables-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.383452 great-tables-0.5.0/docs/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.383452 great-tables-0.5.0/docs/_extensions/machow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.391452 great-tables-0.5.0/docs/_extensions/machow/interlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.391452 great-tables-0.5.0/docs/articles/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/articles/intro.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.395452 great-tables-0.5.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/GT_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/datasets.png
--rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/gt_parts_of_a_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/gt_sp500_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/gt_workflow_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/tables_from_the_web.png
--rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/assets/the_components_of_a_table.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.395452 great-tables-0.5.0/docs/blog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.403452 great-tables-0.5.0/docs/blog/design-philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/a_simple_table.png
--rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/cave_grids.png
--rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
--rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/computer_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
--rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
--rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
--rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/design-philosophy/visicalc.png
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.403452 great-tables-0.5.0/docs/blog/introduction-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/introduction-0.2.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.403452 great-tables-0.5.0/docs/blog/introduction-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/introduction-0.3.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.403452 great-tables-0.5.0/docs/blog/introduction-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/introduction-0.4.0/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/introduction_great_tables.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.403452 great-tables-0.5.0/docs/blog/polars-styling/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/polars-styling/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/polars-styling/table-preview.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.407452 great-tables-0.5.0/docs/blog/superbowl-squares/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/superbowl-squares/_code.py
--rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/superbowl-squares/games.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/blog/superbowl-squares/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.407452 great-tables-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.407452 great-tables-0.5.0/docs/examples/sports-earnings/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/basketball.png
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/boxing.png
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/golf.png
--rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/soccer.png
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/sports_earnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/examples/sports-earnings/tennis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.411452 great-tables-0.5.0/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/basic-column-labels.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/basic-formatting.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/basic-header.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/basic-stub.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/basic-styling.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/colorizing-with-data.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/column-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/nanoplots.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/row-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/table-theme-options.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/get-started/table-theme-premade.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 15:35:35.000000 great-tables-0.5.0/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.419452 great-tables-0.5.0/great_tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_boxhead.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.419452 great-tables-0.5.0/great_tables/_data_color/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_data_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_data_color/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27097 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_data_color/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_data_color/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_databackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)   151762 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    41041 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)    44734 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)    33451 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    74575 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_row_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_source_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24954 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54227 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    27178 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/_utils_render_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.419452 great-tables-0.5.0/great_tables/css/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/css/gt_colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/css/gt_styles_default.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.427452 great-tables-0.5.0/great_tables/data/
--rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/01-countrypops.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/02-sza.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/03-gtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/04-sp500.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/05-pizzaplace.csv
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/06-exibble.csv
--rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/07-towny.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/08-metro.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/09-constants.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/10-illness.csv
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/11-islands.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.435452 great-tables-0.5.0/great_tables/data/metro_images/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_10.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_11.svg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_12.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_13.svg
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_14.svg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_3bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_7bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/metro_9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/rer_A.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/rer_B.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/rer_C.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/rer_D.svg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/rer_E.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T11.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/tram_T9.svg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_H.svg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_J.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_K.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_L.svg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_N.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_P.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_R.svg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/metro_images/transilien_U.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/x-airquality.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/x_currencies.csv
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/x_currency_symbols.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/x_default_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/data/x_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16032 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 15:35:35.000000 great-tables-0.5.0/great_tables/vals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.443452 great-tables-0.5.0/great_tables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-04-12 15:35:40.000000 great-tables-0.5.0/great_tables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-12 15:35:40.000000 great-tables-0.5.0/great_tables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:35:40.000000 great-tables-0.5.0/great_tables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 15:35:40.000000 great-tables-0.5.0/great_tables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 15:35:40.000000 great-tables-0.5.0/great_tables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-12 15:35:35.000000 great-tables-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 15:35:35.000000 great-tables-0.5.0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:35:40.443452 great-tables-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.439452 great-tables-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.439452 great-tables-0.5.0/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_export.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_formats.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_locations.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_options.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    31640 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_repr.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_scss.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_tbl_data.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/__snapshots__/test_utils_render_html.ambr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.443452 great-tables-0.5.0/tests/data_color/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:35:40.443452 great-tables-0.5.0/tests/data_color/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/data_color/__snapshots__/test_data_color.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/data_color/test_data_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/data_color/test_data_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test__boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test__formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test__stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    53098 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test__utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    53431 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_formats_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-12 15:35:35.000000 great-tables-0.5.0/tests/test_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.708802 great_tables-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/scripts/no_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.652801 great_tables-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/ci-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-03 19:41:15.000000 great_tables-0.5.1/.github/workflows/code-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 19:41:15.000000 great_tables-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 19:41:15.000000 great_tables-0.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 19:41:15.000000 great_tables-0.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 19:41:15.000000 great_tables-0.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 19:41:15.000000 great_tables-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-03 19:41:15.000000 great_tables-0.5.1/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-03 19:41:15.000000 great_tables-0.5.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-03 19:41:15.000000 great_tables-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 19:41:15.000000 great_tables-0.5.1/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-03 19:41:15.000000 great_tables-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-03 19:41:15.000000 great_tables-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 19:41:15.000000 great_tables-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-03 19:41:20.708802 great_tables-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-03 19:41:15.000000 great_tables-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.648801 great_tables-0.5.1/docs/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.648801 great_tables-0.5.1/docs/_extensions/machow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.656801 great_tables-0.5.1/docs/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/articles/intro.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/GT_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_parts_of_a_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_sp500_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/gt_workflow_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/tables_from_the_web.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/assets/the_components_of_a_table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/blog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.660801 great_tables-0.5.1/docs/blog/bring-your-own-df/
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/bring-your-own-df/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/design-philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/a_simple_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/cave_grids.png
+-rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
+-rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/computer_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
+-rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/design-philosophy/visicalc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.2.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.3.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.668801 great_tables-0.5.1/docs/blog/introduction-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction-0.4.0/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/introduction_great_tables.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/blog/polars-styling/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/polars-styling/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/polars-styling/table-preview.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/blog/superbowl-squares/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/games.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/blog/superbowl-squares/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.672801 great_tables-0.5.1/docs/examples/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/_data/power_cie_prepared_tbl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.676801 great_tables-0.5.1/docs/examples/sports-earnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/basketball.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/boxing.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/golf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/soccer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/sports_earnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/examples/sports-earnings/tennis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.676801 great_tables-0.5.1/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-column-labels.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-formatting.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-header.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-stub.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/basic-styling.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/colorizing-with-data.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/column-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/nanoplots.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/row-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/table-theme-options.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/get-started/table-theme-premade.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-03 19:41:15.000000 great_tables-0.5.1/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_boxhead.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/_data_color/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_data_color/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_databackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148122 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14766 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74156 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_row_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_source_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24908 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55215 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27299 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.684801 great_tables-0.5.1/great_tables/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/css/gt_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/css/gt_styles_default.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.692802 great_tables-0.5.1/great_tables/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/01-countrypops.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/02-sza.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/03-gtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/04-sp500.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/05-pizzaplace.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/06-exibble.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/07-towny.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/08-metro.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/09-constants.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/10-illness.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/11-islands.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.700801 great_tables-0.5.1/great_tables/data/metro_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_10.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_12.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_14.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_3bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_7bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/metro_9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_A.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_B.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_C.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_D.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/rer_E.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/tram_T9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_H.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_J.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_K.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_L.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_N.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_P.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_R.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/metro_images/transilien_U.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x-airquality.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_currencies.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_currency_symbols.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_default_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/data/x_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 19:41:15.000000 great_tables-0.5.1/great_tables/vals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/great_tables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 19:41:20.000000 great_tables-0.5.1/great_tables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-03 19:41:15.000000 great_tables-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 19:41:15.000000 great_tables-0.5.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:41:20.708802 great_tables-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_export.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_formats.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_locations.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_options.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_repr.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_scss.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_tbl_data.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/__snapshots__/test_utils_render_html.ambr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/data_color/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:41:20.704802 great_tables-0.5.1/tests/data_color/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/__snapshots__/test_data_color.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/test_data_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/data_color/test_data_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54510 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test__utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_formats_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-03 19:41:15.000000 great_tables-0.5.1/tests/test_utils_render_html.py
```

### Comparing `great-tables-0.5.0/.github/CODE_OF_CONDUCT.md` & `great_tables-0.5.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/CONTRIBUTING.md` & `great_tables-0.5.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/ISSUE_TEMPLATE/bug.md` & `great_tables-0.5.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/ISSUE_TEMPLATE/feature.md` & `great_tables-0.5.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/ISSUE_TEMPLATE/question.md` & `great_tables-0.5.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `great_tables-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/scripts/no_pandas.py` & `great_tables-0.5.1/.github/scripts/no_pandas.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/workflows/ci-docs.yaml` & `great_tables-0.5.1/.github/workflows/ci-docs.yaml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/workflows/ci-tests.yaml` & `great_tables-0.5.1/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.github/workflows/code-checks.yaml` & `great_tables-0.5.1/.github/workflows/code-checks.yaml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.gitignore` & `great_tables-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/.pre-commit-config.yaml` & `great_tables-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/CODE_OF_CONDUCT.md` & `great_tables-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/CONTRIBUTING.md` & `great_tables-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/LICENSE` & `great_tables-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/Makefile` & `great_tables-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/PKG-INFO` & `great_tables-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.0 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.5.1 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `great-tables-0.5.0/README.md` & `great_tables-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/_extensions/machow/interlinks/interlinks.lua` & `great_tables-0.5.1/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/_quarto.yml` & `great_tables-0.5.1/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/articles/intro.qmd` & `great_tables-0.5.1/docs/articles/intro.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/GT_logo.svg` & `great_tables-0.5.1/docs/assets/GT_logo.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/datasets.png` & `great_tables-0.5.1/docs/assets/datasets.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/gt_parts_of_a_table.svg` & `great_tables-0.5.1/docs/assets/gt_parts_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/gt_sp500_table.svg` & `great_tables-0.5.1/docs/assets/gt_sp500_table.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/gt_workflow_diagram.svg` & `great_tables-0.5.1/docs/assets/gt_workflow_diagram.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/tables_from_the_web.png` & `great_tables-0.5.1/docs/assets/tables_from_the_web.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/assets/the_components_of_a_table.svg` & `great_tables-0.5.1/docs/assets/the_components_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/a_simple_table.png` & `great_tables-0.5.1/docs/blog/design-philosophy/a_simple_table.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/cave_grids.png` & `great_tables-0.5.1/docs/blog/design-philosophy/cave_grids.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png` & `great_tables-0.5.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/computer_tables.png` & `great_tables-0.5.1/docs/blog/design-philosophy/computer_tables.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/index.qmd` & `great_tables-0.5.1/docs/blog/design-philosophy/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png` & `great_tables-0.5.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png` & `great_tables-0.5.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png` & `great_tables-0.5.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/design-philosophy/visicalc.png` & `great_tables-0.5.1/docs/blog/design-philosophy/visicalc.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/introduction-0.2.0/index.qmd` & `great_tables-0.5.1/docs/blog/introduction-0.2.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/introduction-0.3.0/index.qmd` & `great_tables-0.5.1/docs/blog/introduction-0.3.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/introduction-0.4.0/index.qmd` & `great_tables-0.5.1/docs/blog/introduction-0.4.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/introduction_great_tables.qmd` & `great_tables-0.5.1/docs/blog/introduction_great_tables.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/polars-styling/index.qmd` & `great_tables-0.5.1/docs/blog/polars-styling/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/polars-styling/table-preview.png` & `great_tables-0.5.1/docs/blog/polars-styling/table-preview.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/superbowl-squares/_code.py` & `great_tables-0.5.1/docs/blog/superbowl-squares/_code.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/superbowl-squares/games.csv` & `great_tables-0.5.1/docs/blog/superbowl-squares/games.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/blog/superbowl-squares/index.qmd` & `great_tables-0.5.1/docs/blog/superbowl-squares/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/basketball.png` & `great_tables-0.5.1/docs/examples/sports-earnings/basketball.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/boxing.png` & `great_tables-0.5.1/docs/examples/sports-earnings/boxing.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/golf.png` & `great_tables-0.5.1/docs/examples/sports-earnings/golf.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/index.ipynb` & `great_tables-0.5.1/docs/examples/sports-earnings/index.ipynb`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/soccer.png` & `great_tables-0.5.1/docs/examples/sports-earnings/soccer.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/sports_earnings.csv` & `great_tables-0.5.1/docs/examples/sports-earnings/sports_earnings.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/examples/sports-earnings/tennis.png` & `great_tables-0.5.1/docs/examples/sports-earnings/tennis.png`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/basic-column-labels.qmd` & `great_tables-0.5.1/docs/get-started/basic-column-labels.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/basic-formatting.qmd` & `great_tables-0.5.1/docs/get-started/basic-formatting.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/basic-header.qmd` & `great_tables-0.5.1/docs/get-started/basic-header.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/basic-stub.qmd` & `great_tables-0.5.1/docs/get-started/basic-stub.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/basic-styling.qmd` & `great_tables-0.5.1/docs/get-started/basic-styling.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -228,9 +228,9 @@
 )
 ```
 
 ## Learning more
 
 * API Docs:
   - [`GT.tab_style()`](/reference/GT.tab_style.qmd).
-  - [`style.*` and `loc.*` functions`](/reference/index.qmd#location-targeting-and-styling-classes).
-  - [`from_column()`](/reference/from_column.qmd)
+  - [`style.*` and `loc.*` functions](/reference/index.qmd#location-targeting-and-styling-classes).
+  - [`from_column()`](/reference/from_column.qmd).
```

### Comparing `great-tables-0.5.0/docs/get-started/colorizing-with-data.qmd` & `great_tables-0.5.1/docs/get-started/colorizing-with-data.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/column-selection.qmd` & `great_tables-0.5.1/docs/get-started/column-selection.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/index.qmd` & `great_tables-0.5.1/docs/get-started/index.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/nanoplots.qmd` & `great_tables-0.5.1/docs/get-started/nanoplots.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/overview.qmd` & `great_tables-0.5.1/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/row-selection.qmd` & `great_tables-0.5.1/docs/get-started/row-selection.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/table-theme-options.qmd` & `great_tables-0.5.1/docs/get-started/table-theme-options.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/get-started/table-theme-premade.qmd` & `great_tables-0.5.1/docs/get-started/table-theme-premade.qmd`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/docs/styles.css` & `great_tables-0.5.1/docs/styles.css`

 * *Files 3% similar despite different names*

```diff
@@ -138,7 +138,11 @@
 #quarto-search > div > button {
     background-color: white;
     border-radius: 50px;
     width: 150%;
     padding-right: 7px;
     vertical-align: middle;
 }
+
+.shrink-example .cell-output table {
+    zoom: 60%;
+}
```

### Comparing `great-tables-0.5.0/great_tables/__init__.py` & `great_tables-0.5.1/great_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/_boxhead.py` & `great_tables-0.5.1/great_tables/_boxhead.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional, Any
-from typing_extensions import Self
+from typing import TYPE_CHECKING
 
+from ._locations import resolve_cols_c
 from ._utils import _assert_list_is_subset
+from ._tbl_data import SelectExpr
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
-def cols_label(self: GTSelf, **kwargs: Any) -> GTSelf:
+def cols_label(self: GTSelf, **kwargs: str) -> GTSelf:
     """
     Relabel one or more columns.
 
     Column labels can be modified from their default values (the names of the columns from the
     input table data). When you create a table object using [`GT()`](`great_tables.GT`), column
     names effectively become the column labels. While this serves as a good first approximation,
     column names aren't often appealing as column labels in an output table. The `cols_label()`
@@ -86,29 +87,28 @@
     """
 
     # If nothing is provided, return `data` unchanged
     if len(kwargs) == 0:
         return self
 
     mod_columns = list(kwargs.keys())
-    new_labels = list(kwargs.values())
 
     # Get the full list of column names for the data
     column_names = self._boxhead._get_columns()
 
     # Stop function if any of the column names specified are not in `cols_labels`
     # msg: "All column names provided must exist in the input `.data` table."
     _assert_list_is_subset(mod_columns, set_list=column_names)
 
     boxhead = self._boxhead._set_column_labels(kwargs)
 
     return self._replace(_boxhead=boxhead)
 
 
-def cols_align(self: GTSelf, align: str = "left", columns: Optional[str] = None) -> GTSelf:
+def cols_align(self: GTSelf, align: str = "left", columns: SelectExpr = None) -> GTSelf:
     """
     Set the alignment of one or more columns.
 
     The `cols_align()` method sets the alignment of one or more columns. The `align` argument
     can be set to one of `"left"`, `"center"`, or `"right"` and the `columns` argument can be
     used to specify which columns to apply the alignment to. If `columns` is not specified, the
     alignment is applied to all columns.
@@ -159,9 +159,11 @@
     # Upgrade `columns` to a list if `columns` is a string and not None
     if isinstance(columns, str):
         columns = [columns]
         _assert_list_is_subset(columns, set_list=column_names)
     elif columns is None:
         columns = column_names
 
+    sel_cols = resolve_cols_c(data=self, expr=columns)
+
     # Set the alignment for each column
-    return self._replace(_boxhead=self._boxhead._set_column_aligns(columns, align=align))
+    return self._replace(_boxhead=self._boxhead._set_column_aligns(sel_cols, align=align))
```

### Comparing `great-tables-0.5.0/great_tables/_data_color/base.py` & `great_tables-0.5.1/great_tables/_data_color/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from __future__ import annotations
-from typing import (
-    TYPE_CHECKING,
-    Union,
-    List,
-    Optional,
-    Tuple,
-)
-from typing_extensions import TypeAlias
 
-from .constants import DEFAULT_PALETTE, COLOR_NAME_TO_HEX, ALL_PALETTES
+from typing import TYPE_CHECKING
 
-from great_tables._tbl_data import is_na, DataFrameLike
-from great_tables.style import fill, text
-from great_tables.loc import body
 import numpy as np
+from great_tables._tbl_data import DataFrameLike, is_na
+from great_tables.loc import body
+from great_tables.style import fill, text
+from typing_extensions import TypeAlias
+
+from .constants import ALL_PALETTES, COLOR_NAME_TO_HEX, DEFAULT_PALETTE
 
 if TYPE_CHECKING:
     from great_tables._types import GTSelf
 
 
+RGBColor: TypeAlias = tuple[int, int, int]
+
+
 def data_color(
     self: GTSelf,
-    columns: Union[str, List[str], None] = None,
-    palette: Union[str, List[str], None] = None,
-    domain: Union[List[str], List[float], List[int], None] = None,
-    na_color: Optional[str] = None,
-    alpha: Optional[Union[int, float]] = None,
+    columns: str | list[str] | None = None,
+    palette: str | list[str] | None = None,
+    domain: list[str] | list[int] | list[float] | None = None,
+    na_color: str | None = None,
+    alpha: int | float | None = None,
     reverse: bool = False,
     autocolor_text: bool = True,
 ) -> GTSelf:
     """
     Perform data cell colorization.
 
     It's possible to add color to data cells according to their values with the `data_color()`
@@ -181,38 +179,32 @@
     # If palette is not provided, use a default palette
     if palette is None:
         palette = DEFAULT_PALETTE
     elif isinstance(palette, str):
         # Check if the `palette` value refers to a ColorBrewer or viridis palette
         # and, if it is, then convert it to a list of hexadecimal color values; otherwise,
         # convert it to a list (this assumes that the value is a single color)
-        if palette in ALL_PALETTES:
-            palette = ALL_PALETTES[palette]
-        else:
-            palette = [palette]
+        palette = ALL_PALETTES.get(palette, [palette])
 
     # Reverse the palette if `reverse` is set to `True`
     if reverse:
         palette = palette[::-1]
 
     # Standardize values in `palette` to hexadecimal color values
     palette = _html_color(colors=palette, alpha=alpha)
 
     # Set a flag to indicate whether or not the domain should be calculated automatically
-    if domain is None:
-        autocalc_domain = True
-    else:
-        autocalc_domain = False
+    autocalc_domain = domain is None
 
     # Get the internal data table
     data_table = self._tbl_data
 
     # If `columns` is a single value, convert it to a list; if it is None then
     # get a list of all columns in the table body
-    columns_resolved: List[str]
+    columns_resolved: list[str]
 
     if isinstance(columns, str):
         columns_resolved = [columns]
     elif columns is None:
         columns_resolved = data_table.columns
     else:
         columns_resolved = columns
@@ -264,26 +256,26 @@
         color_vals = color_scale_fn(scaled_vals)
 
         # Replace 'None' and 'np.nan' values in `color_vals` with the `na_color=` color
         color_vals = [na_color if is_na(data_table, x) else x for x in color_vals]
 
         # for every color value in color_vals, apply a fill to the corresponding cell
         # by using `tab_style()`
-        for i, _ in enumerate(color_vals):
+        for i, color_val in enumerate(color_vals):
             if autocolor_text:
-                fgnd_color = _ideal_fgnd_color(bgnd_color=color_vals[i])
+                fgnd_color = _ideal_fgnd_color(bgnd_color=color_val)
 
                 gt_obj = gt_obj.tab_style(
-                    style=[text(color=fgnd_color), fill(color=color_vals[i])],
+                    style=[text(color=fgnd_color), fill(color=color_val)],
                     locations=body(columns=col, rows=[i]),
                 )
 
             else:
                 gt_obj = gt_obj.tab_style(
-                    style=fill(color=color_vals[i]), locations=body(columns=col, rows=[i])
+                    style=fill(color=color_val), locations=body(columns=col, rows=[i])
                 )
     return gt_obj
 
 
 def _ideal_fgnd_color(bgnd_color: str, light: str = "#FFFFFF", dark: str = "#000000") -> str:
     # Remove alpha value from hexadecimal color value in `bgnd_color=`
     bgnd_color = _remove_alpha(colors=[bgnd_color])[0]
@@ -323,41 +315,41 @@
 
     # Calculate the contrast ratio between the two colors
     contrast_ratio = (max(l_1, l_2) + 0.05) / (min(l_1, l_2) + 0.05)
 
     return contrast_ratio
 
 
-def _hex_to_rgb(hex_color: str) -> Tuple[int, int, int]:
+def _hex_to_rgb(hex_color: str) -> RGBColor:
     """
     Convert a hexadecimal color value to RGB.
 
     Parameters
     ----------
     hex_color
         The hexadecimal color value.
 
     Returns
     -------
-    Tuple[int, int, int]
+    RGBColor
         The RGB values.
     """
 
     # If the hexadecimal color value is in the #RRGGBBAA format, then we need to remove the
     # alpha value from it before converting it to RGB
     if len(hex_color) == 9:
         hex_color = hex_color[:-2]
 
     # Convert the hexadecimal color value to RGB
     rgb = tuple(int(hex_color[i : i + 2], 16) for i in (1, 3, 5))
 
-    return rgb
+    return rgb  # type: ignore
 
 
-def _relative_luminance(rgb: Tuple[int, int, int]) -> float:
+def _relative_luminance(rgb: RGBColor) -> float:
     """
     Calculate the relative luminance of an RGB color.
 
     Parameters
     ----------
     rgb
         The RGB color.
@@ -398,15 +390,15 @@
         x_frac = x_frac / 12.92
     else:
         x_frac = ((x_frac + 0.055) / 1.055) ** 2.4
 
     return x_frac
 
 
-def _html_color(colors: List[str], alpha: Optional[Union[int, float]] = None) -> List[str]:
+def _html_color(colors: list[str], alpha: int | float | None = None) -> list[str]:
     """
     Normalize HTML colors.
 
     Input colors can be color names (e.g., `"green"`, `"steelblue"`, etc.) or colors in hexadecimal
     format with or without an alpha component (either #RRGGBB or #RRGGBBAA). Output will be a list
     of hexadecimal colors of the same length as the input but it will contain #RRGGBB and #RRGGBBAA
     colors.
@@ -427,15 +419,15 @@
     # color value but only if it doesn't already exist
     if alpha is not None:
         colors = _add_alpha(colors=colors, alpha=alpha)
 
     return colors
 
 
-def _add_alpha(colors: List[str], alpha: Union[int, float]) -> List[str]:
+def _add_alpha(colors: list[str], alpha: int | float) -> list[str]:
     # If `alpha` is an integer, then convert it to a float
     if isinstance(alpha, int):
         alpha = float(alpha)
 
     # If `alpha` is not between 0 and 1, then throw an error
     if alpha < 0 or alpha > 1:
         raise ValueError(
@@ -455,15 +447,15 @@
 
         # Add the alpha value to the color value
         colors[i] = color + _float_to_hex(alpha)
 
     return colors
 
 
-def _remove_alpha(colors: List[str]) -> List[str]:
+def _remove_alpha(colors: list[str]) -> list[str]:
     # Loop through the colors and remove the alpha value from each one
     for i in range(len(colors)):
         color = colors[i]
         # If the color value is already in the `#RRGGBB` format, then we need to add the
         # alpha value to it before removing the alpha value
         if _is_standard_hex_col([color])[0]:
             color = color + "FF"
@@ -498,19 +490,19 @@
     # If the hexadecimal value is only one character long, then add a leading '0'
     if len(x_hex) == 1:
         x_hex = "0" + x_hex
 
     return x_hex
 
 
-def _color_name_to_hex(colors: List[str]) -> List[str]:
+def _color_name_to_hex(colors: list[str]) -> list[str]:
     # If any of the colors are in the color_name_dict, then replace them with the
     # corresponding hexadecimal value
 
-    hex_colors: List[str] = []
+    hex_colors: list[str] = []
 
     for color in colors:
 
         if _is_hex_col([color])[0]:
             hex_colors.append(color)
         else:
             try:
@@ -519,32 +511,32 @@
                 raise ValueError(
                     f"Invalid color name provided ({color}). Please ensure that all colors are valid CSS3 or X11 color names."
                 )
 
     return hex_colors
 
 
-def _color_name_list() -> List[str]:
+def _color_name_list() -> list[str]:
     return list(COLOR_NAME_TO_HEX)
 
 
 def _is_short_hex(color: str) -> bool:
     import re
 
     pattern = r"^#[0-9a-fA-F]{3}([0-9a-fA-F])?$"
     return re.match(pattern, color) is not None
 
 
-def _is_hex_col(colors: List[str]) -> List[bool]:
+def _is_hex_col(colors: list[str]) -> list[bool]:
     import re
 
     return [bool(re.match(r"^#[0-9a-fA-F]{6}([0-9a-fA-F]{2})?$", color)) for color in colors]
 
 
-def _is_standard_hex_col(colors: List[str]) -> List[bool]:
+def _is_standard_hex_col(colors: list[str]) -> list[bool]:
     import re
 
     return [bool(re.match(r"^#[0-9a-fA-F]{6}$", color)) for color in colors]
 
 
 def _expand_short_hex(hex_color: str) -> str:
     """
@@ -559,41 +551,31 @@
     # If the hex color is not a short hexadecimal color value, return the original value
     if not _is_short_hex(color=hex_color):
         return hex_color
 
     # Get the hex color without the leading '#'
     hex_color = hex_color[1:]
 
-    # Get the first character of the hex color
-    first_char = hex_color[0]
-
-    # Get the second character of the hex color
-    second_char = hex_color[1]
-
-    # Get the third character of the hex color
-    third_char = hex_color[2]
-
     # Return the expanded 6-digit hexadecimal color value
-    expanded = "#" + first_char + first_char + second_char + second_char + third_char + third_char
+    expanded = "#" + "".join(x * 2 for x in hex_color)
     expanded = expanded.upper()
     return expanded
 
 
 def _rescale_numeric(
-    df: DataFrameLike, vals: List[Union[int, float]], domain: List[float]
-) -> List[float]:
+    df: DataFrameLike, vals: list[int | float], domain: list[float]
+) -> list[float]:
     """
     Rescale numeric values
 
     Rescale the numeric values in `vals=` to the range [0, 1] using the domain provided.
     """
 
     # Get the minimum and maximum values from `domain`
-    domain_min = domain[0]
-    domain_max = domain[1]
+    domain_min, domain_max = domain
 
     # Get the range of values in `domain`
     domain_range = domain_max - domain_min
 
     if domain_range == 0:
         # In the case where the domain range is 0, all scaled values in `vals` will be `0`
         scaled_vals = [0.0 if not is_na(df, x) else x for x in vals]
@@ -604,16 +586,16 @@
     # Add NA values to any values in `scaled_vals` that are not in the [0, 1] range
     scaled_vals = [x if not is_na(df, x) and (x >= 0 and x <= 1) else np.nan for x in scaled_vals]
 
     return scaled_vals
 
 
 def _rescale_factor(
-    df: DataFrameLike, vals: List[Union[int, float]], domain: List[float], palette: List[str]
-) -> List[float]:
+    df: DataFrameLike, vals: list[int | float], domain: list[float], palette: list[str]
+) -> list[float]:
     """
     Rescale factor values
 
     Rescale the factor values in `vals=` to the range [0, 1] using the domain provided.
     """
 
     domain_length = len(domain)
@@ -631,15 +613,15 @@
         vals=[domain.index(x) if x in domain else np.nan for x in vals],
         domain=[0, domain_length],
     )
 
     return scaled_vals
 
 
-def _get_domain_numeric(df: DataFrameLike, vals: List[Union[int, float]]) -> List[float]:
+def _get_domain_numeric(df: DataFrameLike, vals: list[int | float]) -> list[float]:
     """
     Get the domain of numeric values.
 
     Get the domain of numeric values in `vals=` as a list of two values: the min and max values.
     """
 
     # Exclude any NA values from `vals`
@@ -651,27 +633,25 @@
 
     # Create the domain
     domain = [domain_min, domain_max]
 
     return domain
 
 
-def _get_domain_factor(df: DataFrameLike, vals: List[str]) -> List[str]:
+def _get_domain_factor(df: DataFrameLike, vals: list[str]) -> list[str]:
     """
     Get the domain of factor values.
 
     Get the domain of factor values in `vals=` as a list of the unique values in the order provided.
     """
 
     # Exclude any NA values from `vals`
     vals = [x for x in vals if not is_na(df, x)]
 
     # Create the domain by getting the unique values in `vals` in order provided
-    unique_list: List[str] = []
-    seen: List[str] = []
+    seen: list[str] = []
 
     for item in vals:
         if item not in seen:
-            unique_list.append(item)
             seen.append(item)
 
     return seen
```

### Comparing `great-tables-0.5.0/great_tables/_data_color/constants.py` & `great_tables-0.5.1/great_tables/_data_color/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 DEFAULT_PALETTE = [
     "#000000",
     "#DF536B",
     "#61D04F",
     "#2297E6",
     "#28E2E5",
     "#CD0BBC",
```

### Comparing `great-tables-0.5.0/great_tables/_data_color/palettes.py` & `great_tables-0.5.1/great_tables/_data_color/palettes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Palette classes for translating data to color values.
 
 Note that this code is largely a pure python port of the mizani gradient_n_pal code.
 """
 
-from bisect import bisect
-from math import isnan, isinf
-from typing import TypedDict, Tuple
-from typing_extensions import TypeAlias
+from __future__ import annotations
 
-from .base import _html_color, _hex_to_rgb
+from bisect import bisect
+from math import isinf, isnan
+from typing import TypedDict
 
-RGBColor: TypeAlias = Tuple[int, int, int]
+from .base import RGBColor, _hex_to_rgb, _html_color
 
 
 def rgb_to_hex(rgb: RGBColor) -> str:
     return f"#{rgb[0]:02x}{rgb[1]:02x}{rgb[2]:02x}"
 
 
 # data ---------------------------------------------------------------------------------------------
```

### Comparing `great-tables-0.5.0/great_tables/_databackend.py` & `great_tables-0.5.1/great_tables/_databackend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 import importlib
 
 from abc import ABCMeta
 
 
 def _load_class(mod_name: str, cls_name: str):
```

### Comparing `great-tables-0.5.0/great_tables/_export.py` & `great_tables-0.5.1/great_tables/_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
-from ._utils import _try_import
-from typing import Literal, TYPE_CHECKING
-from typing_extensions import TypeAlias
+
 import tempfile
+from typing import TYPE_CHECKING, Literal
+
+from typing_extensions import TypeAlias
+
+from ._utils import _try_import
 
 if TYPE_CHECKING:
     # Note that as_raw_html uses methods on the GT class, not just data
     from .gt import GT
 
 
 def as_raw_html(
```

### Comparing `great-tables-0.5.0/great_tables/_formats.py` & `great_tables-0.5.1/great_tables/_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 from __future__ import annotations
 
-import babel
-
+import math
+from datetime import date, datetime, time
 from decimal import Decimal
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    ClassVar,
-    TypeVar,
-    TypedDict,
-    Union,
-    List,
-    Tuple,
-    cast,
-    Optional,
-    Dict,
-    Literal,
-)
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Literal, TypedDict, TypeVar, cast
+
+import babel
+from babel.dates import format_date, format_datetime, format_time
 from typing_extensions import TypeAlias
-from ._tbl_data import PlExpr, SelectExpr, is_na, to_list, _get_column_dtype
-from ._gt_data import GTData, FormatFns, FormatFn, FormatInfo
-from ._locale import _get_locales_data, _get_default_locales_data, _get_currencies_data
-from ._locations import resolve_rows_i, resolve_cols_c
+
+from ._gt_data import FormatFn, FormatFns, FormatInfo, GTData
+from ._helpers import px
+from ._locale import _get_currencies_data, _get_default_locales_data, _get_locales_data
+from ._locations import resolve_cols_c, resolve_rows_i
+from ._tbl_data import PlExpr, SelectExpr, _get_column_dtype, is_na, to_list
 from ._text import _md_html
 from ._utils import _str_detect, _str_replace
 from ._utils_nanoplots import _generate_nanoplot
-import math
-from datetime import datetime, date, time
-from babel.dates import format_date, format_time, format_datetime
-from pathlib import Path
 
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 T = TypeVar("T")
 DateStyle: TypeAlias = Literal[
@@ -72,18 +60,18 @@
     "zero",
     "remove",
 ]
 
 
 def fmt(
     self: GTSelf,
-    fns: Union[FormatFn, FormatFns],
+    fns: FormatFn | FormatFns,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
-    is_substitution=False,
+    rows: int | list[int] | None = None,
+    is_substitution: bool = False,
 ) -> GTSelf:
     """
     Set a column format with a formatter function.
 
     The `fmt()` method provides a way to execute custom formatting functionality with raw data
     values in a way that can consider all output contexts.
 
@@ -129,27 +117,27 @@
 
     return self._replace(_formats=[*self._formats, formatter])
 
 
 def fmt_number(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     scale_by: float = 1,
     compact: bool = False,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format numeric values.
 
     With numeric values within a table's body cells, we can perform number-based formatting so that
     the targeted values are rendered with a higher consideration for tabular presentation.
     Furthermore, there is finer control over numeric formatting with the following options:
@@ -276,26 +264,29 @@
 
     # Use locale-based marks if a locale ID is provided
     sep_mark = _get_locale_sep_mark(default=sep_mark, use_seps=use_seps, locale=locale)
     dec_mark = _get_locale_dec_mark(default=dec_mark, locale=locale)
 
     # Generate a function that will operate on single `x` values in the table body
     def fmt_number_fn(
-        x: float,
+        x: float | None,
         decimals: int = decimals,
-        n_sigfig: Optional[int] = n_sigfig,
+        n_sigfig: int | None = n_sigfig,
         drop_trailing_zeros: bool = drop_trailing_zeros,
         drop_trailing_dec_mark: bool = drop_trailing_dec_mark,
         use_seps: bool = use_seps,
         scale_by: float = scale_by,
         compact: bool = compact,
         sep_mark: str = sep_mark,
         dec_mark: str = dec_mark,
         force_sign: bool = force_sign,
     ):
+        if is_na(self._tbl_data, x):
+            return x
+
         # Scale `x` value by a defined `scale_by` value
         x = x * scale_by
 
         # Determine whether the value is positive
         is_negative = _has_negative_value(value=x)
 
         if compact:
@@ -336,22 +327,22 @@
 
     return fmt(self, fns=fmt_number_fn, columns=columns, rows=rows)
 
 
 def fmt_integer(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     use_seps: bool = True,
     scale_by: float = 1,
     compact: bool = False,
     pattern: str = "{x}",
     sep_mark: str = ",",
     force_sign: bool = False,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as integers.
 
     With numeric values in one or more table columns, we can perform number-based formatting so that
     the targeted values are always rendered as integer values.
 
@@ -506,27 +497,27 @@
 
     return fmt(self, fns=fmt_integer_fn, columns=columns, rows=rows)
 
 
 def fmt_scientific(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     scale_by: float = 1,
     exp_style: str = "x10n",
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign_m: bool = False,
     force_sign_n: bool = False,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values to scientific notation.
 
     With numeric values in a table, we can perform formatting so that the targeted values are
     rendered in scientific notation, where extremely large or very small numbers can be expressed in
     a more practical fashion. Here, numbers are written in the form of a mantissa (`m`) and an
@@ -660,15 +651,15 @@
     sep_mark = _get_locale_sep_mark(default=sep_mark, use_seps=use_seps, locale=locale)
     dec_mark = _get_locale_dec_mark(default=dec_mark, locale=locale)
 
     # Generate a function that will operate on single `x` values in the table body
     def fmt_scientific_fn(
         x: float,
         decimals: int = decimals,
-        n_sigfig: Optional[int] = n_sigfig,
+        n_sigfig: int | None = n_sigfig,
         drop_trailing_zeros: bool = drop_trailing_zeros,
         drop_trailing_dec_mark: bool = drop_trailing_dec_mark,
         scale_by: float = scale_by,
         exp_style: str = exp_style,
         sep_mark: str = sep_mark,
         dec_mark: str = dec_mark,
         force_sign_m: bool = force_sign_m,
@@ -691,16 +682,15 @@
             decimals=decimals,
             n_sigfig=n_sigfig,
             dec_mark=dec_mark,
         )
 
         sci_parts = x_sci_notn.split("E")
 
-        m_part = sci_parts[0]
-        n_part = sci_parts[1]
+        m_part, n_part = sci_parts
 
         # Remove trailing zeros and decimal marks from the `m_part`
         if drop_trailing_zeros:
             m_part = m_part.rstrip("0")
         if drop_trailing_dec_mark:
             m_part = m_part.rstrip(".")
 
@@ -768,27 +758,27 @@
 
     return fmt(self, fns=fmt_scientific_fn, columns=columns, rows=rows)
 
 
 def fmt_percent(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     decimals: int = 2,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     scale_values: bool = True,
     use_seps: bool = True,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     placement: str = "right",
     incl_space: bool = False,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as a percentage.
 
     With numeric values in a **gt** table, we can perform percentage-based formatting. It is assumed
     the input numeric values are proportional values and, in this case, the values will be
     automatically multiplied by `100` before decorating with a percent sign (the other case is
@@ -970,28 +960,28 @@
 
     return fmt(self, fns=fmt_percent_fn, columns=columns, rows=rows)
 
 
 def fmt_currency(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
-    currency: Optional[str] = None,
+    rows: int | list[int] | None = None,
+    currency: str | None = None,
     use_subunits: bool = True,
-    decimals: Optional[int] = None,
+    decimals: int | None = None,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     scale_by: float = 1,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     placement: str = "left",
     incl_space: bool = False,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as currencies.
 
     With numeric values in a **gt** table, we can perform currency-based formatting with the
     `fmt_currency()` method. This supports both automatic formatting with a three-letter currency
     code. We have fine control over the conversion from numeric values to currency values, where we
@@ -1213,15 +1203,15 @@
 
     return fmt(self, fns=fmt_currency_fn, columns=columns, rows=rows)
 
 
 def fmt_roman(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     case: str = "upper",
     pattern: str = "{x}",
 ) -> GTSelf:
     """
     Format values as Roman numerals.
 
     With numeric values in a **gt** table we can transform those to Roman numerals, rounding values
@@ -1323,27 +1313,27 @@
 
     return fmt(self, fns=fmt_roman_fn, columns=columns, rows=rows)
 
 
 def fmt_bytes(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     standard: str = "decimal",
     decimals: int = 1,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = True,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     incl_space: bool = True,
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as bytes.
 
     With numeric values in a table, we can transform those to values of bytes with human readable
     units. The `fmt_bytes()` method allows for the formatting of byte sizes to either of two common
     representations: (1) with decimal units (powers of 1000, examples being `"kB"` and `"MB"`), and
@@ -1478,17 +1468,17 @@
         base = 1024
         byte_units = ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB"]
 
     # Generate a function that will operate on single `x` values in the table body
     def fmt_bytes_fn(
         x: float,
         base: int = base,
-        byte_units: List[str] = byte_units,
+        byte_units: list[str] = byte_units,
         decimals: int = decimals,
-        n_sigfig: Optional[int] = n_sigfig,
+        n_sigfig: int | None = n_sigfig,
         drop_trailing_zeros: bool = drop_trailing_zeros,
         drop_trailing_dec_mark: bool = drop_trailing_dec_mark,
         use_seps: bool = use_seps,
         sep_mark: str = sep_mark,
         dec_mark: str = dec_mark,
         force_sign: bool = force_sign,
         incl_space: bool = incl_space,
@@ -1561,18 +1551,18 @@
 
     return fmt(self, fns=fmt_bytes_fn, columns=columns, rows=rows)
 
 
 def fmt_date(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     date_style: DateStyle = "iso",
     pattern: str = "{x}",
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as dates.
 
     Format input values to time values using one of 17 preset date styles. Input can be in the form
     of `date` type or as a ISO-8601 string (in the form of `YYYY-MM-DD HH:MM:SS` or `YYYY-MM-DD`).
 
@@ -1670,27 +1660,25 @@
     locale = _normalize_locale(locale=locale)
 
     # Get the date format string based on the `date_style` value
     date_format_str = _get_date_format(date_style=date_style)
 
     # Generate a function that will operate on single `x` values in the table body
     def fmt_date_fn(
-        x: Any, date_format_str: str = date_format_str, locale: Union[str, None] = locale
+        x: Any, date_format_str: str = date_format_str, locale: str | None = locale
     ) -> str:
         # If the `x` value is a Pandas 'NA', then return the same value
         if is_na(self._tbl_data, x):
             return x
 
         # If `x` is a string, we assume it is an ISO date string and convert it to a date object
         if isinstance(x, str):
-            # Stop if `x` is not a valid ISO date string
-            _validate_iso_date_str(x=x)
 
             # Convert the ISO date string to a date object
-            x = _iso_to_date(x)
+            x = _iso_str_to_date(x)
 
         else:
             # Stop if `x` is not a valid date object
             _validate_date_obj(x=x)
 
         # Fix up the locale for `format_date()` by replacing any hyphens with underscores
         if locale is None:
@@ -1709,18 +1697,18 @@
 
     return fmt(self, fns=fmt_date_fn, columns=columns, rows=rows)
 
 
 def fmt_time(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     time_style: TimeStyle = "iso",
     pattern: str = "{x}",
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as times.
 
     Format input values to time values using one of 5 preset time styles. Input can be in the form
     of `time` values, or strings in the ISO 8601 forms of `HH:MM:SS` or `YYYY-MM-DD HH:MM:SS`.
 
@@ -1806,30 +1794,25 @@
     locale = _normalize_locale(locale=locale)
 
     # Get the time format string based on the `time_style` value
     time_format_str = _get_time_format(time_style=time_style)
 
     # Generate a function that will operate on single `x` values in the table body
     def fmt_time_fn(
-        x: Any, time_format_str: str = time_format_str, locale: Union[str, None] = locale
+        x: Any, time_format_str: str = time_format_str, locale: str | None = locale
     ) -> str:
         # If the `x` value is a Pandas 'NA', then return the same value
         if is_na(self._tbl_data, x):
             return x
 
         # If `x` is a string, assume it is an ISO time string and convert it to a time object
         if isinstance(x, str):
-            # Stop if `x` is not a valid ISO time string
-            _validate_iso_time_str(x=x)
-
-            # Ensure that a seconds value is present in the ISO time string
-            x = _normalize_iso_time_str(x=x)
 
             # Convert the ISO time string to a time object
-            x = _iso_to_time(x)
+            x = _iso_str_to_time(x)
 
         else:
             # Stop if `x` is not a valid time object
             _validate_time_obj(x=x)
 
         # Fix up the locale for `format_time()` by replacing any hyphens with underscores
         if locale is None:
@@ -1848,20 +1831,20 @@
 
     return fmt(self, fns=fmt_time_fn, columns=columns, rows=rows)
 
 
 def fmt_datetime(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     date_style: DateStyle = "iso",
     time_style: TimeStyle = "iso",
     sep: str = " ",
     pattern: str = "{x}",
-    locale: Union[str, None] = None,
+    locale: str | None = None,
 ) -> GTSelf:
     """
     Format values as datetimes.
 
     Format input values to datetime values using one of 17 preset date styles and one of 5 preset
     time styles. Input can be in the form of `datetime` values, or strings in the ISO 8601 forms of
     `YYYY-MM-DD HH:MM:SS` or `YYYY-MM-DD`.
@@ -1969,33 +1952,28 @@
     # Generate a function that will operate on single `x` values in the table body using both
     # the date and time format strings
     def fmt_datetime_fn(
         x: Any,
         date_format_str: str = date_format_str,
         time_format_str: str = time_format_str,
         sep: str = sep,
-        locale: Union[str, None] = locale,
+        locale: str | None = locale,
     ) -> str:
         # If the `x` value is a Pandas 'NA', then return the same value
         if is_na(self._tbl_data, x):
             return x
 
         # From the date and time format strings, create a datetime format string
         datetime_format_str = f"{date_format_str}'{sep}'{time_format_str}"
 
         # If `x` is a string, assume it is an ISO datetime string and convert it to a datetime object
         if isinstance(x, str):
-            # Stop if `x` is not a valid ISO datetime string
-            _validate_iso_datetime_str(x=x)
-
-            # Ensure that a seconds value is present in the ISO datetime string
-            x = _normalize_iso_datetime_str(x=x)
 
             # Convert the ISO datetime string to a datetime object
-            x = _iso_to_datetime(x)
+            x = _iso_str_to_datetime(x)
 
         else:
             # Stop if `x` is not a valid datetime object
             _validate_datetime_obj(x=x)
 
         # Fix up the locale for `format_datetime()` by replacing any hyphens with underscores
         if locale is None:
@@ -2011,67 +1989,18 @@
             x_formatted = pattern.replace("{x}", x_formatted)
 
         return x_formatted
 
     return fmt(self, fns=fmt_datetime_fn, columns=columns, rows=rows)
 
 
-def _validate_iso_datetime_str(x: str) -> None:
-    """
-    Validate an ISO datetime string.
-
-    Parameters
-    ----------
-    x
-        The string to validate.
-
-    Raises
-    ------
-    ValueError
-        Raised if the string is not a valid ISO datetime string.
-    """
-
-    import re
-
-    # Define the regex pattern for a valid ISO datetime string
-    _ISO_DATETIME_REGEX = r"^\d{4}-\d{2}-\d{2}(T| )\d{2}:\d{2}(:\d{2})?$"
-
-    # Use regex to determine if string is a valid ISO datetime string
-    if not re.match(_ISO_DATETIME_REGEX, x):
-        raise ValueError(f'"{x}" is not a valid ISO datetime string')
-
-    return
-
-
-def _normalize_iso_datetime_str(x: str) -> str:
-    """
-    Normalize an ISO datetime string.
-
-    Parameters
-    ----------
-    x
-        The string to normalize.
-
-    Returns
-    -------
-    str
-        The normalized string.
-    """
-
-    # If the string does not have a seconds value, then add one
-    if len(x) == 16:
-        x = x + ":00"
-
-    return x
-
-
 def fmt_markdown(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
 ) -> GTSelf:
     """
     Format Markdown text.
 
     Any Markdown-formatted text in the incoming cells will be transformed during render when using
     the `fmt_markdown()` method.
 
@@ -2110,17 +2039,17 @@
 
         return x_formatted
 
     return fmt(self, fns=fmt_markdown_fn, columns=columns, rows=rows)
 
 
 def _value_to_decimal_notation(
-    value: Union[int, float],
+    value: int | float,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
 ) -> str:
@@ -2156,32 +2085,32 @@
             drop_trailing_zeros=drop_trailing_zeros,
             use_seps=use_seps,
             sep_mark=sep_mark,
             dec_mark=dec_mark,
         )
 
     # Drop the trailing decimal mark if it is present
-    if drop_trailing_dec_mark is True:
+    if drop_trailing_dec_mark:
         result = result.rstrip(dec_mark)
 
     # Add in a trailing decimal mark under specific circumstances
     if drop_trailing_dec_mark is False and dec_mark not in result:
         result = result + dec_mark
 
     # Force the positive sign to be present if the `force_sign` option is taken
     if is_positive and force_sign:
         result = "+" + result
 
     return result
 
 
 def _value_to_scientific_notation(
-    value: Union[int, float],
+    value: int | float,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     dec_mark: str = ".",
 ) -> str:
     """
     Scientific notation.
 
     Returns a string value with the correct precision and 10s exponent. An 'E' is placed between
     the decimal value and 10s exponent.
@@ -2201,15 +2130,15 @@
         + "E"
         + str(ten_power)
     )
 
     return result
 
 
-def _value_to_engineering_notation(value: Union[int, float], n_sigfig: int, exp_style: str) -> str:
+def _value_to_engineering_notation(value: int | float, n_sigfig: int, exp_style: str) -> str:
     """
     Engineering notation.
 
     Returns a string value with the correct precision and an exponent that is divisible by three.
     The `exp_style` text is placed between the decimal value and the exponent.
     """
 
@@ -2225,15 +2154,15 @@
         + str(eng_power)
     )
 
     return result
 
 
 def _format_number_n_sigfig(
-    value: Union[int, float],
+    value: int | float,
     n_sigfig: int,
     use_seps: bool = True,
     sep_mark: str = ",",
     dec_mark: str = ".",
     preserve_integer: bool = False,
 ) -> str:
     sig_digits, power, is_negative = _get_number_profile(value, n_sigfig)
@@ -2269,15 +2198,15 @@
     # Combine the integer and decimal parts
     result = formatted_integer + formatted_decimal
 
     return result
 
 
 def _format_number_fixed_decimals(
-    value: Union[int, float],
+    value: int | float,
     decimals: int,
     drop_trailing_zeros: bool = False,
     use_seps: bool = True,
     sep_mark: str = ",",
     dec_mark: str = ".",
 ) -> str:
     # If `number` is a string, cast it into a float
@@ -2323,24 +2252,24 @@
         formatted_integer = "-" + formatted_integer
 
     # Combine the integer and decimal parts
     result = formatted_integer + formatted_decimal
 
     # Drop any trailing zeros if option is taken (this purposefully doesn't apply to numbers
     # formatted to a specific number of significant digits)
-    if drop_trailing_zeros is True:
+    if drop_trailing_zeros:
         result = result.rstrip("0")
 
     return result
 
 
 def _format_number_compactly(
-    value: Union[int, float],
+    value: int | float,
     decimals: int,
-    n_sigfig: Optional[int],
+    n_sigfig: int | None,
     drop_trailing_zeros: bool,
     drop_trailing_dec_mark: bool,
     use_seps: bool,
     sep_mark: str,
     dec_mark: str,
     force_sign: bool,
 ) -> str:
@@ -2395,15 +2324,15 @@
 
 def _expand_exponential_to_full_string(str_number: str) -> str:
     decimal_number = Decimal(str_number)
     formatted_number = "{:f}".format(decimal_number)
     return formatted_number
 
 
-def _get_number_profile(value: Union[int, float], n_sigfig: int) -> tuple[str, int, bool]:
+def _get_number_profile(value: int | float, n_sigfig: int) -> tuple[str, int, bool]:
     """
     Get key components of a number for decimal number formatting.
 
     Returns a tuple containing: (1) a string value of significant digits, (2) an
     exponent to get the decimal mark to the proper location, and (3) a boolean
     value that's True if the value is less than zero (i.e., negative).
     """
@@ -2424,15 +2353,15 @@
             power -= 1
 
         sig_digits = str(int(round(value * 10.0**power)))
 
     return sig_digits, int(-power), is_negative
 
 
-def _get_sci_parts(value: Union[int, float], n_sigfig: int) -> tuple[bool, str, int, int]:
+def _get_sci_parts(value: int | float, n_sigfig: int) -> tuple[bool, str, int, int]:
     """
     Returns the properties for constructing a number in scientific notation.
     """
 
     value = float(value)
     sig_digits, power, is_negative = _get_number_profile(value, n_sigfig)
 
@@ -2477,32 +2406,32 @@
     else:
         out = digits + (dec_mark if digits[-1] == "0" and len(digits) > 1 else "")
 
     return out
 
 
 def _listify(
-    x: Union[T, List[T], None],
-    default: Callable[[], List[T]],
-) -> List[T]:
+    x: T | list[T] | None,
+    default: Callable[[], list[T]],
+) -> list[T]:
     """
     Convert the input into a list.
 
     Parameters
     ----------
     x
         The input value to be converted into a list. It can be a single value of type T, a list of
         values of type T, or None.
     default
         A callable that returns a default list when the input value is None.
 
     Returns
     -------
 
-    List[T]: The converted list.
+    list[T]: The converted list.
 
     Raises:
         None
 
     Examples:
         _listify(5, lambda: [1, 2, 3])  # Output: [5]
         _listify([1, 2, 3], lambda: [4, 5, 6])  # Output: [1, 2, 3]
@@ -2512,31 +2441,31 @@
         return default()
     elif not isinstance(x, list):
         return [x]
     else:
         return cast(Any, x)
 
 
-def _has_negative_value(value: Union[int, float]) -> bool:
+def _has_negative_value(value: int | float) -> bool:
     return value < 0
 
 
-def _has_positive_value(value: Union[int, float]) -> bool:
+def _has_positive_value(value: int | float) -> bool:
     return value > 0
 
 
-def _has_zero_value(value: Union[int, float]) -> bool:
+def _has_zero_value(value: int | float) -> bool:
     return value == 0
 
 
-def _has_sci_order_zero(value: Union[int, float]) -> bool:
+def _has_sci_order_zero(value: int | float) -> bool:
     return (value >= 1 and value < 10) or (value <= -1 and value > -10) or value == 0
 
 
-def _context_exp_marks() -> List[str]:
+def _context_exp_marks() -> list[str]:
     return [" \u00D7 10<sup style='font-size: 65%;'>", "</sup>"]
 
 
 def _context_exp_str(exp_style: str) -> str:
     if exp_style == "low-ten":
         # For the 'low-ten' style, use a specialized `exp_str` string value
         exp_str = "<sub style='font-size: 65%;'>10</sub>"
@@ -2580,15 +2509,15 @@
     if len(filtered_pd_df) != 1:
         raise Exception(
             "Internal Error, the filtered table doesn't result in a table of exactly one row."
         )
     return filtered_pd_df[0]
 
 
-def _get_locale_sep_mark(default: str, use_seps: bool, locale: Union[str, None] = None) -> str:
+def _get_locale_sep_mark(default: str, use_seps: bool, locale: str | None = None) -> str:
     # If `use_seps` is False, then force `sep_mark` to be an empty string
     # TODO: what does an empty string signify? Where is this used? Is it the right choice here?
     if not use_seps:
         return ""
 
     # If `locale` is NULL then return the default `sep_mark`
     if locale is None:
@@ -2608,15 +2537,15 @@
     # Replace any `""` or "\u00a0" with `" "` since an empty string actually
     # signifies a space character, and, we want to normalize to a simple space
     sep_mark = " " if sep_mark == "" or sep_mark == "\u00a0" else sep_mark
 
     return sep_mark
 
 
-def _get_locale_dec_mark(default: str, locale: Union[str, None] = None) -> str:
+def _get_locale_dec_mark(default: str, locale: str | None = None) -> str:
     # If `locale` is NULL then return the default `dec_mark`
     if locale is None:
         return default
 
     # Get the correct `decimal` value row from the locales lookup table
     pd_df_row = _filter_pd_df_to_row(pd_df=_get_locales_data(), column="locale", filter_expr=locale)
 
@@ -2629,15 +2558,15 @@
     # TODO: we control this data and should enforce this in the data schema
     if not isinstance(dec_mark, str):
         raise TypeError(f"Variable type mismatch. Expected str, got {type(dec_mark)}.")
 
     return dec_mark
 
 
-def _get_locales_list() -> List[str]:
+def _get_locales_list() -> list[str]:
     """
     Returns a list of locales as strings.
 
     Raises:
         TypeError: If the first element of the locale list is not a string.
     """
 
@@ -2650,15 +2579,15 @@
     # TODO: we control this data and should enforce this in the data schema
     locale_list: Any
     if not isinstance(locale_list[0], str):
         raise TypeError("Variable type mismatch. Expected str, got something entirely different.")
     return locale_list
 
 
-def _validate_locale(locale: Union[str, None] = None) -> None:
+def _validate_locale(locale: str | None = None) -> None:
     """
     Validates the given locale string against a list of supported locales.
 
     Args:
         locale (str or None): The locale string to validate. If None, the function returns without
         doing anything.
 
@@ -2678,18 +2607,16 @@
 
     # Stop if the `locale` provided isn't a valid one
     if supplied_locale not in locales_list and supplied_locale not in default_locales_list:
         raise ValueError(
             f"The normalized locale name `{supplied_locale}` is not in the list of locales."
         )
 
-    return
-
 
-def _normalize_locale(locale: Union[str, None] = None) -> Union[str, None]:
+def _normalize_locale(locale: str | None = None) -> str | None:
     """
     Normalize the given locale string by replacing any underscores with hyphens and resolving any default locales into their base names.
 
     Args:
         locale (str or None): The locale string to normalize. If None, returns None.
 
     Returns:
@@ -2727,15 +2654,15 @@
             "Great Tables uses the libraries like babel for locale-based work. "
             "See the babel.Locale class for more on locale handling."
         )
 
     return supplied_locale
 
 
-def _resolve_locale(x: GTData, locale: Union[str, None] = None) -> Union[str, None]:
+def _resolve_locale(x: GTData, locale: str | None = None) -> str | None:
     # Get the locale from the locale value set globally; note that this may also be None
     # but a None value will eventually be resolved to the 'en' locale
     locale = x._locale._locale if locale is None else locale
 
     # An 'undetermined' locale should map back to the 'en' locale
     if locale == "und":
         locale = "en"
@@ -2745,15 +2672,15 @@
     locale = _normalize_locale(locale=locale)
 
     _validate_locale(locale=locale)
 
     return locale
 
 
-def _get_locale_currency_code(locale: Union[str, None] = None) -> str:
+def _get_locale_currency_code(locale: str | None = None) -> str:
     """
     Given a locale, returns the corresponding currency code. If no locale is provided,
     returns the currency code for the United States ('USD').
 
     Args:
         locale (str or None): A string representing the locale for which to retrieve the
             currency code. If None, the currency code for the United States ('USD') is returned.
@@ -2843,25 +2770,25 @@
     # TODO: how do users know what currencies are supported?
     if currency not in codes:
         raise ValueError(
             f"The supplied currency `{currency}` is not in the list of supported currencies."
         )
 
 
-def _get_currency_decimals(currency: str, decimals: Optional[int], use_subunits: bool) -> int:
+def _get_currency_decimals(currency: str, decimals: int | None, use_subunits: bool) -> int:
     """
     Returns the number of decimal places to use for a given currency.
 
     If `decimals` is not None, it is returned. Otherwise, if `use_subunits` is True,
     the number of decimal places is determined by the currency's exponent. Otherwise,
     the number of decimal places is 0.
 
     Args:
         currency (str): The currency code.
-        decimals (Optional[int]): The number of decimal places to use, if specified.
+        decimals (int | None): The number of decimal places to use, if specified.
         use_subunits (bool): Whether to use subunits for the currency.
 
     Returns:
         int: The number of decimal places to use.
     """
 
     # If `decimals` is not None, return it
@@ -2932,18 +2859,16 @@
     # Check that the input `n_sigfig` is not `None`
     if not isinstance(n_sigfig, int):
         raise TypeError("Any input for `n_sigfig` must be an integer.")
     # The value of `n_sigfig` must be greater than or equal to 1
     if n_sigfig < 1:
         raise ValueError("The value for `n_sigfig` must be greater than or equal to `1`.")
 
-    return
-
 
-def _round_rhu(x: Union[float, int], digits: int = 0) -> float:
+def _round_rhu(x: int | float, digits: int = 0) -> float:
     """
     Rounds a number using the 'Round-Half-Up' (R-H-U) algorithm.
 
     Args:
         x (float): The number to round.
         digits (int): The number of digits to round to.
 
@@ -3011,18 +2936,16 @@
 
     Raises:
         ValueError: If the case argument is not 'upper' or 'lower'.
     """
     if case not in ["upper", "lower"]:
         raise ValueError(f"The `case` argument must be either 'upper' or 'lower' (not '{case}').")
 
-    return
 
-
-def _get_date_formats_dict() -> Dict[str, str]:
+def _get_date_formats_dict() -> dict[str, str]:
     date_formats = {
         "iso": "y-MM-dd",
         "wday_month_day_year": "EEEE, MMMM d, y",
         "wd_m_day_year": "EEE, MMM d, y",
         "wday_day_month_year": "EEEE d MMMM y",
         "month_day_year": "MMMM d, y",
         "m_day_year": "MMM d, y",
@@ -3038,15 +2961,15 @@
         "year_week": "y-'W'ww",
         "year_quarter": "y-'Q'Q",
     }
 
     return date_formats
 
 
-def _get_time_formats_dict() -> Dict[str, str]:
+def _get_time_formats_dict() -> dict[str, str]:
     time_formats = {
         "iso": "HH:mm:ss",
         "iso-short": "HH:mm",
         "h_m_s_p": "h:mm:ss a",
         "h_m_p": "h:mm a",
         "h_p": "h a",
     }
@@ -3114,16 +3037,14 @@
 
     Returns:
         None
     """
     if date_style not in _get_date_formats_dict():
         raise ValueError(f"date_style must be one of: {', '.join(_get_date_formats_dict().keys())}")
 
-    return
-
 
 def _validate_time_style(time_style: str) -> None:
     """
     Validate the time style.
 
     Args:
         time_style (str): The time style to validate.
@@ -3133,120 +3054,52 @@
 
     Returns:
         None
     """
     if time_style not in _get_time_formats_dict():
         raise ValueError(f"time_style must be one of: {', '.join(_get_time_formats_dict().keys())}")
 
-    return
 
-
-def _iso_to_date(x: str) -> date:
-    """
-    Converts a string in ISO format (YYYY-MM-DD) to a date object.
-
-    Args:
-        x (str): The string to be converted.
-
-    Returns:
-        date: The converted date object.
-    """
-    return datetime.strptime(x, "%Y-%m-%d").date()
-
-
-def _iso_to_time(x: str) -> time:
+def _iso_str_to_time(x: str) -> time:
     """
     Converts a string in ISO format to a time object.
 
     Args:
         x (str): The string to be converted.
 
     Returns:
         time: The converted time object.
     """
-    return datetime.strptime(x, "%H:%M:%S").time()
+    return time.fromisoformat(x)
 
 
-def _iso_to_datetime(x: str) -> datetime:
+def _iso_str_to_datetime(x: str) -> datetime:
     """
     Converts a string in ISO format to a datetime object.
 
     Args:
         x (str): The string to be converted.
 
     Returns:
         datetime: The converted datetime object.
     """
-    return datetime.strptime(x, "%Y-%m-%d %H:%M:%S")
-
-
-def _validate_iso_date_str(x: str) -> None:
-    """
-    Validates if the given string is a valid ISO date string in the format 'YYYY-MM-DD'.
-
-    Args:
-        x (str): The string to be validated.
-
-    Raises:
-        ValueError: If the string is not a valid ISO date string.
-
-    Returns:
-        None
-    """
-    try:
-        datetime.strptime(x, "%Y-%m-%d")
-    except ValueError:
-        raise ValueError(
-            f"Invalid ISO date string: '{x}'. The string must be in the format 'YYYY-MM-DD'."
-        )
-
-    return
-
-
-def _validate_iso_time_str(x: str) -> None:
-    """
-    Validates if the input string `x` is a valid ISO time string.
+    return datetime.fromisoformat(x)
 
-    Args:
-        x (str): The input string to be validated.
-
-    Raises:
-        ValueError: If `x` is not a valid ISO time string (HH:MM:SS or HH:MM).
 
-    Returns:
-        None
+def _iso_str_to_date(x: str) -> date:
     """
-    try:
-        datetime.strptime(x, "%H:%M:%S")
-    except ValueError:
-        try:
-            datetime.strptime(x, "%H:%M")
-        except ValueError:
-            raise ValueError(
-                f"Invalid ISO time string: '{x}'."
-                " The string must be in the format 'HH:MM:SS' or 'HH:MM'."
-            )
-
-    return
-
-
-def _normalize_iso_time_str(x: str) -> str:
-    """
-    Normalize the input ISO time string by expanding it to include the seconds component if necessary.
+    Converts a string in ISO format to a date object.
 
     Args:
-        x (str): The input ISO time string.
+        x (str): The string to be converted.
 
     Returns:
-        str: The normalized ISO time string.
+        date: The converted date object.
     """
-    if len(x) == 5:
-        x = x + ":00"
-
-    return x
+    return datetime.fromisoformat(x).date()
 
 
 def _validate_date_obj(x: Any) -> None:
     """
     Validate if the given object is a valid date object.
 
     Args:
@@ -3257,16 +3110,14 @@
 
     Returns:
         None
     """
     if not isinstance(x, date):
         raise ValueError(f"Invalid date object: '{x}'. The object must be a date object.")
 
-    return
-
 
 def _validate_time_obj(x: Any) -> None:
     """
     Validate if the given object is a valid time object.
 
     Args:
         x (Any): The object to be validated.
@@ -3276,16 +3127,14 @@
 
     Returns:
         None
     """
     if not isinstance(x, time):
         raise ValueError(f"Invalid time object: '{x}'. The object must be a time object.")
 
-    return
-
 
 def _validate_datetime_obj(x: Any) -> None:
     """
     Validate if the given object is a valid datetime object.
 
     Args:
         x (Any): The object to be validated.
@@ -3295,21 +3144,19 @@
 
     Returns:
         None
     """
     if not isinstance(x, datetime):
         raise ValueError(f"Invalid datetime object: '{x}'. The object must be a datetime object.")
 
-    return
-
 
 def fmt_image(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     height: str | int | None = None,
     width: str | int | None = None,
     sep: str = " ",
     path: str | Path | None = None,
     file_pattern: str = "{}",
     encode: bool = True,
 ) -> GTSelf:
@@ -3429,15 +3276,15 @@
         else:
             files = [val]
 
         # TODO: if we allowing height and width to be set based on column values, then
         # they could end up as bespoke types like np int64, etc..
         # We should ensure we process those before hitting FmtImage
         if isinstance(self.height, (int, float)):
-            height = f"{self.height}px"
+            height = px(self.height)
         else:
             height = self.height
 
         # TODO: note that only height can be numeric in the R program. Is this on purpose?
         # In any event, raising explicitly for numeric width below.
         if isinstance(self.width, (int, float)):
             raise NotImplementedError("The width argument must be specified as a string.")
@@ -3478,15 +3325,14 @@
 
         with open(filename, "rb") as f:
             encoded = base64.b64encode(f.read()).decode()
 
         mime_type = cls._get_mime_type(filename)
 
         return f"data: {mime_type}; base64,{encoded}"
-        ...
 
     @staticmethod
     def _get_mime_type(filename: str) -> str:
         from pathlib import Path
 
         # note that we strip off the leading "."
         suffix = Path(filename).suffix[1:]
@@ -3510,24 +3356,24 @@
 
         return f'<img src="{uri}" style="{style_string}">'
 
 
 def fmt_nanoplot(
     self: GTSelf,
     columns: str | None = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     plot_type: PlotType = "line",
     plot_height: str = "2em",
     missing_vals: MissingVals = "marker",
     autoscale: bool = False,
-    reference_line: Optional[Union[str, int, float]] = None,
-    reference_area: Optional[List[Any]] = None,
-    expand_x: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
-    expand_y: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
-    options: Optional[Dict[str, Any]] = None,
+    reference_line: str | int | float | None = None,
+    reference_area: list[Any] | None = None,
+    expand_x: list[int] | list[float] | list[int | float] | None = None,
+    expand_y: list[int] | list[float] | list[int | float] | None = None,
+    options: dict[str, Any] | None = None,
 ) -> GTSelf:
     """Format data for nanoplot visualizations.
 
     The `fmt_nanoplot()` method is used to format data for nanoplot visualizations. This method
     allows for the creation of a variety of different plot types, including line, bar, and scatter
     plots.
 
@@ -3772,34 +3618,33 @@
     # Generate a function that will operate on single `x` values in the table body using both
     # the date and time format strings
     def fmt_nanoplot_fn(
         x: Any,
         plot_type: PlotType = plot_type,
         plot_height: str = plot_height,
         missing_vals: MissingVals = missing_vals,
-        reference_line: Optional[Union[str, int, float]] = reference_line,
-        reference_area: Optional[List[Any]] = reference_area,
-        all_single_y_vals: Optional[List[Union[int, float]]] = all_single_y_vals,
-        options_plots: Dict[str, Any] = options_plots,
+        reference_line: str | int | float | None = reference_line,
+        reference_area: list[Any] | None = reference_area,
+        all_single_y_vals: list[int | float] | None = all_single_y_vals,
+        options_plots: dict[str, Any] = options_plots,
     ) -> str:
         # If the `x` value is a Pandas 'NA', then return the same value
         # We have to pass in a dataframe to this function. Everything action that
         # requires a dataframe import should go through _tbl_data.
         if is_na(data_tbl, x):
             return x
 
         # Generate data vals from the input `x` value
         x = _generate_data_vals(data_vals=x)
 
         # TODO: where are tuples coming from? Need example / tests that induce tuples
         # If `x` is a tuple, then we have x and y values; otherwise, we only have y values
         if isinstance(x, tuple):
 
-            y_vals = x[1]
-            x_vals = x[0]
+            x_vals, y_vals = x
 
             # Ensure that both objects are lists
             if not isinstance(x_vals, list) or not isinstance(y_vals, list):
                 raise ValueError("The 'x' and 'y' values must be lists.")
 
             # Ensure that the lists contain only numeric values (ints and floats)
             if not all(isinstance(val, (int, float)) for val in x_vals):
@@ -3829,36 +3674,36 @@
 
         return nanoplot
 
     return fmt(self, fns=fmt_nanoplot_fn, columns=columns, rows=rows)
 
 
 def _generate_data_vals(
-    data_vals: Any, is_x_axis=False
-) -> Union[List[float], Tuple[List[float], List[float]]]:
+    data_vals: Any, is_x_axis: bool = False
+) -> list[float] | tuple[list[float], list[float]]:
     """
     Generate a list of data values from the input data.
 
     Args:
         data_vals (Any): The input data values.
 
     Returns:
-        List[Any]: A list of data values.
+        list[Any]: A list of data values.
     """
 
     import re
 
     if isinstance(data_vals, list):
 
         # If the list contains string values, determine whether they are date values
         if all(isinstance(val, str) for val in data_vals):
             if not is_x_axis:
                 raise ValueError("Only the x-axis of a nanoplot allows strings.")
             if re.search(r"\d{1,4}-\d{2}-\d{2}", data_vals[0]):
-                data_vals = [_iso_to_date(val) for val in data_vals]
+                data_vals = [_iso_str_to_date(val) for val in data_vals]
 
                 # Transform the date values to numeric values
                 data_vals = [val.toordinal() for val in data_vals]
 
         # If the cell value is a list of floats/ints, then return the same value
 
         # Check that the values within the list are numeric; missing values are allowed
@@ -3921,23 +3766,23 @@
     else:
         # Raise not implemented
         raise NotImplementedError("The input data values must be a string.")
 
     return data_vals
 
 
-def _process_number_stream(data_vals: str) -> List[float]:
+def _process_number_stream(data_vals: str) -> list[float]:
     """
     Process a string of numeric values and convert to a list of floats.
 
     Args:
         data_vals (str): The string of numeric values.
 
     Returns:
-        List[float]: A list of numeric values.
+        list[float]: A list of numeric values.
     """
 
     import re
 
     number_stream = re.sub(r"[;,]", " ", data_vals)
     number_stream = re.sub(r"\\[|\\]", " ", number_stream)
     number_stream = re.sub(r"^\\s+|\\s+$", "", number_stream)
@@ -3945,26 +3790,25 @@
     number_stream = [re.sub(r"[\\(\\)a-dA-Df-zF-Z]", "", val) for val in number_stream]
     number_stream = [float(val) for val in number_stream]
 
     return number_stream
 
 
 import re
-from typing import List
 
 
-def _process_time_stream(data_vals: str) -> List[float]:
+def _process_time_stream(data_vals: str) -> list[float]:
     """
     Process a string of time values and convert to a list of floats.
 
     Args:
         data_vals (str): The string of time values.
 
     Returns:
-        List[float]: A list of time values.
+        list[float]: A list of time values.
     """
 
     time_stream = re.split(r"\s*[;,]\s*", data_vals)
     time_stream = [val.replace("T", " ") for val in time_stream]
     time_stream_vals = [float(val) for val in time_stream]
 
     return time_stream_vals
```

### Comparing `great-tables-0.5.0/great_tables/_formats_vals.py` & `great_tables-0.5.1/great_tables/_formats_vals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from __future__ import annotations
-from ._gt_data import GTData
-from ._tbl_data import to_frame, SeriesLike
-from great_tables.gt import _get_column_of_values, GT
+
+from typing import TYPE_CHECKING, Any
+
 from great_tables import GT
-from typing import List, Any, Union, Optional, TYPE_CHECKING
+from great_tables.gt import GT, _get_column_of_values
+from typing_extensions import TypeAlias
+
+from ._gt_data import GTData
+from ._tbl_data import SeriesLike, to_frame
 
 if TYPE_CHECKING:
     from ._formats import DateStyle, TimeStyle
     from ._tbl_data import SeriesLike
 
 
-def _make_one_col_table(vals: Union[Any, List[Any], SeriesLike]) -> GT:
+X: TypeAlias = "Any | list[Any] | SeriesLike"
+
+
+def _make_one_col_table(vals: X) -> GT:
     """
     Create a one-column table from a list of values.
 
-    Args:
-        val_list (Union[Any, List[Any]]): The list of values to be converted into a table.
+    Parameters
+    ----------
+    x
+        The list of values to be converted into a table.
 
-    Returns:
-        GTData: The GTData object representing the one-column table.
+    Returns
+    -------
+        GT: The GT object representing the one-column table.
     """
 
     # Upgrade a single value to a list
     if not isinstance(vals, (tuple, list, SeriesLike)):
         vals = [vals]
     elif isinstance(vals, tuple):
         # anticipating a tuple may be too defensive
@@ -34,28 +44,28 @@
 
     # Convert the list to a Pandas DataFrame and then to a GTData object
     gt_obj = GT(df, auto_align=False)
     return gt_obj
 
 
 def val_fmt_number(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     scale_by: float = 1,
     compact: bool = False,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format numeric values.
 
     With numeric values in a list, we can perform number-based formatting so that the values are
     rendered with some level of precision. The following major options are available:
 
     - decimals: choice of the number of decimal places, option to drop trailing zeros, and a choice
@@ -124,15 +134,15 @@
         notation with `accounting = True`.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_number(
         columns="x",
@@ -152,23 +162,23 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_integer(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     use_seps: bool = True,
     scale_by: float = 1,
     compact: bool = False,
     pattern: str = "{x}",
     sep_mark: str = ",",
     force_sign: bool = False,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as integers.
 
     With numeric values in a list, we can perform number-based formatting so that the input values
     are always rendered as integer values. The following major options are available:
 
     We can have fine control over integer formatting with the following options:
@@ -213,15 +223,15 @@
         notation with `accounting = True`.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_integer(
         columns="x",
@@ -236,28 +246,28 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_scientific(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     decimals: int = 2,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     scale_by: float = 1,
     exp_style: str = "x10n",
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign_m: bool = False,
     force_sign_n: bool = False,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values to scientific notation.
 
     With numeric values in a list, we can perform formatting so that the input values are rendered
     in scientific notation, where extremely large or very small numbers can be expressed in a more
     practical fashion. Here, numbers are written in the form of a mantissa (`m`) and an exponent
     (`n`) with the construction *m* x 10^*n* or *m*E*n*. The mantissa component is a number between
@@ -330,15 +340,15 @@
         numbers will display a sign.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_scientific(
         columns="x",
@@ -358,28 +368,28 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_percent(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     decimals: int = 2,
     drop_trailing_zeros: bool = False,
     drop_trailing_dec_mark: bool = True,
     scale_values: bool = True,
     use_seps: bool = True,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     placement: str = "right",
     incl_space: bool = False,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as a percentage.
 
     With numeric values in a list, we can perform percentage-based formatting. It is assumed the
     input numeric values are proportional values and, in this case, the values will be automatically
     multiplied by `100` before decorating with a percent sign (the other case is accommodated though
     setting `scale_values` to `False`). For more control over percentage formatting, we can use the
@@ -447,15 +457,15 @@
         is to not introduce a space character.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_percent(
         columns="x",
@@ -475,29 +485,29 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_currency(
-    x: Union[Any, List[Any], SeriesLike],
-    currency: Optional[str] = None,
+    x: X,
+    currency: str | None = None,
     use_subunits: bool = True,
-    decimals: Optional[int] = None,
+    decimals: int | None = None,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     scale_by: float = 1,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     placement: str = "left",
     incl_space: bool = False,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as currencies.
 
     With numeric values, we can perform currency-based formatting with the `val_fmt_currency()`
     function. This supports both automatic formatting with a three-letter currency code. We have
     fine control over the conversion from numeric values to currency values, where we could take
     advantage of the following options:
@@ -568,15 +578,15 @@
         default is to not introduce a space character.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_currency(
         columns="x",
@@ -597,18 +607,18 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_roman(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     case: str = "upper",
     pattern: str = "{x}",
-) -> List[str]:
+) -> list[str]:
     """
     Format values as Roman numerals.
 
     With numeric values we can transform those to Roman numerals, rounding values as necessary.
 
     Parameters
     ----------
@@ -620,15 +630,15 @@
     pattern
         A formatting pattern that allows for decoration of the formatted value. The formatted value
         is represented by the `{x}` (which can be used multiple times, if needed) and all other
         characters will be interpreted as string literals.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_roman(
         columns="x",
@@ -638,28 +648,28 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_bytes(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     standard: str = "decimal",
     decimals: int = 1,
-    n_sigfig: Optional[int] = None,
+    n_sigfig: int | None = None,
     drop_trailing_zeros: bool = True,
     drop_trailing_dec_mark: bool = True,
     use_seps: bool = True,
     pattern: str = "{x}",
     sep_mark: str = ",",
     dec_mark: str = ".",
     force_sign: bool = False,
     incl_space: bool = True,
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as bytes.
 
     With numeric values in a list, we can transform those to values of bytes with human readable
     units. The `val_fmt_bytes()` function allows for the formatting of byte sizes to either of two
     common representations: (1) with decimal units (powers of 1000, examples being `"kB"` and
     `"MB"`), and (2) with binary units (powers of 1024, examples being `"KiB"` and `"MiB"`). It is
@@ -723,15 +733,15 @@
         default is to not introduce a space character.
     locale
         An optional locale identifier that can be used for formatting values according the locale's
         rules. Examples include `"en"` for English (United States) and `"fr"` for French (France).
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_bytes(
         columns="x",
@@ -751,19 +761,19 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_date(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     date_style: DateStyle = "iso",
     pattern: str = "{x}",
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as dates.
 
     Format input values to time values using one of 17 preset date styles. Input can be in the form
     of `date` type or as a ISO-8601 string (in the form of `YYYY-MM-DD HH:MM:SS` or `YYYY-MM-DD`).
 
     Parameters
@@ -810,15 +820,15 @@
     | 17 | `"year_quarter"`      | `"2000-Q1"`             |
 
     We can use the `info_date_style()` function within the console to view a similar table of date
     styles with example output.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_date(
         columns="x",
@@ -829,19 +839,19 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_time(
-    x: Union[Any, List[Any], SeriesLike],
+    x: X,
     time_style: TimeStyle = "iso",
     pattern: str = "{x}",
-    locale: Union[str, None] = None,
-) -> List[str]:
+    locale: str | None = None,
+) -> list[str]:
     """
     Format values as times.
 
     Format input values to time values using one of 5 preset time styles. Input can be in the form
     of `time` values, or strings in the ISO 8601 forms of `HH:MM:SS` or `YYYY-MM-DD HH:MM:SS`.
 
     Parameters
@@ -876,15 +886,15 @@
     | 5  | `"h_p"`       | `"2 PM"`                        | 12h           |
 
     We can use the `info_time_style()` function within the console to view a similar table of time
     styles with example output.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_time(
         columns="x",
@@ -895,29 +905,29 @@
 
     vals_fmt = _get_column_of_values(gt=gt_obj_fmt, column_name="x", context="html")
 
     return vals_fmt
 
 
 def val_fmt_markdown(
-    x: Union[Any, List[Any], SeriesLike],
-) -> List[str]:
+    x: X,
+) -> list[str]:
     """
     Format Markdown text.
 
     Any Markdown-formatted text can be transformed to HTML when using the `fmt_markdown()` function.
 
     Parameters
     ----------
     x
         A list of values to be formatted.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of formatted values is returned.
     """
 
     gt_obj: GTData = _make_one_col_table(vals=x)
 
     gt_obj_fmt = gt_obj.fmt_markdown(
         columns="x",
```

### Comparing `great-tables-0.5.0/great_tables/_gt_data.py` & `great_tables-0.5.1/great_tables/_gt_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 from __future__ import annotations
 
 import copy
 import re
+from collections.abc import Sequence
+from dataclasses import dataclass, field, replace
+from enum import Enum, auto
+from typing import Any, Callable, TypeVar, overload
 
-from typing import overload, TypeVar, Dict, Optional
 from typing_extensions import Self, TypeAlias
-from dataclasses import dataclass, field, replace
-from ._utils import _str_detect
-from ._tbl_data import create_empty_frame, to_list, validate_frame, copy_data
 
 # TODO: move this class somewhere else (even gt_data could work)
-
 from ._styles import CellStyle
-
-# Note that we replace with with collections.abc after python 3.8
-from typing import Sequence
+from ._tbl_data import (
+    DataFrameLike,
+    TblData,
+    _get_cell,
+    _set_cell,
+    copy_data,
+    create_empty_frame,
+    get_column_names,
+    n_rows,
+    to_list,
+    validate_frame,
+)
+from ._utils import _str_detect
 
 T = TypeVar("T")
 
 
 # GT Data ----
-from dataclasses import dataclass
-
 __GT = None
 
 
 @dataclass(frozen=True)
 class GTData:
     _tbl_data: TblData
     _body: Body
@@ -132,29 +139,26 @@
     def __eq__(self, other: Any) -> bool:
         return (type(self) is type(other)) and (self._d == other._d)
 
 
 # Body ----
 __Body = None
 
-from typing import Union, List, Any
-from ._tbl_data import DataFrameLike, TblData, _get_cell, _set_cell
-
 
 # TODO: it seems like this could just be a DataFrameLike object?
 # Similar to TblData now being a DataFrame, rather than its own class
 # I've left for now, and have just implemented concretes for it in
 # _tbl_data.py
 class Body:
     body: TblData
 
     def __init__(self, body: TblData):
         self.body = body
 
-    def render_formats(self, data_tbl: TblData, formats: List[FormatInfo], context: Any):
+    def render_formats(self, data_tbl: TblData, formats: list[FormatInfo], context: Any):
         for fmt in formats:
             eval_func = getattr(fmt.func, context, fmt.func.default)
             if eval_func is None:
                 raise Exception("Internal Error")
             for col, row in fmt.cells.resolve():
                 result = eval_func(_get_cell(data_tbl, row, col))
                 if isinstance(result, FormatterSkipElement):
@@ -176,19 +180,14 @@
 
         return cls(empty_df)
 
 
 # Boxhead ----
 __Boxhead = None
 
-from typing import Optional, List
-from enum import Enum, auto
-
-from ._tbl_data import TblData, get_column_names
-
 
 class ColumnAlignment(Enum):
     left = auto()
     center = auto()
     right = auto()
     justify = auto()
 
@@ -201,17 +200,17 @@
 
 
 @dataclass(frozen=True)
 class ColInfo:
     # TODO: Make var readonly
     var: str
     type: ColInfoTypeEnum = ColInfoTypeEnum.default
-    column_label: Optional[str] = None
-    column_align: Optional[ColumnAlignment] = None
-    column_width: Optional[str] = None
+    column_label: str | None = None
+    column_align: ColumnAlignment | None = None
+    column_width: str | None = None
 
     # The components of the boxhead are:
     # `var` (obtained from column names)
     # `column_label` (obtained from column names)
     # `column_align` = None
     # `column_width` = None
 
@@ -229,22 +228,22 @@
 
     @property
     def defaulted_align(self) -> str:
         return "center" if self.column_align is None else str(self.column_align)
 
 
 class Boxhead(_Sequence[ColInfo]):
-    _d: List[ColInfo]
+    _d: list[ColInfo]
 
     def __init__(
         self,
         data: TblData | list[ColInfo],
         auto_align: bool = True,
-        rowname_col: Optional[str] = None,
-        groupname_col: Optional[str] = None,
+        rowname_col: str | None = None,
+        groupname_col: str | None = None,
     ):
         if isinstance(data, list):
             self._d = data
         else:
             # Obtain the column names from the data and initialize the
             # `_boxhead` from that
             column_names = get_column_names(data)
@@ -277,15 +276,15 @@
             elif col.type == ColInfoTypeEnum.row_group:
                 new_col = replace(col, type=ColInfoTypeEnum.default)
                 self._d[ii] = new_col
 
     def set_cols_hidden(self, colnames: list[str]):
         # TODO: validate that colname is in the boxhead
         res: list[ColInfo] = []
-        for ii, col in enumerate(self._d):
+        for col in self._d:
             if col.var in colnames:
                 new_col = replace(col, type=ColInfoTypeEnum.hidden)
                 res.append(new_col)
             else:
                 res.append(col)
 
         return self.__class__(res)
@@ -327,15 +326,15 @@
                 # dtype to 'character-numeric'
                 if all(number_like_matches):
                     dtype = "character-numeric"
 
             col_classes.append(dtype)
 
         # Get a list of `align` values by translating the column classes
-        align: List[str] = []
+        align: list[str] = []
 
         for col_class in col_classes:
             # Ensure that `col_class` is lowercase
             col_class = str(col_class).lower()
 
             # Translate the column classes to an alignment value of 'left', 'right', or 'center'
             if col_class == "character-numeric":
@@ -356,87 +355,87 @@
                 align.append("center")
             elif col_class == "list":
                 align.append("center")
             else:
                 align.append("center")
 
         # Set the alignment for each column in the boxhead
-        new_cols: List[ColInfo] = []
+        new_cols: list[ColInfo] = []
         for col, alignment in zip(self._d, align):
             new_cols.append(replace(col, column_align=alignment))
 
         self._d = new_cols
 
-    def vars_from_type(self, type: ColInfoTypeEnum) -> List[str]:
+    def vars_from_type(self, type: ColInfoTypeEnum) -> list[str]:
         return [x.var for x in self._d if x.type == type]
 
-    def reorder(self, vars: List[str]) -> Self:
+    def reorder(self, vars: list[str]) -> Self:
         boxh_vars = [col.var for col in self]
         if set(vars) != set(boxh_vars):
             raise ValueError("Reordering vars must contain all boxhead vars.")
 
         new_order = [boxh_vars.index(var) for var in vars]
 
         return self[new_order]
 
     # Get a list of columns
-    def _get_columns(self) -> List[str]:
+    def _get_columns(self) -> list[str]:
         return [x.var for x in self._d]
 
     # Get a list of column labels
-    def _get_column_labels(self) -> List[str | None]:
+    def _get_column_labels(self) -> list[str | None]:
         return [x.column_label for x in self._d]
 
     # Set column label
-    def _set_column_labels(self, col_labels: Dict[str, str]) -> Self:
-        out_cols: List[ColInfo] = []
+    def _set_column_labels(self, col_labels: dict[str, str]) -> Self:
+        out_cols: list[ColInfo] = []
         for x in self._d:
             new_label = col_labels.get(x.var, None)
             if new_label is not None:
                 out_cols.append(replace(x, column_label=new_label))
             else:
                 out_cols.append(x)
 
         return self.__class__(out_cols)
 
     # Set column alignments
-    def _set_column_aligns(self, columns: List[str], align: str) -> Self:
+    def _set_column_aligns(self, columns: list[str], align: str) -> Self:
         set_cols = set(columns)
-        out_cols: List[ColInfo] = []
+        out_cols: list[ColInfo] = []
         for x in self._d:
             if x.var in set_cols:
                 out_cols.append(replace(x, column_align=align))
             else:
                 out_cols.append(x)
 
         return self.__class__(out_cols)
 
     # Get a list of column widths
-    def _get_column_widths(self) -> List[str | None]:
+    def _get_column_widths(self) -> list[str | None]:
         return [x.column_width for x in self._d]
 
     # Get a list of visible columns
-    def _get_default_columns(self) -> List[ColInfo]:
+    def _get_default_columns(self) -> list[ColInfo]:
         default_columns = [x for x in self._d if x.type == ColInfoTypeEnum.default]
         return default_columns
 
-    def _get_stub_column(self) -> Optional[ColInfo]:
+    def _get_stub_column(self) -> ColInfo | None:
         stub_column = [x for x in self._d if x.type == ColInfoTypeEnum.stub]
         if len(stub_column) == 0:
             return None
         return stub_column[0]
 
     # Get a list of visible column labels
-    def _get_default_column_labels(self) -> List[str | None]:
+    def _get_default_column_labels(self) -> list[str | None]:
         default_column_labels = [
             x.column_label for x in self._d if x.type == ColInfoTypeEnum.default
         ]
         return default_column_labels
 
-    def _get_default_alignments(self) -> List[str]:
+    def _get_default_alignments(self) -> list[str]:
         # Extract alignment strings to only include 'default'-type columns
         alignments = [str(x.column_align) for x in self._d if x.type == ColInfoTypeEnum.default]
         return alignments
 
     # Get the alignment for a specific var value
     def _get_boxhead_get_alignment_by_var(self, var: str) -> str:
         # Get the column alignments and also the alignment class names
@@ -474,15 +473,15 @@
         # for the width of the stub at build time to fully obtain the number
         # of visible columns in the built table
         n_data_cols = n_data_cols + len(stub_layout)
 
         return n_data_cols
 
     def _set_column_width(self, colname: str, width: str) -> Self:
-        out_cols: List[ColInfo] = []
+        out_cols: list[ColInfo] = []
 
         colnames = [x.var for x in self._d]
 
         if colname not in colnames:
             raise ValueError(f"Column name {colname} not found in table.")
 
         for x in self._d:
@@ -493,24 +492,22 @@
 
         return self.__class__(out_cols)
 
 
 # Stub ----
 __Stub = None
 
-from ._tbl_data import TblData, n_rows
-
 
 @dataclass(frozen=True)
 class RowInfo:
     # TODO: Make `rownum_i` readonly
     rownum_i: int
-    group_id: Optional[str] = None
-    rowname: Optional[str] = None
-    group_label: Optional[str] = None
+    group_id: str | None = None
+    rowname: str | None = None
+    group_label: str | None = None
     built: bool = False
 
     # The components of the stub are:
     # `rownum_i` (The initial row indices for the table at ingest time)
     # `group_id` = None
     # `rowname` = None
     # `group_label` = None
@@ -570,25 +567,23 @@
         # If there aren't any row groups then the result is always False
         if len(row_groups) < 1:
             return False
 
         # Given that there are row groups, we need to look at the option `row_group_as_column` to
         # determine whether they populate a column located in the stub; if set as True then that's
         # the return value
-        row_group_as_column = options.row_group_as_column.value
-
-        row_group_as_column: Any
+        row_group_as_column: Any = options.row_group_as_column.value
         if not isinstance(row_group_as_column, bool):
             raise TypeError(
                 "Variable type mismatch. Expected bool, got something entirely different."
             )
 
         return row_group_as_column
 
-    def _get_stub_layout(self, row_groups: RowGroups, options: Options) -> List[str]:
+    def _get_stub_layout(self, row_groups: RowGroups, options: Options) -> list[str]:
         # Determine which stub components are potentially present as columns
         stub_rownames_is_column = "row_id" in self._get_stub_components()
         stub_groupnames_is_column = self._stub_group_names_has_column(
             row_groups=row_groups, options=options
         )
 
         # Get the potential total number of columns in the table stub
@@ -617,25 +612,25 @@
 
         return stub_layout
 
 
 # Row groups ----
 __RowGroups = None
 
-RowGroups: TypeAlias = List[str]
+RowGroups: TypeAlias = list[str]
 
 # Group rows ----
 __GroupRows = None
 
 
 @dataclass(frozen=True)
 class GroupRowInfo:
     group_id: str
     group_label: str | None = None
-    indices: list[int] = field(default_factory=lambda: [])
+    indices: list[int] = field(default_factory=list)
     # row_start: int | None = None
     # row_end: int | None = None
     has_summary_rows: bool = False
     summary_row_side: str | None = None
 
     def defaulted_label(self) -> str:
         """Return a group label that has been defaulted."""
@@ -646,15 +641,15 @@
 class MISSING_GROUP:
     """Represent a category of all missing group levels in data."""
 
 
 class GroupRows(_Sequence[GroupRowInfo]):
     _d: list[GroupRowInfo]
 
-    def __init__(self, data: list[GroupRowInfo] | DataFrameLike, group_key: Optional[str] = None):
+    def __init__(self, data: list[GroupRowInfo] | DataFrameLike, group_key: str | None = None):
         if isinstance(data, list):
             self._d = data
 
         elif group_key is None:
             self._d = []
 
         # otherwise, instantiate from a table of data
@@ -700,16 +695,16 @@
 @dataclass(frozen=True)
 class SpannerInfo:
     spanner_id: str
     spanner_level: int
     spanner_label: str | None = None
     spanner_units: str | None = None
     spanner_pattern: str | None = None
-    vars: list[str] = field(default_factory=lambda: [])
-    built: Optional[str] = None
+    vars: list[str] = field(default_factory=list)
+    built: str | None = None
 
     def built_label(self) -> str:
         """Return a list of spanner labels that have been built."""
         label = self.built if self.built is not None else self.spanner_label
         if label is None:
             raise ValueError("Spanner label must be a string and not None.")
         return label
@@ -752,139 +747,119 @@
     def append_entry(self, span: SpannerInfo) -> Self:
         return self.__class__(self._d + [span])
 
 
 # Heading ---
 __Heading = None
 
-from typing import Optional, Union, List
-
 
 @dataclass(frozen=True)
 class Heading:
-    title: Optional[str] = None
-    subtitle: Optional[str] = None
-    preheader: Optional[Union[str, List[str]]] = None
+    title: str | None = None
+    subtitle: str | None = None
+    preheader: str | list[str] | None = None
 
 
 # Stubhead ----
 __Stubhead = None
 
-from typing import Optional
-
-Stubhead: TypeAlias = Optional[str]
+Stubhead: TypeAlias = "str | None"
 
 
 # Sourcenotes ----
 __Sourcenotes = None
 
-from typing import List
-
-
-SourceNotes = List[str]
+SourceNotes = list[str]
 
 # Footnotes ----
 __Footnotes = None
 
-from typing import Optional, List
-from enum import Enum, auto
-
 
 class FootnotePlacement(Enum):
     left = auto()
     right = auto()
     auto = auto()
 
 
 @dataclass(frozen=True)
 class FootnoteInfo:
-    locname: Optional[str] = None
-    grpname: Optional[str] = None
-    colname: Optional[str] = None
-    locnum: Optional[int] = None
-    rownum: Optional[int] = None
-    colnum: Optional[int] = None
-    footnotes: Optional[List[str]] = None
-    placement: Optional[FootnotePlacement] = None
+    locname: str | None = None
+    grpname: str | None = None
+    colname: str | None = None
+    locnum: int | None = None
+    rownum: int | None = None
+    colnum: int | None = None
+    footnotes: list[str] | None = None
+    placement: FootnotePlacement | None = None
 
 
-Footnotes: TypeAlias = List[FootnoteInfo]
+Footnotes: TypeAlias = list[FootnoteInfo]
 
 # Styles ----
 __Styles = None
 
-from typing import List, Optional
-
 
 @dataclass(frozen=True)
 class StyleInfo:
     locname: str
     locnum: int
-    grpname: Optional[str] = None
-    colname: Optional[str] = None
-    rownum: Optional[int] = None
-    colnum: Optional[int] = None
-    styles: List[CellStyle] = field(default_factory=list)
+    grpname: str | None = None
+    colname: str | None = None
+    rownum: int | None = None
+    colnum: int | None = None
+    styles: list[CellStyle] = field(default_factory=list)
 
 
-Styles: TypeAlias = List[StyleInfo]
+Styles: TypeAlias = list[StyleInfo]
 
 # Locale ----
 __Locale = None
 
-from typing import Optional
-
 
 class Locale:
-    locale: Optional[str]
+    locale: str | None
 
-    def __init__(self, locale: Optional[str]):
-        self._locale: Union[str, None] = locale
+    def __init__(self, locale: str | None):
+        self._locale: str | None = locale
 
 
 # Formats ----
 __Formats = None
 
-from typing import Any, Callable, TypeVar, Union, List, Optional, Tuple
-
-from ._tbl_data import n_rows
-
 
 class FormatterSkipElement:
     """Represent that nothing should be saved for a formatted value."""
 
 
 FormatFn = Callable[[Any], "str | FormatterSkipElement"]
 
 
 class FormatFns:
-    html: Optional[FormatFn]
-    latex: Optional[FormatFn]
-    rtf: Optional[FormatFn]
-    default: Optional[FormatFn]
+    html: FormatFn | None
+    latex: FormatFn | None
+    rtf: FormatFn | None
+    default: FormatFn | None
 
     def __init__(self, **kwargs: FormatFn):
         for format in ["html", "latex", "rtf", "default"]:
-            if kwargs.get(format):
-                setattr(self, format, kwargs[format])
+            if fmt := kwargs.get(format):
+                setattr(self, format, fmt)
 
 
 class CellSubset:
-    def __init__(self):
-        pass
 
-    def resolve(self) -> List[Tuple[str, int]]:
+    def resolve(self) -> list[tuple[str, int]]:
         raise NotImplementedError("Not implemented")
 
 
 class CellRectangle(CellSubset):
-    cols: List[str]
-    rows: List[int]
+    cols: list[str]
+    rows: list[int]
 
-    def __init__(self, cols: List[str], rows: List[int]):
+    def __init__(self, cols: list[str], rows: list[int]):
         self.cols = cols
         self.rows = rows
 
     def resolve(self):
         return list((col, row) for col in self.cols for row in self.rows)
 
 
@@ -893,33 +868,29 @@
 
     Note that format functions apply to individual values.
     """
 
     func: FormatFns
     cells: CellSubset
 
-    def __init__(self, func: FormatFns, cols: List[str], rows: List[int]):
+    def __init__(self, func: FormatFns, cols: list[str], rows: list[int]):
         self.func = func
         self.cells = CellRectangle(cols, rows)
 
 
 # TODO: this will contain private methods for formatting cell values to strings
 # class Formats:
 #     def __init__(self):
 #         pass
 Formats = list
 
-# Tbl Data ----
-from ._tbl_data import TblData
-
 
 # Options ----
 __Options = None
 
-from typing import Optional, Union, List, Any
 
 default_fonts_list = [
     "-apple-system",
     "BlinkMacSystemFont",
     "Segoe UI",
     "Roboto",
     "Oxygen",
@@ -934,15 +905,15 @@
 
 
 @dataclass(frozen=True)
 class OptionsInfo:
     scss: bool
     category: str
     type: str
-    value: Optional[Union[Any, List[str]]]
+    value: Any
 
 
 @dataclass(frozen=True)
 class Options:
     table_id: OptionsInfo = OptionsInfo(False, "table", "value", None)
     table_caption: OptionsInfo = OptionsInfo(False, "table", "value", None)
     table_width: OptionsInfo = OptionsInfo(True, "table", "px", "auto")
@@ -1146,16 +1117,16 @@
     # page_margin_top: OptionsInfo = OptionsInfo(False, "page", "value", "1.0in")
     # page_margin_bottom: OptionsInfo = OptionsInfo(False, "page", "value", "1.0in")
     # page_header_height: OptionsInfo = OptionsInfo(False, "page", "value", "0.5in")
     # page_footer_height: OptionsInfo = OptionsInfo(False, "page", "value", "0.5in")
     quarto_disable_processing: OptionsInfo = OptionsInfo(False, "quarto", "logical", False)
     quarto_use_bootstrap: OptionsInfo = OptionsInfo(False, "quarto", "logical", False)
 
-    def _get_all_options_keys(self) -> List[Union[str, None]]:
+    def _get_all_options_keys(self) -> list[str | None]:
         return [x.parameter for x in self._options.values()]
 
-    # def _get_option_type(self, option: str) -> Union[Any, List[str]]:
+    # def _get_option_type(self, option: str) -> Any | list[str]:
     #    return self._options[option].type
 
     def _set_option_value(self, option: str, value: Any):
         self._options[option].value = value
         return self
```

### Comparing `great-tables-0.5.0/great_tables/_heading.py` & `great_tables-0.5.1/great_tables/_heading.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Union, List
+
+from typing import TYPE_CHECKING
+
 from ._gt_data import Heading
 from ._text import Text
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
 def tab_header(
     self: GTSelf,
-    title: Union[str, Text],
-    subtitle: Optional[Union[str, Text]] = None,
-    preheader: Optional[Union[str, List[str]]] = None,
+    title: str | Text,
+    subtitle: str | Text | None = None,
+    preheader: str | list[str] | None = None,
 ) -> GTSelf:
     """
     Add a table header.
 
     We can add a table header to the output table that contains a title and even a subtitle with the
     `tab_header()` method. A table header is an optional table component that is positioned above
     the column labels. We have the flexibility to use Markdown or HTML formatting for the header's
```

### Comparing `great-tables-0.5.0/great_tables/_helpers.py` & `great_tables-0.5.1/great_tables/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
-from typing import Union, List, Dict, Literal, Any, Optional, Callable
+from __future__ import annotations
+
 import random
+import string
+from typing import Any, Callable, Literal
+
 from typing_extensions import TypeAlias
+
 from ._text import Text
 
 
 FontStackName: TypeAlias = Literal[
     "system-ui",
     "transitional",
     "old-style",
@@ -19,15 +24,15 @@
     "slab-serif",
     "antique",
     "didone",
     "handwritten",
 ]
 
 
-def px(x: Union[int, float]) -> str:
+def px(x: int | float) -> str:
     """
     Helper for providing a CSS length value in pixels.
 
     For certain parameters, a length value is required. Examples include the setting of font sizes
     (e.g., in `cell_text()`) and thicknesses of lines (e.g., in `cell_borders()`). Setting a length
     in pixels with `px()` allows for an absolute definition of size as opposed to the analogous
     helper function `pct()`.
@@ -44,15 +49,15 @@
         >>> x = gt.px(12)
         >>> x
         >>> print(x)
     """
     return f"{x}px"
 
 
-def pct(x: Union[int, float]) -> str:
+def pct(x: int | float) -> str:
     """
     Helper for providing a CSS length value as a percentage.
 
     A percentage value acts as a length value that is relative to an initial state. For instance an
     80% value for something will size the target to 80% the size of its 'previous' value. This type
     of sizing is useful for sizing up or down a length value with an intuitive measure. This helper
     function can be used for the setting of font sizes (e.g., in `cell_text()`) and altering the
@@ -128,91 +133,33 @@
     -------
     str
         A string that constitutes a random ID value.
     """
     return "".join(random.choices(letters(), k=n))
 
 
-def letters() -> List[str]:
+def letters() -> list[str]:
     """Lowercase letters of the Roman alphabet
 
     Returns:
-        List[str]: the 26 lowercase letters of the Roman alphabet
+        list[str]: the 26 lowercase letters of the Roman alphabet
     """
-    lett = [
-        "a",
-        "b",
-        "c",
-        "d",
-        "e",
-        "f",
-        "g",
-        "h",
-        "i",
-        "j",
-        "k",
-        "l",
-        "m",
-        "n",
-        "o",
-        "p",
-        "q",
-        "r",
-        "s",
-        "t",
-        "u",
-        "v",
-        "w",
-        "x",
-        "y",
-        "z",
-    ]
+    return list(string.ascii_lowercase)
 
-    return lett
 
-
-def LETTERS() -> List[str]:
+def LETTERS() -> list[str]:
     """Uppercase letters of the Roman alphabet
 
     Returns:
-        List[str]: the 26 uppercase letters of the Roman alphabet
+        list[str]: the 26 uppercase letters of the Roman alphabet
     """
-    lett = [
-        "A",
-        "B",
-        "C",
-        "D",
-        "E",
-        "F",
-        "G",
-        "H",
-        "I",
-        "J",
-        "K",
-        "L",
-        "M",
-        "N",
-        "O",
-        "P",
-        "Q",
-        "R",
-        "S",
-        "T",
-        "U",
-        "V",
-        "W",
-        "X",
-        "Y",
-        "Z",
-    ]
-
-    return lett
+    return list(string.ascii_uppercase)
 
 
-def system_fonts(name: FontStackName = "system-ui") -> List[str]:
+def system_fonts(name: FontStackName = "system-ui") -> list[str]:
     """Get a themed font stack that works well across systems.
 
     A font stack can be obtained from `system_fonts()` using one of various keywords such as
     `"system-ui"`, `"old-style"`, and `"humanist"` (there are 15 in total) representing a themed set
     of fonts. These sets comprise a font family that has been tested to work across a wide range of
     computer systems.
 
@@ -223,15 +170,15 @@
         `"transitional"`, `"old-style"`, `"humanist"`, `"geometric-humanist"`,
         `"classical-humanist"`, `"neo-grotesque"`, `"monospace-slab-serif"`, `"monospace-code"`,
         `"industrial"`, `"rounded-sans"`, `"slab-serif"`, `"antique"`, `"didone"`, and
         `"handwritten"`.
 
     Returns
     -------
-    List[str]
+    list[str]
         A list of font names that make up the font stack.
 
     The font stacks and the individual fonts used by platform
     ---------------------------------------------------------
     ### System UI (`"system-ui"`)
 
     ```css
@@ -423,15 +370,15 @@
     Invoking the `system_fonts()` helper function with the `"industrial"` argument will return a
     list of font names that make up the font stack. This is exactly the type of input that the
     `table_font_names` parameter requires.
     """
     return _get_font_stack(name)
 
 
-def _get_font_stack(name: FontStackName = "system-ui", add_emoji=True) -> List[str]:
+def _get_font_stack(name: FontStackName = "system-ui", add_emoji: bool = True) -> list[str]:
     font_stack_names = [
         "system-ui",
         "transitional",
         "old-style",
         "humanist",
         "geometric-humanist",
         "classical-humanist",
@@ -561,15 +508,15 @@
 
 
 # This could probably be removed and nanoplot_options made into a dataclass
 # the built-in dataclass decorator doesn't do any validation / coercion, but
 # we could do that in the a __post_init__ hook. (I would switch it over to a
 # dataclass and then pair on a post_init hook).
 # Check that certain values are either a list or a single value
-def _normalize_listable_nanoplot_options(nano_opt: Any, option_type: Any):
+def _normalize_listable_nanoplot_options(nano_opt: Any, option_type: Any) -> list[Any] | None:
 
     if nano_opt is None:
         return None
 
     if not isinstance(nano_opt, (option_type, list)):
         raise ValueError(f"Nanoplot option must be a {option_type} or a list of {option_type}s")
 
@@ -582,45 +529,45 @@
     if not isinstance(nano_opt, list):
         nano_opt = [nano_opt]
 
     return nano_opt
 
 
 def nanoplot_options(
-    data_point_radius: Optional[Union[int, List[int]]] = None,
-    data_point_stroke_color: Optional[Union[str, List[str]]] = None,
-    data_point_stroke_width: Optional[Union[int, List[int]]] = None,
-    data_point_fill_color: Optional[Union[str, List[str]]] = None,
-    data_line_type: Optional[str] = None,
-    data_line_stroke_color: Optional[str] = None,
-    data_line_stroke_width: Optional[int] = None,
-    data_area_fill_color: Optional[str] = None,
-    data_bar_stroke_color: Optional[Union[str, List[str]]] = None,
-    data_bar_stroke_width: Optional[Union[int, List[int]]] = None,
-    data_bar_fill_color: Optional[Union[str, List[str]]] = None,
-    data_bar_negative_stroke_color: Optional[str] = None,
-    data_bar_negative_stroke_width: Optional[int] = None,
-    data_bar_negative_fill_color: Optional[str] = None,
-    reference_line_color: Optional[str] = None,
-    reference_area_fill_color: Optional[str] = None,
-    vertical_guide_stroke_color: Optional[str] = None,
-    vertical_guide_stroke_width: Optional[int] = None,
-    show_data_points: Optional[bool] = None,
-    show_data_line: Optional[bool] = None,
-    show_data_area: Optional[bool] = None,
-    show_reference_line: Optional[bool] = None,
-    show_reference_area: Optional[bool] = None,
-    show_vertical_guides: Optional[bool] = None,
-    show_y_axis_guide: Optional[bool] = None,
-    interactive_data_values: Optional[bool] = None,
-    y_val_fmt_fn: Optional[Callable[..., str]] = None,
-    y_axis_fmt_fn: Optional[Callable[..., str]] = None,
-    y_ref_line_fmt_fn: Optional[Callable[..., str]] = None,
-    currency: Optional[str] = None,
-) -> Dict[str, Any]:
+    data_point_radius: int | list[int] | None = None,
+    data_point_stroke_color: str | list[str] | None = None,
+    data_point_stroke_width: int | list[int] | None = None,
+    data_point_fill_color: str | list[str] | None = None,
+    data_line_type: str | None = None,
+    data_line_stroke_color: str | None = None,
+    data_line_stroke_width: int | None = None,
+    data_area_fill_color: str | None = None,
+    data_bar_stroke_color: str | list[str] | None = None,
+    data_bar_stroke_width: int | list[int] | None = None,
+    data_bar_fill_color: str | list[str] | None = None,
+    data_bar_negative_stroke_color: str | None = None,
+    data_bar_negative_stroke_width: int | None = None,
+    data_bar_negative_fill_color: str | None = None,
+    reference_line_color: str | None = None,
+    reference_area_fill_color: str | None = None,
+    vertical_guide_stroke_color: str | None = None,
+    vertical_guide_stroke_width: int | None = None,
+    show_data_points: bool | None = None,
+    show_data_line: bool | None = None,
+    show_data_area: bool | None = None,
+    show_reference_line: bool | None = None,
+    show_reference_area: bool | None = None,
+    show_vertical_guides: bool | None = None,
+    show_y_axis_guide: bool | None = None,
+    interactive_data_values: bool | None = None,
+    y_val_fmt_fn: Callable[..., str] | None = None,
+    y_axis_fmt_fn: Callable[..., str] | None = None,
+    y_ref_line_fmt_fn: Callable[..., str] | None = None,
+    currency: str | None = None,
+) -> dict[str, Any]:
     """
     Helper for setting the options for a nanoplot.
 
     When using `cols_nanoplot()`, the defaults for the generated nanoplots can be modified with
     `nanoplot_options()` within the `options=` argument.
 
     Parameters
```

### Comparing `great-tables-0.5.0/great_tables/_locale.py` & `great_tables-0.5.1/great_tables/_locale.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from csv import DictReader
-from typing import Any, Optional, TypedDict, cast
+from typing import Any, TypedDict, cast
+
 from importlib_resources import files
 
 DATA_MOD = files("great_tables") / "data"
 
 
 def read_csv(fname: str) -> list[dict[str, Any]]:
     with open(fname) as f:
         return list(DictReader(f))
 
 
 class Locale:
-    locale: Optional[str]
+    locale: str | None
 
     def __init__(self, locale: str | None = ""):
         if locale is None or locale == "":
             locale = "en"
         self._locale = locale
```

### Comparing `great-tables-0.5.0/great_tables/_locations.py` & `great_tables-0.5.1/great_tables/_locations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 import itertools
-
 from dataclasses import dataclass
 from functools import singledispatch
-from typing import TYPE_CHECKING, Literal, List, Callable, Union
+from typing import TYPE_CHECKING, Any, Callable, Literal
+
 from typing_extensions import TypeAlias
 
 # note that types like Spanners are only used in annotations for concretes of the
 # resolve generic, but we need to import at runtime, due to singledispatch looking
 # up annotations
-from ._gt_data import GTData, FootnoteInfo, Spanners, ColInfoTypeEnum, StyleInfo, FootnotePlacement
-from ._tbl_data import eval_select, eval_transform, PlExpr, PlDataFrame
+from ._gt_data import ColInfoTypeEnum, FootnoteInfo, FootnotePlacement, GTData, Spanners, StyleInfo
 from ._styles import CellStyle
-
+from ._tbl_data import PlDataFrame, PlExpr, eval_select, eval_transform
 
 if TYPE_CHECKING:
     from ._gt_data import TblData
     from ._tbl_data import SelectExpr
 
 # Misc Types ===========================================================================
 
 PlacementOptions: TypeAlias = Literal["auto", "left", "right"]
-RowSelectExpr: TypeAlias = Union[List[int], PlExpr, Callable[["TblData"], bool], None]
+RowSelectExpr: TypeAlias = 'list[int] | PlExpr | Callable[["TblData"], bool] | None'
 
 # Locations ============================================================================
 # TODO: these are called cells_* in gt. I prefixed them with Loc just to keep things
 # straight while going through helpers.R, but no strong opinion on naming!
 
 
 @dataclass
@@ -167,16 +166,15 @@
 def resolve_vector_l(expr: list[str], candidates: list[str], item_label: str) -> list[bool]:
     """Return list of logical index for candidates, selected by expr."""
 
     if not (isinstance(expr, list) and all(isinstance(x, str) for x in expr)):
         raise NotImplementedError("Selecting entries currently requires a list of strings.")
 
     set_expr = set(expr)
-    if set_expr - set(candidates):
-        missing = set_expr - set(candidates)
+    if missing := (set_expr - set(candidates)):
         raise ValueError(f"Cannot find these entries: {missing}")
 
     return [candidate in set_expr for candidate in candidates]
 
 
 def resolve_cols_c(
     data: GTData,
@@ -280,15 +278,15 @@
       * filter-like: _.cyl == 4
 
     Unlike tidyselect::eval_select, this function returns names in
     the order they appear in the data (rather than ordered by selectors).
     """
 
     if isinstance(expr, (str, int)):
-        expr: List["str | int"] = [expr]
+        expr: list[str | int] = [expr]
 
     if isinstance(data, GTData):
         if expr is None:
             if null_means == "everything":
                 return [(row.rowname, ii) for ii, row in enumerate(data._stub)]
             else:
                 return []
@@ -306,24 +304,26 @@
 
         selected = [
             (name, ii)
             for ii, name in enumerate(row_names)
             if (name in target_names or ii in target_pos)
         ]
         return selected
+
     elif isinstance(expr, PlExpr):
         # TODO: decide later on the name supplied to `name`
         # with_row_index supercedes with_row_count
         frame: PlDataFrame = data._tbl_data
         meth_row_number = getattr(frame, "with_row_index", None)
         if not meth_row_number:
             meth_row_number = frame.with_row_count
 
         result = meth_row_number(name="__row_number__").filter(expr)
         return [(row_names[ii], ii) for ii in result["__row_number__"]]
+
     elif callable(expr):
         res: "list[bool]" = eval_transform(data._tbl_data, expr)
         if not all(map(lambda x: isinstance(x, bool), res)):
             raise ValueError(
                 "If you select rows using a callable, it must take a DataFrame, "
                 "and return a boolean Series."
             )
@@ -341,15 +341,15 @@
     )
 
 
 # Resolve generic ======================================================================
 
 
 @singledispatch
-def resolve(loc: Loc, *args, **kwargs) -> "Loc | List[CellPos]":
+def resolve(loc: Loc, *args: Any, **kwargs: Any) -> Loc | list[CellPos]:
     """Return a copy of location with lookups resolved (e.g. tidyselect on columns)."""
     raise NotImplementedError(f"Unsupported location type: {type(loc)}")
 
 
 @resolve.register
 def _(loc: LocColumnSpanners, spanners: Spanners) -> LocColumnSpanners:
     # unique labels (with order preserved)
@@ -359,15 +359,15 @@
     resolved_spanners = [spanner_ids[idx] for idx in resolved_spanners_idx]
 
     # Create a list object
     return LocColumnSpanners(ids=resolved_spanners)
 
 
 @resolve.register
-def _(loc: LocBody, data: GTData) -> List[CellPos]:
+def _(loc: LocBody, data: GTData) -> list[CellPos]:
     cols = resolve_cols_i(data=data, expr=loc.columns)
     rows = resolve_rows_i(data=data, expr=loc.rows)
 
     # TODO: dplyr arranges by `Var1`, and does distinct (since you can tidyselect the same
     # thing multiple times
     cell_pos = [
         CellPos(col[1], row[1], colname=col[0]) for col, row in itertools.product(cols, rows)
@@ -376,21 +376,21 @@
     return cell_pos
 
 
 # Style generic ========================================================================
 
 
 @singledispatch
-def set_style(loc: Loc, data: GTData, style: List[str]) -> GTData:
+def set_style(loc: Loc, data: GTData, style: list[str]) -> GTData:
     """Set style for location."""
     raise NotImplementedError(f"Unsupported location type: {type(loc)}")
 
 
 @set_style.register
-def _(loc: LocTitle, data: GTData, style: List[CellStyle]) -> GTData:
+def _(loc: LocTitle, data: GTData, style: list[CellStyle]) -> GTData:
     # validate ----
     for entry in style:
         entry._raise_if_requires_data(loc)
 
     # set ----
     if loc.groups == "title":
         info = StyleInfo(locname="title", locnum=1, styles=style)
@@ -399,16 +399,16 @@
     else:
         raise ValueError(f"Unknown title group: {loc.groups}")
 
     return data._styles.append(info)
 
 
 @set_style.register
-def _(loc: LocBody, data: GTData, style: List[CellStyle]) -> GTData:
-    positions: List[CellPos] = resolve(loc, data)
+def _(loc: LocBody, data: GTData, style: list[CellStyle]) -> GTData:
+    positions: list[CellPos] = resolve(loc, data)
 
     # evaluate any column expressions in styles
     style_ready = [entry._evaluate_expressions(data._tbl_data) for entry in style]
 
     all_info: list[StyleInfo] = []
     for col_pos in positions:
         row_styles = [entry._from_row(data._tbl_data, col_pos.row) for entry in style_ready]
```

### Comparing `great-tables-0.5.0/great_tables/_options.py` & `great_tables-0.5.1/great_tables/_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,170 +1,172 @@
 from __future__ import annotations
+
 from dataclasses import dataclass, fields, replace
-from typing import TYPE_CHECKING, ClassVar, Optional, Union, List, cast, Dict, Any
+from typing import TYPE_CHECKING, ClassVar, cast
+
 from great_tables import _utils
 
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
 def tab_options(
     self: GTSelf,
-    container_width: Optional[str] = None,
-    container_height: Optional[str] = None,
-    container_overflow_x: Optional[str] = None,
-    container_overflow_y: Optional[str] = None,
-    table_width: Optional[str] = None,
-    table_layout: Optional[str] = None,
-    # table_align: Optional[str] = None,
-    table_margin_left: Optional[str] = None,
-    table_margin_right: Optional[str] = None,
-    table_background_color: Optional[str] = None,
-    # table_additional_css: Optional[str] = None,
-    table_font_names: Optional[Union[str, List[str]]] = None,
-    table_font_size: Optional[str] = None,
-    table_font_weight: Optional[str] = None,
-    table_font_style: Optional[str] = None,
-    table_font_color: Optional[str] = None,
-    table_font_color_light: Optional[str] = None,
-    table_border_top_style: Optional[str] = None,
-    table_border_top_width: Optional[str] = None,
-    table_border_top_color: Optional[str] = None,
-    table_border_bottom_style: Optional[str] = None,
-    table_border_bottom_width: Optional[str] = None,
-    table_border_bottom_color: Optional[str] = None,
-    table_border_left_style: Optional[str] = None,
-    table_border_left_width: Optional[str] = None,
-    table_border_left_color: Optional[str] = None,
-    table_border_right_style: Optional[str] = None,
-    table_border_right_width: Optional[str] = None,
-    table_border_right_color: Optional[str] = None,
-    heading_background_color: Optional[str] = None,
-    heading_align: Optional[str] = None,
-    heading_title_font_size: Optional[str] = None,
-    heading_title_font_weight: Optional[str] = None,
-    heading_subtitle_font_size: Optional[str] = None,
-    heading_subtitle_font_weight: Optional[str] = None,
-    heading_padding: Optional[str] = None,
-    heading_padding_horizontal: Optional[str] = None,
-    heading_border_bottom_style: Optional[str] = None,
-    heading_border_bottom_width: Optional[str] = None,
-    heading_border_bottom_color: Optional[str] = None,
-    heading_border_lr_style: Optional[str] = None,
-    heading_border_lr_width: Optional[str] = None,
-    heading_border_lr_color: Optional[str] = None,
-    column_labels_background_color: Optional[str] = None,
-    column_labels_font_size: Optional[str] = None,
-    column_labels_font_weight: Optional[str] = None,
-    column_labels_text_transform: Optional[str] = None,
-    column_labels_padding: Optional[str] = None,
-    column_labels_padding_horizontal: Optional[str] = None,
-    column_labels_vlines_style: Optional[str] = None,
-    column_labels_vlines_width: Optional[str] = None,
-    column_labels_vlines_color: Optional[str] = None,
-    column_labels_border_top_style: Optional[str] = None,
-    column_labels_border_top_width: Optional[str] = None,
-    column_labels_border_top_color: Optional[str] = None,
-    column_labels_border_bottom_style: Optional[str] = None,
-    column_labels_border_bottom_width: Optional[str] = None,
-    column_labels_border_bottom_color: Optional[str] = None,
-    column_labels_border_lr_style: Optional[str] = None,
-    column_labels_border_lr_width: Optional[str] = None,
-    column_labels_border_lr_color: Optional[str] = None,
-    column_labels_hidden: Optional[bool] = None,
-    row_group_background_color: Optional[str] = None,
-    row_group_font_size: Optional[str] = None,
-    row_group_font_weight: Optional[str] = None,
-    row_group_text_transform: Optional[str] = None,
-    row_group_padding: Optional[str] = None,
-    row_group_padding_horizontal: Optional[str] = None,
-    row_group_border_top_style: Optional[str] = None,
-    row_group_border_top_width: Optional[str] = None,
-    row_group_border_top_color: Optional[str] = None,
-    row_group_border_bottom_style: Optional[str] = None,
-    row_group_border_bottom_width: Optional[str] = None,
-    row_group_border_bottom_color: Optional[str] = None,
-    row_group_border_left_style: Optional[str] = None,
-    row_group_border_left_width: Optional[str] = None,
-    row_group_border_left_color: Optional[str] = None,
-    row_group_border_right_style: Optional[str] = None,
-    row_group_border_right_width: Optional[str] = None,
-    row_group_border_right_color: Optional[str] = None,
-    # row_group_default_label: Optional[str] = None,
-    row_group_as_column: Optional[bool] = None,
-    table_body_hlines_style: Optional[str] = None,
-    table_body_hlines_width: Optional[str] = None,
-    table_body_hlines_color: Optional[str] = None,
-    table_body_vlines_style: Optional[str] = None,
-    table_body_vlines_width: Optional[str] = None,
-    table_body_vlines_color: Optional[str] = None,
-    table_body_border_top_style: Optional[str] = None,
-    table_body_border_top_width: Optional[str] = None,
-    table_body_border_top_color: Optional[str] = None,
-    table_body_border_bottom_style: Optional[str] = None,
-    table_body_border_bottom_width: Optional[str] = None,
-    table_body_border_bottom_color: Optional[str] = None,
-    stub_background_color: Optional[str] = None,
-    stub_font_size: Optional[str] = None,
-    stub_font_weight: Optional[str] = None,
-    stub_text_transform: Optional[str] = None,
-    stub_border_style: Optional[str] = None,
-    stub_border_width: Optional[str] = None,
-    stub_border_color: Optional[str] = None,
-    stub_row_group_font_size: Optional[str] = None,
-    stub_row_group_font_weight: Optional[str] = None,
-    stub_row_group_text_transform: Optional[str] = None,
-    stub_row_group_border_style: Optional[str] = None,
-    stub_row_group_border_width: Optional[str] = None,
-    stub_row_group_border_color: Optional[str] = None,
-    data_row_padding: Optional[str] = None,
-    data_row_padding_horizontal: Optional[str] = None,
-    # summary_row_background_color: Optional[str] = None,
-    # summary_row_text_transform: Optional[str] = None,
-    # summary_row_padding: Optional[str] = None,
-    # summary_row_padding_horizontal: Optional[str] = None,
-    # summary_row_border_style: Optional[str] = None,
-    # summary_row_border_width: Optional[str] = None,
-    # summary_row_border_color: Optional[str] = None,
-    # grand_summary_row_background_color: Optional[str] = None,
-    # grand_summary_row_text_transform: Optional[str] = None,
-    # grand_summary_row_padding: Optional[str] = None,
-    # grand_summary_row_padding_horizontal: Optional[str] = None,
-    # grand_summary_row_border_style: Optional[str] = None,
-    # grand_summary_row_border_width: Optional[str] = None,
-    # grand_summary_row_border_color: Optional[str] = None,
-    # footnotes_background_color: Optional[str] = None,
-    # footnotes_font_size: Optional[str] = None,
-    # footnotes_padding: Optional[str] = None,
-    # footnotes_padding_horizontal: Optional[str] = None,
-    # footnotes_border_bottom_style: Optional[str] = None,
-    # footnotes_border_bottom_width: Optional[str] = None,
-    # footnotes_border_bottom_color: Optional[str] = None,
-    # footnotes_border_lr_style: Optional[str] = None,
-    # footnotes_border_lr_width: Optional[str] = None,
-    # footnotes_border_lr_color: Optional[str] = None,
-    # footnotes_marks: Optional[Union[str, List[str]]] = None,
-    # footnotes_multiline: Optional[bool] = None,
-    # footnotes_sep: Optional[str] = None,
-    source_notes_background_color: Optional[str] = None,
-    source_notes_font_size: Optional[str] = None,
-    source_notes_padding: Optional[str] = None,
-    source_notes_padding_horizontal: Optional[str] = None,
-    source_notes_border_bottom_style: Optional[str] = None,
-    source_notes_border_bottom_width: Optional[str] = None,
-    source_notes_border_bottom_color: Optional[str] = None,
-    source_notes_border_lr_style: Optional[str] = None,
-    source_notes_border_lr_width: Optional[str] = None,
-    source_notes_border_lr_color: Optional[str] = None,
-    source_notes_multiline: Optional[bool] = None,
-    source_notes_sep: Optional[str] = None,
-    # row_striping_background_color: Optional[str] = None,
-    # row_striping_include_stub: Optional[bool] = None,
-    # row_striping_include_table_body: Optional[bool] = None,
+    container_width: str | None = None,
+    container_height: str | None = None,
+    container_overflow_x: str | None = None,
+    container_overflow_y: str | None = None,
+    table_width: str | None = None,
+    table_layout: str | None = None,
+    # table_align: str | None = None,
+    table_margin_left: str | None = None,
+    table_margin_right: str | None = None,
+    table_background_color: str | None = None,
+    # table_additional_css: str | None = None,
+    table_font_names: str | list[str] | None = None,
+    table_font_size: str | None = None,
+    table_font_weight: str | None = None,
+    table_font_style: str | None = None,
+    table_font_color: str | None = None,
+    table_font_color_light: str | None = None,
+    table_border_top_style: str | None = None,
+    table_border_top_width: str | None = None,
+    table_border_top_color: str | None = None,
+    table_border_bottom_style: str | None = None,
+    table_border_bottom_width: str | None = None,
+    table_border_bottom_color: str | None = None,
+    table_border_left_style: str | None = None,
+    table_border_left_width: str | None = None,
+    table_border_left_color: str | None = None,
+    table_border_right_style: str | None = None,
+    table_border_right_width: str | None = None,
+    table_border_right_color: str | None = None,
+    heading_background_color: str | None = None,
+    heading_align: str | None = None,
+    heading_title_font_size: str | None = None,
+    heading_title_font_weight: str | None = None,
+    heading_subtitle_font_size: str | None = None,
+    heading_subtitle_font_weight: str | None = None,
+    heading_padding: str | None = None,
+    heading_padding_horizontal: str | None = None,
+    heading_border_bottom_style: str | None = None,
+    heading_border_bottom_width: str | None = None,
+    heading_border_bottom_color: str | None = None,
+    heading_border_lr_style: str | None = None,
+    heading_border_lr_width: str | None = None,
+    heading_border_lr_color: str | None = None,
+    column_labels_background_color: str | None = None,
+    column_labels_font_size: str | None = None,
+    column_labels_font_weight: str | None = None,
+    column_labels_text_transform: str | None = None,
+    column_labels_padding: str | None = None,
+    column_labels_padding_horizontal: str | None = None,
+    column_labels_vlines_style: str | None = None,
+    column_labels_vlines_width: str | None = None,
+    column_labels_vlines_color: str | None = None,
+    column_labels_border_top_style: str | None = None,
+    column_labels_border_top_width: str | None = None,
+    column_labels_border_top_color: str | None = None,
+    column_labels_border_bottom_style: str | None = None,
+    column_labels_border_bottom_width: str | None = None,
+    column_labels_border_bottom_color: str | None = None,
+    column_labels_border_lr_style: str | None = None,
+    column_labels_border_lr_width: str | None = None,
+    column_labels_border_lr_color: str | None = None,
+    column_labels_hidden: bool | None = None,
+    row_group_background_color: str | None = None,
+    row_group_font_size: str | None = None,
+    row_group_font_weight: str | None = None,
+    row_group_text_transform: str | None = None,
+    row_group_padding: str | None = None,
+    row_group_padding_horizontal: str | None = None,
+    row_group_border_top_style: str | None = None,
+    row_group_border_top_width: str | None = None,
+    row_group_border_top_color: str | None = None,
+    row_group_border_bottom_style: str | None = None,
+    row_group_border_bottom_width: str | None = None,
+    row_group_border_bottom_color: str | None = None,
+    row_group_border_left_style: str | None = None,
+    row_group_border_left_width: str | None = None,
+    row_group_border_left_color: str | None = None,
+    row_group_border_right_style: str | None = None,
+    row_group_border_right_width: str | None = None,
+    row_group_border_right_color: str | None = None,
+    # row_group_default_label: str | None = None,
+    row_group_as_column: bool | None = None,
+    table_body_hlines_style: str | None = None,
+    table_body_hlines_width: str | None = None,
+    table_body_hlines_color: str | None = None,
+    table_body_vlines_style: str | None = None,
+    table_body_vlines_width: str | None = None,
+    table_body_vlines_color: str | None = None,
+    table_body_border_top_style: str | None = None,
+    table_body_border_top_width: str | None = None,
+    table_body_border_top_color: str | None = None,
+    table_body_border_bottom_style: str | None = None,
+    table_body_border_bottom_width: str | None = None,
+    table_body_border_bottom_color: str | None = None,
+    stub_background_color: str | None = None,
+    stub_font_size: str | None = None,
+    stub_font_weight: str | None = None,
+    stub_text_transform: str | None = None,
+    stub_border_style: str | None = None,
+    stub_border_width: str | None = None,
+    stub_border_color: str | None = None,
+    stub_row_group_font_size: str | None = None,
+    stub_row_group_font_weight: str | None = None,
+    stub_row_group_text_transform: str | None = None,
+    stub_row_group_border_style: str | None = None,
+    stub_row_group_border_width: str | None = None,
+    stub_row_group_border_color: str | None = None,
+    data_row_padding: str | None = None,
+    data_row_padding_horizontal: str | None = None,
+    # summary_row_background_color: str | None = None,
+    # summary_row_text_transform: str | None = None,
+    # summary_row_padding: str | None = None,
+    # summary_row_padding_horizontal: str | None = None,
+    # summary_row_border_style: str | None = None,
+    # summary_row_border_width: str | None = None,
+    # summary_row_border_color: str | None = None,
+    # grand_summary_row_background_color: str | None = None,
+    # grand_summary_row_text_transform: str | None = None,
+    # grand_summary_row_padding: str | None = None,
+    # grand_summary_row_padding_horizontal: str | None = None,
+    # grand_summary_row_border_style: str | None = None,
+    # grand_summary_row_border_width: str | None = None,
+    # grand_summary_row_border_color: str | None = None,
+    # footnotes_background_color: str | None = None,
+    # footnotes_font_size: str | None = None,
+    # footnotes_padding: str | None = None,
+    # footnotes_padding_horizontal: str | None = None,
+    # footnotes_border_bottom_style: str | None = None,
+    # footnotes_border_bottom_width: str | None = None,
+    # footnotes_border_bottom_color: str | None = None,
+    # footnotes_border_lr_style: str | None = None,
+    # footnotes_border_lr_width: str | None = None,
+    # footnotes_border_lr_color: str | None = None,
+    # footnotes_marks: str | list[str] | None = None,
+    # footnotes_multiline: bool | None = None,
+    # footnotes_sep: str | None = None,
+    source_notes_background_color: str | None = None,
+    source_notes_font_size: str | None = None,
+    source_notes_padding: str | None = None,
+    source_notes_padding_horizontal: str | None = None,
+    source_notes_border_bottom_style: str | None = None,
+    source_notes_border_bottom_width: str | None = None,
+    source_notes_border_bottom_color: str | None = None,
+    source_notes_border_lr_style: str | None = None,
+    source_notes_border_lr_width: str | None = None,
+    source_notes_border_lr_color: str | None = None,
+    source_notes_multiline: bool | None = None,
+    source_notes_sep: str | None = None,
+    # row_striping_background_color: str | None = None,
+    # row_striping_include_stub: bool | None = None,
+    # row_striping_include_table_body: bool | None = None,
 ) -> GTSelf:
     """
     Modify the table output options.
 
     Modify the options available in a table. These options are named by the components, the
     subcomponents, and the element that can adjusted.
 
@@ -541,15 +543,15 @@
         k: replace(getattr(self._options, k), value=v) for k, v in modified_args.items()
     }
     new_options = replace(self._options, **new_options_info)
 
     return self._replace(_options=new_options)
 
 
-def opt_footnote_marks(self: GTSelf, marks: Union[str, List[str]] = "numbers") -> GTSelf:
+def opt_footnote_marks(self: GTSelf, marks: str | list[str] = "numbers") -> GTSelf:
     """
     Option to modify the set of footnote marks
     Alter the footnote marks for any footnotes that may be present in the table. Either a list
     of marks can be provided (including Unicode characters), or, a specific keyword could be
     used to signify a preset sequence. This method serves as a shortcut for using
     `tab_options(footnotes_marks=<marks>)`
 
@@ -867,15 +869,15 @@
 
     return tab_options(self, **dict(zip(horizontal_padding_params, new_horizontal_padding_vals)))
 
 
 def opt_all_caps(
     self: GTSelf,
     all_caps: bool = True,
-    locations: Union[str, List[str]] = ["column_labels", "stub", "row_group"],
+    locations: str | list[str] = ["column_labels", "stub", "row_group"],
 ) -> GTSelf:
     """
     Option to use all caps in select table locations.
 
     Sometimes an all-capitalized look is suitable for a table. By using `opt_all_caps()`, we can
     transform characters in the column labels, the stub, and in all row groups in this way (and
     there's control over which of these locations are transformed). This method serves as a
@@ -923,29 +925,29 @@
       .tab_source_note(source_note="This is only a subset of the dataset.")
       .opt_all_caps()
     )
     ```
     """
 
     # If providing a scalar string value, normalize it to be in a list
-    if type(locations).__name__ != "list":
+    if not isinstance(locations, list):
         locations = _utils._str_scalar_to_list(cast(str, locations))
 
     # Ensure that the `locations` value is a list of strings
     _utils._assert_str_list(locations)
 
     # TODO: Ensure that all values within `locations` are valid
 
     # Set new options for `locations` selected, or, reset to default options
     # if `all_caps` is False
     # TODO: the code constantly reassigns res, in order to prepare for a
     # world where options are not mutating the GT options object.
     # TODO: is there a way to set multiple options at once?
     res = self
-    if all_caps is True:
+    if all_caps:
         if "column_labels" in locations:
             res = tab_options(res, column_labels_font_size="80%")
             res = tab_options(res, column_labels_font_weight="bolder")
             res = tab_options(res, column_labels_text_transform="uppercase")
 
         if "stub" in locations:
             res = tab_options(res, stub_font_size="80%")
@@ -1110,16 +1112,16 @@
     omit_keys = {
         "summary_row_background_color",
         "grand_summary_row_background_color",
         "row_striping_background_color",
         "table_outline_color",
     }
 
-    def dict_omit_keys(dict, omit_keys) -> Dict[str, str]:
-        return {x: dict[x] for x in dict if x not in omit_keys}
+    def dict_omit_keys(dict: dict[str, str], omit_keys: set[str]) -> dict[str, str]:
+        return {x: v for x, v in dict.items() if x not in omit_keys}
 
     params = dict_omit_keys(dict=params, omit_keys=omit_keys)
 
     mapped_params = StyleMapper(**params).map_all()
 
     # Apply the style parameters to the table using the `tab_options()` method
     res = tab_options(self=self, **mapped_params)
@@ -1157,19 +1159,19 @@
         "stub_border_color": ["stub_border_color"],
         "data_hlines_style": ["table_body_hlines_style"],
         "data_hlines_color": ["table_body_hlines_color"],
         "data_vlines_style": ["table_body_vlines_style"],
         "data_vlines_color": ["table_body_vlines_color"],
     }
 
-    def map_entry(self, name: str):
+    def map_entry(self, name: str) -> dict[str, list[str]]:
         return {k: getattr(self, name) for k in self.mappings[name]}
 
-    def map_all(self):
-        items = {}
+    def map_all(self) -> dict[str, list[str]]:
+        items: dict[str, list[str]] = {}
         for field in fields(self):
             items.update(self.map_entry(field.name))
         return items
 
 
 _dict_styles_colors_params = {
     "gray-1": {
```

### Comparing `great-tables-0.5.0/great_tables/_render.py` & `great_tables-0.5.1/great_tables/_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 from typing import Literal
 
 IDE_ENV_FLAGS = {
     "default": {"make_page": False, "all_important": False},
     "quarto": {"make_page": False, "all_important": False},
     "databricks": {"make_page": False, "all_important": False},
```

### Comparing `great-tables-0.5.0/great_tables/_scss.py` & `great_tables-0.5.1/great_tables/_scss.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
-from importlib_resources import files
 import re
-
 from dataclasses import fields
 from functools import partial
-from typing import Optional
 from string import Template
 
+from importlib_resources import files
+
+from ._data_color.base import _html_color, _ideal_fgnd_color
 from ._gt_data import GTData
+from ._helpers import pct, px
 from ._utils import _as_css_font_family_attr, _unique_set
-from ._data_color.base import _html_color, _ideal_fgnd_color
 
 DEFAULTS_TABLE_BACKGROUND = (
     "heading_background_color",
     "column_labels_background_color",
     "row_group_background_color",
     "stub_background_color",
     "stub_row_group_background_color",
@@ -35,53 +35,61 @@
     "summary_row_background_color",
     "grand_summary_row_background_color",
     "footnotes_background_color",
     "source_notes_background_color",
 )
 
 
-def font_color(color: str, table_font_color: str, table_font_color_light: str) -> str:
+def font_color(color: str, dark_option: str, light_option: str) -> str:
+    """Return either dark_option or light_option, whichever is higher contrast with color.
+
+    Handles common html color kinds (like transparent), and always returns a hex color.
+    """
+
+    # Normalize return options to hex colors
+    dark_normalized = _html_color(colors=[dark_option])[0]
+    light_normalized = _html_color(colors=[light_option])[0]
 
     if color == "transparent":
         # With the `transparent` color, the font color should have the same value
-        # as the `table_font_color` option since the background will be transparent
-        return table_font_color
+        # as the `dark_option` option since the background will be transparent
+        return dark_normalized
     if color in ["currentcolor", "currentColor"]:
         # With two variations of `currentColor` value, normalize to `currentcolor`
         return "currentcolor"
     if color in ["inherit", "initial", "unset"]:
         # For the other valid CSS color attribute values, we should pass them through
         return color
 
     # Normalize the color to a hexadecimal value
     color_normalized = _html_color(colors=[color])
 
     # Determine the ideal font color given the different background colors
     ideal_font_color = _ideal_fgnd_color(
         bgnd_color=color_normalized[0],
-        light=table_font_color,
-        dark=table_font_color_light,
+        light=light_normalized,
+        dark=dark_normalized,
     )
 
     return ideal_font_color
 
 
 def css_add(value: str | int, amount: int):
     if isinstance(value, int):
         return value + amount
     elif value.endswith("px"):
-        return f"{int(value[:-2]) + amount}px"
+        return px(int(value[:-2]) + amount)
     elif value.endswith("%"):
-        return f"{int(value[:-1]) + amount}%"
+        return pct(int(value[:-1]) + amount)
     else:
         raise NotImplementedError(f"Unable to add to CSS value: {value}")
 
 
 def compile_scss(
-    data: GTData, id: Optional[str], compress: bool = True, all_important: bool = False
+    data: GTData, id: str | None, compress: bool = True, all_important: bool = False
 ) -> str:
     """Return CSS for styling a table, based on options set."""
 
     # Obtain the SCSS options dictionary
     options = {field.name: getattr(data._options, field.name) for field in fields(data._options)}
 
     # Get collection of parameters that pertain to SCSS ----
@@ -89,16 +97,16 @@
     scss_defaults = {k: params.get("table_background_color") for k in DEFAULTS_TABLE_BACKGROUND}
     scss_params = {**scss_defaults, **params}
 
     # font color variables
     # TODO: at this stage, the params below (e.g. table_font_color) have to exist, right?
     p_font_color = partial(
         font_color,
-        table_font_color=params["table_font_color"],
-        table_font_color_light=params["table_font_color_light"],
+        dark_option=params["table_font_color"],
+        light_option=params["table_font_color_light"],
     )
 
     font_params = {f"font_color_{k}": p_font_color(scss_params[k]) for k in FONT_COLOR_VARS}
 
     final_params = {
         **scss_params,
         **font_params,
```

### Comparing `great-tables-0.5.0/great_tables/_source_notes.py` & `great_tables-0.5.1/great_tables/_source_notes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
+
 from ._text import Text
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
-def tab_source_note(data: GTSelf, source_note: Union[str, Text]) -> GTSelf:
+def tab_source_note(data: GTSelf, source_note: str | Text) -> GTSelf:
     """
     Add a source note citation.
 
     Add a source note to the footer part of the table. A source note is useful for citing the data
     included in the table. Several can be added to the footer, simply use the `tab_source_note()`
     method multiple times and they will be inserted in the order provided. We can use Markdown
     formatting for the note, or, if the table is intended for HTML output, we can include HTML
```

### Comparing `great-tables-0.5.0/great_tables/_spanners.py` & `great_tables-0.5.1/great_tables/_spanners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 import itertools
+from typing import TYPE_CHECKING, Any
 
-from typing import TYPE_CHECKING, Union, List, Dict, Optional, Any
-
-from ._gt_data import Spanners, SpannerInfo
-from ._tbl_data import SelectExpr
+from ._gt_data import SpannerInfo, Spanners
 from ._locations import resolve_cols_c
+from ._tbl_data import SelectExpr
 
 if TYPE_CHECKING:
     from ._gt_data import Boxhead
     from ._types import GTSelf
 
 
-SpannerMatrix = List[Dict[str, Union[str, None]]]
+SpannerMatrix = "list[dict[str, str | None]]"
 
 
 def tab_spanner(
     data: GTSelf,
     label: str,
     columns: SelectExpr = None,
-    spanners: Union[list[str], str, None] = None,
-    level: Optional[int] = None,
-    id: Optional[str] = None,
+    spanners: str | list[str] | None = None,
+    level: int | None = None,
+    id: str | None = None,
     gather: bool = True,
     replace: bool = False,
 ) -> GTSelf:
     """
     Insert a spanner above a selection of column headings.
 
     This part of the table contains, at a minimum, column labels and, optionally, an unlimited
@@ -463,15 +462,15 @@
 
     sel_cols = resolve_cols_c(data=data, expr=columns)
 
     vars = [col.var for col in data._boxhead]
 
     if not len(sel_cols):
         raise Exception("No columns selected.")
-    elif not all([col in vars for col in columns]):
+    elif not all(col in vars for col in sel_cols):
         raise ValueError("All `columns` must exist and be visible in the input `data` table.")
 
     # New boxhead with hidden columns
     new_boxhead = data._boxhead.set_cols_hidden(sel_cols)
 
     return data._replace(_boxhead=new_boxhead)
 
@@ -565,15 +564,15 @@
             yield next_el, 1
 
 
 def is_equal(x: Any, y: Any) -> bool:
     return x is not None and x == y
 
 
-def cols_width(data: GTSelf, cases: Dict[str, str]) -> GTSelf:
+def cols_width(data: GTSelf, cases: dict[str, str]) -> GTSelf:
     """Set the widths of columns.
 
     Manual specifications of column widths can be performed using the `cols_width()` method. We
     choose which columns get specific widths. This can be in units of pixels or as percentages.
     Width assignments are supplied inside of a dictionary where columns are the keys and the
     corresponding width is the value.
```

### Comparing `great-tables-0.5.0/great_tables/_stub.py` & `great_tables-0.5.1/great_tables/_stub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
-from ._gt_data import Stub, RowGroups
+
+from ._gt_data import RowGroups, Stub
 from .utils_render_common import get_row_reorder_df
 
 
 def reorder_stub_df(stub_df: Stub, row_groups: RowGroups) -> Stub:
     """
     Reorders the components of the stub object based on the given row groups.
```

### Comparing `great-tables-0.5.0/great_tables/_stubhead.py` & `great_tables-0.5.1/great_tables/_stubhead.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union
+
+from typing import TYPE_CHECKING
+
 from ._text import Text
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
-def tab_stubhead(self: GTSelf, label: Union[str, Text]) -> GTSelf:
+def tab_stubhead(self: GTSelf, label: str | Text) -> GTSelf:
     """
     Add label text to the stubhead.
 
     Add a label to the stubhead of a table. The stubhead is the lone element that is positioned
     left of the column labels, and above the stub. If a stub does not exist, then there is no
     stubhead (so no change will be made when using this method in that case). We have the
     flexibility to use Markdown formatting for the stubhead label (through use of the
```

### Comparing `great-tables-0.5.0/great_tables/_styles.py` & `great_tables-0.5.1/great_tables/_styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, fields, replace
-from typing import TYPE_CHECKING, Any, Callable, Literal, List, Union
-from typing_extensions import Self, TypeAlias
+from typing import TYPE_CHECKING, Any, Callable, Literal, Union
 
-from ._tbl_data import TblData, _get_cell, PlExpr, eval_transform
+from typing_extensions import Self, TypeAlias
 
+from ._helpers import px
+from ._tbl_data import PlExpr, TblData, _get_cell, eval_transform
 
 if TYPE_CHECKING:
     from ._locations import Loc
 
 
 # Cell Styles ==========================================================================
 # TODO: stubbed out the styles in helpers.R as dataclasses while I was reading it,
@@ -261,15 +262,15 @@
     -------
     CellStyleFill
         A CellStyleFill object, which is used for a `styles` argument if specifying a cell fill
         value.
     """
 
     color: str | ColumnExpr
-    # alpha: Optional[float] = None
+    # alpha: float | None = None
 
     def _to_html_style(self) -> str:
         return f"background-color: {self.color};"
 
 
 @dataclass
 class CellStyleBorders(CellStyle):
@@ -299,42 +300,42 @@
     -------
     CellStyleBorders
         A CellStyleBorders object, which is used for a `styles` argument if specifying cell borders.
     """
 
     sides: (
         Literal["all", "top", "bottom", "left", "right"]
-        | List[Literal["all", "top", "bottom", "left", "right"]]
+        | list[Literal["all", "top", "bottom", "left", "right"]]
         | ColumnExpr
     ) = "all"
     color: str | ColumnExpr = "#000000"
     style: str | ColumnExpr = "solid"
     weight: str | ColumnExpr = "1px"
 
     def _to_html_style(self) -> str:
         # If sides is an empty list, return an empty string
-        if self.sides == []:
+        if isinstance(self.sides, list) and not self.sides:
             return ""
 
         # If self.sides is a string, convert to a list
         if isinstance(self.sides, str):
             self.sides = [self.sides]
 
         # If 'all' is provided then call the function recursively with all sides
         if "all" in self.sides:
             return CellStyleBorders(sides=["top", "bottom", "left", "right"])._to_html_style()
 
         weight = self.weight
         if isinstance(weight, int):
-            weight = f"{weight}px"
+            weight = px(weight)
 
         color = self.color
         style = self.style
 
-        border_css_list: List[str] = []
+        border_css_list: list[str] = []
         for side in self.sides:
             if side not in ["top", "bottom", "left", "right"]:
                 raise ValueError(f"Invalid side '{side}' provided.")
             border_css_list.append(f"border-{side}: {weight} {style} {color};")
 
         border_css = "".join(border_css_list)
         return border_css
```

### Comparing `great-tables-0.5.0/great_tables/_substitution.py` & `great_tables-0.5.1/great_tables/_substitution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
-from ._tbl_data import DataFrameLike, SelectExpr, is_na
-from ._gt_data import FormatterSkipElement, FormatInfo
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Literal
+
 from ._formats import fmt
-from ._text import _process_text, Text
+from ._gt_data import FormatterSkipElement
 from ._helpers import html
-
-
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Type, Union, Literal, List
+from ._tbl_data import DataFrameLike, SelectExpr, is_na
+from ._text import Text, _process_text
 
 if TYPE_CHECKING:
     from ._types import GTSelf
 
 
 def _convert_missing(context: Literal["html"], el: str):
     """Convert el to a context specific representation."""
@@ -28,15 +27,15 @@
 
     return el
 
 
 def sub_missing(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     missing_text: str | Text | None = None,
 ) -> GTSelf:
     """
     Substitute missing values in the table body.
 
     Wherever there is missing data (i.e., `None` values) customizable content may present better
     than the standard representation of missing values that would otherwise appear. The
@@ -94,15 +93,15 @@
     subber = SubMissing(self._tbl_data, missing_text)
     return fmt(self, fns=subber.to_html, columns=columns, rows=rows, is_substitution=True)
 
 
 def sub_zero(
     self: GTSelf,
     columns: SelectExpr = None,
-    rows: Union[int, List[int], None] = None,
+    rows: int | list[int] | None = None,
     zero_text: str = "nil",
 ) -> GTSelf:
     """
     Substitute zero values in the table body.
 
     Wherever there is numerical data that are zero in value, replacement text may be better for
     explanatory purposes. The `sub_zero()` function allows for this replacement through its
```

### Comparing `great-tables-0.5.0/great_tables/_tab_create_modify.py` & `great_tables-0.5.1/great_tables/_tab_create_modify.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     Parameters
     ----------
     style
         The styles to use for the cells at the targeted `locations`. The `style.text()`,
         `style.fill()`, and `style.borders()` classes can be used here to more easily generate valid
         styles.
-    location
+    locations
         The cell or set of cells to be associated with the style. The `loc.body()` class can be used
         here to easily target body cell locations.
 
     Examples
     --------
     Let's use a small subset of the `exibble` dataset to demonstrate how to use `tab_style()` to
     target specific cells and apply styles to them. We'll start by creating the `exibble_sm` table
```

### Comparing `great-tables-0.5.0/great_tables/_tbl_data.py` & `great_tables-0.5.1/great_tables/_tbl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import warnings
-
 from functools import singledispatch
-from typing import Any, Dict, List, Optional, Union, Callable, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
+
 from typing_extensions import TypeAlias
 
 from ._databackend import AbstractBackend
 
 
 # Define databackend types ----
 # These are resolved lazily (e.g. on isinstance checks) when run dynamically,
@@ -87,19 +87,19 @@
 
     TblData = DataFrameLike
 
 
 # utils ----
 
 
-def _raise_not_implemented(data):
+def _raise_not_implemented(data: Any):
     raise NotImplementedError(f"Unsupported data type: {type(data)}")
 
 
-def _raise_pandas_required(msg):
+def _raise_pandas_required(msg: Any):
     raise ImportError(msg)
 
 
 class Agnostic:
     """This class dispatches a generic in a DataFrame agnostic way.
 
     It is available for generics like is_na.
@@ -124,15 +124,15 @@
 @copy_data.register(PlDataFrame)
 def _(data: PlDataFrame):
     return data.clone()
 
 
 # get_column_names ----
 @singledispatch
-def get_column_names(data: DataFrameLike) -> List[str]:
+def get_column_names(data: DataFrameLike) -> list[str]:
     """Get a list of column names from the input data table"""
     _raise_not_implemented(data)
 
 
 @get_column_names.register(PdDataFrame)
 def _(data: PdDataFrame):
     return data.columns.tolist()
@@ -150,35 +150,35 @@
 def n_rows(data: DataFrameLike) -> int:
     """Get the number of rows from the input data table"""
     raise _raise_not_implemented(data)
 
 
 @n_rows.register(PdDataFrame)
 @n_rows.register(PlDataFrame)
-def _(data):
+def _(data: Any) -> int:
     return len(data)
 
 
 # _get_cell ----
 
 
 @singledispatch
 def _get_cell(data: DataFrameLike, row: int, column: str) -> Any:
     """Get the content from a single cell in the input data table"""
 
     _raise_not_implemented(data)
 
 
 @_get_cell.register(PlDataFrame)
-def _(data, row: int, column: str):
+def _(data: Any, row: int, column: str) -> Any:
     return data[column][row]
 
 
 @_get_cell.register(PdDataFrame)
-def _(data, row, col):
+def _(data: Any, row: int, col: str) -> Any:
     col_ii = data.columns.get_loc(col)
 
     if not isinstance(col_ii, int):
         raise ValueError("Column named " + col + " matches multiple columns.")
 
     return data.iloc[row, col_ii]
 
@@ -188,23 +188,23 @@
 
 @singledispatch
 def _set_cell(data: DataFrameLike, row: int, column: str, value: Any):
     _raise_not_implemented(data)
 
 
 @_set_cell.register(PdDataFrame)
-def _(data, row: int, column: str, value: Any):
+def _(data, row: int, column: str, value: Any) -> None:
     # TODO: This assumes column names are unique
     # if this is violated, get_loc will return a mask
     col_indx = data.columns.get_loc(column)
     data.iloc[row, col_indx] = value
 
 
 @_set_cell.register(PlDataFrame)
-def _(data, row: int, column: str, value: Any):
+def _(data, row: int, column: str, value: Any) -> None:
     data[row, column] = value
 
 
 # _get_column_dtype ----
 
 
 @singledispatch
@@ -213,46 +213,46 @@
     return data[column].dtype
 
 
 # reorder ----
 
 
 @singledispatch
-def reorder(data: DataFrameLike, rows: List[int], columns: List[str]) -> DataFrameLike:
+def reorder(data: DataFrameLike, rows: list[int], columns: list[str]) -> DataFrameLike:
     """Return a re-ordered DataFrame."""
     _raise_not_implemented(data)
 
 
 @reorder.register
-def _(data: PdDataFrame, rows: List[int], columns: List[str]) -> PdDataFrame:
+def _(data: PdDataFrame, rows: list[int], columns: list[str]) -> PdDataFrame:
     # note that because loc is label based, we need
     # reset index to allow us to use integer indexing on the rows
     # note that this means the index is not preserved when reordering pandas
     return data.iloc[rows, :].loc[:, columns]
 
 
 @reorder.register
-def _(data: PlDataFrame, rows: List[int], columns: List[str]) -> PlDataFrame:
+def _(data: PlDataFrame, rows: list[int], columns: list[str]) -> PlDataFrame:
     return data[rows, columns]
 
 
 # group_splits ----
 @singledispatch
-def group_splits(data: DataFrameLike, group_key: str) -> Dict[Any, List[int]]:
+def group_splits(data: DataFrameLike, group_key: str) -> dict[Any, list[int]]:
     raise NotImplementedError(f"Unsupported data type: {type(data)}")
 
 
 @group_splits.register
-def _(data: PdDataFrame, group_key: str) -> Dict[Any, List[int]]:
+def _(data: PdDataFrame, group_key: str) -> dict[Any, list[int]]:
     g_df = data.groupby(group_key)
     return {k: list(v) for k, v in g_df.indices.items()}
 
 
 @group_splits.register
-def _(data: PlDataFrame, group_key: str) -> Dict[Any, List[int]]:
+def _(data: PlDataFrame, group_key: str) -> dict[Any, list[int]]:
     # TODO: should ensure row count name isn't already in data
     import polars as pl
 
     # with_row_index supercedes with_row_count
     meth_row_number = getattr(data, "with_row_index", None)
     if not meth_row_number:
         meth_row_number = data.with_row_count
@@ -262,34 +262,36 @@
     res = dict(zip(groups[group_key].to_list(), groups["__row_count__"].to_list()))
     return res
 
 
 # eval_select ----
 
 SelectExpr: TypeAlias = Union[
-    List["str | int"],
+    list["str | int"],
     PlSelectExpr,
     str,
     int,
     Callable[[str], bool],
     None,
 ]
-_NamePos: TypeAlias = List[Tuple[str, int]]
+_NamePos: TypeAlias = list[tuple[str, int]]
 
 
 @singledispatch
 def eval_select(data: DataFrameLike, expr: SelectExpr, strict: bool = True) -> _NamePos:
     """Return a list of column names selected by expr."""
 
     raise NotImplementedError(f"Unsupported type: {type(expr)}")
 
 
 @eval_select.register
 def _(
-    data: PdDataFrame, expr: Union[List[Union[str, int]], Callable[[str], bool]], strict=True
+    data: PdDataFrame,
+    expr: Union[list[Union[str, int]], Callable[[str], bool]],
+    strict: bool = True,
 ) -> _NamePos:
     if isinstance(expr, (str, int)):
         expr = [expr]
 
     if isinstance(expr, list):
         return _eval_select_from_list(list(data.columns), expr)
     elif callable(expr):
@@ -298,15 +300,15 @@
         col_pos = {k: ii for ii, k in enumerate(list(data.columns))}
         return [(col, col_pos[col]) for col in data.columns if expr(col)]
 
     raise NotImplementedError(f"Unsupported selection expr: {expr}")
 
 
 @eval_select.register
-def _(data: PlDataFrame, expr: Union[List[str], _selector_proxy_], strict=True) -> _NamePos:
+def _(data: PlDataFrame, expr: Union[list[str], _selector_proxy_], strict: bool = True) -> _NamePos:
     # TODO: how to annotate type of a polars selector?
     # Seems to be polars.selectors._selector_proxy_.
     from polars import Expr
     from polars import selectors
 
     if isinstance(expr, (str, int)):
         expr = [expr]
@@ -321,15 +323,17 @@
         raise TypeError(f"Unsupported selection expr type: {type(expr)}")
 
     # I don't think there's a way to get the columns w/o running the selection
     final_columns = selectors.expand_selector(data, expr)
     return [(col, col_pos[col]) for col in final_columns]
 
 
-def _eval_select_from_list(columns: list[str], expr: list[str | int]) -> list[tuple[str, int]]:
+def _eval_select_from_list(
+    columns: list[str], expr: list[Union[str, int]]
+) -> list[tuple[str, int]]:
     col_pos = {k: ii for ii, k in enumerate(columns)}
 
     # TODO: should prohibit duplicate names in expr?
     res: list[tuple[str, int]] = []
     for col in expr:
         if isinstance(col, str):
             if col in col_pos:
@@ -424,53 +428,53 @@
     import polars as pl
 
     exprs = [pl.col(name).fill_null(replacement[name]) for name in df.columns]
     return df.select(exprs)
 
 
 @singledispatch
-def to_list(ser: SeriesLike) -> List[Any]:
+def to_list(ser: SeriesLike) -> list[Any]:
     raise NotImplementedError(f"Unsupported type: {type(ser)}")
 
 
 @to_list.register
-def _(ser: PdSeries) -> List[Any]:
+def _(ser: PdSeries) -> list[Any]:
     return ser.tolist()
 
 
 @to_list.register
-def _(ser: PlSeries) -> List[Any]:
+def _(ser: PlSeries) -> list[Any]:
     return ser.to_list()
 
 
 # mutate ----
 
 
 @singledispatch
-def eval_transform(df: DataFrameLike, expr: Any) -> List[Any]:
+def eval_transform(df: DataFrameLike, expr: Any) -> list[Any]:
     raise NotImplementedError(f"Unsupported type: {type(df)}")
 
 
 @eval_transform.register
-def _(df: PdDataFrame, expr: Callable[[PdDataFrame], PdSeries]) -> List[Any]:
+def _(df: PdDataFrame, expr: Callable[[PdDataFrame], PdSeries]) -> list[Any]:
     res = expr(df)
 
     if not isinstance(res, PdSeries):
         raise ValueError(f"Result must be a pandas Series. Received {type(res)}")
     elif not len(res) == len(df):
         raise ValueError(
             f"Result must be same length as input data. Observed different lengths."
             f"\n\nInput data: {len(df)}.\nResult: {len(res)}."
         )
 
     return res.to_list()
 
 
 @eval_transform.register
-def _(df: PlDataFrame, expr: PlExpr) -> List[Any]:
+def _(df: PlDataFrame, expr: PlExpr) -> list[Any]:
     df_res = df.select(expr)
 
     if len(df_res.columns) > 1:
         raise ValueError(f"Result must be a single column. Received {len(df_res.columns)} columns.")
     else:
         res = df_res[df_res.columns[0]]
```

### Comparing `great-tables-0.5.0/great_tables/_text.py` & `great_tables-0.5.1/great_tables/_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from typing import Union, List, Literal
-from dataclasses import dataclass
+from __future__ import annotations
+
 import html
+import re
+from dataclasses import dataclass
+from typing import Literal, Union
 
 import commonmark
-import re
 
 
 @dataclass
 class Text:
     text: str
     type: Literal["from_markdown", "html"]
 
 
 class StringBuilder:
-    pieces: List[Union[str, "StringBuilder"]]
+    pieces: list[Union[str, "StringBuilder"]]
 
     def __init__(self, *args: Union[str, "StringBuilder"]):
         self.pieces = list(args)
 
-    def _collect(self, lst: List[str]):
+    def _collect(self, lst: list[str]):
         for piece in self.pieces:
             if isinstance(piece, str):
                 lst.append(piece)
             else:
                 piece._collect(lst)
 
     def make_string(self) -> str:
         lst = []
         self._collect(lst)
         return "".join(lst)
 
-    def append(self, *args: str):
+    def append(self, *args: str) -> None:
         self.pieces.extend(args)
 
-    def prepend(self, *args: str):
+    def prepend(self, *args: str) -> None:
         self.pieces[0:0] = args
 
 
 def _md_html(x: str) -> str:
     str = commonmark.commonmark(x)
     return re.sub(r"^<p>|</p>\n$", "", str)
 
 
-def _process_text(x: Union[Text, str, None]) -> str:
+def _process_text(x: str | Text | None) -> str:
     if x is None:
         return ""
 
     if isinstance(x, str):
         text = x
         type = "plaintext"
     else:
@@ -59,13 +61,13 @@
         x_out = text
     else:
         x_out = _html_escape(text)
 
     return x_out
 
 
-def _process_text_id(x: Union[Text, str, None]) -> str:
+def _process_text_id(x: str | Text | None) -> str:
     return _process_text(x)
 
 
 def _html_escape(x: str) -> str:
     return html.escape(x)
```

### Comparing `great-tables-0.5.0/great_tables/_utils.py` & `great_tables-0.5.1/great_tables/_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from typing import Optional, Union, List, Any
+from __future__ import annotations
+
 import importlib
-from types import ModuleType
 import json
 import re
+from types import ModuleType
+from typing import Any
 
 from ._tbl_data import PdDataFrame
 
 
-def _try_import(name: str, pip_install_line: Optional[str] = None) -> ModuleType:
+def _try_import(name: str, pip_install_line: str | None = None) -> ModuleType:
     try:
         return importlib.import_module(name)
     except ImportError:
         if pip_install_line is not None:
             raise ImportError(
                 f"Module {name} not found. Run the following to install."
                 f"\n\n`{pip_install_line}`"
             ) from None
         else:
             raise ImportError(f"Module {name} not found.")
 
 
-def heading_has_title(title: Optional[str]) -> bool:
+def heading_has_title(title: str | None) -> bool:
     return title is not None
 
 
-def heading_has_subtitle(subtitle: Optional[str]) -> bool:
+def heading_has_subtitle(subtitle: str | None) -> bool:
     return subtitle is not None
 
 
-def _match_arg(x: str, lst: List[str]) -> str:
+def _match_arg(x: str, lst: list[str]) -> str:
     # Ensure that `lst` has at least one element
     if len(lst) == 0:
         raise ValueError("The `lst` object must contain at least one element.")
 
     # Ensure that all elements in `lst` are strings
     if not all(isinstance(el, str) for el in lst):
         raise ValueError("All elements in the `lst` object must be strings.")
@@ -48,69 +50,67 @@
     if len(matched) == 0:
         raise ValueError(f"The supplied value (`{x}`) is not an allowed option.")
 
     return matched.pop()
 
 
 def _assert_str_scalar(x: Any) -> None:
-    if type(x).__name__ != "str":
+    if not isinstance(x, str):
         raise AssertionError(f"The supplied value (`{x}`) is not a string.")
 
 
 def _assert_str_list(x: Any) -> None:
-    if type(x).__name__ != "list":
+    if not isinstance(x, list):
         raise AssertionError(f"The supplied value (`{x}`) is not a list.")
     if not all(map(lambda x: isinstance(x, str), x)):
         raise AssertionError("Not all elements of the supplied list are strings.")
 
 
-def _assert_str_in_set(x: str, set: List[str]):
-    while x not in set:
+def _assert_str_in_set(x: str, set: list[str]) -> None:
+    if x not in set:
         raise AssertionError(f"The string `{x}` is not part of the defined `set`.")
 
 
-def _assert_list_is_subset(x: List[Any], set_list: List[Any]) -> None:
+def _assert_list_is_subset(x: list[Any], set_list: list[Any]) -> None:
     if not set(x).issubset(set(set_list)):
         raise AssertionError("The columns provided are not present in the table.")
 
-    return
-
 
-def _str_scalar_to_list(x: str):
+def _str_scalar_to_list(x: str) -> list[str]:
     _assert_str_scalar(x)
     return [x]
 
 
-def _unique_set(x: Union[List[Any], None]) -> Union[List[Any], None]:
+def _unique_set(x: list[Any] | None) -> list[Any] | None:
     if x is None:
         return None
     return list({k: True for k in x})
 
 
-def _as_css_font_family_attr(fonts: List[str], value_only: bool = False) -> str:
+def _as_css_font_family_attr(fonts: list[str], value_only: bool = False) -> str:
     fonts_w_spaces = list(map(lambda x: f"'{x}'" if " " in x else x, fonts))
 
     fonts_str = ", ".join(fonts_w_spaces)
 
-    if value_only is True:
+    if value_only:
         return fonts_str
 
     return f"font-family: {fonts_str};"
 
 
 def _object_as_dict(v: Any) -> Any:
     try:
         return v.object_as_dict()
     except Exception:
         pass
     if isinstance(v, PdDataFrame):
         return v.to_dict()
-    if type(v) in [tuple, list]:
+    if isinstance(v, (tuple, list)):
         return list(_object_as_dict(i) for i in v)
-    if type(v) == dict:
+    if isinstance(v, dict):
         return dict((k, _object_as_dict(val)) for (k, val) in v.items())
     if type(v) == type(_object_as_dict):  # FIXME figure out how to get "function"
         return f"<function {v.__name__}>"
     try:
         d = vars(v)
     except TypeError:
         try:
@@ -121,38 +121,38 @@
     return dict((k, _object_as_dict(v)) for (k, v) in d.items())
 
 
 def prettify_gt_object(v: Any) -> str:
     return json.dumps(_object_as_dict(v), indent=2)
 
 
-def _collapse_list_elements(lst, separator=""):
+def _collapse_list_elements(lst: list[Any], separator: str = "") -> str:
     """
     Concatenates all elements of a list into a single string, separated by a given separator.
 
     Args:
         lst (list): The list to be collapsed.
         separator (str, optional): The separator to be used. Defaults to "".
 
     Returns:
         str: The collapsed string.
     """
     return separator.join(lst)
 
 
-def _insert_into_list(lst: List[Any], el: Any) -> List[Any]:
+def _insert_into_list(lst: list[Any], el: Any) -> list[Any]:
     """
     Inserts an element into the beginning of a list and returns the updated list.
 
     Args:
-        lst (List[Any]): The list to insert the element into.
+        lst (list[Any]): The list to insert the element into.
         el (Any): The element to insert.
 
     Returns:
-        List[Any]: The updated list with the element inserted at the beginning.
+        list[Any]: The updated list with the element inserted at the beginning.
     """
     lst.insert(0, el)
     return lst
 
 
 def _str_replace(string: str, pattern: str, replace: str) -> str:
     return string.replace(pattern, replace)
```

### Comparing `great-tables-0.5.0/great_tables/_utils_nanoplots.py` & `great_tables-0.5.1/great_tables/_utils_nanoplots.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Optional, List, Union, Any, Dict, Callable
-import numpy as np
+from __future__ import annotations
 
-from great_tables._utils import _match_arg
+from typing import Any, Callable
+
+import numpy as np
 from great_tables._tbl_data import Agnostic, is_na
+from great_tables._utils import _match_arg
 
 REFERENCE_LINE_KEYWORDS = ["mean", "median", "min", "max", "q1", "q3"]
 
 
 def _is_na(x: Any) -> bool:
     return is_na(Agnostic(), x)
 
@@ -39,56 +41,54 @@
         ValueError("The input cannot be a list. It must be a single value.")
 
     return isinstance(x, (str))
 
 
 # This determines whether an entire list of values are integer-like; this skips
 # over missing values and returns a single boolean
-def _is_integerlike(val_list: List[Any]) -> bool:
+def _is_integerlike(val_list: list[Any]) -> bool:
     """
     Determine whether an entire list of values are integer-like; this skips
     over missing values and returns a single boolean.
     """
 
     # If the list is empty, return False
     if len(val_list) == 0:
         return False
 
     return all((isinstance(val, (int, np.integer)) or _is_na(val)) for val in val_list)
 
 
-def _any_na_in_list(x: List[Any]) -> bool:
+def _any_na_in_list(x: list[Any]) -> bool:
     """
     Determine whether a list of values contains any missing values.
     """
 
     return any(_is_na(val) for val in x)
 
 
-def _check_any_na_in_list(x: List[Union[int, float]]) -> None:
+def _check_any_na_in_list(x: list[int | float]) -> None:
     """
     Check whether a list of values contains any missing values; if so, raise an error.
     """
 
     if _any_na_in_list(x):
         raise ValueError("The list of values cannot contain missing values.")
 
-    return None
-
 
 # Remove missing values from a list of values
-def _remove_na_from_list(x: List[Union[int, float]]) -> List[Union[int, float]]:
+def _remove_na_from_list(x: list[int | float]) -> list[int | float]:
     """
     Remove missing values from a list of values.
     """
 
     return [val for val in x if not _is_na(val)]
 
 
-def _normalize_option_list(option_list: Union[Any, List[Any]], num_y_vals: int) -> List[Any]:
+def _normalize_option_list(option_list: Any | list[Any], num_y_vals: int) -> list[Any]:
     """
     Normalize an option list to have the same length as the number of `y` values.
     """
 
     # If `option_list` is a single value, then make it a list
     if not isinstance(option_list, list):
         option_list = [option_list]
@@ -98,28 +98,28 @@
 
     if len(option_list) == 1:
         option_list = [option_list[0]] * num_y_vals
 
     return option_list
 
 
-def calc_ref_value(val_or_calc: "int | float | str", data) -> Union[int, float]:
+def calc_ref_value(val_or_calc: "int | float | str", data) -> int | float:
     if _val_is_numeric(val_or_calc):
         return val_or_calc
     elif _val_is_str(val_or_calc) and val_or_calc in REFERENCE_LINE_KEYWORDS:
         return _generate_ref_line_from_keyword(vals=data, keyword=val_or_calc)
 
     raise ValueError(f"Unsupported nanoplot area value: {val_or_calc}")
 
 
 def _format_number_compactly(
-    val: Union[int, float],
-    currency: Optional[str] = None,
+    val: int | float,
+    currency: str | None = None,
     as_integer: bool = False,
-    fn: Optional[Callable[..., str]] = None,
+    fn: Callable[..., str] | None = None,
 ) -> str:
     """
     Format a single numeric value compactly, using a currency if provided.
     """
 
     from great_tables.vals import fmt_currency, fmt_scientific, fmt_integer, fmt_number
 
@@ -268,107 +268,103 @@
 #
 # Collection of general functions to calculate the mean, min, max, median,
 # and other statistical measures from a list of values; the list should not
 # be expected to contain any missing values so we won't guard against them here
 #
 
 
-def _gt_mean(x: List[Union[int, float]]) -> float:
+def _gt_mean(x: list[int | float]) -> float:
     """
     Calculate the mean of a list of values.
     """
 
     return sum(x) / len(x)
 
 
-def _gt_min(x: List[Union[int, float]]) -> Union[int, float]:
+def _gt_min(x: list[int | float]) -> int | float:
     """
     Calculate the minimum value from a list of values.
     """
     return min(x)
 
 
-def _gt_max(x: List[Union[int, float]]) -> Union[int, float]:
+def _gt_max(x: list[int | float]) -> int | float:
     """
     Calculate the maximum value from a list of values.
     """
     return max(x)
 
 
-def _gt_median(x: List[Union[int, float]]) -> Union[int, float]:
+def _gt_median(x: list[int | float]) -> int | float:
     """
     Calculate the median of a list of values.
     """
     x.sort()
     n = len(x)
     if n % 2 == 0:
         return (x[n // 2 - 1] + x[n // 2]) / 2
     else:
         return x[n // 2]
 
 
-def _gt_first(x: List[Union[int, float]]) -> Union[int, float]:
+def _gt_first(x: list[int | float]) -> int | float:
     """
     Get the first value from a list of values.
     """
     return x[0]
 
 
-def _gt_last(x: List[Union[int, float]]) -> Union[int, float]:
+def _gt_last(x: list[int | float]) -> int | float:
     """
     Get the last value from a list of values.
     """
     return x[-1]
 
 
-def _gt_quantile(x: List[Union[int, float]], q: float) -> Union[int, float]:
+def _gt_quantile(x: list[int | float], q: float) -> int | float:
     """
     Calculate the quantile of a list of values.
     """
     x.sort()
     n = len(x)
     return x[int(n * q)]
 
 
-def _gt_q1(x: List[Union[int, float]]) -> float:
+def _gt_q1(x: list[int | float]) -> float:
     """
     Calculate the first quartile of a list of values.
     """
     return _gt_quantile(x, 0.25)
 
 
-def _gt_q3(x: List[Union[int, float]]) -> float:
+def _gt_q3(x: list[int | float]) -> float:
     """
     Calculate the third quartile of a list of values.
     """
     return _gt_quantile(x, 0.75)
 
 
-def _flatten_list(x: List[Any]) -> Union[List[float], List[int], List[Union[int, float]]]:
+def _flatten_list(x: list[Any]) -> list[int] | list[float] | list[int | float]:
     """
     Flatten a list of values.
     """
 
     flat_list = []
-
-    # Iterate through the outer list
     for element in x:
-        if type(element) is list:
-            # If the element is of type list, iterate through the sublist
-            for item in element:
-                flat_list.append(item)
+        if isinstance(element, list):
+            flat_list.extend(_flatten_list(element))
         else:
             flat_list.append(element)
     return flat_list
 
 
 def _get_extreme_value(
-    *args: Union[int, float],
+    *args: int | float,
     stat: str = "max",
-) -> Union[int, float]:
+) -> int | float:
     """
     Get either the maximum or minimum value from a list of numeric values.
     """
 
     # Ensure that `stat` is either 'max' or 'min'
     _match_arg(stat, lst=["max", "min"])
 
@@ -388,17 +384,15 @@
         extreme_val = max(val_list)
     else:
         extreme_val = min(val_list)
 
     return extreme_val
 
 
-def _generate_ref_line_from_keyword(
-    vals: List[Union[int, float]], keyword: str
-) -> Union[int, float]:
+def _generate_ref_line_from_keyword(vals: list[int | float], keyword: str) -> int | float:
     """
     Generate a value for a reference line from a valid keyword.
     """
 
     _match_arg(
         x=keyword,
         lst=REFERENCE_LINE_KEYWORDS,
@@ -425,17 +419,15 @@
         ref_line = _gt_q1(vals)
     else:
         ref_line = _gt_q3(vals)
 
     return ref_line
 
 
-def _normalize_vals(
-    x: Union[List[Union[int, float]], List[int], List[float]]
-) -> List[Union[int, float]]:
+def _normalize_vals(x: list[int] | list[float] | list[int | float]) -> list[int | float]:
     """
     Normalize a list of numeric values to be between 0 and 1. Account for missing values.
     """
 
     x_missing = [i for i, val in enumerate(x) if _is_na(val)]
     mean_x = np.mean([val for val in x if not _is_na(val)])
     x = [mean_x if _is_na(val) else val for val in x]
@@ -448,23 +440,23 @@
     x = [np.nan if i in x_missing else val for i, val in enumerate(x)]
     return x
 
 
 # TODO: example nanoplot showing when jitter vals might be applied
 # Looks like it's on the x-axis:
 # GT(pd.DataFrame({'x': [{"x": [1, 1, 1], "y": [2, 3, 4]}]})).fmt_nanoplot("x")
-def _jitter_vals(x: List[Union[int, float]], amount: float) -> List[Union[int, float]]:
+def _jitter_vals(x: list[int | float], amount: float) -> list[int | float]:
     """
     Jitter a list of numeric values by a small amount.
     """
 
     return [val + np.random.uniform(-amount, amount) for val in x]
 
 
-def _normalize_to_dict(**kwargs: List[Union[int, float]]) -> Dict[str, List[Union[int, float]]]:
+def _normalize_to_dict(**kwargs: list[int | float]) -> dict[str, list[int | float]]:
     """
     Normalize a collection of numeric values to be between 0 and 1. Account for missing values.
     This only accepts values (scalar or list) associated with keyword arguments. A dictionary
     is returned with the same keys but the values are normalized lists. This is done so that
     any disparate collection of normalized values are distinguishable by their original keys.
     """
 
@@ -518,23 +510,23 @@
     show_data_points: bool,
     show_data_line: bool,
     show_data_area: bool,
     show_reference_line: bool,
     show_reference_area: bool,
     show_vertical_guides: bool,
     show_y_axis_guide: bool,
-    ref_area_tags: Optional[str] = None,
-    area_path_tags: Optional[str] = None,
-    data_path_tags: Optional[str] = None,
-    zero_line_tags: Optional[str] = None,
-    bar_tags: Optional[str] = None,
-    ref_line_tags: Optional[str] = None,
-    circle_tags: Optional[str] = None,
-    g_y_axis_tags: Optional[str] = None,
-    g_guide_tags: Optional[str] = None,
+    ref_area_tags: str | None = None,
+    area_path_tags: str | None = None,
+    data_path_tags: str | None = None,
+    zero_line_tags: str | None = None,
+    bar_tags: str | None = None,
+    ref_line_tags: str | None = None,
+    circle_tags: str | None = None,
+    g_y_axis_tags: str | None = None,
+    g_guide_tags: str | None = None,
 ) -> str:
     """
     Construct an SVG nanoplot from a collection of SVG tags.
     """
 
     # For the optional strings, transform None to an empty string
     ref_area_tags = "" if ref_area_tags is None or show_reference_area is False else ref_area_tags
@@ -547,39 +539,39 @@
     g_y_axis_tags = "" if g_y_axis_tags is None or show_y_axis_guide is False else g_y_axis_tags
     g_guide_tags = "" if g_guide_tags is None or show_vertical_guides is False else g_guide_tags
 
     return f'<div><svg role="img" viewBox="{viewbox}" style="height: {svg_height}; margin-left: auto; margin-right: auto; font-size: inherit; overflow: visible; vertical-align: middle; position:relative;">{svg_defs}{svg_style}{ref_area_tags}{area_path_tags}{data_path_tags}{zero_line_tags}{bar_tags}{ref_line_tags}{circle_tags}{g_y_axis_tags}{g_guide_tags}</svg></div>'
 
 
 def _generate_nanoplot(
-    y_vals: Union[List[Union[int, float]], List[int], List[float]],
-    y_ref_line: Optional[str] = None,
-    y_ref_area: Optional[str] = None,
-    x_vals: "List[Union[int, float]] | None" = None,
-    expand_x: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
-    expand_y: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
+    y_vals: list[int] | list[float] | list[int | float],
+    y_ref_line: str | None = None,
+    y_ref_area: str | None = None,
+    x_vals: list[int | float] | None = None,
+    expand_x: list[int] | list[float] | list[int | float] | None = None,
+    expand_y: list[int] | list[float] | list[int | float] | None = None,
     missing_vals: str = "marker",
-    all_y_vals: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
-    all_single_y_vals: Optional[Union[List[Union[int, float]], List[int], List[float]]] = None,
+    all_y_vals: list[int] | list[float] | list[int | float] | None = None,
+    all_single_y_vals: list[int] | list[float] | list[int | float] | None = None,
     plot_type: str = "line",
     data_line_type: str = "curved",
-    currency: Optional[str] = None,
-    y_val_fmt_fn: Optional[Callable[..., str]] = None,
-    y_axis_fmt_fn: Optional[Callable[..., str]] = None,
-    y_ref_line_fmt_fn: Optional[Callable[..., str]] = None,
-    data_point_radius: Union[int, List[int]] = 10,
-    data_point_stroke_color: Union[str, List[str]] = "#FFFFFF",
-    data_point_stroke_width: Union[int, List[int]] = 4,
-    data_point_fill_color: Union[str, List[str]] = "#FF0000",
+    currency: str | None = None,
+    y_val_fmt_fn: Callable[..., str] | None = None,
+    y_axis_fmt_fn: Callable[..., str] | None = None,
+    y_ref_line_fmt_fn: Callable[..., str] | None = None,
+    data_point_radius: int | list[int] = 10,
+    data_point_stroke_color: str | list[str] = "#FFFFFF",
+    data_point_stroke_width: int | list[int] = 4,
+    data_point_fill_color: str | list[str] = "#FF0000",
     data_line_stroke_color: str = "#4682B4",
     data_line_stroke_width: int = 8,
     data_area_fill_color: str = "#FF0000",
-    data_bar_stroke_color: Union[str, List[str]] = "#3290CC",
-    data_bar_stroke_width: Union[int, List[int]] = 4,
-    data_bar_fill_color: Union[str, List[str]] = "#3FB5FF",
+    data_bar_stroke_color: str | list[str] = "#3290CC",
+    data_bar_stroke_width: int | list[int] = 4,
+    data_bar_fill_color: str | list[str] = "#3FB5FF",
     data_bar_negative_stroke_color: str = "#CC3243",
     data_bar_negative_stroke_width: int = 4,
     data_bar_negative_fill_color: str = "#D75A68",
     reference_line_color: str = "#75A8B0",
     reference_area_fill_color: str = "#A6E6F2",
     vertical_guide_stroke_color: str = "#911EB4",
     vertical_guide_stroke_width: int = 12,
@@ -629,15 +621,15 @@
     g_guide_tags = None
 
     # Initialize the `single_horizontal_plot` variable with `False`
     single_horizontal_plot = False
 
     # If the number of `y` values in a list is zero or if all consist of NA values,
     # return an empty string
-    if type(y_vals) is list and len(y_vals) == 0:
+    if isinstance(y_vals, list) and len(y_vals) == 0:
         return ""
 
     # If all `y` values are NA, return an empty string
     # TODO: all([]) evaluates to True. In that case does this produce the intended behavior?
     if isinstance(y_vals, list) and all(_map_is_na(y_vals)):
         return ""
 
@@ -705,22 +697,22 @@
         y_vals = y_vals.dropna()
 
         if x_vals is not None:
             # Remove the corresponding `x` values for the removed `y` values
             x_vals = x_vals[y_vals.index]
 
     # Get the number of data points for `y`
-    if type(y_vals) is list:
+    if isinstance(y_vals, list):
         num_y_vals = len(y_vals)
     else:
         num_y_vals = 1
 
     # If `y_vals` is a scalar value we requested a 'line' or 'bar' plot, then
     # reset several parameters
-    if type(y_vals) in [int, float] and plot_type in ["line", "bar"]:
+    if isinstance(y_vals, (int, float)) and plot_type in ["line", "bar"]:
 
         single_horizontal_plot = True
         show_data_points = True
         show_data_line = True
         show_data_area = False
         show_reference_line = False
         show_reference_area = False
@@ -1426,14 +1418,15 @@
         ref_area_tags = f'<path d="{ref_area_path}" stroke="transparent" stroke-width="2" fill="{fill}" fill-opacity="0.8"></path>'
 
     #
     # Generate y-axis guide
     #
 
     if show_y_axis_guide:
+        is_all_intify_y_axis = len(y_vals) == _get_n_intlike(y_vals)
 
         rect_tag = f'<rect x="{left_x}" y="{top_y}" width="{safe_x_d + 15}" height="{bottom_y}" stroke="transparent" stroke-width="0" fill="transparent"></rect>'
 
         if _is_integerlike(val_list=[y_scale_max]) and _is_integerlike(val_list=[y_scale_min]):
             y_axis_guide_vals_integerlike = True
         else:
             y_axis_guide_vals_integerlike = False
@@ -1449,25 +1442,30 @@
         y_value_min_label = _format_number_compactly(
             val=y_scale_min,
             currency=currency,
             as_integer=y_axis_guide_vals_integerlike,
             fn=y_axis_fmt_fn,
         )
 
+        if is_all_intify_y_axis:
+            y_value_max_label = _remove_exponent(y_value_max_label)
+            y_value_min_label = _remove_exponent(y_value_min_label)
+
         text_strings_min = f'<text x="{left_x}" y="{safe_y_d + data_y_height + safe_y_d - data_y_height / 25}" fill="transparent" stroke="transparent" font-size="25">{y_value_min_label}</text>'
 
         text_strings_max = f'<text x="{left_x}" y="{safe_y_d + data_y_height / 25}" fill="transparent" stroke="transparent" font-size="25">{y_value_max_label}</text>'
 
         g_y_axis_tags = f'<g class="y-axis-line">{rect_tag}{text_strings_max}{text_strings_min}</g>'
 
     #
     # Generate vertical data point guidelines
     #
 
     if show_vertical_guides:
+        is_all_intify_v_guides = len(y_vals) == _get_n_intlike(y_vals)
 
         g_guide_strings = []
 
         for i, _ in enumerate(data_x_points):
 
             rect_strings_i = f'<rect x="{data_x_points[i] - 10}" y="{top_y}" width="20" height="{bottom_y}" stroke="transparent" stroke-width="{vertical_guide_stroke_width}" fill="transparent"></rect>'
 
@@ -1477,14 +1475,17 @@
             )
 
             x_text = data_x_points[i] + 10
 
             if y_value_i == "NA":
                 x_text = x_text + 2
 
+            if is_all_intify_v_guides:
+                y_value_i = _remove_exponent(y_value_i)
+
             text_strings_i = f'<text x="{x_text}" y="{safe_y_d + 5}" fill="transparent" stroke="transparent" font-size="30px">{y_value_i}</text>'
 
             g_guide_strings_i = f'<g class="vert-line">{rect_strings_i}{text_strings_i}</g>'
 
             g_guide_strings.append(g_guide_strings_i)
 
         g_guide_tags = "".join(g_guide_strings)
@@ -1567,7 +1568,46 @@
         ref_line_tags=ref_line_tags,
         circle_tags=circle_tags,
         g_y_axis_tags=g_y_axis_tags,
         g_guide_tags=g_guide_tags,
     )
 
     return nanoplot_svg
+
+
+def _is_intlike(n: Any, scaled_by: float = 1e17) -> bool:
+    """
+    https://stackoverflow.com/a/71373152
+    """
+    import numbers
+    from decimal import Decimal
+
+    if isinstance(n, str):
+        try:
+            # Replacement of minus sign (U+2212) with hyphen (necessary in some locales)
+            n = float(n.replace("−", "-"))
+        except ValueError:
+            return False
+    elif isinstance(n, Decimal):
+        n = float(n)
+    return isinstance(n, numbers.Real) and ((n * scaled_by - int(n) * scaled_by) == 0)
+
+
+def _get_n_intlike(nums: list[Any]) -> int:
+    return len([n for n in nums if _is_intlike(n)])
+
+
+def _remove_exponent(n: "str | int | float") -> int:
+    """
+    https://docs.python.org/3/library/decimal.html#decimal-faq
+    """
+    from decimal import Decimal
+
+    if isinstance(n, str):
+        # Replacement of minus sign (U+2212) with hyphen (necessary in some locales)
+        n = str(n).replace("−", "-")
+    d = Decimal(n)
+    if d == d.to_integral():
+        x = d.quantize(Decimal(1))
+    else:
+        x = d.normalize()
+    return int(x)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `great-tables-0.5.0/great_tables/_utils_render_html.py` & `great_tables-0.5.1/great_tables/_utils_render_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from great_tables._spanners import spanners_print_matrix, seq_groups
+from __future__ import annotations
+
+from itertools import chain, groupby
+from typing import Any, cast
+
+from great_tables._spanners import seq_groups, spanners_print_matrix
+from htmltools import HTML, TagList, css, tags
+
 from ._gt_data import GTData
-from ._tbl_data import n_rows, _get_cell, cast_frame_to_string, replace_null_frame
-from typing import List, Any, cast
-from htmltools import tags, HTML, css, TagList
-from itertools import groupby, chain
+from ._tbl_data import _get_cell, cast_frame_to_string, n_rows, replace_null_frame
 from ._text import StringBuilder, _process_text, _process_text_id
-from .utils_render_common import get_row_reorder_df
+from ._utils import heading_has_subtitle, heading_has_title
 
 
 def create_heading_component_h(data: GTData) -> StringBuilder:
     result = StringBuilder()
 
     title = data._heading.title
     subtitle = data._heading.subtitle
 
-    has_title = title is not None
-    has_subtitle = subtitle is not None
+    has_title = heading_has_title(title)
+    has_subtitle = heading_has_subtitle(subtitle)
 
     # If there is no title or heading component, then return an empty string
     if not has_title and not has_subtitle:
         return result
 
     # Raise an error if there is a subtitle but no title
     if not has_title and has_subtitle:
@@ -437,43 +441,45 @@
     has_two_col_stub = "group_label" in stub_layout
     has_groups = data._row_groups is not None and len(data._row_groups) > 0
 
     # If there is a stub, then prepend that to the `column_vars` list
     if stub_var is not None:
         column_vars = [stub_var] + column_vars
 
-    body_rows: List[str] = []
+    body_rows: list[str] = []
 
     # iterate over rows (ordered by groupings)
     prev_group_label = None
 
     ordered_index = data._group_rows.indices_map(n_rows(data._tbl_data))
 
     for i, group_label in ordered_index:
-        body_cells: List[str] = []
+        body_cells: list[str] = []
 
         if has_stub_column and has_groups and not has_two_col_stub:
             colspan_value = data._boxhead._get_effective_number_of_columns(
                 stub=data._stub, row_groups=data._row_groups, options=data._options
             )
 
             # Generate a row that contains the row group label (this spans the entire row) but
             # only if `i` indicates there should be a row group label
             if group_label != prev_group_label:
                 group_class = (
                     "gt_empty_group_heading" if group_label == "" else "gt_group_heading_row"
                 )
 
-                body_cells.append(
-                    f"<tr class={group_class}>"
-                    f'  <th class="gt_group_heading" colspan="{colspan_value}">'
-                    + group_label
-                    + "</th></tr>"
-                )
+                group_row = f"""  <tr class="{group_class}">
+    <th class="gt_group_heading" colspan="{colspan_value}">{group_label}</th>
+  </tr>"""
+
+                prev_group_label = group_label
+
+                body_rows.append(group_row)
 
+        # Create a single cell and append result to `body_cells`
         for colinfo in column_vars:
             cell_content: Any = _get_cell(tbl_data, i, colinfo.var)
             cell_str: str = str(cell_content)
 
             # Determine whether the current cell is the stub cell
             if has_stub_column:
                 is_stub_cell = colinfo.var == stub_var.var
@@ -494,26 +500,28 @@
                 style_entries = list(chain(*[x.styles for x in styles_i]))
                 rendered_styles = [el._to_html_style() for el in style_entries]
                 cell_styles = f'style="{" ".join(rendered_styles)}"' + " "
             else:
                 cell_styles = ""
 
             if is_stub_cell:
-                body_cells.append('  <th class="gt_row gt_left gt_stub">' + cell_str + "</th>")
+                body_cells.append(f"""    <th class="gt_row gt_left gt_stub">{cell_str}</th>""")
             else:
                 body_cells.append(
-                    f'  <td {cell_styles}class="gt_row gt_{cell_alignment}">' + cell_str + "</td>"
+                    f"""    <td {cell_styles}class="gt_row gt_{cell_alignment}">{cell_str}</td>"""
                 )
 
         prev_group_label = group_label
-        body_rows.append("<tr>\n" + "\n".join(body_cells) + "\n</tr>")
+        body_rows.append("  <tr>\n" + "\n".join(body_cells) + "\n  </tr>")
 
     all_body_rows = "\n".join(body_rows)
 
-    return f'<tbody class="gt_table_body">\n{all_body_rows}\n</tbody>'
+    return f"""<tbody class="gt_table_body">
+{all_body_rows}
+</tbody>"""
 
 
 def create_source_notes_component_h(data: GTData) -> str:
     source_notes = data._source_notes
 
     # If there are no source notes, then return an empty string
     if source_notes == []:
@@ -530,15 +538,15 @@
     )
 
     # Handle the multiline source notes case (each note takes up one line)
     if multiline:
         # Create the source notes component as a series of `<tr><td>` (one per
         # source note) inside of a `<tfoot>`
 
-        source_notes_tr: List[str] = []
+        source_notes_tr: list[str] = []
 
         for note in source_notes:
             note_str = _process_text(note)
 
             source_notes_tr.append(
                 f"""
   <tr>
@@ -557,15 +565,15 @@
 
     # TODO: Perform HTML escaping on the separator text and
     # transform space characters to non-breaking spaces
 
     # Create the source notes component as a single `<tr><td>` inside
     # of a `<tfoot>`
 
-    source_note_list: List[str] = []
+    source_note_list: list[str] = []
     for note in source_notes:
         note_str = _process_text(note)
         source_note_list.append(note_str)
 
     source_notes_str_joined = separator.join(source_note_list)
 
     source_notes_component = f"""<tfoot>
```

### Comparing `great-tables-0.5.0/great_tables/css/gt_colors.scss` & `great_tables-0.5.1/great_tables/css/gt_colors.scss`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/css/gt_styles_default.scss` & `great_tables-0.5.1/great_tables/css/gt_styles_default.scss`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/01-countrypops.csv` & `great_tables-0.5.1/great_tables/data/01-countrypops.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/02-sza.csv` & `great_tables-0.5.1/great_tables/data/02-sza.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/03-gtcars.csv` & `great_tables-0.5.1/great_tables/data/03-gtcars.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/04-sp500.csv` & `great_tables-0.5.1/great_tables/data/04-sp500.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/05-pizzaplace.csv` & `great_tables-0.5.1/great_tables/data/05-pizzaplace.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/06-exibble.csv` & `great_tables-0.5.1/great_tables/data/06-exibble.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/07-towny.csv` & `great_tables-0.5.1/great_tables/data/07-towny.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/08-metro.csv` & `great_tables-0.5.1/great_tables/data/08-metro.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/09-constants.csv` & `great_tables-0.5.1/great_tables/data/09-constants.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/10-illness.csv` & `great_tables-0.5.1/great_tables/data/10-illness.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/11-islands.csv` & `great_tables-0.5.1/great_tables/data/11-islands.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/__init__.py` & `great_tables-0.5.1/great_tables/data/__init__.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_10.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_10.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_11.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_11.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_12.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_12.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_13.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_13.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_14.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_14.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_2.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_2.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_3.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_3.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_3bis.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_3bis.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_5.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_5.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_6.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_6.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_7bis.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_7bis.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_8.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_8.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/metro_9.svg` & `great_tables-0.5.1/great_tables/data/metro_images/metro_9.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/rer_A.svg` & `great_tables-0.5.1/great_tables/data/metro_images/rer_A.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/rer_B.svg` & `great_tables-0.5.1/great_tables/data/metro_images/rer_B.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/rer_C.svg` & `great_tables-0.5.1/great_tables/data/metro_images/rer_C.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/rer_D.svg` & `great_tables-0.5.1/great_tables/data/metro_images/rer_D.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/rer_E.svg` & `great_tables-0.5.1/great_tables/data/metro_images/rer_E.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T1.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T1.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T11.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T11.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T13.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T13.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T2.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T2.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T3a.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T3a.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T3b.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T3b.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T4.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T4.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T5.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T5.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T6.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T6.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T7.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T7.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T8.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T8.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/tram_T9.svg` & `great_tables-0.5.1/great_tables/data/metro_images/tram_T9.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_H.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_H.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_J.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_J.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_K.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_K.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_L.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_L.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_N.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_N.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_P.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_P.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_R.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_R.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/metro_images/transilien_U.svg` & `great_tables-0.5.1/great_tables/data/metro_images/transilien_U.svg`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/x-airquality.csv` & `great_tables-0.5.1/great_tables/data/x-airquality.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/x_currencies.csv` & `great_tables-0.5.1/great_tables/data/x_currencies.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/x_default_locales.csv` & `great_tables-0.5.1/great_tables/data/x_default_locales.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/data/x_locales.csv` & `great_tables-0.5.1/great_tables/data/x_locales.csv`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/gt.py` & `great_tables-0.5.1/great_tables/gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 from __future__ import annotations
 
-from typing import Any, List
-from typing_extensions import Self
+from typing import Any
 
-import copy
+from typing_extensions import Self
 
 from great_tables._gt_data import GTData
 
 # Main gt imports ----
 from great_tables._body import body_reassemble
 from great_tables._boxhead import cols_align, cols_label
 from great_tables._data_color import data_color
 from great_tables._export import as_raw_html, save
 from great_tables._formats import (
     fmt,
-    fmt_number,
-    fmt_percent,
-    fmt_integer,
-    fmt_scientific,
-    fmt_currency,
     fmt_bytes,
-    fmt_roman,
+    fmt_currency,
     fmt_date,
-    fmt_time,
     fmt_datetime,
-    fmt_markdown,
     fmt_image,
+    fmt_integer,
+    fmt_markdown,
     fmt_nanoplot,
+    fmt_number,
+    fmt_percent,
+    fmt_roman,
+    fmt_scientific,
+    fmt_time,
 )
-from great_tables._substitution import sub_missing, sub_zero
 from great_tables._heading import tab_header
 from great_tables._helpers import random_id
 from great_tables._options import (
-    tab_options,
     opt_align_table_header,
     opt_all_caps,
     opt_footnote_marks,
-    opt_row_striping,
-    opt_vertical_padding,
     opt_horizontal_padding,
-    opt_table_outline,
+    opt_row_striping,
     opt_stylize,
+    opt_table_outline,
+    opt_vertical_padding,
+    tab_options,
 )
+from great_tables._render import infer_render_env_defaults
 from great_tables._source_notes import tab_source_note
 from great_tables._spanners import (
-    tab_spanner,
+    cols_hide,
     cols_move,
-    cols_move_to_start,
     cols_move_to_end,
-    cols_hide,
+    cols_move_to_start,
     cols_width,
+    tab_spanner,
 )
 from great_tables._stub import reorder_stub_df
 from great_tables._stubhead import tab_stubhead
-from great_tables._tbl_data import n_rows, _get_cell
+from great_tables._substitution import sub_missing, sub_zero
+from great_tables._tab_create_modify import tab_style
+from great_tables._tbl_data import _get_cell, n_rows
 from great_tables._utils_render_html import (
-    create_heading_component_h,
-    create_columns_component_h,
+    _get_table_defs,
     create_body_component_h,
-    create_source_notes_component_h,
+    create_columns_component_h,
     create_footnotes_component_h,
-    _get_table_defs,
+    create_heading_component_h,
+    create_source_notes_component_h,
 )
-from great_tables._tab_create_modify import tab_style
-from great_tables._render import infer_render_env_defaults
-
 
 __all__ = ["GT"]
 
 
 # =============================================================================
 # GT class
 # =============================================================================
@@ -401,52 +399,35 @@
 <body>
 {finalized_table}
 </body>
 </html>
             """
         return finalized_table
 
-    def _finalize_html_table(
-        style: str, quarto_disable_processing: str, quarto_use_bootstrap: str, *args: Any
-    ) -> str:
-        from htmltools import tags
-
-        html_tbl = tags.table(
-            data_quarto_disable_processing=quarto_disable_processing,
-            data_quarto_bootstrap=quarto_use_bootstrap,
-            *args,
-            class_="gt_table",
-            style=style,
-        )
-
-        html_tbl = str(html_tbl)
-
-        return html_tbl
-
 
 # =============================================================================
 # End of GT class
 # =============================================================================
 
 
 # =============================================================================
 # Functions that operate on GT objects
 # =============================================================================
 
 
-def _get_column_labels(gt: GT, context: str) -> List[str]:
+def _get_column_labels(gt: GT, context: str) -> list[str]:
     gt_built = gt._build_data(context=context)
     column_labels = [x.column_label for x in gt_built._boxhead]
     return column_labels
 
 
-def _get_column_of_values(gt: GT, column_name: str, context: str) -> List[str]:
+def _get_column_of_values(gt: GT, column_name: str, context: str) -> list[str]:
     gt_built = gt._build_data(context=context)
     tbl_data = gt_built._body.body
-    cell_values: List[str] = []
+    cell_values: list[str] = []
 
     for i in range(n_rows(tbl_data)):
         cell_content: Any = _get_cell(tbl_data, i, column_name)
         cell_str: str = str(cell_content)
         cell_values.append(cell_str)
 
     return cell_values
```

### Comparing `great-tables-0.5.0/great_tables/shiny.py` & `great_tables-0.5.1/great_tables/shiny.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/great_tables/utils_render_common.py` & `great_tables-0.5.1/great_tables/utils_render_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Tuple
+from typing import TYPE_CHECKING
+
+from typing_extensions import TypeAlias
 
 if TYPE_CHECKING:
     from ._gt_data import RowGroups, Stub
 
 
-TupleStartFinal = Tuple[int, int]
+TupleStartFinal: TypeAlias = tuple[int, int]
 
 
 def get_row_reorder_df(groups: RowGroups, stub_df: Stub) -> list[TupleStartFinal]:
     # Get the number of non-None entries in the `groupname_col`
     n_stub_entries = len([entry for entry in stub_df if entry.group_id is not None])
 
     # Raise a ValueError if there are row group entries but no RowGroups
@@ -32,14 +34,14 @@
 
     # From running test_body_reassemble():
     # print(groups_pos)
     # [0, 1, 0, 1] <- correct
     # [1, 0, 1, 0] <- wrong
 
     # the index that when used on the rows will sort them by the order in groups
-    start_pos = list(range(len(groups_pos)))
+    start_pos = range(len(groups_pos))
     sort_indx = sorted(start_pos, key=lambda ii: groups_pos[ii])
 
     # From running test_body_reassemble():
     # [(0, 0), (1, 2), (2, 1), (3, 3)] <- correct
     # [(0, 1), (1, 3), (2, 0), (3, 2)] <- wrong
     return list(zip(start_pos, sort_indx))
```

### Comparing `great-tables-0.5.0/great_tables.egg-info/PKG-INFO` & `great_tables-0.5.1/great_tables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.0 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.5.1 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `great-tables-0.5.0/great_tables.egg-info/SOURCES.txt` & `great_tables-0.5.1/great_tables.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 docs/assets/gt_parts_of_a_table.svg
 docs/assets/gt_sp500_table.svg
 docs/assets/gt_workflow_diagram.svg
 docs/assets/tables_from_the_web.png
 docs/assets/the_components_of_a_table.svg
 docs/blog/index.qmd
 docs/blog/introduction_great_tables.qmd
+docs/blog/bring-your-own-df/index.qmd
 docs/blog/design-philosophy/a_simple_table.png
 docs/blog/design-philosophy/cave_grids.png
 docs/blog/design-philosophy/composition_of_a_table_in_GT.png
 docs/blog/design-philosophy/computer_tables.png
 docs/blog/design-philosophy/index.qmd
 docs/blog/design-philosophy/nippur_cuneiform_tablet.png
 docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
@@ -53,14 +54,15 @@
 docs/blog/introduction-0.4.0/index.qmd
 docs/blog/polars-styling/index.qmd
 docs/blog/polars-styling/table-preview.png
 docs/blog/superbowl-squares/_code.py
 docs/blog/superbowl-squares/games.csv
 docs/blog/superbowl-squares/index.qmd
 docs/examples/index.qmd
+docs/examples/_data/power_cie_prepared_tbl.csv
 docs/examples/sports-earnings/basketball.png
 docs/examples/sports-earnings/boxing.png
 docs/examples/sports-earnings/golf.png
 docs/examples/sports-earnings/index.ipynb
 docs/examples/sports-earnings/soccer.png
 docs/examples/sports-earnings/sports_earnings.csv
 docs/examples/sports-earnings/tennis.png
@@ -193,24 +195,26 @@
 tests/test_dependencies.py
 tests/test_export.py
 tests/test_formats.py
 tests/test_formats_nanoplots.py
 tests/test_gt.py
 tests/test_gt_data.py
 tests/test_heading.py
+tests/test_helpers.py
 tests/test_locations.py
 tests/test_options.py
 tests/test_repr.py
 tests/test_scss.py
 tests/test_shiny.py
 tests/test_spanners.py
 tests/test_styles.py
 tests/test_substitutions.py
 tests/test_tab_create_modify.py
 tests/test_tbl_data.py
+tests/test_utils.py
 tests/test_utils_render_common.py
 tests/test_utils_render_html.py
 tests/__snapshots__/test_export.ambr
 tests/__snapshots__/test_formats.ambr
 tests/__snapshots__/test_locations.ambr
 tests/__snapshots__/test_options.ambr
 tests/__snapshots__/test_repr.ambr
```

### Comparing `great-tables-0.5.0/pyproject.toml` & `great_tables-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_export.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_export.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -60,64 +60,68 @@
   <tr class="gt_col_headings">
     <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id=""></th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="num">num</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="char">char</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="currency">currency</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-  <tr class=gt_group_heading_row>  <th class="gt_group_heading" colspan="4">grp_a</th></tr>
-    <th class="gt_row gt_left gt_stub">row_1</th>
-    <td class="gt_row gt_right">0.11</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td class="gt_row gt_right">$49.95</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_2</th>
-    <td class="gt_row gt_right">2.22</td>
-    <td class="gt_row gt_left">banana</td>
-    <td class="gt_row gt_right">$17.95</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_3</th>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td class="gt_row gt_right">$1.39</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_4</th>
-    <td class="gt_row gt_right">444.40</td>
-    <td class="gt_row gt_left">durian</td>
-    <td class="gt_row gt_right">$65,100.00</td>
-  </tr>
-  <tr>
-  <tr class=gt_group_heading_row>  <th class="gt_group_heading" colspan="4">grp_b</th></tr>
-    <th class="gt_row gt_left gt_stub">row_5</th>
-    <td class="gt_row gt_right">5,550.00</td>
-    <td class="gt_row gt_left"><NA></td>
-    <td class="gt_row gt_right">$1,325.81</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_6</th>
-    <td class="gt_row gt_right">nan</td>
-    <td class="gt_row gt_left">fig</td>
-    <td class="gt_row gt_right">$13.26</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_7</th>
-    <td class="gt_row gt_right">777,000.00</td>
-    <td class="gt_row gt_left">grapefruit</td>
-    <td class="gt_row gt_right"><NA></td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">row_8</th>
-    <td class="gt_row gt_right">8,880,000.00</td>
-    <td class="gt_row gt_left">honeydew</td>
-    <td class="gt_row gt_right">$0.44</td>
-  </tr>
+    <tr class="gt_group_heading_row">
+      <th class="gt_group_heading" colspan="4">grp_a</th>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_1</th>
+      <td class="gt_row gt_right">0.11</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td class="gt_row gt_right">$49.95</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_2</th>
+      <td class="gt_row gt_right">2.22</td>
+      <td class="gt_row gt_left">banana</td>
+      <td class="gt_row gt_right">$17.95</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_3</th>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td class="gt_row gt_right">$1.39</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_4</th>
+      <td class="gt_row gt_right">444.40</td>
+      <td class="gt_row gt_left">durian</td>
+      <td class="gt_row gt_right">$65,100.00</td>
+    </tr>
+    <tr class="gt_group_heading_row">
+      <th class="gt_group_heading" colspan="4">grp_b</th>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_5</th>
+      <td class="gt_row gt_right">5,550.00</td>
+      <td class="gt_row gt_left"><NA></td>
+      <td class="gt_row gt_right">$1,325.81</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_6</th>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_left">fig</td>
+      <td class="gt_row gt_right">$13.26</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_7</th>
+      <td class="gt_row gt_right">777,000.00</td>
+      <td class="gt_row gt_left">grapefruit</td>
+      <td class="gt_row gt_right"><NA></td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">row_8</th>
+      <td class="gt_row gt_right">8,880,000.00</td>
+      <td class="gt_row gt_left">honeydew</td>
+      <td class="gt_row gt_right">$0.44</td>
+    </tr>
   </tbody>
     <tfoot class="gt_sourcenotes">
     
     <tr>
       <td class="gt_sourcenote" colspan="4">This is only a subset of the dataset.</td>
     </tr>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 # serializer version: 1 # name: test_html_string_generated '''
 DDaattaa lliissttiinngg ffrroomm eexxiibbbbllee
 eexxiibbbbllee iiss aa GGrreeaatt TTaabblleess ddaattaasseett..
       nnuumm          cchhaarr       ccuurrrreennccyy
 ggrrpp__aa
+rrooww__11 0.11         apricot    $49.95
 rrooww__22 2.22         banana     $17.95
 rrooww__33 33.33        coconut    $1.39
 rrooww__44 444.40       durian     $65,100.00
 ggrrpp__bb
-rrooww__66 nan          fig        $13.26
+rrooww__55 5,550.00                $1,325.81
+rrooww__66              fig        $13.26
 rrooww__77 777,000.00   grapefruit
 rrooww__88 8,880,000.00 honeydew   $0.44
 This is only a subset of the dataset.
 ''' # ---
```

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_formats.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_formats.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -11,195 +11,195 @@
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="time">time</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="datetime">datetime</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="currency">currency</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="row">row</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" scope="col" id="group">group</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1.11 × 10<sup style='font-size: 65%;'>−1</sup></td>
-    <td class="gt_row gt_left">apricot</td>
-    <td class="gt_row gt_left">one</td>
-    <td class="gt_row gt_right">15 January 2015</td>
-    <td class="gt_row gt_right">13:35</td>
-    <td class="gt_row gt_right">2018-01-01 02:22</td>
-    <td class="gt_row gt_right">$49.95</td>
-    <td class="gt_row gt_left">row_1</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.22</td>
-    <td class="gt_row gt_left">banana</td>
-    <td class="gt_row gt_left">two</td>
-    <td class="gt_row gt_right">15 February 2015</td>
-    <td class="gt_row gt_right">14:40</td>
-    <td class="gt_row gt_right">2018-02-02 14:33</td>
-    <td class="gt_row gt_right">$17.95</td>
-    <td class="gt_row gt_left">row_2</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">3.33 × 10<sup style='font-size: 65%;'>1</sup></td>
-    <td class="gt_row gt_left">coconut</td>
-    <td class="gt_row gt_left">three</td>
-    <td class="gt_row gt_right">15 March 2015</td>
-    <td class="gt_row gt_right">15:45</td>
-    <td class="gt_row gt_right">2018-03-03 03:44</td>
-    <td class="gt_row gt_right">$1.39</td>
-    <td class="gt_row gt_left">row_3</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">4.44 × 10<sup style='font-size: 65%;'>2</sup></td>
-    <td class="gt_row gt_left">durian</td>
-    <td class="gt_row gt_left">four</td>
-    <td class="gt_row gt_right">15 April 2015</td>
-    <td class="gt_row gt_right">16:50</td>
-    <td class="gt_row gt_right">2018-04-04 15:55</td>
-    <td class="gt_row gt_right">$65,100.00</td>
-    <td class="gt_row gt_left">row_4</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">5.55 × 10<sup style='font-size: 65%;'>3</sup></td>
-    <td class="gt_row gt_left"><NA></td>
-    <td class="gt_row gt_left">five</td>
-    <td class="gt_row gt_right">15 May 2015</td>
-    <td class="gt_row gt_right">17:55</td>
-    <td class="gt_row gt_right">2018-05-05 04:00</td>
-    <td class="gt_row gt_right">$1,325.81</td>
-    <td class="gt_row gt_left">row_5</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_left">fig</td>
-    <td class="gt_row gt_left">six</td>
-    <td class="gt_row gt_right">15 June 2015</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">2018-06-06 16:11</td>
-    <td class="gt_row gt_right">$13.26</td>
-    <td class="gt_row gt_left">row_6</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">7.77 × 10<sup style='font-size: 65%;'>5</sup></td>
-    <td class="gt_row gt_left">grapefruit</td>
-    <td class="gt_row gt_left">seven</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">19:10</td>
-    <td class="gt_row gt_right">2018-07-07 05:22</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_left">row_7</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">8.88 × 10<sup style='font-size: 65%;'>6</sup></td>
-    <td class="gt_row gt_left">honeydew</td>
-    <td class="gt_row gt_left">eight</td>
-    <td class="gt_row gt_right">15 August 2015</td>
-    <td class="gt_row gt_right">20:20</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">$0.44</td>
-    <td class="gt_row gt_left">row_8</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1.11 × 10<sup style='font-size: 65%;'>−1</sup></td>
+      <td class="gt_row gt_left">apricot</td>
+      <td class="gt_row gt_left">one</td>
+      <td class="gt_row gt_right">15 January 2015</td>
+      <td class="gt_row gt_right">13:35</td>
+      <td class="gt_row gt_right">2018-01-01 02:22</td>
+      <td class="gt_row gt_right">$49.95</td>
+      <td class="gt_row gt_left">row_1</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.22</td>
+      <td class="gt_row gt_left">banana</td>
+      <td class="gt_row gt_left">two</td>
+      <td class="gt_row gt_right">15 February 2015</td>
+      <td class="gt_row gt_right">14:40</td>
+      <td class="gt_row gt_right">2018-02-02 14:33</td>
+      <td class="gt_row gt_right">$17.95</td>
+      <td class="gt_row gt_left">row_2</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">3.33 × 10<sup style='font-size: 65%;'>1</sup></td>
+      <td class="gt_row gt_left">coconut</td>
+      <td class="gt_row gt_left">three</td>
+      <td class="gt_row gt_right">15 March 2015</td>
+      <td class="gt_row gt_right">15:45</td>
+      <td class="gt_row gt_right">2018-03-03 03:44</td>
+      <td class="gt_row gt_right">$1.39</td>
+      <td class="gt_row gt_left">row_3</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">4.44 × 10<sup style='font-size: 65%;'>2</sup></td>
+      <td class="gt_row gt_left">durian</td>
+      <td class="gt_row gt_left">four</td>
+      <td class="gt_row gt_right">15 April 2015</td>
+      <td class="gt_row gt_right">16:50</td>
+      <td class="gt_row gt_right">2018-04-04 15:55</td>
+      <td class="gt_row gt_right">$65,100.00</td>
+      <td class="gt_row gt_left">row_4</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">5.55 × 10<sup style='font-size: 65%;'>3</sup></td>
+      <td class="gt_row gt_left"><NA></td>
+      <td class="gt_row gt_left">five</td>
+      <td class="gt_row gt_right">15 May 2015</td>
+      <td class="gt_row gt_right">17:55</td>
+      <td class="gt_row gt_right">2018-05-05 04:00</td>
+      <td class="gt_row gt_right">$1,325.81</td>
+      <td class="gt_row gt_left">row_5</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_left">fig</td>
+      <td class="gt_row gt_left">six</td>
+      <td class="gt_row gt_right">15 June 2015</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">2018-06-06 16:11</td>
+      <td class="gt_row gt_right">$13.26</td>
+      <td class="gt_row gt_left">row_6</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">7.77 × 10<sup style='font-size: 65%;'>5</sup></td>
+      <td class="gt_row gt_left">grapefruit</td>
+      <td class="gt_row gt_left">seven</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">19:10</td>
+      <td class="gt_row gt_right">2018-07-07 05:22</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_left">row_7</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">8.88 × 10<sup style='font-size: 65%;'>6</sup></td>
+      <td class="gt_row gt_left">honeydew</td>
+      <td class="gt_row gt_left">eight</td>
+      <td class="gt_row gt_right">15 August 2015</td>
+      <td class="gt_row gt_right">20:20</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">$0.44</td>
+      <td class="gt_row gt_left">row_8</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
   </tbody>
   
   
   
   '''
 # ---
 # name: test_format_snap
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1.11 × 10<sup style='font-size: 65%;'>−1</sup></td>
-    <td class="gt_row gt_left">apricot</td>
-    <td class="gt_row gt_left">one</td>
-    <td class="gt_row gt_right">15 January 2015</td>
-    <td class="gt_row gt_right">13:35</td>
-    <td class="gt_row gt_right">2018-01-01 02:22</td>
-    <td class="gt_row gt_right">$49.95</td>
-    <td class="gt_row gt_left">row_1</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.22</td>
-    <td class="gt_row gt_left">banana</td>
-    <td class="gt_row gt_left">two</td>
-    <td class="gt_row gt_right">15 February 2015</td>
-    <td class="gt_row gt_right">14:40</td>
-    <td class="gt_row gt_right">2018-02-02 14:33</td>
-    <td class="gt_row gt_right">$17.95</td>
-    <td class="gt_row gt_left">row_2</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">3.33 × 10<sup style='font-size: 65%;'>1</sup></td>
-    <td class="gt_row gt_left">coconut</td>
-    <td class="gt_row gt_left">three</td>
-    <td class="gt_row gt_right">15 March 2015</td>
-    <td class="gt_row gt_right">15:45</td>
-    <td class="gt_row gt_right">2018-03-03 03:44</td>
-    <td class="gt_row gt_right">$1.39</td>
-    <td class="gt_row gt_left">row_3</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">4.44 × 10<sup style='font-size: 65%;'>2</sup></td>
-    <td class="gt_row gt_left">durian</td>
-    <td class="gt_row gt_left">four</td>
-    <td class="gt_row gt_right">15 April 2015</td>
-    <td class="gt_row gt_right">16:50</td>
-    <td class="gt_row gt_right">2018-04-04 15:55</td>
-    <td class="gt_row gt_right">$65,100.00</td>
-    <td class="gt_row gt_left">row_4</td>
-    <td class="gt_row gt_left">grp_a</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">5.55 × 10<sup style='font-size: 65%;'>3</sup></td>
-    <td class="gt_row gt_left"><NA></td>
-    <td class="gt_row gt_left">five</td>
-    <td class="gt_row gt_right">15 May 2015</td>
-    <td class="gt_row gt_right">17:55</td>
-    <td class="gt_row gt_right">2018-05-05 04:00</td>
-    <td class="gt_row gt_right">$1,325.81</td>
-    <td class="gt_row gt_left">row_5</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_left">fig</td>
-    <td class="gt_row gt_left">six</td>
-    <td class="gt_row gt_right">15 June 2015</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">2018-06-06 16:11</td>
-    <td class="gt_row gt_right">$13.26</td>
-    <td class="gt_row gt_left">row_6</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">7.77 × 10<sup style='font-size: 65%;'>5</sup></td>
-    <td class="gt_row gt_left">grapefruit</td>
-    <td class="gt_row gt_left">seven</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">19:10</td>
-    <td class="gt_row gt_right">2018-07-07 05:22</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_left">row_7</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">8.88 × 10<sup style='font-size: 65%;'>6</sup></td>
-    <td class="gt_row gt_left">honeydew</td>
-    <td class="gt_row gt_left">eight</td>
-    <td class="gt_row gt_right">15 August 2015</td>
-    <td class="gt_row gt_right">20:20</td>
-    <td class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">$0.44</td>
-    <td class="gt_row gt_left">row_8</td>
-    <td class="gt_row gt_left">grp_b</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1.11 × 10<sup style='font-size: 65%;'>−1</sup></td>
+      <td class="gt_row gt_left">apricot</td>
+      <td class="gt_row gt_left">one</td>
+      <td class="gt_row gt_right">15 January 2015</td>
+      <td class="gt_row gt_right">13:35</td>
+      <td class="gt_row gt_right">2018-01-01 02:22</td>
+      <td class="gt_row gt_right">$49.95</td>
+      <td class="gt_row gt_left">row_1</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.22</td>
+      <td class="gt_row gt_left">banana</td>
+      <td class="gt_row gt_left">two</td>
+      <td class="gt_row gt_right">15 February 2015</td>
+      <td class="gt_row gt_right">14:40</td>
+      <td class="gt_row gt_right">2018-02-02 14:33</td>
+      <td class="gt_row gt_right">$17.95</td>
+      <td class="gt_row gt_left">row_2</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">3.33 × 10<sup style='font-size: 65%;'>1</sup></td>
+      <td class="gt_row gt_left">coconut</td>
+      <td class="gt_row gt_left">three</td>
+      <td class="gt_row gt_right">15 March 2015</td>
+      <td class="gt_row gt_right">15:45</td>
+      <td class="gt_row gt_right">2018-03-03 03:44</td>
+      <td class="gt_row gt_right">$1.39</td>
+      <td class="gt_row gt_left">row_3</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">4.44 × 10<sup style='font-size: 65%;'>2</sup></td>
+      <td class="gt_row gt_left">durian</td>
+      <td class="gt_row gt_left">four</td>
+      <td class="gt_row gt_right">15 April 2015</td>
+      <td class="gt_row gt_right">16:50</td>
+      <td class="gt_row gt_right">2018-04-04 15:55</td>
+      <td class="gt_row gt_right">$65,100.00</td>
+      <td class="gt_row gt_left">row_4</td>
+      <td class="gt_row gt_left">grp_a</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">5.55 × 10<sup style='font-size: 65%;'>3</sup></td>
+      <td class="gt_row gt_left"><NA></td>
+      <td class="gt_row gt_left">five</td>
+      <td class="gt_row gt_right">15 May 2015</td>
+      <td class="gt_row gt_right">17:55</td>
+      <td class="gt_row gt_right">2018-05-05 04:00</td>
+      <td class="gt_row gt_right">$1,325.81</td>
+      <td class="gt_row gt_left">row_5</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_left">fig</td>
+      <td class="gt_row gt_left">six</td>
+      <td class="gt_row gt_right">15 June 2015</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">2018-06-06 16:11</td>
+      <td class="gt_row gt_right">$13.26</td>
+      <td class="gt_row gt_left">row_6</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">7.77 × 10<sup style='font-size: 65%;'>5</sup></td>
+      <td class="gt_row gt_left">grapefruit</td>
+      <td class="gt_row gt_left">seven</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">19:10</td>
+      <td class="gt_row gt_right">2018-07-07 05:22</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_left">row_7</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">8.88 × 10<sup style='font-size: 65%;'>6</sup></td>
+      <td class="gt_row gt_left">honeydew</td>
+      <td class="gt_row gt_left">eight</td>
+      <td class="gt_row gt_right">15 August 2015</td>
+      <td class="gt_row gt_right">20:20</td>
+      <td class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">$0.44</td>
+      <td class="gt_row gt_left">row_8</td>
+      <td class="gt_row gt_left">grp_b</td>
+    </tr>
   </tbody>
   '''
 # ---
```

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_options.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_options.ambr`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_repr.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_repr.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -51,22 +51,22 @@
   <table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
   
   <tr class="gt_col_headings">
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="x">x</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="y">y</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
   </tbody>
   
   
   </table>
   
   </div>
           
@@ -124,22 +124,22 @@
   <table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
   
   <tr class="gt_col_headings">
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="x">x</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="y">y</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
   </tbody>
   
   
   </table>
   
   </div>
           
@@ -197,22 +197,22 @@
   <table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
   
   <tr class="gt_col_headings">
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="x">x</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="y">y</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
   </tbody>
   
   
   </table>
   
   </div>
           
@@ -270,22 +270,22 @@
   <table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
   
   <tr class="gt_col_headings">
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="x">x</th>
     <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" scope="col" id="y">y</th>
   </tr>
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
   </tbody>
   
   
   </table>
   
   </div>
```

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_scss.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_scss.ambr`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/tests/__snapshots__/test_utils_render_html.ambr` & `great_tables-0.5.1/tests/__snapshots__/test_utils_render_html.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 # serializer version: 1
 # name: test_body_multiple_locations
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="background-color: red;" class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td style="background-color: red;" class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td style="background-color: red;" class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td style="background-color: red;" class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td style="background-color: red;" class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td style="background-color: red;" class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_body_multiple_styles
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="background-color: red; border-left: 1px solid #000000;" class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td style="background-color: red; border-left: 1px solid #000000;" class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_render_groups_reordered
   '''
   <tbody class="gt_table_body">
-  <tr>
-  <tr class=gt_group_heading_row>  <th class="gt_group_heading" colspan="2">A</th></tr>
-    <th class="gt_row gt_left gt_stub">0</th>
-    <td class="gt_row gt_right">00</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">2</th>
-    <td class="gt_row gt_right">22</td>
-  </tr>
-  <tr>
-  <tr class=gt_group_heading_row>  <th class="gt_group_heading" colspan="2">B</th></tr>
-    <th class="gt_row gt_left gt_stub">1</th>
-    <td class="gt_row gt_right">11</td>
-  </tr>
-  <tr>
-    <th class="gt_row gt_left gt_stub">3</th>
-    <td class="gt_row gt_right">33</td>
-  </tr>
+    <tr class="gt_group_heading_row">
+      <th class="gt_group_heading" colspan="2">A</th>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">0</th>
+      <td class="gt_row gt_right">00</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">2</th>
+      <td class="gt_row gt_right">22</td>
+    </tr>
+    <tr class="gt_group_heading_row">
+      <th class="gt_group_heading" colspan="2">B</th>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">1</th>
+      <td class="gt_row gt_right">11</td>
+    </tr>
+    <tr>
+      <th class="gt_row gt_left gt_stub">3</th>
+      <td class="gt_row gt_right">33</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_source_notes_snap
   '''
     <tfoot class="gt_sourcenotes">
     
@@ -84,184 +88,184 @@
   
   </tfoot>
   '''
 # ---
 # name: test_styling_data_01
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: red;" class="gt_row gt_right">0.1111</td>
-    <td style="color: red;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td style="color: red;" class="gt_row gt_right">2.222</td>
-    <td style="color: red;" class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td style="color: red;" class="gt_row gt_right">33.33</td>
-    <td style="color: red;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td style="color: red;" class="gt_row gt_right">0.1111</td>
+      <td style="color: red;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td style="color: red;" class="gt_row gt_right">2.222</td>
+      <td style="color: red;" class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td style="color: red;" class="gt_row gt_right">33.33</td>
+      <td style="color: red;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_02
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="color: red;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td style="color: red;" class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="color: red;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="color: red;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td style="color: red;" class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="color: red;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_03
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="color: red;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="color: red;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="color: red;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="color: red;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_04
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_05
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_06
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_07
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="border-left: 1px solid #000000;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="border-left: 1px solid #000000;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="border-left: 1px solid #000000;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="border-left: 1px solid #000000;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_08
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="border-left: 1px solid #000000;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="border-left: 1px solid #000000;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="border-left: 1px solid #000000;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="border-left: 1px solid #000000;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_09
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_styling_data_10
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td style="border-top: 1px solid #000000;border-bottom: 1px solid #000000;border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">apricot</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td style="border-top: 1px solid #000000;border-bottom: 1px solid #000000;border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">coconut</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td style="border-top: 1px solid #000000;border-bottom: 1px solid #000000;border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">apricot</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td style="border-top: 1px solid #000000;border-bottom: 1px solid #000000;border-left: 1px solid #000000;border-right: 1px solid #000000;" class="gt_row gt_left">coconut</td>
+    </tr>
   </tbody>
   '''
 # ---
```

### Comparing `great-tables-0.5.0/tests/data_color/__snapshots__/test_data_color.ambr` & `great_tables-0.5.1/tests/data_color/__snapshots__/test_data_color.ambr`

 * *Files 11% similar despite different names*

```diff
@@ -1,588 +1,588 @@
 # serializer version: 1
 # name: test_all_missing_from_multiple_rows_pd
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">6</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">6</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_all_missing_from_multiple_rows_pl
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
-    <td class="gt_row gt_right">6</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
+      <td class="gt_row gt_right">6</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_all_values_have_zero_range_domain_pd
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2.0</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2.0</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #808080;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #808080;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">6</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2.0</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2.0</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #808080;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #808080;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">6</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_all_values_have_zero_range_domain_pl
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #808080;" class="gt_row gt_right">None</td>
-    <td class="gt_row gt_right">5</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #808080;" class="gt_row gt_right">None</td>
-    <td class="gt_row gt_right">6</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">2</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #808080;" class="gt_row gt_right">None</td>
+      <td class="gt_row gt_right">5</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #808080;" class="gt_row gt_right">None</td>
+      <td class="gt_row gt_right">6</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_autocolor_text_false[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="background-color: #5c5200;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="background-color: #077c00;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="background-color: #5c5200;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="background-color: #077c00;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_autocolor_text_false[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="background-color: #5c5200;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="background-color: #077c00;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="background-color: #5c5200;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="background-color: #077c00;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_colorbrewer_snap
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #f7fcf5;" class="gt_row gt_right">1</td>
-    <td style="color: #FFFFFF; background-color: #00441b;" class="gt_row gt_right">10</td>
-    <td class="gt_row gt_left">one</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #c7e9c0;" class="gt_row gt_right">2</td>
-    <td style="color: #000000; background-color: #238b45;" class="gt_row gt_right">9</td>
-    <td class="gt_row gt_left">two</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #74c476;" class="gt_row gt_right">3</td>
-    <td style="color: #000000; background-color: #74c476;" class="gt_row gt_right">8</td>
-    <td class="gt_row gt_left">three</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #238b45;" class="gt_row gt_right">4</td>
-    <td style="color: #000000; background-color: #c7e9c0;" class="gt_row gt_right">7</td>
-    <td class="gt_row gt_left">four</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #00441b;" class="gt_row gt_right">5</td>
-    <td style="color: #000000; background-color: #f7fcf5;" class="gt_row gt_right">6</td>
-    <td class="gt_row gt_left">five</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #f7fcf5;" class="gt_row gt_right">1</td>
+      <td style="color: #FFFFFF; background-color: #00441b;" class="gt_row gt_right">10</td>
+      <td class="gt_row gt_left">one</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #c7e9c0;" class="gt_row gt_right">2</td>
+      <td style="color: #000000; background-color: #238b45;" class="gt_row gt_right">9</td>
+      <td class="gt_row gt_left">two</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #74c476;" class="gt_row gt_right">3</td>
+      <td style="color: #000000; background-color: #74c476;" class="gt_row gt_right">8</td>
+      <td class="gt_row gt_left">three</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #238b45;" class="gt_row gt_right">4</td>
+      <td style="color: #000000; background-color: #c7e9c0;" class="gt_row gt_right">7</td>
+      <td class="gt_row gt_left">four</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #00441b;" class="gt_row gt_right">5</td>
+      <td style="color: #000000; background-color: #f7fcf5;" class="gt_row gt_right">6</td>
+      <td class="gt_row gt_left">five</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_domain_na_color_reverse_snap[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #5c5200;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #FFFFFF; background-color: #077c00;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #5c5200;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #FFFFFF; background-color: #077c00;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_domain_na_color_reverse_snap[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #5c5200;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #FFFFFF; background-color: #077c00;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #5c5200;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #FFFFFF; background-color: #077c00;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_domain_na_color_snap[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #a32e00;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #f80400;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #a32e00;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #f80400;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_domain_na_color_snap[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #a32e00;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #f80400;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #a32e00;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #f80400;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #0000FF;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_overlapping_domain[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #673498;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #673498;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_overlapping_domain[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #673498;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #673498;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_palette_snap[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #fe0100;" class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #ec0a00;" class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #fe0100;" class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #ec0a00;" class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_palette_snap[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #fe0100;" class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #ec0a00;" class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #fe0100;" class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #ec0a00;" class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #ff0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_simple_df_snap
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1</td>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">10</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">one</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_right">2</td>
-    <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_right">9</td>
-    <td style="color: #000000; background-color: #4cbd81;" class="gt_row gt_left">two</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">3</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">8</td>
-    <td style="color: #FFFFFF; background-color: #9653ca;" class="gt_row gt_left">three</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1</td>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">10</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">one</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_right">2</td>
+      <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_right">9</td>
+      <td style="color: #000000; background-color: #4cbd81;" class="gt_row gt_left">two</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">3</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">8</td>
+      <td style="color: #FFFFFF; background-color: #9653ca;" class="gt_row gt_left">three</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_simple_exibble_snap[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">0.1111</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">apricot</td>
-    <td style="color: #FFFFFF; background-color: #010001;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #070304;" class="gt_row gt_right">2.222</td>
-    <td style="color: #000000; background-color: #80b156;" class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #752b38;" class="gt_row gt_right">33.33</td>
-    <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_left">coconut</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">444.4</td>
-    <td style="color: #000000; background-color: #d73a91;" class="gt_row gt_left">durian</td>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">0.1111</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">apricot</td>
+      <td style="color: #FFFFFF; background-color: #010001;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #070304;" class="gt_row gt_right">2.222</td>
+      <td style="color: #000000; background-color: #80b156;" class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #752b38;" class="gt_row gt_right">33.33</td>
+      <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_left">coconut</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">444.4</td>
+      <td style="color: #000000; background-color: #d73a91;" class="gt_row gt_left">durian</td>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_simple_exibble_snap[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">0.1111</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">apricot</td>
-    <td style="color: #FFFFFF; background-color: #010001;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #070304;" class="gt_row gt_right">2.222</td>
-    <td style="color: #000000; background-color: #80b156;" class="gt_row gt_left">banana</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #752b38;" class="gt_row gt_right">33.33</td>
-    <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_left">coconut</td>
-    <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">444.4</td>
-    <td style="color: #000000; background-color: #d73a91;" class="gt_row gt_left">durian</td>
-    <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">0.1111</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_left">apricot</td>
+      <td style="color: #FFFFFF; background-color: #010001;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #070304;" class="gt_row gt_right">2.222</td>
+      <td style="color: #000000; background-color: #80b156;" class="gt_row gt_left">banana</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #752b38;" class="gt_row gt_right">33.33</td>
+      <td style="color: #000000; background-color: #25bce6;" class="gt_row gt_left">coconut</td>
+      <td style="color: #FFFFFF; background-color: #000000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">444.4</td>
+      <td style="color: #000000; background-color: #d73a91;" class="gt_row gt_left">durian</td>
+      <td style="color: #000000; background-color: #9e9e9e;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_subset_domain[pandas]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_subset_domain[polars]
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td class="gt_row gt_right">0.1111</td>
-    <td class="gt_row gt_left">apricot</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">2.222</td>
-    <td class="gt_row gt_left">banana</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">33.33</td>
-    <td class="gt_row gt_left">coconut</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
-  </tr>
-  <tr>
-    <td class="gt_row gt_right">444.4</td>
-    <td class="gt_row gt_left">durian</td>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">65100.0</td>
-  </tr>
+    <tr>
+      <td class="gt_row gt_right">0.1111</td>
+      <td class="gt_row gt_left">apricot</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">49.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">2.222</td>
+      <td class="gt_row gt_left">banana</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">17.95</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">33.33</td>
+      <td class="gt_row gt_left">coconut</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">1.39</td>
+    </tr>
+    <tr>
+      <td class="gt_row gt_right">444.4</td>
+      <td class="gt_row gt_left">durian</td>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">65100.0</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_data_color_viridis_snap
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #440154;" class="gt_row gt_right">1</td>
-    <td style="color: #000000; background-color: #fde725;" class="gt_row gt_right">10</td>
-    <td class="gt_row gt_left">one</td>
-  </tr>
-  <tr>
-    <td style="color: #FFFFFF; background-color: #3b518a;" class="gt_row gt_right">2</td>
-    <td style="color: #000000; background-color: #5fc861;" class="gt_row gt_right">9</td>
-    <td class="gt_row gt_left">two</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #22908c;" class="gt_row gt_right">3</td>
-    <td style="color: #000000; background-color: #22908c;" class="gt_row gt_right">8</td>
-    <td class="gt_row gt_left">three</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #5fc861;" class="gt_row gt_right">4</td>
-    <td style="color: #FFFFFF; background-color: #3b518a;" class="gt_row gt_right">7</td>
-    <td class="gt_row gt_left">four</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #fde725;" class="gt_row gt_right">5</td>
-    <td style="color: #FFFFFF; background-color: #440154;" class="gt_row gt_right">6</td>
-    <td class="gt_row gt_left">five</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #440154;" class="gt_row gt_right">1</td>
+      <td style="color: #000000; background-color: #fde725;" class="gt_row gt_right">10</td>
+      <td class="gt_row gt_left">one</td>
+    </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #3b518a;" class="gt_row gt_right">2</td>
+      <td style="color: #000000; background-color: #5fc861;" class="gt_row gt_right">9</td>
+      <td class="gt_row gt_left">two</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #22908c;" class="gt_row gt_right">3</td>
+      <td style="color: #000000; background-color: #22908c;" class="gt_row gt_right">8</td>
+      <td class="gt_row gt_left">three</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #5fc861;" class="gt_row gt_right">4</td>
+      <td style="color: #FFFFFF; background-color: #3b518a;" class="gt_row gt_right">7</td>
+      <td class="gt_row gt_left">four</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #fde725;" class="gt_row gt_right">5</td>
+      <td style="color: #FFFFFF; background-color: #440154;" class="gt_row gt_right">6</td>
+      <td class="gt_row gt_left">five</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_and_missing_pd
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_and_missing_pl
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_center">None</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_from_multiple_rows_pd
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1.0</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1.0</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right"><NA></td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_from_multiple_rows_pl
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
-  <tr>
-    <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">None</td>
-    <td class="gt_row gt_right">4</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
+    <tr>
+      <td style="color: #000000; background-color: #FF0000;" class="gt_row gt_right">None</td>
+      <td class="gt_row gt_right">4</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_pd
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
   </tbody>
   '''
 # ---
 # name: test_single_value_pl
   '''
   <tbody class="gt_table_body">
-  <tr>
-    <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
-    <td class="gt_row gt_right">3</td>
-  </tr>
+    <tr>
+      <td style="color: #FFFFFF; background-color: #008000;" class="gt_row gt_right">1</td>
+      <td class="gt_row gt_right">3</td>
+    </tr>
   </tbody>
   '''
 # ---
```

### Comparing `great-tables-0.5.0/tests/data_color/test_data_color.py` & `great_tables-0.5.1/tests/data_color/test_data_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from great_tables import GT, style
-from great_tables.data import exibble
-from great_tables._utils_render_html import create_body_component_h
-from great_tables._gt_data import StyleInfo, CellStyle
 from typing import Type, TypeVar
 
 import numpy as np
 import pandas as pd
 import polars as pl
 import pytest
+from great_tables import GT, style
+from great_tables._gt_data import CellStyle, StyleInfo
 from great_tables._tbl_data import DataFrameLike
-
+from great_tables._utils_render_html import create_body_component_h
+from great_tables.data import exibble
 
 T_CellStyle = TypeVar("T_CellStyle", bound=CellStyle)
 
 params_frames = [pytest.param(pd.DataFrame, id="pandas"), pytest.param(pl.DataFrame, id="polars")]
 
 
 @pytest.fixture(params=params_frames, scope="function")
```

### Comparing `great-tables-0.5.0/tests/data_color/test_data_color_utils.py` & `great_tables-0.5.1/tests/data_color/test_data_color_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import math
-import pandas as pd
+
 import numpy as np
+import pandas as pd
 import pytest
 from great_tables._data_color.base import (
-    _ideal_fgnd_color,
+    _add_alpha,
+    _color_name_to_hex,
+    _expand_short_hex,
+    _float_to_hex,
+    _get_domain_factor,
+    _get_domain_numeric,
     _get_wcag_contrast_ratio,
     _hex_to_rgb,
-    _relative_luminance,
-    _srgb,
     _html_color,
-    _add_alpha,
-    _remove_alpha,
-    _float_to_hex,
-    _color_name_to_hex,
-    _is_short_hex,
+    _ideal_fgnd_color,
     _is_hex_col,
+    _is_short_hex,
     _is_standard_hex_col,
-    _expand_short_hex,
+    _relative_luminance,
+    _remove_alpha,
     _rescale_numeric,
-    _get_domain_numeric,
-    _get_domain_factor,
+    _srgb,
 )
 from great_tables._data_color.palettes import GradientPalette
 
 
 def test_ideal_fgnd_color_dark_contrast():
     bgnd_color = "#FFFFFF"  # White background color
     fgnd_color = _ideal_fgnd_color(bgnd_color)
@@ -591,14 +592,19 @@
 
     # len(color) != len(values)
     with pytest.raises(ValueError) as exc_info:
         GradientPalette(["red", "blue"], values=[0, 1.1, 1])
 
     assert "Received 3 values and 2 colors" in exc_info.value.args[0]
 
+    with pytest.raises(NotImplementedError) as exc_info:
+        GradientPalette([(255, 0, 0), (0, 255, 0)])
+
+    assert "Currently, rgb tuples can't be passed directly." in exc_info.value.args[0]
+
 
 def test_gradient_n_pal_out_of_bounds_raises():
     palette = GradientPalette(["red", "blue"])
 
     with pytest.raises(ValueError) as exc_info:
         palette([0, 1.1])
```

### Comparing `great-tables-0.5.0/tests/test__stubhead.py` & `great_tables-0.5.1/tests/test__stubhead.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/tests/test__utils_nanoplots.py` & `great_tables-0.5.1/tests/test__utils_nanoplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-import pytest
 import numpy as np
+import pytest
+
+
+from typing import Any, Union
+from decimal import Decimal
 from great_tables._utils_nanoplots import (
-    _val_is_numeric,
-    _val_is_str,
-    _is_integerlike,
-    _normalize_option_list,
-    _normalize_vals,
-    _normalize_to_dict,
-    calc_ref_value,
+    _flatten_list,
     _format_number_compactly,
-    _gt_mean,
-    _gt_min,
-    _gt_max,
-    _gt_median,
+    _generate_nanoplot,
+    _generate_ref_line_from_keyword,
+    _get_extreme_value,
+    _get_n_intlike,
     _gt_first,
     _gt_last,
-    _gt_quantile,
+    _gt_max,
+    _gt_mean,
+    _gt_median,
+    _gt_min,
     _gt_q1,
     _gt_q3,
-    _flatten_list,
-    _get_extreme_value,
-    _generate_ref_line_from_keyword,
-    _generate_nanoplot,
+    _gt_quantile,
+    _is_integerlike,
+    _is_intlike,
+    _normalize_option_list,
+    _normalize_to_dict,
+    _normalize_vals,
+    _remove_exponent,
+    _val_is_numeric,
+    _val_is_str,
+    calc_ref_value,
 )
-from typing import List, Union, Any
 
-Y_VALS: "list[int | float]" = [-5.3, 6.3, -2.3, 0, 2.3, 6.7, 14.2, 0, 2.3, 13.3]
-X_VALS = [1.2, 3.4, 4.2, 5.0, 5.8, 6.7, 8.3, 10.2, 10.9, 12.2]
+Y_VALS: list[Union[int, float]] = [-5.3, 6.3, -2.3, 0, 2.3, 6.7, 14.2, 0, 2.3, 13.3]
+X_VALS: list[Union[int, float]] = [1.2, 3.4, 4.2, 5.0, 5.8, 6.7, 8.3, 10.2, 10.9, 12.2]
 
-CASES: "list[dict[str, Any]]" = [
+CASES: list[dict[str, Any]] = [
     dict(y_vals=Y_VALS),
     dict(y_vals=Y_VALS, y_ref_line=0),
     dict(y_vals=Y_VALS, y_ref_line="mean"),
     dict(y_vals=Y_VALS, y_ref_area=[0.1, 5.3]),
     # could test that its output is equiv to above
     dict(y_vals=Y_VALS, y_ref_area=[5.3, 0.1]),
     dict(y_vals=Y_VALS, y_ref_area=["min", "median"]),
@@ -163,15 +169,15 @@
                 1.0,
             ],
         ),
         ([-5.3, -2.3, -23.2, 0], [0.771551724137931, 0.9008620689655172, 0.0, 1.0]),
     ],
 )
 def test_normalize_vals(
-    vals: Union[List[Union[int, float]], List[int], List[float]], dst: List[Union[int, float]]
+    vals: Union[list[Union[int, float]], list[int], list[float]], dst: list[Union[int, float]]
 ):
     res = _normalize_vals(vals)
     assert res == dst
 
 
 def test_normalize_to_dict():
     # Test case 1: Normalization with no missing values
@@ -347,45 +353,45 @@
         ([1], 1.0),
         ([1, 1], 1.0),
         ([1, 2, 3], 2.0),
         ([-5, 0.1, 5], 0.033333333333333215),
         ([2.1e15, 2342, 5.3e8], 700000176667447.4),
     ],
 )
-def test_gt_mean(num: List[Union[int, float]], dst: float):
+def test_gt_mean(num: list[Union[int, float]], dst: float):
     res = _gt_mean(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
         ([1], 1.0),
         ([1, 1], 1.0),
         ([1, 2, 3], 1.0),
         ([-5, 0.1, 5], -5.0),
         ([2.1e15, 2342, 5.3e8], 2342),
     ],
 )
-def test_gt_min(num: List[Union[int, float]], dst: float):
+def test_gt_min(num: list[Union[int, float]], dst: float):
     res = _gt_min(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
         ([1], 1.0),
         ([1, 1], 1.0),
         ([1, 2, 3], 3.0),
         ([-5, 0.1, 5], 5.0),
         ([2.1e15, 2342, 5.3e8], 2100000000000000.0),
     ],
 )
-def test_gt_max(num: List[Union[int, float]], dst: float):
+def test_gt_max(num: list[Union[int, float]], dst: float):
     res = _gt_max(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
@@ -393,15 +399,15 @@
         ([1, 1], 1.0),
         ([1, 2, 3], 2.0),
         ([1, 2, 3, 4], 2.5),
         ([-5, 0.1, 5], 0.1),
         ([2.1e15, 2342, 5.3e8], 5.3e8),
     ],
 )
-def test_gt_median(num: List[Union[int, float]], dst: float):
+def test_gt_median(num: list[Union[int, float]], dst: float):
     res = _gt_median(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
@@ -409,15 +415,15 @@
         ([1, 1], 1.0),
         ([3, 2, 1], 3.0),
         ([1, 2, 3, 4], 1.0),
         ([-5, 0.1, 5], -5.0),
         ([0, 2.1e15, 2342, 5.3e8, 0, -2343], 0),
     ],
 )
-def test_gt_first(num: List[Union[int, float]], dst: float):
+def test_gt_first(num: list[Union[int, float]], dst: float):
     res = _gt_first(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
@@ -425,15 +431,15 @@
         ([1, 1], 1.0),
         ([3, 2, 1], 1.0),
         ([1, 2, 3, 4], 4.0),
         ([-5, 0.1, 5], 5.0),
         ([0, 2.1e15, 2342, 5.3e8, 0, -2343], -2343.0),
     ],
 )
-def test_gt_last(num: List[Union[int, float]], dst: float):
+def test_gt_last(num: list[Union[int, float]], dst: float):
     res = _gt_last(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,q,dst",
     [
@@ -465,15 +471,15 @@
         ([1, 3, 3, 3, 5], 0.6, 3.0),
         ([1, 3, 3, 3, 5], 0.7, 3.0),
         ([1, 3, 3, 3, 5], 0.8, 5.0),
         ([1, 3, 3, 3, 5], 0.9, 5.0),
         # ([1, 3, 3, 3, 5], 1.0, 5.0), # TODO: causes 'IndexError: list index out of range'
     ],
 )
-def test_gt_quantile(num: List[Union[int, float]], q: float, dst: float):
+def test_gt_quantile(num: list[Union[int, float]], q: float, dst: float):
     res = _gt_quantile(num, q=q)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
@@ -485,15 +491,15 @@
         ([1, 2, 2, 3, 3, 3, 4, 4], 2.0),
         ([0.01, 0.5, 0.25, 1, 2, 2, 3, 3, 3, 4, 4], 0.5),
         ([-5, 0.1, 5], -5.0),
         ([1, 1, 1, 0.5, 1.2], 1.0),
         ([0, 2.1e15, 2342, 5.3e8, 0, -2343], 0.0),
     ],
 )
-def test_gt_q_1(num: List[Union[int, float]], dst: float):
+def test_gt_q_1(num: list[Union[int, float]], dst: float):
     res = _gt_q1(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,dst",
     [
@@ -505,15 +511,15 @@
         ([1, 2, 2, 3, 3, 3, 4, 4], 4.0),
         ([0.01, 0.5, 0.25, 1, 2, 2, 3, 3, 3, 4, 4], 3.0),
         ([-5, 0.1, 5], 5.0),
         ([1, 1, 1, 0.5, 1.2], 1.0),
         ([0, 2.1e15, 2342, 5.3e8, 0, -2343], 5.3e8),
     ],
 )
-def test_gt_q_3(num: List[Union[int, float]], dst: float):
+def test_gt_q_3(num: list[Union[int, float]], dst: float):
     res = _gt_q3(num)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "lst,dst",
     [
@@ -523,15 +529,15 @@
         ([3, 2.2, None, [None]], [3, 2.2, None, None]),
         ([1, 2, 3, [22, -3.4], 4], [1, 2, 3, 22, -3.4, 4]),
         ([1, 2.2, [9.2], 2.2, 3, 4, []], [1, 2.2, 9.2, 2.2, 3, 4]),
         ([[], 1.2, [], [], 2.2, [9.2], 2.2, [3, 4], []], [1.2, 2.2, 9.2, 2.2, 3, 4]),
         ([], []),
     ],
 )
-def test_flatten_list(lst: List[Any], dst: List[Any]):
+def test_flatten_list(lst: list[Any], dst: list[Any]):
     res = _flatten_list(lst)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "lst,stat,dst",
     [
@@ -547,15 +553,15 @@
         ([[1], [3, 2, 3], [None], None, 0.5, 9.2], "max", 9.2),
         ([[3, 2.2, 1], [3, 2.2, 1]], "min", 1),
         ([[3, 2.2, 1], [3, 2.2, 1]], "max", 3),
         ([[-13.2, 2.2, None, 14.3], [None, None]], "min", -13.2),
         ([[-13.2, 2.2, None, 14.3], [None, None]], "max", 14.3),
     ],
 )
-def test_get_extreme_value(lst: List[Any], stat: str, dst: List[Any]):
+def test_get_extreme_value(lst: list[Any], stat: str, dst: list[Any]):
     res = _get_extreme_value(*lst, stat=stat)
     assert res == dst
 
 
 @pytest.mark.parametrize(
     "num,keyword,dst",
     [
@@ -587,30 +593,30 @@
         ([-13.2, 2.2, 14.3, 2.3, 25.3, -3.1, 0, 3.93, 6.23, 0.92, -3.2], "q3", 6.23),
         # TODO: errors below due to restrictive keyword check
         # ([-13.2, 2.2, 14.3, 2.3, 25.3, -3.1, 0, 3.93, 6.23, 0.92, -3.2], "first", -13.2),
         # ([-13.2, 2.2, 14.3, 2.3, 25.3, -3.1, 0, 3.93, 6.23, 0.92, -3.2], "last", -3.2),
     ],
 )
 def test_generate_ref_line_from_keyword(
-    num: List[Union[int, float]], keyword: str, dst: Union[int, float]
+    num: list[Union[int, float]], keyword: str, dst: Union[int, float]
 ):
     res = _generate_ref_line_from_keyword(num, keyword=keyword)
     assert res == dst
 
 
 def _is_nanoplot_output(nanoplot_str: str):
     import re
 
     return bool(re.match("^<div><svg.*</svg></div>$", nanoplot_str))
 
 
-def _nanoplot_has_tag_attrs(nanoplot_str: str, tag: str, attrs: List[tuple[str, str]]) -> bool:
+def _nanoplot_has_tag_attrs(nanoplot_str: str, tag: str, attrs: list[tuple[str, str]]) -> bool:
     import re
 
-    found: List[bool] = []
+    found: list[bool] = []
 
     for i, _ in enumerate(attrs):
         attrs_i = attrs[i]
         attr_str = f'{attrs_i[0]}="{attrs_i[1]}"'
 
         found_i = bool(re.search(f"<{tag}.*?{attr_str}.*?</{tag}>", nanoplot_str))
 
@@ -1997,7 +2003,62 @@
         _generate_nanoplot(y_vals=[5.3, 6.3, 7.2], x_vals=[1, 2.5])
 
 
 @pytest.mark.xfail
 def test_nanoplot_unknown_plot_type():
     with pytest.raises(ValueError):
         _generate_nanoplot(y_vals=[1, 2, 3], plot_type="unknown")
+
+
+@pytest.mark.parametrize(
+    "n, bool_",
+    [
+        (0, True),
+        (0.0, True),
+        (1, True),
+        (1.0, True),
+        (-12, True),
+        (-12.0, True),
+        ("-12", True),
+        ("−12", True),  # not regular `-`
+        (Decimal("1"), True),
+        (Decimal("1.0"), True),
+        (2.151515, False),
+        (-12.49849, False),
+        ("-12.49849", False),
+        ("−12.49849", False),  # not regular `-`
+        (Decimal("2.151515"), False),
+        ("abc", False),
+        (["abc"], False),
+        (tuple("abc"), False),
+        (set("abc"), False),
+        (dict.fromkeys("abc", object), False),
+    ],
+)
+def test_is_intlike(n: Any, bool_: bool):
+    assert _is_intlike(n) is bool_
+
+
+@pytest.mark.parametrize(
+    "nums, n",
+    [
+        (["1.0", 2.0, 3.00, Decimal(4), "-5.0"], 5),
+        (["1.1", 2.2, 3.03, "abc", "−12.49849"], 0),  # not regular `-`
+    ],
+)
+def test_get_n_intlike(nums: list[Any], n: int):
+    assert _get_n_intlike(nums) == n
+
+
+@pytest.mark.parametrize(
+    "n, result",
+    [
+        ("1.0", 1),
+        (2.0, 2),
+        (3.00, 3),
+        (Decimal(4), 4),
+        ("-5.0", -5),
+        ("−5.0", -5),  # not regular `-`
+    ],
+)
+def test_remove_exponent(n: "int | float | str", result: int):
+    assert _remove_exponent(n) == result
```

### Comparing `great-tables-0.5.0/tests/test_export.py` & `great_tables-0.5.1/tests/test_export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import pytest
-from great_tables import GT, md, exibble
 import time
 from pathlib import Path
 
+import pytest
+from great_tables import GT, exibble, md
+
 
 @pytest.fixture
 def gt_tbl():
     gt_tbl = (
         GT(
             exibble[["num", "char", "currency", "row", "group"]],
             rowname_col="row",
```

### Comparing `great-tables-0.5.0/tests/test_formats.py` & `great_tables-0.5.1/tests/test_formats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-from typing import Union
+import re
+from typing import Any, Union
+
 import pandas as pd
 import polars as pl
 import pytest
-import re
-
-from great_tables import GT
-from great_tables.data import exibble
-from great_tables.gt import _get_column_of_values
+from great_tables import GT, _locale
 from great_tables._data_color.base import _html_color
-from great_tables._utils_render_html import create_body_component_h
 from great_tables._formats import (
-    _format_number_fixed_decimals,
-    _expand_exponential_to_full_string,
-    fmt,
     FmtImage,
-    DateStyle,
-    TimeStyle,
-    _normalize_locale,
-    _get_locale_sep_mark,
-    _get_locale_dec_mark,
-    _get_locale_currency_code,
+    _expand_exponential_to_full_string,
+    _format_number_fixed_decimals,
     _get_currency_str,
+    _get_locale_currency_code,
+    _get_locale_dec_mark,
+    _get_locale_sep_mark,
+    _normalize_locale,
     _validate_locale,
+    fmt,
 )
-from great_tables._locations import RowSelectExpr
-from great_tables import _locale
-
-from typing import List, Dict, Any, Tuple, Union
+from great_tables._utils_render_html import create_body_component_h
+from great_tables.data import exibble
+from great_tables.gt import _get_column_of_values
 
 
 def assert_rendered_body(snapshot, gt):
     built = gt._build_data("html")
     body = create_body_component_h(built)
 
     assert snapshot == body
@@ -1069,15 +1063,15 @@
     assert x == ["12.345.678,12346", "1,00000", "0,00000", "\u2212" + "12.345.678,12346"]
 
 
 # ------------------------------------------------------------------------------
 # Tests of `fmt_currency()`
 # ------------------------------------------------------------------------------
 
-FMT_CURRENCY_CASES: List[Tuple[dict[str, Any], List[str]]] = [
+FMT_CURRENCY_CASES: list[tuple[dict[str, Any], list[str]]] = [
     (dict(), ["$1,234,567.00", "−$5,432.37"]),
     (dict(currency="USD"), ["$1,234,567.00", "−$5,432.37"]),
     (dict(currency="EUR"), ["&#8364;1,234,567.00", "−&#8364;5,432.37"]),
     (dict(use_subunits=False), ["$1,234,567", "−$5,432"]),
     (dict(use_subunits=False, decimals=4), ["$1,234,567.0000", "−$5,432.3700"]),
     (dict(decimals=4), ["$1,234,567.0000", "−$5,432.3700"]),
     (
@@ -1088,15 +1082,15 @@
     (dict(placement="right"), ["1,234,567.00$", "−5,432.37$"]),
     (dict(placement="right", incl_space=True), ["1,234,567.00 $", "−5,432.37 $"]),
     (dict(incl_space=True), ["$ 1,234,567.00", "−$ 5,432.37"]),
 ]
 
 
 @pytest.mark.parametrize("fmt_currency_kwargs,x_out", FMT_CURRENCY_CASES)
-def test_fmt_currency_case(fmt_currency_kwargs: dict[str, Any], x_out: List[str]):
+def test_fmt_currency_case(fmt_currency_kwargs: dict[str, Any], x_out: list[str]):
     df = pd.DataFrame({"x": [1234567, -5432.37]})
     gt = GT(df).fmt_currency(columns="x", **fmt_currency_kwargs)
     x = _get_column_of_values(gt, column_name="x", context="html")
     assert x == x_out
 
 
 def test_fmt_currency_force_sign():
@@ -1154,39 +1148,98 @@
 
     gt = GT(df_fmt_time).fmt_time(columns="x", time_style="h_p")
     x = _get_column_of_values(gt, column_name="x", context="html")
     assert x == ["10 AM", "1 PM", "11 PM"]
 
 
 # ------------------------------------------------------------------------------
+# Test `fmt_date()`
+# ------------------------------------------------------------------------------
+
+
+def test_fmt_date():
+
+    df = pd.DataFrame(
+        {
+            "x": [
+                "2020-05-20",
+                "2020-05-20 22:30",
+                "2020-05-20T22:30",
+                "2020-05-20 22:30:05",
+                "2020-05-20 22:30:05.824",
+            ]
+        }
+    )
+
+    gt = GT(df).fmt_date(columns="x", date_style="wd_m_day_year")
+    x = _get_column_of_values(gt, column_name="x", context="html")
+    assert x == [
+        "Wed, May 20, 2020",
+        "Wed, May 20, 2020",
+        "Wed, May 20, 2020",
+        "Wed, May 20, 2020",
+        "Wed, May 20, 2020",
+    ]
+
+
+# ------------------------------------------------------------------------------
 # Test `fmt_datetime()`
 # ------------------------------------------------------------------------------
 
 
 def test_fmt_datetime():
 
     df = pd.DataFrame(
         {
             "x": [
                 "2023-01-05 00:00:00",
                 "2013-05-15 23:15",
+                "2020-05-20",
+                "2020-05-20 22:30",
+                "2020-05-20T22:30",
+                "2020-05-20 22:30:05",
+                "2020-05-20T22:30:05.232",
             ]
         }
     )
 
     gt = GT(df).fmt_datetime(
         columns="x", date_style="wday_month_day_year", time_style="h_m_s_p", sep=" at "
     )
     x = _get_column_of_values(gt, column_name="x", context="html")
     assert x == [
         "Thursday, January 5, 2023 at 12:00:00 AM",
         "Wednesday, May 15, 2013 at 11:15:00 PM",
+        "Wednesday, May 20, 2020 at 12:00:00 AM",
+        "Wednesday, May 20, 2020 at 10:30:00 PM",
+        "Wednesday, May 20, 2020 at 10:30:00 PM",
+        "Wednesday, May 20, 2020 at 10:30:05 PM",
+        "Wednesday, May 20, 2020 at 10:30:05 PM",
     ]
 
 
+def test_fmt_datetime_bad_date_style_raises():
+
+    df = pd.DataFrame(
+        {
+            "x": [
+                "2023-01-05 00:00:00",
+                "2013-05-15 23:15",
+            ]
+        }
+    )
+
+    with pytest.raises(ValueError) as exc_info:
+        gt = GT(df).fmt_datetime(
+            columns="x", date_style="quarter_month_day_year", time_style="h_m_s_p", sep=" at "
+        )
+
+    assert "date_style must be one of:" in exc_info.value.args[0]
+
+
 # ------------------------------------------------------------------------------
 # Test `fmt_bytes()`
 # ------------------------------------------------------------------------------
 @pytest.mark.parametrize(
     "src,dst",
     [
         (-3, "−3 B"),
@@ -1215,15 +1268,15 @@
         (
             dict(standard="binary", use_seps=False, force_sign=True, incl_space=False),
             [902487216348759693489128343269],
             ["+746519.9YiB"],
         ),
     ],
 )
-def test_fmt_bytes_case(fmt_bytes_kwargs: dict[str, Any], x_in: List[float], x_out: List[str]):
+def test_fmt_bytes_case(fmt_bytes_kwargs: dict[str, Any], x_in: list[float], x_out: list[str]):
     df = pd.DataFrame({"x": x_in})
     gt = GT(df).fmt_bytes(columns="x", **fmt_bytes_kwargs)
     x = _get_column_of_values(gt, column_name="x", context="html")
     assert x == x_out
 
 
 # ------------------------------------------------------------------------------
@@ -1244,14 +1297,21 @@
 def test_fmt_roman_lower():
 
     gt = GT(df_fmt_roman).fmt_roman(columns="x", case="lower")
     x = _get_column_of_values(gt, column_name="x", context="html")
     assert x == ["mccxxxiv", "n", "n", "i", "i", "xcix", "ex terminis"]
 
 
+def test_fmt_roman_bad_case_raises():
+    with pytest.raises(ValueError) as exc_info:
+        gt = GT(df_fmt_roman).fmt_roman(columns="x", case="case")
+
+    assert "The `case` argument must be either 'upper' or 'lower'" in exc_info.value.args[0]
+
+
 # ------------------------------------------------------------------------------
 # Test `fmt_markdown()`
 # ------------------------------------------------------------------------------
 
 
 def test_fmt_markdown():
     df = pd.DataFrame(
@@ -1399,18 +1459,18 @@
 
 
 # ------------------------------------------------------------------------------
 # Test `fmt_nanoplot()`
 # ------------------------------------------------------------------------------
 
 
-def _nanoplot_has_tag_attrs(nanoplot_str: str, tag: str, attrs: List[tuple[str, str]]) -> bool:
+def _nanoplot_has_tag_attrs(nanoplot_str: str, tag: str, attrs: list[tuple[str, str]]) -> bool:
     import re
 
-    found: List[bool] = []
+    found: list[bool] = []
 
     for i, _ in enumerate(attrs):
         attrs_i = attrs[i]
         attr_str = f'{attrs_i[0]}="{attrs_i[1]}"'
 
         found_i = bool(re.search(f"<{tag}.*?{attr_str}.*?</{tag}>", nanoplot_str))
 
@@ -1427,15 +1487,15 @@
             {"x": [-12.0, -5.0, 6.0, 3.0, 0.0, 8.0, -7.0]},
             {"x": [2, 0, 15, 7, 8, 10, 1, 24, 17, 13, 6]},
         ],
     }
 )
 
 
-FMT_NANOPLOT_CASES: List[dict[str, Any]] = [
+FMT_NANOPLOT_CASES: list[dict[str, Any]] = [
     # 1. default case
     dict(),
     # 2. reference line with 0 value
     dict(reference_line=0),
     # 3. reference line using a string
     dict(reference_line="mean"),
     # 4. use of a reference area
```

### Comparing `great-tables-0.5.0/tests/test_formats_nanoplots.py` & `great_tables-0.5.1/tests/test_formats_nanoplots.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import pytest
+from typing import Any
 
-from typing import Any, List
+import pytest
 from great_tables._formats import _generate_data_vals, _process_number_stream
 
 
 @pytest.mark.parametrize(
     "src", ["1 2 3", "1  2, 3", "a1 b2 c3", [1, 2, 3], {"x": [1, 2, 3]}, {"any_name": [1, 2, 3]}]
 )
 def test_generate_data_vals(src: Any):
@@ -57,10 +57,10 @@
         ("1,   2,3, 4.5", [1, 2, 3, 4.5]),
         ("1.1; 2;3;   4.5", [1.1, 2, 3, 4.5]),
         (" 1.1, 2 3;   4.5 5 ", [1.1, 2, 3, 4.5, 5]),
         (" 1.342e12, 2.e-2 3,  4.55634 -5.23 ", [1.342e12, 2.0e-2, 3, 4.55634, -5.23]),
         (" +1.342e12, +2.E-2 +3,  4.55634 -5.23 ", [1.342e12, 2.0e-2, 3, 4.55634, -5.23]),
     ],
 )
-def test_process_number_stream(src: str, dst: List[float]):
+def test_process_number_stream(src: str, dst: list[float]):
     res = _process_number_stream(data_vals=src)
     assert res == dst
```

### Comparing `great-tables-0.5.0/tests/test_gt.py` & `great_tables-0.5.1/tests/test_gt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import pandas as pd
 import pytest
-
 from great_tables import GT
-from great_tables._gt_data import RowGroups
-import pandas as pd
+
 
 # Generate a gt Table object for assertion testing
 data = [{"a": 5, "b": 15}, {"a": 15, "b": 2000}]
 pd_data = pd.DataFrame(data)
 
 
 @pytest.fixture
```

### Comparing `great-tables-0.5.0/tests/test_gt_data.py` & `great_tables-0.5.1/tests/test_gt_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pandas as pd
-
-from great_tables._gt_data import Stub, RowInfo, Boxhead, ColInfo
-from great_tables._gt_data import RowGroups
+from great_tables._gt_data import Boxhead, ColInfo, RowInfo, Stub
 
 
 def test_stub_construct_manual():
     stub = Stub([RowInfo(0), RowInfo(1)])
     assert stub[0] == RowInfo(0)
```

### Comparing `great-tables-0.5.0/tests/test_locations.py` & `great_tables-0.5.1/tests/test_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import pandas as pd
 import polars as pl
 import pytest
-
+from great_tables import GT
+from great_tables._gt_data import Spanners
 from great_tables._locations import (
-    LocColumnSpanners,
+    CellPos,
     LocBody,
+    LocColumnSpanners,
     LocTitle,
-    CellPos,
     resolve,
-    resolve_vector_i,
     resolve_cols_i,
     resolve_rows_i,
+    resolve_vector_i,
     set_style,
 )
 from great_tables._styles import CellStyleText, FromColumn
-from great_tables._gt_data import Spanners, SpannerInfo
-from great_tables import GT
 
 
 def test_resolve_vector_i():
     assert resolve_vector_i(["x", "a"], ["a", "b", "x"], "") == [0, 2]
 
 
 def test_resolve_cols_i_gt_data():
```

### Comparing `great-tables-0.5.0/tests/test_options.py` & `great_tables-0.5.1/tests/test_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import pytest
-from great_tables import GT, md, exibble
+from great_tables import GT, exibble, md
 from great_tables._scss import compile_scss
 
 
 def test_options_overwrite():
     df = pd.DataFrame({"x": [1, 2, 3]})
     gt = GT(df)
```

### Comparing `great-tables-0.5.0/tests/test_repr.py` & `great_tables-0.5.1/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `great-tables-0.5.0/tests/test_scss.py` & `great_tables-0.5.1/tests/test_scss.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,26 @@
 )
 def test_font_color(src, dst):
     res = font_color(src, "#000000", "#FFFFFF")
     assert res == dst
 
 
 @pytest.mark.parametrize(
+    "src, dst",
+    [
+        ("transparent", "#000000"),
+        ("currentColor", "currentcolor"),
+        ("black", "#FFFFFF"),
+    ],
+)
+def test_font_color_normalizes_table_color_names(src, dst):
+    assert font_color(src, "black", "white") == dst
+
+
+@pytest.mark.parametrize(
     "src,dst",
     [
         ("1px", "2px"),
         ("1%", "2%"),
         (1, 2),
     ],
 )
```

### Comparing `great-tables-0.5.0/tests/test_styles.py` & `great_tables-0.5.1/tests/test_styles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import polars as pl
-
-from great_tables._styles import FromColumn, CellStyleText
+from great_tables._styles import CellStyleText, FromColumn
 
 
 def test_from_column_replace():
     """FromColumn is replaced by the specified column's value in a row of data"""
 
     df = pd.DataFrame({"x": [1, 2], "color": ["red", "blue"]})
     from_col = FromColumn("color")
```

### Comparing `great-tables-0.5.0/tests/test_substitutions.py` & `great_tables-0.5.1/tests/test_substitutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from math import nan
+
+import numpy as np
 import pandas as pd
 import polars as pl
 import polars.testing
-import numpy as np
 import pytest
-
 from great_tables import GT
-from great_tables._tbl_data import DataFrameLike, _get_cell, to_list
-from great_tables._substitution import SubMissing, SubZero
 from great_tables._gt_data import FormatterSkipElement
-from math import nan
+from great_tables._substitution import SubMissing, SubZero
+from great_tables._tbl_data import DataFrameLike, to_list
 
 params_frames = [pytest.param(pd.DataFrame, id="pandas"), pytest.param(pl.DataFrame, id="polars")]
 
 
 @pytest.fixture(params=params_frames, scope="function")
 def df(request) -> DataFrameLike:
     return request.param({"col1": [None, nan, 0]})
```

### Comparing `great-tables-0.5.0/tests/test_tab_create_modify.py` & `great_tables-0.5.1/tests/test_tab_create_modify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import pytest
 import pandas as pd
-
-from great_tables._tab_create_modify import tab_style
+import pytest
 from great_tables import GT
-from great_tables._styles import CellStyleFill
 from great_tables._locations import LocBody
+from great_tables._styles import CellStyleFill
+from great_tables._tab_create_modify import tab_style
 
 
 @pytest.fixture
 def gt():
     return GT(pd.DataFrame({"x": [1, 2], "y": [4, 5]}))
```

### Comparing `great-tables-0.5.0/tests/test_tbl_data.py` & `great_tables-0.5.1/tests/test_tbl_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import pandas as pd
 import polars as pl
 import polars.testing
 import pytest
-
 from great_tables._tbl_data import (
+    DataFrameLike,
+    SeriesLike,
     _get_cell,
     _get_column_dtype,
     _set_cell,
+    create_empty_frame,
+    eval_select,
     get_column_names,
-    DataFrameLike,
-    SeriesLike,
     reorder,
-    eval_select,
-    create_empty_frame,
-    validate_frame,
     to_frame,
-    to_list,
+    validate_frame,
 )
 
-
 params_frames = [pytest.param(pd.DataFrame, id="pandas"), pytest.param(pl.DataFrame, id="polars")]
 params_series = [pytest.param(pd.Series, id="pandas"), pytest.param(pl.Series, id="polars")]
 
 
 @pytest.fixture(params=params_frames, scope="function")
 def df(request) -> pd.DataFrame:
     return request.param({"col1": [1, 2, 3], "col2": ["a", "b", "c"], "col3": [4.0, 5.0, 6.0]})
```

### Comparing `great-tables-0.5.0/tests/test_utils_render_common.py` & `great_tables-0.5.1/tests/test_utils_render_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from great_tables._gt_data import RowGroups, Stub, RowInfo
-from great_tables.utils_render_common import get_row_reorder_df
 import pytest
+from great_tables._gt_data import RowInfo, Stub
+from great_tables.utils_render_common import get_row_reorder_df
 
 
 def test_get_row_reorder_df_simple():
     groups = ["b", "a"]
     stub = Stub([RowInfo(0, "a"), RowInfo(1, "b"), RowInfo(2, "a")])
 
     start_end = get_row_reorder_df(groups, stub)
```

### Comparing `great-tables-0.5.0/tests/test_utils_render_html.py` & `great_tables-0.5.1/tests/test_utils_render_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pandas as pd
-import pytest
-
-from great_tables import GT, exibble, md, html, style, loc
-from great_tables._utils_render_html import create_source_notes_component_h, create_body_component_h
+from great_tables import GT, exibble, html, loc, md, style
+from great_tables._utils_render_html import create_body_component_h, create_source_notes_component_h
 
 small_exibble = exibble[["num", "char"]].head(3)
 
 
 def assert_rendered_source_notes(snapshot, gt):
     built = gt._build_data("html")
     source_notes = create_source_notes_component_h(built)
```

