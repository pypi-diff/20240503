# Comparing `tmp/json-schema-for-humans-0.9.1.tar.gz` & `tmp/json_schema_for_humans-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-schema-for-humans-0.9.1.tar", last modified: Sat May 16 17:08:58 2020, max compression
+gzip compressed data, was "json_schema_for_humans-1.0.0.tar", max compression
```

## Comparing `json-schema-for-humans-0.9.1.tar` & `json_schema_for_humans-1.0.0.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      469 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (116)      319 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)      563 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/Gemfile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_data/examples.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_includes/
--rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/array.json
--rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/array_advanced.json
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/basic.json
--rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/combining_not.json
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/combining_oneOf.json
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/geo.json
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/multiple_types.json
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/pattern_properties.json
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/references.json
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_default.json
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_definitions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_descriptions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_examples.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/assets/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     4387 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/array.html
--rw-r--r--   0 runner    (1001) docker     (116)     3063 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/array_advanced.html
--rw-r--r--   0 runner    (1001) docker     (116)     3062 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/basic.html
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/combining_not.html
--rw-r--r--   0 runner    (1001) docker     (116)     3562 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/combining_oneOf.html
--rw-r--r--   0 runner    (1001) docker     (116)     3214 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/deprecated.html
--rw-r--r--   0 runner    (1001) docker     (116)     2746 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/geo.html
--rw-r--r--   0 runner    (1001) docker     (116)     3636 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/multiple_types.html
--rw-r--r--   0 runner    (1001) docker     (116)     4602 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/pattern_properties.html
--rw-r--r--   0 runner    (1001) docker     (116)    15495 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/references.html
--rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.css
--rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     4097 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_default.html
--rw-r--r--   0 runner    (1001) docker     (116)     7091 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_definitions.html
--rw-r--r--   0 runner    (1001) docker     (116)    10657 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_descriptions.html
--rw-r--r--   0 runner    (1001) docker     (116)     5425 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_examples.html
--rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)      694 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16626 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.css
--rw-r--r--   0 runner    (1001) docker     (116)     1955 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.js
--rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/templates/
--rw-r--r--   0 runner    (1001) docker     (116)    14994 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/templates/schema_doc.template.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2780 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      394 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      845 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/array.json
--rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/array_advanced.json
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/basic.json
--rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/combining_not.json
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/combining_oneOf.json
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (116)      742 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/description_with_ref.json
--rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/geo.json
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/multiple_types.json
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/pattern_properties.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/final.json
--rw-r--r--   0 runner    (1001) docker     (116)      325 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/intermediate.json
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/references.json
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/top_level_array.json
--rw-r--r--   0 runner    (1001) docker     (116)      427 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/top_level_combining.json
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_default.json
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_definitions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_descriptions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_examples.json
--rw-r--r--   0 runner    (1001) docker     (116)      648 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_special_chars.json
--rw-r--r--   0 runner    (1001) docker     (116)    13527 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/generate_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      145 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tox.ini
+-rw-r--r--   0        0        0      560 2024-05-03 20:42:56.131221 json_schema_for_humans-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0    10150 2024-05-03 20:42:56.131221 json_schema_for_humans-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/__init__.py
+-rw-r--r--   0        0        0     3990 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/cli.py
+-rw-r--r--   0        0        0     1911 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/const.py
+-rw-r--r--   0        0        0     6086 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/generate.py
+-rw-r--r--   0        0        0     7505 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/generation_configuration.py
+-rw-r--r--   0        0        0     8592 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/jinja_filters.py
+-rw-r--r--   0        0        0    18895 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/md_template.py
+-rw-r--r--   0        0        0        0 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/__init__.py
+-rw-r--r--   0        0        0    30645 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/intermediate_representation.py
+-rw-r--r--   0        0        0     3323 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_importer.py
+-rw-r--r--   0        0        0      970 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_keyword.py
+-rw-r--r--   0        0        0    23120 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_node.py
+-rw-r--r--   0        0        0     2987 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_to_render.py
+-rw-r--r--   0        0        0     3588 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/template_renderer.py
+-rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/badge_type.html
+-rw-r--r--   0        0        0     1162 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/base.html
+-rw-r--r--   0        0        0      673 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/breadcrumbs.html
+-rw-r--r--   0        0        0     4563 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/content.html
+-rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/macro_restriction.html
+-rw-r--r--   0        0        0     6357 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/schema_doc.css
+-rw-r--r--   0        0        0     1994 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_array.html
+-rw-r--r--   0        0        0     1886 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_conditional_subschema.html
+-rw-r--r--   0        0        0      529 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_not.html
+-rw-r--r--   0        0        0     2057 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0      707 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/tabbed_section.html
+-rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/badge_type.html
+-rw-r--r--   0        0        0     2017 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/base.html
+-rw-r--r--   0        0        0      716 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/breadcrumbs.html
+-rw-r--r--   0        0        0     4862 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/content.html
+-rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/macro_restriction.html
+-rw-r--r--   0        0        0     6415 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.css
+-rw-r--r--   0        0        0     2567 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.js
+-rw-r--r--   0        0        0     1259 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.min.js
+-rw-r--r--   0        0        0     1990 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_array.html
+-rw-r--r--   0        0        0     2038 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_conditional_subschema.html
+-rw-r--r--   0        0        0      652 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_not.html
+-rw-r--r--   0        0        0     2824 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0     1141 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/tabbed_section.html
+-rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/badge_type.html
+-rw-r--r--   0        0        0     1560 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/base.html
+-rw-r--r--   0        0        0      716 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/breadcrumbs.html
+-rw-r--r--   0        0        0     4946 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/content.html
+-rw-r--r--   0        0        0   155758 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/bootstrap-4.3.1.min.css
+-rw-r--r--   0        0        0     6411 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/overpass300,400,600,800.css
+-rw-r--r--   0        0        0     6415 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/schema_doc.css
+-rw-r--r--   0        0        0    27348 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GhU9vyww.woff2
+-rw-r--r--   0        0        0    38720 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GlU9s.woff2
+-rw-r--r--   0        0        0    16688 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GoU9vyww.woff2
+-rw-r--r--   0        0        0     7480 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GqU9vyww.woff2
+-rw-r--r--   0        0        0    37468 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GrU9vyww.woff2
+-rw-r--r--   0        0        0    58072 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/bootstrap-4.3.1.min.js
+-rw-r--r--   0        0        0    88145 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/jquery-3.4.1.min.js
+-rw-r--r--   0        0        0     1259 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/schema_doc.min.js
+-rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/macro_restriction.html
+-rw-r--r--   0        0        0     1990 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_array.html
+-rw-r--r--   0        0        0     2038 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_conditional_subschema.html
+-rw-r--r--   0        0        0      652 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_not.html
+-rw-r--r--   0        0        0     2824 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0     1141 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/tabbed_section.html
+-rw-r--r--   0        0        0      616 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/base.md
+-rw-r--r--   0        0        0      287 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/breadcrumbs.md
+-rw-r--r--   0        0        0     3122 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/content.md
+-rw-r--r--   0        0        0     1436 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_array.md
+-rw-r--r--   0        0        0      951 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_conditional_subschema.md
+-rw-r--r--   0        0        0      101 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_description.md
+-rw-r--r--   0        0        0      479 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_examples.md
+-rw-r--r--   0        0        0      177 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_not.md
+-rw-r--r--   0        0        0      125 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_one_of.md
+-rw-r--r--   0        0        0     1323 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_properties_details.md
+-rw-r--r--   0        0        0      314 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_undocumented_required_properties.md
+-rw-r--r--   0        0        0      446 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/tabbed_section.md
+-rw-r--r--   0        0        0      615 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/base.md
+-rw-r--r--   0        0        0      306 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/breadcrumbs.md
+-rw-r--r--   0        0        0     3031 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/content.md
+-rw-r--r--   0        0        0     1436 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_array.md
+-rw-r--r--   0        0        0      951 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_conditional_subschema.md
+-rw-r--r--   0        0        0      101 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_description.md
+-rw-r--r--   0        0        0      190 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_examples.md
+-rw-r--r--   0        0        0      177 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_not.md
+-rw-r--r--   0        0        0      125 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_one_of.md
+-rw-r--r--   0        0        0     1400 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_properties_details.md
+-rw-r--r--   0        0        0      314 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_undocumented_required_properties.md
+-rw-r--r--   0        0        0      504 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/tabbed_section.md
+-rw-r--r--   0        0        0     3786 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templating_utils.py
+-rw-r--r--   0        0        0     1875 2024-05-03 20:43:14.543290 json_schema_for_humans-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11651 1970-01-01 00:00:00.000000 json_schema_for_humans-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `json-schema-for-humans-0.9.1/LICENSE` & `json_schema_for_humans-1.0.0/LICENSE.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright 2019 Coveo Solutions Inc.
- 
+
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
- 
+
     http://www.apache.org/licenses/LICENSE-2.0
- 
+
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
```

### Comparing `json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.js` & `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,29 @@
 $(document).on('click', 'a[href^="#"]', function(event) {
     event.preventDefault();
     history.pushState({}, '', this.href);
 });
 
+function flashElement(elementId) {
+    // $( "#" + elementId ).fadeOut(100).fadeIn(200).fadeOut(100).fadeIn(500);
+    myElement = document.getElementById(elementId);
+    myElement.classList.add("jsfh-animated-property");
+    setTimeout(function() {
+        myElement.classList.remove("jsfh-animated-property");
+    }, 1000);
+}
+
 function setAnchor(anchorLinkDestination) {
     // Set anchor link without reloading
     history.pushState({}, '', anchorLinkDestination);
 }
 
 function anchorOnLoad() {
     // Added to onload on body, checks if there is an anchor link and if so, expand
-    let linkTarget = window.location.hash.split("?")[0].split("&")[0];
+    let linkTarget = decodeURIComponent(window.location.hash.split("?")[0].split("&")[0]);
     if (linkTarget[0] === "#") {
         linkTarget = linkTarget.substr(1);
     }
 
     if (linkTarget.length > 0) {
         anchorLink(linkTarget);
     }
@@ -24,15 +33,15 @@
     const target = $("#" + linkTarget);
     // Find the targeted element to expand and all its parents that can be expanded
     target.parents().addBack().filter(".collapse:not(.show), .tab-pane, [role='tab']").each(
         function(index) {
             if ($(this).hasClass("collapse")) {
                 $(this).collapse("show");
             } else if ($(this).hasClass("tab-pane")) {
-                // We have the pane and not the the tab itself, find the tab
+                // We have the pane and not the tab itself, find the tab
                 const tabToShow = $("a[href='#" + $(this).attr("id") + "']");
                 if (tabToShow) {
                     tabToShow.tab("show");
                 }
             } else if ($(this).attr("role") === "tab") {
                 // The tab is not a parent of underlying elements, the tab pane is
                 // However, it can still be linked directly
@@ -41,13 +50,20 @@
         }
     );
 
     // Wait a little so the user has time to see the page scroll
     // Or maybe it is to be sure everything is expanded before scrolling and I was not able to bind to the bootstrap
     // events in a way that works all the time, we may never know
     setTimeout(function() {
-        document.getElementById(linkTarget).scrollIntoView({
-            block: "center",
-            behavior: "smooth"
-        });
+        let targetElement = document.getElementById(linkTarget);
+        if (targetElement) {
+            targetElement.scrollIntoView({
+                block: "center",
+                behavior: "smooth"
+            });
+            // Flash the element so that the user notices where the link points to
+            setTimeout(function() {
+                flashElement(linkTarget);
+            }, 500);
+        }
     }, 1000);
 }
```

