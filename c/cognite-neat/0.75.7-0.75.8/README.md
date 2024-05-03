# Comparing `tmp/cognite_neat-0.75.7.tar.gz` & `tmp/cognite_neat-0.75.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.75.7.tar", max compression
+gzip compressed data, was "cognite_neat-0.75.8.tar", max compression
```

## Comparing `cognite_neat-0.75.7.tar` & `cognite_neat-0.75.8.tar`

### file list

```diff
@@ -1,259 +1,258 @@
--rw-r--r--   0        0        0    11351 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/LICENSE
--rw-r--r--   0        0        0     6775 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/README.md
--rw-r--r--   0        0        0       61 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3529 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13661 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8107 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423704 2024-05-02 10:32:57.726099 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
--rw-r--r--   0        0        0     2667 2024-05-02 10:32:57.726099 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
--rw-r--r--   0        0        0  6282865 2024-05-02 10:32:57.750103 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
--rw-r--r--   0        0        0   240334 2024-05-02 10:32:57.754104 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/config.py
--rw-r--r--   0        0        0     1227 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-02 10:32:57.762105 cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14947 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14909 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23859 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2399 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2837 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40480 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22715 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12995 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14738 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36814 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5783 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2330 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7727 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      176 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      673 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19612 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1517 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1870 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    14231 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13767 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19900 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4090 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4057 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10405 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12553 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6801 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11925 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7804 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6987 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11085 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4074 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15323 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0     4893 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/_entity.py
--rw-r--r--   0        0        0     5308 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/data_types.py
--rw-r--r--   0        0        0     9885 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/entities.py
--rw-r--r--   0        0        0     7228 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0      522 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/__init__.py
--rw-r--r--   0        0        0    11024 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_base.py
--rw-r--r--   0        0        0    56198 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_architect_rules.py
--rw-r--r--   0        0        0    30789 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_schema.py
--rw-r--r--   0        0        0     2542 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_domain_rules.py
--rw-r--r--   0        0        0    21577 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_information_rules.py
--rw-r--r--   0        0        0     1299 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/__init__.py
--rw-r--r--   0        0        0    12233 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_value.py
--rw-r--r--   0        0        0       68 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11304 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3015 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    22585 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0    10384 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4784 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3929 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29416 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27324 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12728 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2361 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20706 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28111 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4540 2024-05-02 10:32:58.170174 cognite_neat-0.75.7/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.7/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/README.md
+-rw-r--r--   0        0        0       61 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3529 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13661 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8107 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-02 16:06:01.205741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-02 16:06:01.209741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-02 16:06:01.209741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-02 16:06:01.209741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-02 16:06:01.209741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-02 16:06:01.209741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423704 2024-05-02 16:06:01.213741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
+-rw-r--r--   0        0        0     2667 2024-05-02 16:06:01.213741 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282865 2024-05-02 16:06:01.237742 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
+-rw-r--r--   0        0        0   240334 2024-05-02 16:06:01.241742 cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-05-02 16:06:01.249742 cognite_neat-0.75.8/cognite/neat/config.py
+-rw-r--r--   0        0        0     1227 2024-05-02 16:06:01.249742 cognite_neat-0.75.8/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-02 16:06:01.249742 cognite_neat-0.75.8/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-02 16:06:01.249742 cognite_neat-0.75.8/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-02 16:06:01.253742 cognite_neat-0.75.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14980 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-02 16:06:01.257742 cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14909 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23859 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2399 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2837 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40480 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22715 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12995 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14738 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-02 16:06:01.261742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36814 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5783 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2330 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7727 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19608 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-02 16:06:01.265742 cognite_neat-0.75.8/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1870 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    14231 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13767 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    20139 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4100 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4057 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10379 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12676 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6801 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11921 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6947 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11306 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4315 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15338 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     6078 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0    15481 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0    11030 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    11024 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    52589 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    12898 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_dms_rules_write.py
+-rw-r--r--   0        0        0    30777 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2655 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    22015 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0      305 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0      929 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0     3197 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0       68 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11304 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-02 16:06:01.269742 cognite_neat-0.75.8/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    22585 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0    10394 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3929 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29416 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27324 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12728 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2361 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20706 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28111 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-02 16:06:01.273742 cognite_neat-0.75.8/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4540 2024-05-02 16:06:01.661748 cognite_neat-0.75.8/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.8/PKG-INFO
```

### Comparing `cognite_neat-0.75.7/LICENSE` & `cognite_neat-0.75.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/README.md` & `cognite_neat-0.75.8/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/configuration.py` & `cognite_neat-0.75.8/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.75.8/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.75.8/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/explorer.py` & `cognite_neat-0.75.8/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.75.8/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.75.8/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.75.8/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.75.8/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.75.8/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.75.8/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/config.py` & `cognite_neat-0.75.8/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/constants.py` & `cognite_neat-0.75.8/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.8/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.8/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
 import numpy
 import pandas as pd
 from rdflib import RDF, Literal, Namespace, URIRef
 
 from cognite.neat.graph.models import Triple
 from cognite.neat.rules.analysis import InformationArchitectRulesAnalysis
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import ClassEntity, EntityTypes
 from cognite.neat.rules.models.rules import DMSRules, InformationRules
 from cognite.neat.rules.models.rules._information_rules import InformationProperty
-from cognite.neat.rules.models.rules._types import ClassEntity, EntityTypes, XSDValueType
 from cognite.neat.utils.utils import remove_namespace
 
 from ._base import BaseExtractor
 
 
 class MockGraphGenerator(BaseExtractor):
     """
@@ -51,15 +52,15 @@
         if not class_count:
             self.class_count = {
                 class_: 1
                 for class_ in InformationArchitectRulesAnalysis(self.rules).defined_classes(consider_inheritance=True)
             }
         elif all(isinstance(key, str) for key in class_count.keys()):
             self.class_count = {
-                ClassEntity.from_raw(f"{self.rules.metadata.prefix}:{key}"): value for key, value in class_count.items()
+                ClassEntity.load(f"{self.rules.metadata.prefix}:{key}"): value for key, value in class_count.items()
             }
         elif all(isinstance(key, ClassEntity) for key in class_count.keys()):
             self.class_count = cast(dict[ClassEntity, int], class_count)
         else:
             raise ValueError("Class count keys must be of type str! or ClassEntity! or empty dict!")
 
         self.stop_on_exception = stop_on_exception
@@ -143,15 +144,15 @@
         key: [URIRef(namespace[f"{key.suffix}-{i+1}"]) for i in range(value)] for key, value in class_count.items()
     }
 
     # create triple for each class instance defining its type
     triples: list[Triple] = []
     for class_ in class_count:
         triples += [
-            (class_instance_id, RDF.type, URIRef(namespace[class_.suffix]))
+            (class_instance_id, RDF.type, URIRef(namespace[str(class_.suffix)]))
             for class_instance_id in instance_ids[class_]
         ]
 
     # generate triples for connected classes
     for class_ in generation_order:
         triples += _generate_triples_per_class(
             class_, class_property_pairs, sym_pairs, instance_ids, namespace, stop_on_exception
@@ -242,15 +243,15 @@
     rows_to_remove = set(class_linkage[~(class_linkage["source_class"].isin(set(class_count.keys())))].index.values)
     rows_to_remove |= set(class_linkage[~(class_linkage["target_class"].isin(set(class_count.keys())))].index.values)
 
     return class_linkage.drop(list(rows_to_remove))
 
 
 def _generate_mock_data_property_triples(
-    instance_ids: list[URIRef], property_: str, namespace: Namespace, value_type: XSDValueType
+    instance_ids: list[URIRef], property_: str, namespace: Namespace, value_type: DataType
 ) -> list[tuple[URIRef, URIRef, Literal]]:
     """Generates triples for data properties."""
 
     python_type = value_type.python
     triples = []
     for id_ in instance_ids:
         if python_type == int:
@@ -334,15 +335,15 @@
 
     for property_ in class_properties_pairs[class_]:
         if property_.type_ == EntityTypes.data_property:
             triples += _generate_mock_data_property_triples(
                 instance_ids[class_],
                 property_.property_,
                 namespace,
-                cast(XSDValueType, property_.value_type),
+                cast(DataType, property_.value_type),
             )
 
         elif property_.type_ == EntityTypes.object_property:
             triples += _generate_mock_object_property_triples(
                 class_,
                 property_,
                 class_properties_pairs,
```

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.8/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.75.8/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.75.8/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.75.8/cognite/neat/rules/analysis/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models.rules._types import ClassEntity
+from cognite.neat.rules.models.entities import ClassEntity
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 else:
     from backports.strenum import StrEnum
 
 T_Rules = TypeVar("T_Rules", bound=Rules)
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/analysis/_information_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import warnings
 from collections import defaultdict
 from typing import Any, cast
 
 import pandas as pd
 from pydantic import ValidationError
 
+from cognite.neat.rules.models.entities import ClassEntity, EntityTypes, ParentClassEntity, ReferenceEntity
 from cognite.neat.rules.models.rdfpath import TransformationRuleType
 from cognite.neat.rules.models.rules._base import SchemaCompleteness
 from cognite.neat.rules.models.rules._information_rules import InformationClass, InformationProperty, InformationRules
-from cognite.neat.rules.models.rules._types._base import ClassEntity, EntityTypes, ParentClassEntity, ReferenceEntity
 from cognite.neat.utils.utils import get_inheritance_path
 
 from ._base import BaseAnalysis, DataModelingScenario
 
 
 class InformationArchitectRulesAnalysis(BaseAnalysis):
     def __init__(self, rules: InformationRules):
@@ -122,15 +122,15 @@
             class_parent_pairs = self.class_parent_pairs(use_reference=use_reference)
             for class_ in class_parent_pairs:
                 self._add_inherited_properties(class_, class_property_pairs, class_parent_pairs)
 
         return class_property_pairs
 
     def class_inheritance_path(self, class_: ClassEntity | str, use_reference: bool = False) -> list[ClassEntity]:
-        class_ = class_ if isinstance(class_, ClassEntity) else ClassEntity.from_raw(class_)
+        class_ = class_ if isinstance(class_, ClassEntity) else ClassEntity.load(class_)
         class_parent_pairs = self.class_parent_pairs(use_reference)
         return get_inheritance_path(class_, class_parent_pairs)
 
     @classmethod
     def _add_inherited_properties(
         cls,
         class_: ClassEntity,
@@ -324,15 +324,15 @@
             property_dict[definition.property_].append(definition)
         return property_dict
 
     def as_class_dict(self) -> dict[str, InformationClass]:
         """This is to simplify access to classes through dict."""
         class_dict: dict[str, InformationClass] = {}
         for definition in self.rules.classes:
-            class_dict[definition.class_.suffix] = definition
+            class_dict[str(definition.class_.suffix)] = definition
         return class_dict
 
     def subset_rules(self, desired_classes: set[ClassEntity], use_reference: bool = False) -> InformationRules:
         """
         Subset rules to only include desired classes and their properties.
 
         Args:
@@ -394,15 +394,15 @@
             "prefixes": (rules.prefixes or {}).copy(),
             "classes": [],
             "properties": [],
         }
 
         logging.info(f"Reducing data model to only include the following classes: {possible_classes}")
         for class_ in possible_classes:
-            reduced_data_model["classes"].append(class_as_dict[class_.suffix])
+            reduced_data_model["classes"].append(class_as_dict[str(class_.suffix)])
 
         class_property_pairs = self.classes_with_properties(consider_inheritance=False)
 
         for class_, properties in class_property_pairs.items():
             if class_ in possible_classes:
                 reduced_data_model["properties"].extend(properties)
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.75.8/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 from rdflib import DCTERMS, OWL, RDF, RDFS, XSD, BNode, Graph, Literal, Namespace, URIRef
 from rdflib.collection import Collection as GraphCollection
 
 from cognite.neat.constants import DEFAULT_NAMESPACE as NEAT_NAMESPACE
 from cognite.neat.rules import exceptions
 from cognite.neat.rules.analysis import InformationArchitectRulesAnalysis
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import ClassEntity, EntityTypes
 from cognite.neat.rules.models.rules import DMSRules
 from cognite.neat.rules.models.rules._information_rules import (
     InformationClass,
     InformationMetadata,
     InformationProperty,
     InformationRules,
 )
-from cognite.neat.rules.models.rules._types import XSD_VALUE_TYPE_MAPPINGS, EntityTypes
 from cognite.neat.utils.utils import generate_exception_report, remove_namespace
 
 from ._base import BaseExporter
 from ._validation import are_properties_redefined
 
 if sys.version_info >= (3, 11):
     from typing import Self
@@ -110,15 +111,15 @@
             ],
             classes=[
                 OWLClass.from_class(definition, rules.metadata.namespace, rules.prefixes)
                 for definition in rules.classes
             ],
             shapes=[
                 SHACLNodeShape.from_rules(
-                    class_dict[class_.suffix],
+                    class_dict[str(class_.suffix)],
                     list(properties.values()),
                     rules.metadata.namespace,
                 )
                 for class_, properties in InformationArchitectRulesAnalysis(rules).class_property_pairs().items()
             ]
             + [
                 SHACLNodeShape.from_rules(
@@ -245,23 +246,23 @@
 
     @classmethod
     def from_class(cls, definition: InformationClass, namespace: Namespace, prefixes: dict) -> Self:
         if definition.parent and isinstance(definition.parent, list):
             sub_class_of = []
             for parent_class in definition.parent:
                 try:
-                    sub_class_of.append(prefixes[parent_class.prefix][parent_class.suffix])
+                    sub_class_of.append(prefixes[str(parent_class.prefix)][str(parent_class.suffix)])
                 except KeyError:
-                    sub_class_of.append(namespace[parent_class.suffix])
+                    sub_class_of.append(namespace[str(parent_class.suffix)])
         else:
             sub_class_of = None
 
         return cls(
-            id_=namespace[definition.class_.suffix],
-            label=definition.name or definition.class_.suffix,
+            id_=namespace[str(definition.class_.suffix)],
+            label=definition.name or str(definition.class_.suffix),
             comment=definition.description,
             sub_class_of=sub_class_of,
             namespace=namespace,
         )
 
     @property
     def type_triples(self) -> list[tuple]:
@@ -320,20 +321,22 @@
             comment=set(),
             domain=set(),
             range_=set(),
             type_=set(),
         )
         for definition in definitions:
             owl_property.type_.add(OWL[definition.type_])
-            owl_property.range_.add(
-                XSD[definition.value_type.suffix]
-                if definition.value_type.suffix in XSD_VALUE_TYPE_MAPPINGS
-                else namespace[definition.value_type.suffix]
-            )
-            owl_property.domain.add(namespace[definition.class_.suffix])
+
+            if isinstance(definition.value_type, DataType):
+                owl_property.range_.add(XSD[definition.value_type.xsd])
+            elif isinstance(definition.value_type, ClassEntity):
+                owl_property.range_.add(namespace[str(definition.value_type.suffix)])
+            else:
+                raise ValueError(f"Value type {definition.value_type} is not supported")
+            owl_property.domain.add(namespace[str(definition.class_.suffix)])
             owl_property.label.add(definition.name or definition.property_)
             if definition.description:
                 owl_property.comment.add(definition.description)
 
         return owl_property
 
     @field_validator("type_")
@@ -489,20 +492,20 @@
         )
 
     @classmethod
     def from_rules(
         cls, class_definition: InformationClass, property_definitions: list[InformationProperty], namespace: Namespace
     ) -> "SHACLNodeShape":
         if class_definition.parent:
-            parent = [namespace[parent.suffix + "Shape"] for parent in class_definition.parent]
+            parent = [namespace[str(parent.suffix) + "Shape"] for parent in class_definition.parent]
         else:
             parent = None
         return cls(
-            id_=namespace[f"{class_definition.class_.suffix}Shape"],
-            target_class=namespace[class_definition.class_.suffix],
+            id_=namespace[f"{class_definition.class_.suffix!s}Shape"],
+            target_class=namespace[str(class_definition.class_.suffix)],
             parent=parent,
             property_shapes=[SHACLPropertyShape.from_property(prop, namespace) for prop in property_definitions],
             namespace=namespace,
         )
 
 
 class SHACLPropertyShape(OntologyModel):
@@ -548,16 +551,16 @@
     def from_property(cls, definition: InformationProperty, namespace: Namespace) -> "SHACLPropertyShape":
         return cls(
             id_=BNode(),
             path=namespace[definition.property_],
             node_kind=SHACL.IRI if definition.type_ == EntityTypes.object_property else SHACL.Literal,
             expected_value_type=(
                 namespace[f"{definition.value_type.suffix}Shape"]
-                if definition.type_ == EntityTypes.object_property
-                else XSD[definition.value_type.suffix]
+                if isinstance(definition.value_type, ClassEntity)
+                else XSD[definition.value_type.xsd]
             ),
             min_count=definition.min_count,
             max_count=(
                 int(definition.max_count) if definition.max_count and definition.max_count != float("inf") else None
             ),
             namespace=namespace,
         )
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.75.8/cognite/neat/rules/exporters/_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     rules: InformationRules, return_report: bool = False
 ) -> bool | tuple[bool, list[dict]]:
     """Check if data model definitions are valid."""
 
     flag: bool = True
     with warnings.catch_warnings(record=True) as validation_warnings:
         for class_ in rules.classes:
-            if not re.match(VIEW_ID_COMPLIANCE_REGEX, class_.class_.suffix):
+            if not re.match(VIEW_ID_COMPLIANCE_REGEX, str(class_.class_.suffix)):
                 warnings.warn(
                     exceptions.EntityIDNotDMSCompliant(
                         "Class", class_.class_.versioned_id, f"[Classes/Class/{class_.class_.versioned_id}]"
                     ).message,
                     category=exceptions.EntityIDNotDMSCompliant,
                     stacklevel=2,
                 )
                 flag = False
 
         for row, property_ in enumerate(rules.properties):
             # check class id which would resolve as view/container id
-            if not re.match(VIEW_ID_COMPLIANCE_REGEX, property_.class_.suffix):
+            if not re.match(VIEW_ID_COMPLIANCE_REGEX, str(property_.class_.suffix)):
                 warnings.warn(
                     exceptions.EntityIDNotDMSCompliant(
                         "Class", property_.class_.versioned_id, f"[Properties/Class/{row}]"
                     ).message,
                     category=exceptions.EntityIDNotDMSCompliant,
                     stacklevel=2,
                 )
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,32 +6,31 @@
 from cognite.client.data_classes.data_modeling import DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
 from cognite.client.utils import ms_to_datetime
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.importers._base import BaseImporter, Rules
 from cognite.neat.rules.issues import IssueList
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import (
+    ClassEntity,
+    ContainerEntity,
+    DMSUnknownEntity,
+    ViewEntity,
+    ViewPropertyEntity,
+)
 from cognite.neat.rules.models.rules import DMSRules, DMSSchema, RoleTypes
 from cognite.neat.rules.models.rules._base import ExtensionCategory, SchemaCompleteness
 from cognite.neat.rules.models.rules._dms_architect_rules import (
     DMSContainer,
     DMSMetadata,
     DMSProperty,
     DMSView,
     SheetList,
 )
-from cognite.neat.rules.models.rules._types import (
-    ClassEntity,
-    ContainerEntity,
-    DMSValueType,
-    Undefined,
-    Unknown,
-    ViewEntity,
-    ViewPropEntity,
-)
 
 
 class DMSImporter(BaseImporter):
     def __init__(self, schema: DMSSchema, metadata: DMSMetadata | None = None):
         self.schema = schema
         self.metadata = metadata
 
@@ -132,29 +131,29 @@
                         elif isinstance(constraint_obj, dm.UniquenessConstraint):
                             # This does not apply to this property
                             continue
                         else:
                             raise NotImplementedError(f"Constraint type {type(constraint_obj)} not implemented")
 
                     if isinstance(container_prop.type, dm.DirectRelation):
-                        direct_value_type: str | ViewEntity | DMSValueType
+                        direct_value_type: str | ViewEntity | DataType | DMSUnknownEntity
                         if prop.source is None:
                             issue_list.append(
                                 issues.importing.UnknownValueTypeWarning(class_entity.versioned_id, prop_id)
                             )
-                            direct_value_type = ViewPropEntity(prefix=Undefined, suffix=Unknown)
+                            direct_value_type = DMSUnknownEntity()
                         else:
-                            direct_value_type = ViewPropEntity.from_id(prop.source)
+                            direct_value_type = ViewEntity.from_id(prop.source)
 
                         dms_property = DMSProperty(
                             class_=class_entity,
                             property_=prop_id,
                             description=prop.description,
                             name=prop.name,
-                            value_type=cast(ViewPropEntity | DMSValueType, direct_value_type),
+                            value_type=direct_value_type,
                             relation="direct",
                             nullable=container_prop.nullable,
                             default=container_prop.default_value,
                             is_list=False,
                             container=ContainerEntity.from_id(container.as_id()),
                             container_property=prop.container_property_identifier,
                             view=ViewEntity.from_id(view.as_id()),
@@ -164,27 +163,27 @@
                         )
                     else:
                         dms_property = DMSProperty(
                             class_=ClassEntity(prefix=view.space, suffix=view.external_id, version=view.version),
                             property_=prop_id,
                             description=prop.description,
                             name=prop.name,
-                            value_type=cast(ViewPropEntity | DMSValueType, container_prop.type._type),
+                            value_type=cast(ViewPropertyEntity | DataType, container_prop.type._type),
                             nullable=container_prop.nullable,
                             is_list=container_prop.type.is_list,
                             default=container_prop.default_value,
                             container=ContainerEntity.from_id(container.as_id()),
                             container_property=prop.container_property_identifier,
                             view=ViewEntity.from_id(view.as_id()),
                             view_property=prop_id,
                             index=index or None,
                             constraint=unique_constraints or None,
                         )
                 elif isinstance(prop, dm.MultiEdgeConnectionApply):
-                    view_entity = ViewPropEntity.from_id(prop.source)
+                    view_entity = ViewEntity.from_id(prop.source)
                     dms_property = DMSProperty(
                         class_=ClassEntity(prefix=view.space, suffix=view.external_id, version=view.version),
                         property_=prop_id,
                         relation="multiedge",
                         description=prop.description,
                         name=prop.name,
                         value_type=view_entity,
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import Counter
 from collections.abc import Callable, Sequence
+from typing import cast
 
 import cognite.neat.rules.issues.importing
 from cognite.neat.rules import issues
 from cognite.neat.rules.importers._dtdl2rules.spec import (
     DTMI,
     Command,
     CommandV2,
@@ -16,21 +17,17 @@
     PropertyV2,
     Relationship,
     Schema,
     Telemetry,
     TelemetryV2,
 )
 from cognite.neat.rules.issues import IssueList, ValidationIssue
+from cognite.neat.rules.models.data_types import _DATA_TYPE_BY_NAME, DataType, Json, String
+from cognite.neat.rules.models.entities import ClassEntity, ParentClassEntity
 from cognite.neat.rules.models.rules._information_rules import InformationClass, InformationProperty
-from cognite.neat.rules.models.rules._types import (
-    XSD_VALUE_TYPE_MAPPINGS,
-    ClassEntity,
-    ParentClassEntity,
-    XSDValueType,
-)
 
 
 class _DTDLConverter:
     def __init__(self, issues: list[ValidationIssue] | None = None) -> None:
         self.issues: IssueList = IssueList(issues or [])
         self.properties: list[InformationProperty] = []
         self.classes: list[InformationClass] = []
@@ -88,15 +85,20 @@
 
     def convert_interface(self, item: Interface, _: str | None) -> None:
         class_ = InformationClass(
             class_=item.id_.as_class_id(),
             name=item.display_name,
             description=item.description,
             comment=item.comment,
-            parent=[ParentClassEntity.from_raw(parent.as_class_id()) for parent in item.extends or []] or None,
+            parent=[
+                cast(ParentClassEntity, parent_entity)
+                for parent in item.extends or []
+                if isinstance(parent_entity := ParentClassEntity.load(parent.as_class_id()), ParentClassEntity)
+            ]
+            or None,
         )
         self.classes.append(class_)
         for sub_item_or_id in item.contents or []:
             if isinstance(sub_item_or_id, DTMI) and sub_item_or_id not in self._item_by_id:
                 self.issues.append(
                     issues.importing.UnknownPropertyWarning(
                         component_type=item.type,
@@ -119,15 +121,15 @@
             self._missing_parent_warning(item)
             return None
         value_type = self.schema_to_value_type(item.schema_, item)
         if value_type is None:
             return None
 
         prop = InformationProperty(
-            class_=ClassEntity.from_raw(parent),
+            class_=ClassEntity.load(parent),
             property_=item.name,
             name=item.display_name,
             description=item.description,
             comment=item.comment,
             value_type=value_type,
             min_count=min_count,
             max_count=max_count,
@@ -171,15 +173,15 @@
                     reason="Neat does not have a concept of response for commands. This will be ignored.",
                 )
             )
         value_type = self.schema_to_value_type(item.request.schema_, item)
         if value_type is None:
             return
         prop = InformationProperty(
-            class_=ClassEntity.from_raw(parent),
+            class_=ClassEntity.load(parent),
             property_=item.name,
             name=item.display_name,
             description=item.description,
             comment=item.comment,
             value_type=value_type,
             min_count=0,
             max_count=1,
@@ -191,15 +193,15 @@
             self._missing_parent_warning(item)
             return None
 
         value_type = self.schema_to_value_type(item.schema_, item)
         if value_type is None:
             return
         prop = InformationProperty(
-            class_=ClassEntity.from_raw(parent),
+            class_=ClassEntity.load(parent),
             property_=item.name,
             name=item.display_name,
             description=item.description,
             comment=item.comment,
             value_type=value_type,
             min_count=0,
             max_count=1,
@@ -207,30 +209,30 @@
         self.properties.append(prop)
 
     def convert_relationship(self, item: Relationship, parent: str | None) -> None:
         if parent is None:
             self._missing_parent_warning(item)
             return None
         if item.target is not None:
-            value_type: XSDValueType | ClassEntity
+            value_type: DataType | ClassEntity
             if item.target in self._item_by_id:
                 value_type = item.target.as_class_id()
             else:
                 # Falling back to json
                 self.issues.append(
                     cognite.neat.rules.issues.importing.MissingIdentifierError(
                         component_type="Unknown",
                         instance_name=item.target.model_dump(),
                         instance_id=item.target.model_dump(),
                     )
                 )
-                value_type = XSD_VALUE_TYPE_MAPPINGS["json"]
+                value_type = Json()
 
             prop = InformationProperty(
-                class_=ClassEntity.from_raw(parent),
+                class_=ClassEntity.load(parent),
                 property_=item.name,
                 name=item.display_name,
                 description=item.description,
                 min_count=item.min_multiplicity or 0,
                 max_count=item.max_multiplicity or 1,
                 comment=item.comment,
                 value_type=value_type,
@@ -271,21 +273,21 @@
                 min_count=0,
                 max_count=1,
             )
             self.properties.append(prop)
 
     def schema_to_value_type(
         self, schema: Schema | Interface | DTMI | None, item: DTDLBase
-    ) -> XSDValueType | ClassEntity | None:
+    ) -> DataType | ClassEntity | None:
         input_type = self._item_by_id.get(schema) if isinstance(schema, DTMI) else schema
 
         if isinstance(input_type, Enum):
-            return XSD_VALUE_TYPE_MAPPINGS["string"]
-        elif isinstance(input_type, str) and input_type in XSD_VALUE_TYPE_MAPPINGS:
-            return XSD_VALUE_TYPE_MAPPINGS[input_type]
+            return String()
+        elif isinstance(input_type, str) and input_type.casefold() in _DATA_TYPE_BY_NAME:
+            return _DATA_TYPE_BY_NAME[input_type.casefold()]()
         elif isinstance(input_type, str):
             self.issues.append(
                 cognite.neat.rules.issues.importing.UnsupportedPropertyTypeError(
                     component_type=item.type,
                     property_type=input_type,
                     property_name="schema",
                     instance_name=item.display_name,
@@ -297,19 +299,19 @@
             if input_type.id_ is None:
                 self.issues.append(
                     cognite.neat.rules.issues.importing.MissingIdentifierError(
                         component_type=input_type.type,
                         instance_name=input_type.display_name,
                     )
                 )
-                return XSD_VALUE_TYPE_MAPPINGS["json"]
+                return Json()
             else:
                 if isinstance(input_type, Object):
                     self.convert_object(input_type, None)
-                return ClassEntity.from_raw(input_type.id_.as_class_id())
+                return ClassEntity.load(input_type.id_.as_class_id())
         else:
             self.issues.append(
                 issues.importing.UnknownPropertyWarning(
                     component_type=item.type,
                     property_name="schema",
                     instance_name=item.display_name,
                     instance_id=item.id_.model_dump() if item.id_ else None,
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import re
 import warnings
 from abc import ABC
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, TypeAlias
 
 from pydantic import BaseModel, Field, field_validator, model_serializer, model_validator
 
-from cognite.neat.rules.models.rules._types import ClassEntity
+from cognite.neat.rules.models.entities import ClassEntity
 
 if TYPE_CHECKING:
     from pydantic.type_adapter import IncEx
 
 
 # Regex is from the spec: https://github.com/Azure/opendigitaltwins-dtdl/blob/master/DTMI/README.md#validation-regular-expressions
 _DTMI_REGEX = (
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from pathlib import Path
 from typing import Literal, overload
 
 from rdflib import DC, DCTERMS, OWL, RDF, RDFS, SKOS, Graph
 
 from cognite.neat.rules.importers._base import BaseImporter, Rules
 from cognite.neat.rules.issues import IssueList
+from cognite.neat.rules.models.data_types import _XSD_TYPES
 from cognite.neat.rules.models.rules import InformationRules, RoleTypes
-from cognite.neat.rules.models.rules._types import XSD_VALUE_TYPE_MAPPINGS
 
 from ._owl2classes import parse_owl_classes
 from ._owl2metadata import parse_owl_metadata
 from ._owl2properties import parse_owl_properties
 
 
 class OWLImporter(BaseImporter):
@@ -122,15 +122,15 @@
     Args:
         tables: imported tables from owl ontology
 
     Returns:
         Updated tables with missing properties added to containers
     """
 
-    xsd_types = set(XSD_VALUE_TYPE_MAPPINGS.keys())
+    xsd_types = _XSD_TYPES
     candidate_value_types = {definition["Value Type"] for definition in components["Properties"]} - {
         definition["Class"] for definition in components["Classes"]
     }
 
     # to avoid issue of case sensitivity for xsd types
     value_types_lower = {v.lower() for v in candidate_value_types}
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pandas as pd
 from pandas import ExcelFile
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models.rules import RULES_PER_ROLE, DMSRules, DomainRules, InformationRules
 from cognite.neat.rules.models.rules._base import RoleTypes, SchemaCompleteness
+from cognite.neat.rules.models.rules._dms_rules_write import DMSRulesWrite
 from cognite.neat.utils.auxiliary import local_import
 from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_individual_sheet
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 SOURCE_SHEET__TARGET_FIELD__HEADERS = [
     ("Properties", "Properties", "Class"),
@@ -210,15 +211,19 @@
 
         rules_cls = RULES_PER_ROLE[original_role]
         with _handle_issues(
             issue_list,
             error_cls=issues.spreadsheet.InvalidSheetError,
             error_args={"read_info_by_sheet": read_info_by_sheet},
         ) as future:
-            rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
+            rules: Rules
+            if rules_cls is DMSRules:
+                rules = DMSRulesWrite.load(sheets).as_read()
+            else:
+                rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
 
         if future.result == "failure" or issue_list.has_errors:
             return self._return_or_raise(issue_list, errors)
 
         return self._to_output(
             rules,
             issue_list,
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 from typing import Any, Literal, overload
 
 import yaml
 
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList, NeatValidationError, ValidationIssue
-from cognite.neat.rules.models.rules import RULES_PER_ROLE, RoleTypes
+from cognite.neat.rules.models.rules import RULES_PER_ROLE, DMSRules, RoleTypes
+from cognite.neat.rules.models.rules._dms_rules_write import DMSRulesWrite
 
 from ._base import BaseImporter, Rules, _handle_issues
 
 
 class YAMLImporter(BaseImporter):
     """Imports the rules from a YAML file.
 
@@ -93,15 +94,20 @@
             return None, self._read_issues
 
         role_input = RoleTypes(metadata["role"])
         role_enum = RoleTypes(role_input)
         rules_model = RULES_PER_ROLE[role_enum]
 
         with _handle_issues(issue_list) as future:
-            rules = rules_model.model_validate(self.raw_data)
+            rules: Rules
+            if rules_model is DMSRules:
+                rules = DMSRulesWrite.load(self.raw_data).as_read()
+            else:
+                rules = rules_model.model_validate(self.raw_data)
+
         if future.result == "failure":
             if errors == "continue":
                 return None, issue_list
             else:
                 raise issue_list.as_errors()
 
         return self._to_output(rules, issue_list, errors, role)
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/base.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     description = "The source view referred to by the DirectRelation does not exist"
     fix = "Create the source view"
     error_name: ClassVar[str] = "DirectRelationMissingSource"
     view_id: dm.ViewId
     property: str
 
     def message(self) -> str:
-        return f"The source view referred to by {self.view_id}.{self.property} does not exist"
+        return f"The source view referred to by '{self.view_id.external_id}.{self.property}' does not exist."
 
     def dump(self) -> dict[str, Any]:
         output = super().dump()
         output["view_id"] = self.view_id
         output["property"] = self.property
         return output
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.75.8/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/data_types.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/data_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 class DataType(BaseModel):
+    # These are necessary for Pydantic to work
+    # pydantic gets confused as we have no fields.
+    __pydantic_extra__ = None
+    __pydantic_fields_set__ = set()
+    __pydantic_private__ = {}
+
     name: ClassVar[str]
     python: ClassVar[type]
     dms: ClassVar[type[dms.PropertyType]]
     graphql: ClassVar[str]
     xsd: ClassVar[str]
     sql: ClassVar[str]
 
@@ -28,232 +34,249 @@
         return self.model_dump(by_alias=True)
 
     @model_validator(mode="wrap")
     def _load(cls, value: Any, handler: ModelWrapValidatorHandler["DataType"]) -> Any:
         if isinstance(value, cls | dict):
             return value
         elif isinstance(value, str):
-            try:
-                return _DATA_TYPE_BY_NAME[value.casefold()]()
-            except KeyError:
-                raise ValueError(f"Unknown literal type: {value}") from None
+            value_standardized = value.casefold()
+            if cls_ := _DATA_TYPE_BY_DMS_TYPE.get(value_standardized):
+                return cls_()
+            elif cls_ := _DATA_TYPE_BY_NAME.get(value_standardized):
+                return cls_()
+            raise ValueError(f"Unknown literal type: {value}") from None
         raise ValueError(f"Cannot load {cls.__name__} from {value}")
 
     @model_serializer(when_used="unless-none", return_type=str)
     def as_str(self) -> str:
         return str(self)
 
     def __str__(self) -> str:
         return self.name
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self))
 
+    def __hash__(self) -> int:
+        return hash(str(self))
+
+    @classmethod
+    def is_data_type(cls, value: str) -> bool:
+        return value.casefold() in _DATA_TYPE_BY_NAME or value.casefold() in _DATA_TYPE_BY_DMS_TYPE
+
 
 class Boolean(DataType):
     name = "boolean"
     python = bool
     dms = dms.Boolean
     graphql = "Boolean"
-    xsd = "xsd:boolean"
+    xsd = "boolean"
     sql = "BOOLEAN"
 
 
 class Float(DataType):
     name = "float"
     python = float
     dms = dms.Float32
     graphql = "Float"
-    xsd = "xsd:float"
+    xsd = "float"
     sql = "FLOAT"
 
 
 class Double(DataType):
     name = "double"
     python = float
     dms = dms.Float64
     graphql = "Float"
-    xsd = "xsd:double"
+    xsd = "double"
     sql = "FLOAT"
 
 
 class Integer(DataType):
     name = "integer"
     python = int
     dms = dms.Int32
     graphql = "Int"
-    xsd = "xsd:integer"
+    xsd = "integer"
     sql = "INTEGER"
 
 
 class NonPositiveInteger(DataType):
     name = "nonPositiveInteger"
     python = int
     dms = dms.Int32
     graphql = "Int"
-    xsd = "xsd:nonPositiveInteger"
+    xsd = "nonPositiveInteger"
     sql = "INTEGER"
 
 
 class NonNegativeInteger(DataType):
     name = "nonNegativeInteger"
     python = int
     dms = dms.Int32
     graphql = "Int"
-    xsd = "xsd:nonNegativeInteger"
+    xsd = "nonNegativeInteger"
     sql = "INTEGER"
 
 
 class NegativeInteger(DataType):
     name = "negativeInteger"
     python = int
     dms = dms.Int32
     graphql = "Int"
-    xsd = "xsd:negativeInteger"
+    xsd = "negativeInteger"
     sql = "INTEGER"
 
 
 class Long(DataType):
     name = "long"
     python = int
     dms = dms.Int64
     graphql = "Int"
-    xsd = "xsd:long"
+    xsd = "long"
     sql = "BIGINT"
 
 
 class String(DataType):
     name = "string"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class LangString(DataType):
     name = "langString"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class AnyURI(DataType):
     name = "anyURI"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:anyURI"
+    xsd = "anyURI"
     sql = "STRING"
 
 
 class NormalizedString(DataType):
     name = "normalizedString"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:normalizedString"
+    xsd = "normalizedString"
     sql = "STRING"
 
 
 class Token(DataType):
     name = "token"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class DateTime(DataType):
     name = "dateTime"
     python = datetime
     dms = dms.Timestamp
     graphql = "Timestamp"
-    xsd = "xsd:dateTimeStamp"
+    xsd = "dateTimeStamp"
     sql = "TIMESTAMP"
 
 
-class DateTimeStamp(DataType):
-    name = "dateTimeStamp"
+class Timestamp(DataType):
+    name = "timestamp"
     python = datetime
     dms = dms.Timestamp
     graphql = "Timestamp"
-    xsd = "xsd:dateTimeStamp"
+    xsd = "dateTimeStamp"
     sql = "TIMESTAMP"
 
 
-class Timestamp(DataType):
-    name = "timestamp"
+class DateTimeStamp(DataType):
+    name = "dateTimeStamp"
     python = datetime
     dms = dms.Timestamp
     graphql = "Timestamp"
-    xsd = "xsd:dateTimeStamp"
+    xsd = "dateTimeStamp"
     sql = "TIMESTAMP"
 
 
 class Date(DataType):
     name = "date"
     python = date
     dms = dms.Date
     graphql = "String"
-    xsd = "xsd:date"
+    xsd = "date"
     sql = "DATE"
 
 
 class PlainLiteral(DataType):
     name = "PlainLiteral"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:string"
+    xsd = "plainLiteral"
     sql = "STRING"
 
 
 class Literal(DataType):
     name = "Literal"
     python = str
     dms = dms.Text
     graphql = "String"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class Timeseries(DataType):
     name = "timeseries"
     python = dms.TimeSeriesReference
     dms = dms.TimeSeriesReference
     graphql = "TimeSeries"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class File(DataType):
     name = "file"
     python = dms.FileReference
     dms = dms.FileReference
     graphql = "File"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class Sequence(DataType):
     name = "sequence"
     python = dms.SequenceReference
     dms = dms.SequenceReference
     graphql = "Sequence"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 class Json(DataType):
     name = "json"
     python = dms.Json
     dms = dms.Json
     graphql = "Json"
-    xsd = "xsd:string"
+    xsd = "string"
     sql = "STRING"
 
 
 _DATA_TYPE_BY_NAME = {cls.name.casefold(): cls for cls in DataType.__subclasses__()}
+_seen = set()
+_DATA_TYPE_BY_DMS_TYPE = {
+    cls.dms._type.casefold(): cls
+    for cls in DataType.__subclasses__()
+    if cls.dms._type not in _seen and not _seen.add(cls.dms._type)  # type: ignore[func-returns-value]
+}
+del _seen
+_XSD_TYPES = {cls_.xsd for cls_ in _DATA_TYPE_BY_NAME.values()}
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/entities.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rdfpath.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,299 +1,336 @@
+"""
+"""
+
 import re
 import sys
-import threading
-from abc import ABC, abstractmethod
+from collections import Counter
 from functools import total_ordering
-from typing import Annotated, Any, ClassVar, Generic, TypeVar
+from typing import ClassVar, Literal
+
+from pydantic import BaseModel, field_validator
 
-from cognite.client.data_classes.data_modeling.ids import ContainerId, DataModelId, PropertyId, ViewId
-from pydantic import BaseModel, BeforeValidator, Field, PlainSerializer, model_serializer, model_validator
+from cognite.neat.rules import exceptions
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
     from typing_extensions import Self
 
 
+class TransformationRuleType(StrEnum):
+    rdfpath = "rdfpath"
+    rawlookup = "rawlookup"
+    sparql = "sparql"
+
+
+class Lookup(StrEnum):
+    table = "table"
+    key = "key"
+    value = "value"  # type: ignore
+
+
 class EntityTypes(StrEnum):
-    view_non_versioned = "view_non_versioned"
-    subject = "subject"
-    predicate = "predicate"
-    object = "object"
     class_ = "class"
-    parent_class = "parent_class"
     property_ = "property"
-    object_property = "ObjectProperty"
-    data_property = "DatatypeProperty"
-    annotation_property = "AnnotationProperty"
-    object_value_type = "object_value_type"
-    data_value_type = "data_value_type"  # these are strings, floats, ...
-    xsd_value_type = "xsd_value_type"
-    dms_value_type = "dms_value_type"
-    view = "view"
-    reference_entity = "reference_entity"
-    container = "container"
-    datamodel = "datamodel"
     undefined = "undefined"
 
 
-# ALLOWED
-_ALLOWED_PATTERN = r"[^a-zA-Z0-9-_.]"
-
 # FOR PARSING STRINGS:
-_PREFIX_REGEX = r"[a-zA-Z]+[a-zA-Z0-9-_.]*[a-zA-Z0-9]+"
-_SUFFIX_REGEX = r"[a-zA-Z0-9-_.]+[a-zA-Z0-9]|[-_.]*[a-zA-Z0-9]+"
-_VERSION_REGEX = r"[a-zA-Z0-9]([.a-zA-Z0-9_-]{0,41}[a-zA-Z0-9])?"
-_PROPERTY_REGEX = r"[a-zA-Z0-9][a-zA-Z0-9_-]*[a-zA-Z0-9]?"
-_ENTITY_ID_REGEX = rf"{_PREFIX_REGEX}:({_SUFFIX_REGEX})"
-_ENTITY_ID_REGEX_COMPILED = re.compile(rf"^(?P<prefix>{_PREFIX_REGEX}):(?P<suffix>{_SUFFIX_REGEX})$")
-_VERSIONED_ENTITY_REGEX_COMPILED = re.compile(
-    rf"^(?P<prefix>{_PREFIX_REGEX}):(?P<suffix>{_SUFFIX_REGEX})\(version=(?P<version>{_VERSION_REGEX})\)$"
+PREFIX_REGEX = r"[a-zA-Z]+[a-zA-Z0-9-_.]*[a-zA-Z0-9]+"
+SUFFIX_REGEX = r"[a-zA-Z0-9-_.]+[a-zA-Z0-9]|[-_.]*[a-zA-Z0-9]+"
+VERSION_REGEX = r"[a-zA-Z0-9]([.a-zA-Z0-9_-]{0,41}[a-zA-Z0-9])?"
+
+ENTITY_ID_REGEX = rf"{PREFIX_REGEX}:({SUFFIX_REGEX})"
+ENTITY_ID_REGEX_COMPILED = re.compile(rf"^(?P<prefix>{PREFIX_REGEX}):(?P<suffix>{SUFFIX_REGEX})$")
+VERSIONED_ENTITY_REGEX_COMPILED = re.compile(
+    rf"^(?P<prefix>{PREFIX_REGEX}):(?P<suffix>{SUFFIX_REGEX})\(version=(?P<version>{VERSION_REGEX})\)$"
 )
-_CLASS_ID_REGEX = rf"(?P<{EntityTypes.class_}>{_ENTITY_ID_REGEX})"
-_CLASS_ID_REGEX_COMPILED = re.compile(rf"^{_CLASS_ID_REGEX}$")
-_PROPERTY_ID_REGEX = rf"\((?P<{EntityTypes.property_}>{_ENTITY_ID_REGEX})\)"
+CLASS_ID_REGEX = rf"(?P<{EntityTypes.class_}>{ENTITY_ID_REGEX})"
+CLASS_ID_REGEX_COMPILED = re.compile(rf"^{CLASS_ID_REGEX}$")
+PROPERTY_ID_REGEX = rf"\((?P<{EntityTypes.property_}>{ENTITY_ID_REGEX})\)"
 
-_ENTITY_PATTERN = re.compile(r"^(?P<prefix>.*?):?(?P<suffix>[^(:]*)(\((?P<content>[^)]+)\))?$")
+# traversal direction
+DIRECTION_REGEX = r"(?P<direction>(->|<-))"
 
+# steps
+STEP_REGEX = rf"((->|<-){CLASS_ID_REGEX}({PROPERTY_ID_REGEX})?)"
+STEP_REGEX_COMPILED = re.compile(STEP_REGEX)
+STEP_CLASS_REGEX_COMPILED = re.compile(rf"(^{DIRECTION_REGEX}{CLASS_ID_REGEX})$")
+STEP_CLASS_AND_PROPERTY_REGEX_COMPILED = re.compile(rf"(^{DIRECTION_REGEX}{CLASS_ID_REGEX}{PROPERTY_ID_REGEX}$)")
 
-class _Undefined(BaseModel):
-    ...
 
+_traversal = "traversal"
+ORIGIN_REGEX = rf"(?P<origin>{ENTITY_ID_REGEX})"
 
-class _Unknown(BaseModel):
-    def __str__(self) -> str:
-        return "#N/A"
+HOP_REGEX_COMPILED = re.compile(rf"^{ORIGIN_REGEX}(?P<{_traversal}>{STEP_REGEX}+)$")
 
+# grabbing specific property for a class, property can be either object, annotation or data property
+SINGLE_PROPERTY_REGEX_COMPILED = re.compile(rf"^{CLASS_ID_REGEX}{PROPERTY_ID_REGEX}$")
 
-# This is a trick to make Undefined and Unknown singletons
-Undefined = _Undefined()
-Unknown = _Unknown()
+# grabbing all properties for a class
+ALL_PROPERTIES_REGEX_COMPILED = re.compile(rf"^{CLASS_ID_REGEX}\(\*\)$")
 
+ALL_TRAVERSAL_REGEX_COMPILED = (
+    rf"({CLASS_ID_REGEX}\(\*\)|{CLASS_ID_REGEX}{PROPERTY_ID_REGEX}|{ORIGIN_REGEX}(?P<{_traversal}>{STEP_REGEX}+))"
+)
 
-@total_ordering
-class Entity(BaseModel):
-    """Entity is a class or property in OWL/RDF sense."""
+TABLE_REGEX_COMPILED = re.compile(
+    rf"^(?P<{Lookup.table}>{SUFFIX_REGEX})\((?P<{Lookup.key}>{SUFFIX_REGEX}),\s*(?P<{Lookup.value}>{SUFFIX_REGEX})\)$"
+)
 
-    type_: ClassVar[EntityTypes] = EntityTypes.undefined
-    prefix: str | _Undefined = Undefined
-    suffix: str | _Unknown
 
-    @classmethod
-    def load(cls, data: Any) -> Self:
-        return cls.model_validate(data)
+StepDirection = Literal["source", "target", "origin"]
+_direction_by_symbol: dict[str, StepDirection] = {"->": "target", "<-": "source"}
 
-    @model_validator(mode="before")
-    def _load(cls, data: Any) -> dict:
-        if isinstance(data, cls):
-            return data.model_dump()
-        elif isinstance(data, dict):
-            return data
-        elif hasattr(data, "versioned_id"):
-            # Todo: Remove. Is here for backwards compatibility
-            data = data.versioned_id
-        elif not isinstance(data, str):
-            raise ValueError(f"Cannot load {cls.__name__} from {data}")
-
-        return cls._parse(data)
-
-    @model_serializer(when_used="unless-none", return_type=str)
-    def as_str(self) -> str:
-        return str(self)
+Undefined = type(object())
+Unknown = type(object())
 
-    @classmethod
-    def _parse(cls, raw: str) -> dict:
-        if not (result := _ENTITY_PATTERN.match(raw)):
-            return dict(prefix=Undefined, suffix=Unknown)
-        prefix = result.group("prefix") or Undefined
-        suffix = result.group("suffix")
-        content = result.group("content")
-        if content is None:
-            return dict(prefix=prefix, suffix=suffix)
-        extra_args = dict(pair.strip().split("=") for pair in content.split(","))
-        expected_args = {field_.alias or field_name for field_name, field_ in cls.model_fields.items()}
-        for key in list(extra_args):
-            if key not in expected_args:
-                # Todo Warning about unknown key
-                del extra_args[key]
-        return dict(prefix=prefix, suffix=suffix, **extra_args)
-
-    def dump(self) -> str:
-        return str(self)
-
-    def as_tuple(self) -> tuple[str, ...]:
-        # We haver overwritten the serialization to str, so we need to do it manually
-        extra: tuple[str, ...] = tuple(
-            [
-                str(v or "")
-                for field_name in self.model_fields
-                if isinstance(v := getattr(self, field_name), str | None) and field_name not in {"prefix", "suffix"}
-            ]
-        )
-        if isinstance(self.prefix, _Undefined):
-            return str(self.suffix), *extra
-        else:
-            return self.prefix, str(self.suffix), *extra
+
+# mypy does not like the sentinel value, and it is not possible to ignore only the line with it below.
+# so we ignore all errors beyond this point.
+# mypy: ignore-errors
+@total_ordering
+class Entity(BaseModel, arbitrary_types_allowed=True):
+    """Entity is a class or property in OWL/RDF sense."""
+
+    type_: ClassVar[EntityTypes] = EntityTypes.undefined
+    prefix: str | Undefined = Undefined
+    suffix: str | Unknown
+    version: str | None = None
+    name: str | None = None
+    description: str | None = None
 
     def __lt__(self, other: object) -> bool:
-        if not isinstance(other, Entity):
+        if type(self) is not type(other) or not isinstance(other, Entity):
             return NotImplemented
-        return self.as_tuple() < other.as_tuple()
+        return self.versioned_id < other.versioned_id
 
     def __eq__(self, other: object) -> bool:
-        if not isinstance(other, Entity):
+        if type(self) is not type(other) or not isinstance(other, Entity):
             return NotImplemented
-        return self.as_tuple() == other.as_tuple()
+        return self.versioned_id == other.versioned_id
 
     def __hash__(self) -> int:
-        return hash(str(self))
+        return hash(self.versioned_id)
 
-    def __str__(self) -> str:
-        return self.id
-
-    def __repr__(self) -> str:
-        # We have overwritten the serialization to str, so we need to do it manually
-        model_dump = ((k, v) for k in self.model_fields if (v := getattr(self, k)) is not None)
-        args = ",".join([f"{k}={v}" for k, v in model_dump])
-        return f"{self.type_.value}({args})"
+    def as_non_versioned_entity(self) -> Self:
+        return self.from_string(f"{self.prefix}:{self.suffix}")
 
     @property
     def id(self) -> str:
-        # We have overwritten the serialization to str, so we need to do it manually
-        model_dump = (
-            (field.alias or field_name, v)
-            for field_name, field in self.model_fields.items()
-            if (v := getattr(self, field_name)) is not None and field_name not in {"prefix", "suffix"}
-        )
-        args = ",".join([f"{k}={v}" for k, v in model_dump])
-        if self.prefix is Undefined:
-            base_id = str(self.suffix)
+        if self.suffix is Unknown:
+            return "#N/A"
+        elif self.prefix is Undefined:
+            return self.suffix
         else:
-            base_id = f"{self.prefix}:{self.suffix!s}"
-        if args:
-            return f"{base_id}({args})"
-        else:
-            return base_id
+            return f"{self.prefix}:{self.suffix}"
 
     @property
     def versioned_id(self) -> str:
-        # Todo: Remove. Is here for backwards compatibility
-        return self.id
+        if self.version is None:
+            return self.id
+        else:
+            return f"{self.id}(version={self.version})"
+
+    @property
+    def space(self) -> str:
+        """Returns entity space in CDF."""
+        return self.prefix
+
+    @property
+    def external_id(self) -> str:
+        """Returns entity external id in CDF."""
+        return self.suffix
 
-    def as_non_versioned_entity(self) -> str:
-        # Todo: Remove. Is here for backwards compatibility
-        if self.prefix is Undefined:
-            return f"{self.suffix!s}"
-        return f"{self.prefix}:{self.suffix!s}"
+    def __repr__(self):
+        return self.versioned_id
 
+    def __str__(self):
+        return self.versioned_id
 
-class ClassEntity(Entity):
-    type_: ClassVar[EntityTypes] = EntityTypes.class_
-    version: str | None = None
+    @classmethod
+    def from_string(cls, entity_string: str, base_prefix: str | None = None) -> Self:
+        if entity_string == "#N/A":
+            return cls(prefix=Undefined, suffix=Unknown)
+        elif result := VERSIONED_ENTITY_REGEX_COMPILED.match(entity_string):
+            return cls(
+                prefix=result.group("prefix"),
+                suffix=result.group("suffix"),
+                version=result.group("version"),
+            )
+        elif result := ENTITY_ID_REGEX_COMPILED.match(entity_string):
+            return cls(prefix=result.group("prefix"), suffix=result.group("suffix"))
+        elif base_prefix and re.match(SUFFIX_REGEX, entity_string) and re.match(PREFIX_REGEX, base_prefix):
+            return cls(prefix=base_prefix, suffix=entity_string)
+        else:
+            raise ValueError(f"{cls.__name__} is expected to be prefix:suffix, got {entity_string}")
+
+    @classmethod
+    def from_list(cls, entity_strings: list[str], base_prefix: str | None = None) -> list[Self]:
+        return [
+            cls.from_string(entity_string=entity_string, base_prefix=base_prefix) for entity_string in entity_strings
+        ]
 
 
-class ParentClassEntity(ClassEntity):
-    type_: ClassVar[EntityTypes] = EntityTypes.parent_class
+class Step(BaseModel):
+    class_: Entity
+    property: Entity | None = None  # only terminal step has property
+    direction: StepDirection
 
-    def as_class_entity(self) -> ClassEntity:
-        return ClassEntity(prefix=self.prefix, suffix=self.suffix, version=self.version)
+    @classmethod
+    def from_string(cls, raw: str, **kwargs) -> Self:
+        if result := STEP_CLASS_AND_PROPERTY_REGEX_COMPILED.match(raw):
+            return cls(
+                class_=Entity.from_string(result.group(EntityTypes.class_)),
+                property=Entity.from_string(result.group(EntityTypes.property_)),
+                direction=_direction_by_symbol[result.group("direction")],
+                **kwargs,
+            )
+        elif result := STEP_CLASS_REGEX_COMPILED.match(raw):
+            return cls(
+                class_=Entity.from_string(result.group(EntityTypes.class_)),
+                direction=_direction_by_symbol[result.group("direction")],
+            )  # type: ignore
+        msg = f"Invalid step {raw}, expected in one of the following forms:"
+        msg += " ->prefix:suffix, <-prefix:suffix, ->prefix:suffix(prefix:suffix) or <-prefix:suffix(prefix:suffix)"
+        raise ValueError(msg)
 
 
-T_ID = TypeVar("T_ID", bound=ContainerId | ViewId | DataModelId | PropertyId)
+class Traversal(BaseModel):
+    class_: Entity
 
 
-class DMSEntity(Entity, Generic[T_ID], ABC):
-    type_: ClassVar[EntityTypes] = EntityTypes.undefined
-    default_space_by_thread: ClassVar[dict[threading.Thread, str]] = {}
-    suffix: str
+class SingleProperty(Traversal):
+    property: Entity
 
     @classmethod
-    def set_default_space(cls, space: str) -> None:
-        cls.default_space_by_thread[threading.current_thread()] = space
+    def from_string(cls, class_: str, property_: str) -> Self:
+        return cls(class_=Entity.from_string(class_), property=Entity.from_string(property_))
 
-    @property
-    def space(self) -> str:
-        """Returns entity space in CDF."""
-        if isinstance(self.prefix, _Undefined):
-            return self.default_space_by_thread.get(threading.current_thread(), "MISSING")
-        else:
-            return self.prefix
 
-    @property
-    def external_id(self) -> str:
-        """Returns entity external id in CDF."""
-        return self.suffix
+class AllReferences(Traversal):
+    @classmethod
+    def from_string(cls, class_: str) -> Self:
+        return cls(class_=Entity.from_string(class_))
 
-    @abstractmethod
-    def as_id(self) -> T_ID:
-        raise NotImplementedError("Method as_id must be implemented in subclasses")
 
+class AllProperties(Traversal):
+    @classmethod
+    def from_string(cls, class_: str) -> Self:
+        return cls(class_=Entity.from_string(class_))
 
-class ContainerEntity(DMSEntity[ContainerId]):
-    type_: ClassVar[EntityTypes] = EntityTypes.container
 
-    def as_id(self) -> ContainerId:
-        return ContainerId(space=self.space, external_id=self.external_id)
+class Origin(BaseModel):
+    class_: Entity
 
+    @field_validator("class_", mode="before")
+    def process_if_string(cls, value):
+        return Entity.from_string(value) if isinstance(value, str) else value
 
-class DMSVersionedEntity(DMSEntity[T_ID], ABC):
-    version: str | None = None
-    default_version_by_thread: ClassVar[dict[threading.Thread, str]] = {}
 
-    @property
-    def version_with_fallback(self) -> str:
-        if self.version is not None:
-            return self.version
-        return self.default_version_by_thread.get(threading.current_thread(), "MISSING")
+class Hop(Traversal):
+    """Multi or single hop traversal through graph"""
 
+    traversal: list[Step]
 
-class ViewEntity(DMSVersionedEntity[ViewId]):
-    type_: ClassVar[EntityTypes] = EntityTypes.view
+    @classmethod
+    def from_string(cls, class_: str, traversal: str | list[Step]) -> Self:
+        return cls(
+            class_=Entity.from_string(class_),
+            traversal=(
+                [Step.from_string(result[0]) for result in STEP_REGEX_COMPILED.findall(traversal)]
+                if isinstance(traversal, str)
+                else traversal
+            ),
+        )
 
-    def as_id(
-        self,
-    ) -> ViewId:
-        return ViewId(space=self.space, external_id=self.external_id, version=self.version_with_fallback)
 
+class TableLookup(BaseModel):
+    name: str
+    key: str
+    value: str
 
-class PropertyEntity(DMSVersionedEntity[PropertyId]):
-    type_: ClassVar[EntityTypes] = EntityTypes.property_
-    property_: str = Field(alias="property")
 
-    def as_id(self) -> PropertyId:
-        return PropertyId(
-            source=ViewId(self.space, self.external_id, self.version_with_fallback), property=self.property_
-        )
+class Rule(BaseModel):
+    pass
 
 
-class DataModelEntity(DMSVersionedEntity[DataModelId]):
-    type_: ClassVar[EntityTypes] = EntityTypes.datamodel
+class Query(BaseModel):
+    query: str
 
-    def as_id(self) -> DataModelId:
-        return DataModelId(space=self.space, external_id=self.external_id, version=self.version_with_fallback)
 
+class RDFPath(Rule):
+    traversal: Traversal | Query
 
-class ReferenceEntity(PropertyEntity):
-    type_: ClassVar[EntityTypes] = EntityTypes.reference_entity
 
+class RawLookup(RDFPath):
+    table: TableLookup
 
-def _split_str(v: Any) -> list[str]:
-    if isinstance(v, str):
-        return v.replace(", ", ",").split(",")
-    return v
 
+class SPARQLQuery(RDFPath):
+    traversal: Query
 
-def _join_str(v: list[ClassEntity]) -> str | None:
-    return ",".join([entry.id for entry in v]) if v else None
+
+def parse_traversal(raw: str) -> AllReferences | AllProperties | SingleProperty | Hop:
+    if result := CLASS_ID_REGEX_COMPILED.match(raw):
+        return AllReferences.from_string(class_=result.group(EntityTypes.class_))
+    elif result := ALL_PROPERTIES_REGEX_COMPILED.match(raw):
+        return AllProperties.from_string(class_=result.group(EntityTypes.class_))
+    elif result := SINGLE_PROPERTY_REGEX_COMPILED.match(raw):
+        return SingleProperty.from_string(
+            class_=result.group(EntityTypes.class_), property_=result.group(EntityTypes.property_)
+        )
+    elif result := HOP_REGEX_COMPILED.match(raw):
+        return Hop.from_string(class_=result.group("origin"), traversal=result.group(_traversal))
+    else:
+        raise exceptions.NotValidRDFPath(raw).to_pydantic_custom_error()
+
+
+def parse_table_lookup(raw: str) -> TableLookup:
+    if result := TABLE_REGEX_COMPILED.match(raw):
+        return TableLookup(
+            name=result.group(Lookup.table), key=result.group(Lookup.key), value=result.group(Lookup.value)
+        )
+    raise exceptions.NotValidTableLookUp(raw).to_pydantic_custom_error()
 
 
-ParentEntityList = Annotated[
-    list[ParentClassEntity],
-    BeforeValidator(_split_str),
-    PlainSerializer(
-        _join_str,
-        return_type=str,
-        when_used="unless-none",
-    ),
-]
+def parse_rule(rule_raw: str, rule_type: TransformationRuleType | None) -> RDFPath:
+    match rule_type:
+        case TransformationRuleType.rdfpath:
+            rule_raw = rule_raw.replace(" ", "")
+            return RDFPath(traversal=parse_traversal(rule_raw))
+        case TransformationRuleType.rawlookup:
+            rule_raw = rule_raw.replace(" ", "")
+            if Counter(rule_raw).get("|") != 1:
+                raise exceptions.NotValidRAWLookUp(rule_raw).to_pydantic_custom_error()
+            traversal, table_lookup = rule_raw.split("|")
+            return RawLookup(traversal=parse_traversal(traversal), table=parse_table_lookup(table_lookup))
+        case TransformationRuleType.sparql:
+            return SPARQLQuery(traversal=Query(query=rule_raw))
+        case None:
+            raise ValueError("Rule type must be specified")
+
+
+def is_valid_rule(rule_type: TransformationRuleType, rule_raw: str) -> bool:
+    is_valid_rule = {TransformationRuleType.rdfpath: is_rdfpath, TransformationRuleType.rawlookup: is_rawlookup}[
+        rule_type
+    ]
+    return is_valid_rule(rule_raw)
+
+
+def is_rdfpath(raw: str) -> bool:
+    try:
+        parse_traversal(raw)
+    except ValueError:
+        return False
+    return True
+
+
+def is_rawlookup(raw: str) -> bool:
+    try:
+        parse_rule(raw, TransformationRuleType.rawlookup)
+    except ValueError:
+        return False
+    return True
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/__init__.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_base.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     constr,
     field_validator,
     model_serializer,
     model_validator,
 )
 from pydantic.fields import FieldInfo
 
-from cognite.neat.rules.models.rules._types import ClassType
+from cognite.neat.rules.models.entities import ClassEntity
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
     from typing_extensions import Self
@@ -270,15 +270,15 @@
         exporting a reference model.
         """
         raise NotImplementedError
 
 
 # An sheet entity is either a class or a property.
 class SheetEntity(RuleModel):
-    class_: ClassType = Field(alias="Class")
+    class_: ClassEntity = Field(alias="Class")
     name: str | None = Field(alias="Name", default=None)
     description: str | None = Field(alias="Description", default=None)
 
     @field_validator("*", mode="before")
     def strip_string(cls, value: Any) -> Any:
         if isinstance(value, str):
             return value.strip()
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_architect_rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, cast
 
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import PropertyType as CognitePropertyType
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex
 from cognite.client.data_classes.data_modeling.views import SingleReverseDirectRelationApply, ViewPropertyApply
-from pydantic import Field, field_validator, model_serializer, model_validator
+from pydantic import Field, field_serializer, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo, ValidationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.rules import issues
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import (
+    ClassEntity,
+    ContainerEntity,
+    ContainerEntityList,
+    DMSUnknownEntity,
+    ParentClassEntity,
+    ReferenceEntity,
+    UnknownEntity,
+    URLEntity,
+    ViewEntity,
+    ViewEntityList,
+    ViewPropertyEntity,
+)
 from cognite.neat.rules.models.rules._domain_rules import DomainRules
 
 from ._base import BaseMetadata, BaseRules, ExtensionCategory, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
 from ._dms_schema import DMSSchema, PipelineSchema
 from ._types import (
-    CdfValueType,
-    ClassEntity,
-    ContainerEntity,
-    ContainerListType,
-    ContainerType,
-    DMSValueType,
     ExternalIdType,
-    ParentClassEntity,
     PropertyType,
-    ReferenceEntity,
-    ReferenceType,
     StrListType,
-    Undefined,
     VersionType,
-    ViewEntity,
-    ViewListType,
-    ViewPropEntity,
-    ViewType,
-    XSDValueType,
 )
 
 if TYPE_CHECKING:
     from ._information_rules import InformationRules
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
+_DEFAULT_VERSION = "1"
 
 subclasses = list(CognitePropertyType.__subclasses__())
 _PropertyType_by_name: dict[str, type[CognitePropertyType]] = {}
 for subclass in subclasses:
     subclasses.extend(subclass.__subclasses__())
     if abc.ABC in subclass.__bases__:
         continue
@@ -160,22 +160,22 @@
             updated=datetime.now(),
         )
 
 
 class DMSProperty(SheetEntity):
     property_: PropertyType = Field(alias="Property")
     relation: Literal["direct", "reversedirect", "multiedge"] | None = Field(None, alias="Relation")
-    value_type: CdfValueType = Field(alias="Value Type")
+    value_type: DataType | ViewPropertyEntity | ViewEntity | DMSUnknownEntity = Field(alias="Value Type")
     nullable: bool | None = Field(default=None, alias="Nullable")
     is_list: bool | None = Field(default=None, alias="IsList")
     default: str | int | dict | None = Field(None, alias="Default")
-    reference: ReferenceType = Field(default=None, alias="Reference")
-    container: ContainerType | None = Field(None, alias="Container")
+    reference: URLEntity | ReferenceEntity | None = Field(default=None, alias="Reference", union_mode="left_to_right")
+    container: ContainerEntity | None = Field(None, alias="Container")
     container_property: str | None = Field(None, alias="ContainerProperty")
-    view: ViewType = Field(alias="View")
+    view: ViewEntity = Field(alias="View")
     view_property: str = Field(alias="ViewProperty")
     index: StrListType | None = Field(None, alias="Index")
     constraint: StrListType | None = Field(None, alias="Constraint")
 
     @field_validator("nullable")
     def direct_relation_must_be_nullable(cls, value: Any, info: ValidationInfo) -> None:
         if info.data.get("relation") == "direct" and value is False:
@@ -185,38 +185,47 @@
     @field_validator("container_property", "container")
     def reverse_direct_relation_has_no_container(cls, value, info: ValidationInfo) -> None:
         if info.data.get("relation") == "reversedirect" and value is not None:
             raise ValueError(f"Reverse direct relation must not have container or container property, got {value}")
         return value
 
     @field_validator("value_type", mode="after")
-    def relations_value_type(cls, value: CdfValueType, info: ValidationInfo) -> CdfValueType:
+    def relations_value_type(cls, value: DataType | ClassEntity, info: ValidationInfo) -> DataType | ClassEntity:
         if (relation := info.data["relation"]) is None:
             return value
-        if not isinstance(value, ViewPropEntity):
+        if not isinstance(value, ViewEntity | ViewPropertyEntity | DMSUnknownEntity):
             raise ValueError(f"Relations must have a value type that points to another view, got {value}")
         if relation == "reversedirect" and value.property_ is None:
+            # Todo fix this error message. It have the wrong syntax for how to have a property
             raise ValueError(
                 "Reverse direct relation must set what it is the reverse property of. "
                 f"Which property in {value.versioned_id} is this the reverse of? Expecting"
                 f"{value.versioned_id}:<property>"
             )
         return value
 
+    @field_serializer("value_type", when_used="always")
+    @staticmethod
+    def as_dms_type(value_type: DataType | ViewPropertyEntity | ViewEntity) -> str:
+        if isinstance(value_type, DataType):
+            return value_type.dms._type
+        else:
+            return str(value_type)
+
 
 class DMSContainer(SheetEntity):
-    container: ContainerType = Field(alias="Container")
-    reference: ReferenceType = Field(alias="Reference", default=None)
-    constraint: ContainerListType | None = Field(None, alias="Constraint")
+    container: ContainerEntity = Field(alias="Container")
+    reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
+    constraint: ContainerEntityList | None = Field(None, alias="Constraint")
 
-    def as_container(self, default_space: str) -> dm.ContainerApply:
-        container_id = self.container.as_id(default_space)
+    def as_container(self) -> dm.ContainerApply:
+        container_id = self.container.as_id()
         constraints: dict[str, dm.Constraint] = {}
         for constraint in self.constraint or []:
-            requires = dm.RequiresConstraint(constraint.as_id(default_space))
+            requires = dm.RequiresConstraint(constraint.as_id())
             constraints[f"{constraint.space}_{constraint.external_id}"] = requires
 
         return dm.ContainerApply(
             space=container_id.space,
             external_id=container_id.external_id,
             name=self.name or None,
             description=self.description,
@@ -229,50 +238,51 @@
         constraints: list[ContainerEntity] = []
         for _, constraint_obj in (container.constraints or {}).items():
             if isinstance(constraint_obj, dm.RequiresConstraint):
                 constraints.append(ContainerEntity.from_id(constraint_obj.require))
             # UniquenessConstraint it handled in the properties
         return cls(
             class_=ClassEntity(prefix=container.space, suffix=container.external_id),
-            container=ContainerType(prefix=container.space, suffix=container.external_id),
+            container=ContainerEntity(space=container.space, externalId=container.external_id),
             name=container.name or None,
             description=container.description,
             constraint=constraints or None,
         )
 
 
 class DMSView(SheetEntity):
-    view: ViewType = Field(alias="View")
-    implements: ViewListType | None = Field(None, alias="Implements")
-    reference: ReferenceType = Field(alias="Reference", default=None)
+    view: ViewEntity = Field(alias="View")
+    implements: ViewEntityList | None = Field(None, alias="Implements")
+    reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     filter_: Literal["hasData", "nodeType"] | None = Field(None, alias="Filter")
     in_model: bool = Field(True, alias="InModel")
 
-    def as_view(self, default_space: str, default_version: str) -> dm.ViewApply:
-        view_id = self.view.as_id(False, default_space, default_version)
+    def as_view(self) -> dm.ViewApply:
+        view_id = self.view.as_id()
         return dm.ViewApply(
             space=view_id.space,
             external_id=view_id.external_id,
-            version=view_id.version or default_version,
+            version=view_id.version or _DEFAULT_VERSION,
             name=self.name or None,
             description=self.description,
-            implements=[parent.as_id(False, default_space, default_version) for parent in self.implements or []]
-            or None,
+            implements=[parent.as_id() for parent in self.implements or []] or None,
             properties={},
         )
 
     @classmethod
     def from_view(cls, view: dm.ViewApply, data_model_view_ids: set[dm.ViewId]) -> "DMSView":
         return cls(
             class_=ClassEntity(prefix=view.space, suffix=view.external_id),
-            view=ViewType(prefix=view.space, suffix=view.external_id, version=view.version),
+            view=ViewEntity(space=view.space, externalId=view.external_id, version=view.version),
             description=view.description,
             name=view.name,
             implements=[
-                ViewType(prefix=parent.space, suffix=parent.external_id, version=parent.version)
+                ViewEntity(
+                    space=parent.space, externalId=parent.external_id, version=parent.version or _DEFAULT_VERSION
+                )
                 for parent in view.implements
             ]
             or None,
             in_model=view.as_id() in data_model_view_ids,
         )
 
 
@@ -280,104 +290,34 @@
     metadata: DMSMetadata = Field(alias="Metadata")
     properties: SheetList[DMSProperty] = Field(alias="Properties")
     views: SheetList[DMSView] = Field(alias="Views")
     containers: SheetList[DMSContainer] | None = Field(None, alias="Containers")
     reference: "DMSRules | None" = Field(None, alias="Reference")
 
     @model_validator(mode="after")
-    def set_default_space_and_version(self) -> "DMSRules":
-        default_space = self.metadata.space
-        default_view_version = self.metadata.default_view_version
-        for entity in self.properties:
-            if entity.class_.prefix is Undefined or entity.class_.version is None:
-                entity.class_ = ClassEntity(
-                    prefix=default_space if entity.class_.prefix is Undefined else entity.class_.prefix,
-                    suffix=entity.class_.suffix,
-                    version=default_view_version if entity.class_.version is None else entity.class_.version,
-                )
-            if entity.container and entity.container.space is Undefined:
-                entity.container = ContainerEntity(prefix=default_space, suffix=entity.container.external_id)
-
-            if entity.view and (entity.view.space is Undefined or entity.view.version is None):
-                entity.view = ViewEntity(
-                    prefix=default_space if entity.view.space is Undefined else entity.view.space,
-                    suffix=entity.view.external_id,
-                    version=default_view_version if entity.view.version is None else entity.view.version,
-                )
-            if isinstance(entity.value_type, ViewPropEntity) and (
-                entity.value_type.space is Undefined or entity.value_type.version is None
-            ):
-                entity.value_type = ViewPropEntity(
-                    prefix=default_space if entity.value_type.space is Undefined else entity.value_type.space,
-                    suffix=entity.value_type.suffix,
-                    version=default_view_version if entity.value_type.version is None else entity.value_type.version,
-                    property_=entity.value_type.property_,
-                )
-
-        for container in self.containers or []:
-            if container.class_.prefix is Undefined:
-                container.class_ = ClassEntity(prefix=default_space, suffix=container.class_.suffix)
-            if container.container.space is Undefined:
-                container.container = ContainerEntity(prefix=default_space, suffix=container.container.external_id)
-            container.constraint = [
-                (
-                    ContainerEntity(prefix=default_space, suffix=constraint.external_id)
-                    if constraint.space is Undefined
-                    else constraint
-                )
-                for constraint in container.constraint or []
-            ] or None
-
-        for view in self.views or []:
-            if view.class_.prefix is Undefined or view.class_.version is None:
-                view.class_ = ClassEntity(
-                    prefix=default_space if view.class_.prefix is Undefined else view.class_.prefix,
-                    suffix=view.class_.suffix,
-                    version=default_view_version if view.class_.version is None else view.class_.version,
-                )
-
-            if view.view.space is Undefined or view.view.version is None:
-                view.view = ViewEntity(
-                    prefix=default_space if view.view.space is Undefined else view.view.space,
-                    suffix=view.view.external_id,
-                    version=default_view_version if view.view.version is None else view.view.version,
-                )
-            view.implements = [
-                (
-                    ViewEntity(
-                        prefix=default_space if parent.space is Undefined else parent.space,
-                        suffix=parent.external_id,
-                        version=default_view_version if parent.version is None else parent.version,
-                    )
-                    if parent.space is Undefined or parent.version is None
-                    else parent
-                )
-                for parent in view.implements or []
-            ] or None
-
-        return self
-
-    @model_validator(mode="after")
     def consistent_container_properties(self) -> "DMSRules":
         container_properties_by_id: dict[tuple[ContainerEntity, str], list[tuple[int, DMSProperty]]] = defaultdict(list)
         for prop_no, prop in enumerate(self.properties):
             if prop.container and prop.container_property:
                 container_properties_by_id[(prop.container, prop.container_property)].append((prop_no, prop))
 
         errors: list[cognite.neat.rules.issues.spreadsheet.InconsistentContainerDefinitionError] = []
         for (container, prop_name), properties in container_properties_by_id.items():
             if len(properties) == 1:
                 continue
-            container_id = container.as_id(self.metadata.space)
+            container_id = container.as_id()
             row_numbers = {prop_no for prop_no, _ in properties}
             value_types = {prop.value_type for _, prop in properties if prop.value_type}
             if len(value_types) > 1:
                 errors.append(
                     cognite.neat.rules.issues.spreadsheet.MultiValueTypeError(
-                        container_id, prop_name, row_numbers, {str(v) for v in value_types}
+                        container_id,
+                        prop_name,
+                        row_numbers,
+                        {v.dms._type if isinstance(v, DataType) else str(v) for v in value_types},
                     )
                 )
             list_definitions = {prop.is_list for _, prop in properties if prop.is_list is not None}
             if len(list_definitions) > 1:
                 errors.append(
                     cognite.neat.rules.issues.spreadsheet.MultiValueIsListError(
                         container_id, prop_name, row_numbers, list_definitions
@@ -433,60 +373,54 @@
         if errors:
             raise issues.MultiValueError(errors)
         return self
 
     @model_validator(mode="after")
     def referenced_views_and_containers_are_existing(self) -> "DMSRules":
         # There two checks are done in the same method to raise all the errors at once.
-        defined_views = {view.view.as_id(False, self.metadata.space, self.metadata.version) for view in self.views}
+        defined_views = {view.view.as_id() for view in self.views}
 
         errors: list[issues.NeatValidationError] = []
         for prop_no, prop in enumerate(self.properties):
-            if (
-                prop.view
-                and (view_id := prop.view.as_id(False, self.metadata.space, self.metadata.version)) not in defined_views
-            ):
+            if prop.view and (view_id := prop.view.as_id()) not in defined_views:
                 errors.append(
                     cognite.neat.rules.issues.spreadsheet.NonExistingViewError(
                         column="View",
                         row=prop_no,
                         type="value_error.missing",
                         view_id=view_id,
                         msg="",
                         input=None,
                         url=None,
                     )
                 )
         if self.metadata.schema_ is SchemaCompleteness.complete:
-            defined_containers = {container.container.as_id(self.metadata.space) for container in self.containers or []}
+            defined_containers = {container.container.as_id() for container in self.containers or []}
             for prop_no, prop in enumerate(self.properties):
-                if (
-                    prop.container
-                    and (container_id := prop.container.as_id(self.metadata.space)) not in defined_containers
-                ):
+                if prop.container and (container_id := prop.container.as_id()) not in defined_containers:
                     errors.append(
                         cognite.neat.rules.issues.spreadsheet.NonExistingContainerError(
                             column="Container",
                             row=prop_no,
                             type="value_error.missing",
                             container_id=container_id,
                             msg="",
                             input=None,
                             url=None,
                         )
                     )
             for _container_no, container in enumerate(self.containers or []):
                 for constraint_no, constraint in enumerate(container.constraint or []):
-                    if constraint.as_id(self.metadata.space) not in defined_containers:
+                    if constraint.as_id() not in defined_containers:
                         errors.append(
                             cognite.neat.rules.issues.spreadsheet.NonExistingContainerError(
                                 column="Constraint",
                                 row=constraint_no,
                                 type="value_error.missing",
-                                container_id=constraint.as_id(self.metadata.space),
+                                container_id=constraint.as_id(),
                                 msg="",
                                 input=None,
                                 url=None,
                             )
                         )
         if errors:
             raise issues.MultiValueError(errors)
@@ -580,25 +514,23 @@
             if not self.reference:
                 raise ValueError(
                     "The schema is set to 'extended', but no reference rules are provided to validate against"
                 )
             # This is an extension of the reference rules, we need to merge the two
             rules = self.model_copy(deep=True)
             rules.properties.extend(self.reference.properties.data)
-            existing_views = {view.view.as_id(False) for view in rules.views}
-            rules.views.extend([view for view in self.reference.views if view.view.as_id(False) not in existing_views])
+            existing_views = {view.view.as_id() for view in rules.views}
+            rules.views.extend([view for view in self.reference.views if view.view.as_id() not in existing_views])
             if rules.containers and self.reference.containers:
-                existing_containers = {
-                    container.container.as_id(self.metadata.space) for container in rules.containers.data
-                }
+                existing_containers = {container.container.as_id() for container in rules.containers.data}
                 rules.containers.extend(
                     [
                         container
                         for container in self.reference.containers
-                        if container.container.as_id(self.reference.metadata.space) not in existing_containers
+                        if container.container.as_id() not in existing_containers
                     ]
                 )
             elif not rules.containers and self.reference.containers:
                 rules.containers = self.reference.containers
         else:
             raise ValueError("Unknown schema completeness")
 
@@ -679,15 +611,15 @@
     def as_domain_expert_rules(self) -> DomainRules:
         return _DMSRulesConverter(self).as_domain_rules()
 
     def reference_self(self) -> Self:
         new_rules = self.model_copy(deep=True)
         for prop in new_rules.properties:
             prop.reference = ReferenceEntity(
-                prefix=prop.view.prefix, suffix=prop.view.suffix, version=prop.view.version, property_=prop.property_
+                prefix=prop.view.prefix, suffix=prop.view.suffix, version=prop.view.version, property=prop.property_
             )
         view: DMSView
         for view in new_rules.views:
             view.reference = ReferenceEntity(
                 prefix=view.view.prefix, suffix=view.view.suffix, version=view.view.version
             )
         container: DMSContainer
@@ -709,30 +641,21 @@
     """
 
     def __init__(self, include_pipeline: bool = False, instance_space: str | None = None):
         self.include_pipeline = include_pipeline
         self.instance_space = instance_space
 
     def to_schema(self, rules: DMSRules) -> DMSSchema:
-        default_version = "1"
-        default_space = rules.metadata.space
-
-        container_properties_by_id, view_properties_by_id = self._gather_properties(
-            rules, default_space, default_version
-        )
+        container_properties_by_id, view_properties_by_id = self._gather_properties(rules)
 
-        containers = self._create_containers(rules.containers, container_properties_by_id, default_space)
+        containers = self._create_containers(rules.containers, container_properties_by_id)
 
-        views, node_types = self._create_views_with_node_types(
-            rules.views, view_properties_by_id, default_space, default_version
-        )
+        views, node_types = self._create_views_with_node_types(rules.views, view_properties_by_id)
 
-        views_not_in_model = {
-            view.view.as_id(False, default_space, default_version) for view in rules.views if not view.in_model
-        }
+        views_not_in_model = {view.view.as_id() for view in rules.views if not view.in_model}
         data_model = rules.metadata.as_data_model()
         data_model.views = sorted(
             [view_id for view_id in views.as_ids() if view_id not in views_not_in_model], key=lambda v: v.as_tuple()  # type: ignore[union-attr]
         )
 
         spaces = self._create_spaces(rules.metadata, containers, views, data_model)
 
@@ -766,137 +689,143 @@
             spaces.append(dm.SpaceApply(space=self.instance_space, name=self.instance_space))
         return spaces
 
     def _create_views_with_node_types(
         self,
         dms_views: SheetList[DMSView],
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]],
-        default_space: str,
-        default_version: str,
     ) -> tuple[dm.ViewApplyList, dm.NodeApplyList]:
-        views = dm.ViewApplyList([dms_view.as_view(default_space, default_version) for dms_view in dms_views])
-        dms_view_by_id = {
-            dms_view.view.as_id(False, default_space, default_version): dms_view for dms_view in dms_views
-        }
+        views = dm.ViewApplyList([dms_view.as_view() for dms_view in dms_views])
+        dms_view_by_id = {dms_view.view.as_id(): dms_view for dms_view in dms_views}
 
         for view in views:
             view_id = view.as_id()
             view.properties = {}
             if not (view_properties := view_properties_by_id.get(view_id)):
                 continue
             for prop in view_properties:
                 view_property: ViewPropertyApply
                 if prop.is_list and prop.relation == "direct":
                     # This is not yet supported in the CDF API, a warning has already been issued, here we convert it to
                     # a multi-edge connection.
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version)
+                        source_view_id = prop.value_type.as_id()
+                    elif isinstance(prop.value_type, ViewPropertyEntity):
+                        source_view_id = prop.value_type.as_view_id()
                     else:
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MultiEdgeConnectionApply(
                         type=dm.DirectRelationReference(
-                            space=source.space,
+                            space=source_view_id.space,
                             external_id=f"{prop.view.external_id}.{prop.view_property}",
                         ),
-                        source=source,
+                        source=source_view_id,
                         direction="outwards",
                         name=prop.name,
                         description=prop.description,
                     )
                 elif prop.container and prop.container_property and prop.view_property:
                     container_prop_identifier = prop.container_property
                     extra_args: dict[str, Any] = {}
                     if prop.relation == "direct" and isinstance(prop.value_type, ViewEntity):
-                        extra_args["source"] = prop.value_type.as_id(True, default_space, default_version)
+                        extra_args["source"] = prop.value_type.as_id()
+                    elif isinstance(prop.value_type, DMSUnknownEntity):
+                        extra_args["source"] = None
                     elif prop.relation == "direct" and not isinstance(prop.value_type, ViewEntity):
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MappedPropertyApply(
-                        container=prop.container.as_id(default_space),
+                        container=prop.container.as_id(),
                         container_property_identifier=container_prop_identifier,
                         name=prop.name,
                         description=prop.description,
                         **extra_args,
                     )
                 elif prop.view and prop.view_property and prop.relation == "multiedge":
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version)
+                        source_view_id = prop.value_type.as_id()
                     else:
                         raise ValueError(
                             "Multiedge relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     if isinstance(prop.reference, ReferenceEntity):
-                        ref_view_prop = prop.reference.as_prop_id(default_space, default_version)
+                        ref_view_prop = prop.reference.as_view_property_id()
                         edge_type = dm.DirectRelationReference(
                             space=ref_view_prop.source.space,
                             external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
                         )
                     else:
                         edge_type = dm.DirectRelationReference(
-                            space=source.space,
+                            space=source_view_id.space,
                             external_id=f"{prop.view.external_id}.{prop.view_property}",
                         )
 
                     view_property = dm.MultiEdgeConnectionApply(
                         type=edge_type,
-                        source=source,
+                        source=source_view_id,
                         direction="outwards",
                         name=prop.name,
                         description=prop.description,
                     )
                 elif prop.view and prop.view_property and prop.relation == "reversedirect":
-                    if isinstance(prop.value_type, ViewPropEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version)
+                    if isinstance(prop.value_type, ViewPropertyEntity):
+                        source_prop_id = prop.value_type.as_id()
+                        source_view_id = cast(dm.ViewId, source_prop_id.source)
                     else:
                         raise ValueError(
                             "Reverse direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     source_prop = prop.value_type.property_
                     if source_prop is None:
                         raise ValueError(
                             "Reverse direct relation must set what it is the reverse property of. "
                             f"Which property in {prop.value_type.versioned_id} is this the reverse of? Expecting "
                             f"{prop.value_type.versioned_id}:<property>"
                         )
                     reverse_prop = next(
-                        (prop for prop in view_properties_by_id.get(source, []) if prop.property_ == source_prop), None
+                        (
+                            prop
+                            for prop in view_properties_by_id.get(source_view_id, [])
+                            if prop.property_ == source_prop
+                        ),
+                        None,
                     )
                     if reverse_prop and reverse_prop.relation == "direct" and reverse_prop.is_list:
                         warnings.warn(
                             issues.dms.ReverseOfDirectRelationListWarning(view_id, prop.property_), stacklevel=2
                         )
                         if isinstance(reverse_prop.reference, ReferenceEntity):
-                            ref_view_prop = reverse_prop.reference.as_prop_id(default_space, default_version)
+                            ref_view_prop = reverse_prop.reference.as_view_property_id()
                             edge_type = dm.DirectRelationReference(
                                 space=ref_view_prop.source.space,
                                 external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
                             )
                         else:
                             edge_type = dm.DirectRelationReference(
-                                space=source.space,
+                                space=source_prop_id.source.space,
                                 external_id=f"{reverse_prop.view.external_id}.{reverse_prop.view_property}",
                             )
                         view_property = dm.MultiEdgeConnectionApply(
                             type=edge_type,
-                            source=source,
+                            source=source_prop_id.source,  # type: ignore[arg-type]
                             direction="inwards",
                             name=prop.name,
                             description=prop.description,
                         )
                     else:
                         args: dict[str, Any] = dict(
-                            source=source,
-                            through=dm.PropertyId(source, source_prop),
+                            source=source_view_id,
+                            through=dm.PropertyId(source_prop_id.source, source_prop),
                             description=prop.description,
                             name=prop.name,
                         )
                         reverse_direct_cls: dict[
                             bool | None,
                             type[dm.MultiReverseDirectRelationApply] | type[SingleReverseDirectRelationApply],
                         ] = {
@@ -921,15 +850,15 @@
         for view in views:
             ref_containers = sorted(view.referenced_containers(), key=lambda c: c.as_tuple())
             dms_view = dms_view_by_id.get(view.as_id())
             has_data = dm.filters.HasData(containers=list(ref_containers)) if ref_containers else None
             if dms_view and isinstance(dms_view.reference, ReferenceEntity):
                 # If the view is a reference, we implement the reference view,
                 # and need the filter to match the reference
-                ref_view = dms_view.reference.as_id(False, default_space, default_version)
+                ref_view = dms_view.reference.as_view_id()
                 node_type = dm.filters.Equals(
                     ["node", "type"], {"space": ref_view.space, "externalId": ref_view.external_id}
                 )
             else:
                 node_type = dm.filters.Equals(["node", "type"], {"space": view.space, "externalId": view.external_id})
             if view.as_id() in parent_views:
                 if dms_view and dms_view.filter_ == "nodeType":
@@ -955,30 +884,27 @@
                     view.filter = has_data
         return views, node_types
 
     def _create_containers(
         self,
         dms_container: SheetList[DMSContainer] | None,
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]],
-        default_space: str,
     ) -> dm.ContainerApplyList:
-        containers = dm.ContainerApplyList(
-            [dms_container.as_container(default_space) for dms_container in dms_container or []]
-        )
+        containers = dm.ContainerApplyList([dms_container.as_container() for dms_container in dms_container or []])
         container_to_drop = set()
         for container in containers:
             container_id = container.as_id()
             if not (container_properties := container_properties_by_id.get(container_id)):
                 warnings.warn(issues.dms.EmptyContainerWarning(container_id=container_id), stacklevel=2)
                 container_to_drop.add(container_id)
                 continue
             for prop in container_properties:
                 if prop.container_property is None:
                     continue
-                if isinstance(prop.value_type, DMSValueType):
+                if isinstance(prop.value_type, DataType):
                     type_cls = prop.value_type.dms
                 else:
                     type_cls = dm.DirectRelation
 
                 prop_id = prop.container_property
 
                 if type_cls is dm.DirectRelation:
@@ -1028,34 +954,34 @@
                     if not (isinstance(const, dm.RequiresConstraint) and const.require in container_to_drop)
                 }
         return dm.ContainerApplyList(
             [container for container in containers if container.as_id() not in container_to_drop]
         )
 
     def _gather_properties(
-        self, rules: DMSRules, default_space: str, default_version: str
+        self, rules: DMSRules
     ) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]] = defaultdict(list)
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]] = defaultdict(list)
         for prop in rules.properties:
-            view_id = prop.view.as_id(False, default_space, default_version)
+            view_id = prop.view.as_id()
             view_properties_by_id[view_id].append(prop)
 
             if prop.container and prop.container_property:
                 if prop.relation == "direct" and prop.is_list:
                     warnings.warn(
                         issues.dms.DirectRelationListWarning(
-                            container_id=prop.container.as_id(default_space),
-                            view_id=prop.view.as_id(False, default_space, default_version),
+                            container_id=prop.container.as_id(),
+                            view_id=prop.view.as_id(),
                             property=prop.container_property,
                         ),
                         stacklevel=2,
                     )
                     continue
-                container_id = prop.container.as_id(default_space)
+                container_id = prop.container.as_id()
                 container_properties_by_id[container_id].append(prop)
 
         return container_properties_by_id, view_properties_by_id
 
 
 class _DMSRulesConverter:
     def __init__(self, dms: DMSRules):
@@ -1086,46 +1012,49 @@
             created=dms.created or created or datetime.now(),
             updated=dms.updated or updated or datetime.now(),
         )
 
         classes = [
             InformationClass(
                 # we do not want a version in class as we use URI for the class
-                class_=view.class_.as_non_versioned_entity(),
+                class_=ClassEntity(prefix=view.class_.prefix, suffix=view.class_.suffix),
                 description=view.description,
                 parent=[
                     # we do not want a version in class as we use URI for the class
                     ParentClassEntity(prefix=implemented_view.prefix, suffix=implemented_view.suffix)
                     # We only want parents in the same namespace, parent in a different namespace is a reference
                     for implemented_view in view.implements or []
                     if implemented_view.prefix == view.class_.prefix
                 ],
                 reference=self._get_class_reference(view),
             )
             for view in self.dms.views
         ]
 
         properties: list[InformationProperty] = []
-        value_type: XSDValueType | ClassEntity | str
+        value_type: DataType | ClassEntity | str
         for property_ in self.dms.properties:
-            if isinstance(property_.value_type, DMSValueType):
-                value_type = cast(DMSValueType, property_.value_type).xsd
-            elif isinstance(property_.value_type, ViewEntity):
+            if isinstance(property_.value_type, DataType):
+                value_type = property_.value_type
+            elif isinstance(property_.value_type, ViewEntity | ViewPropertyEntity):
                 value_type = ClassEntity(
                     prefix=property_.value_type.prefix,
                     suffix=property_.value_type.suffix,
                 )
+            elif isinstance(property_.value_type, DMSUnknownEntity):
+                value_type = UnknownEntity()
             else:
                 raise ValueError(f"Unsupported value type: {property_.value_type.type_}")
 
             properties.append(
                 InformationProperty(
-                    class_=property_.class_.as_non_versioned_entity(),
+                    # Removing version
+                    class_=ClassEntity(suffix=property_.class_.suffix, prefix=property_.class_.prefix),
                     property_=property_.view_property,
-                    value_type=cast(XSDValueType | ClassEntity, value_type),
+                    value_type=value_type,
                     description=property_.description,
                     min_count=0 if property_.nullable or property_.nullable is None else 1,
                     max_count=float("inf") if property_.is_list or property_.nullable is None else 1,
                     reference=self._get_property_reference(property_),
                 )
             )
 
@@ -1157,9 +1086,9 @@
         has_container_other_namespace = property_.container and property_.container.prefix != property_.class_.prefix
         if not has_container_other_namespace:
             return None
         container = cast(ContainerEntity, property_.container)
         return ReferenceEntity(
             prefix=container.prefix,
             suffix=container.suffix,
-            property_=property_.container_property,
+            property=property_.container_property,
         )
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_schema.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     MissingContainerPropertyError,
     MissingEdgeViewError,
     MissingParentViewError,
     MissingSourceViewError,
     MissingSpaceError,
     MissingViewError,
 )
-from cognite.neat.rules.models.rules._types._value import DMS_VALUE_TYPE_MAPPINGS
+from cognite.neat.rules.models.data_types import _DATA_TYPE_BY_DMS_TYPE
 from cognite.neat.utils.cdf_loaders import ViewLoader
 from cognite.neat.utils.cdf_loaders.data_classes import RawTableWrite, RawTableWriteList
 from cognite.neat.utils.text import to_camel
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
@@ -573,16 +573,16 @@
             {"from": "externalId", "to": "externalId", "asType": "STRING"},
         ]
         select_rows = ["cast(`externalId` as STRING) as externalId"]
         for prop_name, prop in properties.items():
             container = container_by_id.get(prop.container)
             if container is not None:
                 dms_type = container.properties[prop.container_property_identifier].type._type
-                if dms_type in DMS_VALUE_TYPE_MAPPINGS:
-                    sql_type = DMS_VALUE_TYPE_MAPPINGS[dms_type].sql
+                if dms_type in _DATA_TYPE_BY_DMS_TYPE:
+                    sql_type = _DATA_TYPE_BY_DMS_TYPE[dms_type].sql
                 else:
                     warnings.warn(
                         f"Unknown DMS type '{dms_type}' for property '{prop_name}'", RuntimeWarning, stacklevel=2
                     )
                     sql_type = "STRING"
             else:
                 sql_type = "STRING"
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_domain_rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import math
 from typing import Any, ClassVar
 
 from pydantic import Field, field_serializer, field_validator, model_serializer
 from pydantic_core.core_schema import SerializationInfo
 
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import ClassEntity, ParentEntityList
+
 from ._base import (
     BaseMetadata,
     RoleTypes,
     RuleModel,
     SheetEntity,
     SheetList,
 )
-from ._types import ParentClassType, PropertyType, SemanticValueType, StrOrListType
+from ._types import PropertyType, StrOrListType
 
 
 class DomainMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.domain_expert
     creator: StrOrListType
 
 
 class DomainProperty(SheetEntity):
     property_: PropertyType = Field(alias="Property")
-    value_type: SemanticValueType = Field(alias="Value Type")
+    value_type: DataType | ClassEntity = Field(alias="Value Type")
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
 
     @field_serializer("max_count", when_used="json-unless-none")
     def serialize_max_count(self, value: int | float | None) -> int | float | None | str:
         if isinstance(value, float) and math.isinf(value):
             return None
@@ -36,15 +39,15 @@
         if value is None:
             return float("inf")
         return value
 
 
 class DomainClass(SheetEntity):
     description: str | None = Field(None, alias="Description")
-    parent: ParentClassType = Field(alias="Parent Class")
+    parent: ParentEntityList | None = Field(alias="Parent Class")
 
 
 class DomainRules(RuleModel):
     metadata: DomainMetadata = Field(alias="Metadata")
     properties: SheetList[DomainProperty] = Field(alias="Properties")
     classes: SheetList[DomainClass] | None = Field(None, alias="Classes")
     reference: "DomainRules | None" = Field(None, alias="Reference")
```

### Comparing `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_information_rules.py` & `cognite_neat-0.75.8/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,33 @@
 from pydantic import Field, field_serializer, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.constants import PREFIXES
 from cognite.neat.rules import exceptions
+from cognite.neat.rules.models.data_types import DataType
+from cognite.neat.rules.models.entities import (
+    ClassEntity,
+    ContainerEntity,
+    DMSUnknownEntity,
+    Entity,
+    EntityTypes,
+    ParentClassEntity,
+    ParentEntityList,
+    ReferenceEntity,
+    Undefined,
+    Unknown,
+    UnknownEntity,
+    URLEntity,
+    ViewEntity,
+    ViewPropertyEntity,
+    _UndefinedType,
+    _UnknownType,
+)
 from cognite.neat.rules.models.rdfpath import (
     AllReferences,
     Hop,
     RawLookup,
     SingleProperty,
     SPARQLQuery,
     TransformationRuleType,
@@ -33,34 +52,20 @@
     RuleModel,
     SchemaCompleteness,
     SheetEntity,
     SheetList,
 )
 from ._domain_rules import DomainRules
 from ._types import (
-    ClassEntity,
-    ContainerEntity,
-    Entity,
-    EntityTypes,
     NamespaceType,
-    ParentClassEntity,
-    ParentClassType,
     PrefixType,
     PropertyType,
-    ReferenceEntity,
-    ReferenceType,
-    SemanticValueType,
     StrListType,
-    Undefined,
     VersionType,
-    ViewEntity,
-    ViewPropEntity,
-    XSDValueType,
 )
-from ._types._base import Unknown
 
 if TYPE_CHECKING:
     from ._dms_architect_rules import DMSProperty, DMSRules
 
 
 if sys.version_info >= (3, 11):
     from typing import Self
@@ -114,16 +119,16 @@
         class_: The class ID of the class.
         description: A description of the class.
         parent: The parent class of the class.
         reference: Reference of the source of the information for given resource
         match_type: The match type of the resource being described and the source entity.
     """
 
-    parent: ParentClassType = Field(alias="Parent Class", default=None)
-    reference: ReferenceType = Field(alias="Reference", default=None)
+    parent: ParentEntityList | None = Field(alias="Parent Class", default=None)
+    reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     comment: str | None = Field(alias="Comment", default=None)
 
 
 class InformationProperty(SheetEntity):
     """
     A property is a characteristic of a class. It is a named attribute of a class that describes a range of values
@@ -142,19 +147,19 @@
         rule_type: Rule type for the transformation from source to target representation
                    of knowledge graph. Defaults to None (no transformation)
         rule: Actual rule for the transformation from source to target representation of
               knowledge graph. Defaults to None (no transformation)
     """
 
     property_: PropertyType = Field(alias="Property")
-    value_type: SemanticValueType = Field(alias="Value Type")
+    value_type: DataType | ClassEntity | UnknownEntity = Field(alias="Value Type", union_mode="left_to_right")
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
     default: Any | None = Field(alias="Default", default=None)
-    reference: ReferenceType = Field(alias="Reference", default=None)
+    reference: URLEntity | ReferenceEntity | None = Field(alias="Reference", default=None, union_mode="left_to_right")
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     rule_type: str | TransformationRuleType | None = Field(alias="Rule Type", default=None)
     rule: str | AllReferences | SingleProperty | Hop | RawLookup | SPARQLQuery | Traversal | None = Field(
         alias="Rule", default=None
     )
     comment: str | None = Field(alias="Comment", default=None)
 
@@ -219,17 +224,17 @@
                         self.value_type.python,
                     )
         return self
 
     @property
     def type_(self) -> EntityTypes:
         """Type of property based on value type. Either data (attribute) or object (edge) property."""
-        if self.value_type.type_ == EntityTypes.xsd_value_type:
+        if isinstance(self.value_type, DataType):
             return EntityTypes.data_property
-        elif self.value_type.type_ == EntityTypes.class_:
+        elif isinstance(self.value_type, ClassEntity):
             return EntityTypes.object_property
         else:
             return EntityTypes.undefined
 
     @property
     def is_mandatory(self) -> bool:
         """Returns True if property is mandatory."""
@@ -254,57 +259,57 @@
             return {key: Namespace(value) if isinstance(value, str) else value for key, value in values.items()}
         return values
 
     @model_validator(mode="after")
     def update_entities_prefix(self) -> Self:
         # update expected_value_types
         for property_ in self.properties:
-            if property_.value_type.prefix is Undefined and property_.value_type.suffix is not Unknown:
+            if isinstance(property_.value_type, ClassEntity) and property_.value_type.prefix is Undefined:
                 property_.value_type.prefix = self.metadata.prefix
             if property_.class_.prefix is Undefined:
                 property_.class_.prefix = self.metadata.prefix
 
         # update parent classes
         for class_ in self.classes:
             if class_.parent:
                 for parent in cast(list[ParentClassEntity], class_.parent):
-                    if parent.prefix is Undefined:
+                    if not isinstance(parent.prefix, str):
                         parent.prefix = self.metadata.prefix
             if class_.class_.prefix is Undefined:
                 class_.class_.prefix = self.metadata.prefix
 
         return self
 
     @model_validator(mode="after")
     def validate_schema_completeness(self) -> Self:
         # update expected_value_types
 
         if self.metadata.schema_ == SchemaCompleteness.complete:
-            defined_classes = {class_.class_.versioned_id for class_ in self.classes}
-            referred_classes = {property_.class_.versioned_id for property_ in self.properties} | {
-                parent.versioned_id for class_ in self.classes for parent in class_.parent or []
+            defined_classes = {str(class_.class_) for class_ in self.classes}
+            referred_classes = {str(property_.class_) for property_ in self.properties} | {
+                str(parent) for class_ in self.classes for parent in class_.parent or []
             }
             referred_types = {
-                property_.value_type.versioned_id
+                str(property_.value_type)
                 for property_ in self.properties
-                if property_.type_ == EntityTypes.object_property
-                and not (isinstance(property_.value_type, Entity) and property_.value_type.suffix is Unknown)
+                if isinstance(property_.value_type, Entity)
+                and not isinstance(property_.value_type.suffix, _UnknownType)
             }
             if not referred_classes.issubset(defined_classes) or not referred_types.issubset(defined_classes):
                 missing_classes = referred_classes.difference(defined_classes).union(
                     referred_types.difference(defined_classes)
                 )
                 raise exceptions.IncompleteSchema(missing_classes).to_pydantic_custom_error()
 
         return self
 
     @model_validator(mode="after")
     def validate_class_has_properties_or_parent(self) -> Self:
         defined_classes = {class_.class_ for class_ in self.classes if class_.reference is None}
-        referred_classes = {property_.class_ for property_ in self.properties}
+        referred_classes = {property_.class_ for property_ in self.properties if property_.class_.suffix is not Unknown}
         has_parent_classes = {class_.class_ for class_ in self.classes if class_.parent}
         missing_classes = defined_classes.difference(referred_classes) - has_parent_classes
         if missing_classes:
             warnings.warn(
                 cognite.neat.rules.issues.spreadsheet.ClassNoPropertiesNoParentsWarning(
                     [missing.versioned_id for missing in missing_classes]
                 ),
@@ -353,23 +358,29 @@
     def as_dms_architect_rules(self) -> "DMSRules":
         return _InformationRulesConverter(self).as_dms_architect_rules()
 
     def reference_self(self) -> "InformationRules":
         new_self = self.model_copy(deep=True)
         for prop in new_self.properties:
             prop.reference = ReferenceEntity(
-                prefix=prop.class_.prefix,
+                prefix=prop.class_.prefix
+                if not isinstance(prop.class_.prefix, _UndefinedType)
+                else self.metadata.prefix,
                 suffix=prop.class_.suffix,
                 version=prop.class_.version,
-                property_=prop.property_,
+                property=prop.property_,
             )
 
         for cls_ in new_self.classes:
             cls_.reference = ReferenceEntity(
-                prefix=cls_.class_.prefix, suffix=cls_.class_.suffix, version=cls_.class_.version
+                prefix=cls_.class_.prefix
+                if not isinstance(cls_.class_.prefix, _UndefinedType)
+                else self.metadata.prefix,
+                suffix=cls_.class_.suffix,
+                version=cls_.class_.version,
             )
 
         return new_self
 
 
 class _InformationRulesConverter:
     def __init__(self, information: InformationRules):
@@ -378,15 +389,16 @@
     def as_domain_rules(self) -> DomainRules:
         raise NotImplementedError("DomainRules not implemented yet")
 
     def as_dms_architect_rules(self, created: datetime | None = None, updated: datetime | None = None) -> "DMSRules":
         from ._dms_architect_rules import DMSContainer, DMSMetadata, DMSProperty, DMSRules, DMSView
 
         info_metadata = self.information.metadata
-
+        default_version = info_metadata.version
+        default_space = self._to_space(info_metadata.prefix)
         space = self._to_space(info_metadata.prefix)
 
         metadata = DMSMetadata(
             schema_=info_metadata.schema_,
             space=space,
             version=info_metadata.version,
             external_id=info_metadata.name.replace(" ", "_").lower(),
@@ -394,51 +406,50 @@
             name=info_metadata.name,
             created=created or datetime.now(),
             updated=updated or datetime.now(),
         )
 
         properties_by_class: dict[str, list[DMSProperty]] = defaultdict(list)
         for prop in self.information.properties:
-            properties_by_class[prop.class_.versioned_id].append(self._as_dms_property(prop))
+            properties_by_class[prop.class_.versioned_id].append(
+                self._as_dms_property(prop, default_space, default_version)
+            )
 
         views: list[DMSView] = [
             DMSView(
                 class_=cls_.class_,
                 name=cls_.name,
-                view=ViewPropEntity(prefix=cls_.class_.prefix, suffix=cls_.class_.suffix, version=cls_.class_.version),
+                view=cls_.class_.as_view_entity(default_space, default_version),
                 description=cls_.description,
                 reference=cls_.reference,
                 implements=self._get_view_implements(cls_, info_metadata),
             )
             for cls_ in self.information.classes
         ]
 
         classes_without_properties: set[str] = set()
         for class_ in self.information.classes:
             properties: list[DMSProperty] = properties_by_class.get(class_.class_.versioned_id, [])
             if not properties or all(
-                isinstance(prop.value_type, ViewPropEntity) and prop.relation != "direct" for prop in properties
+                isinstance(prop.value_type, ViewPropertyEntity) and prop.relation != "direct" for prop in properties
             ):
                 classes_without_properties.add(class_.class_.versioned_id)
 
         containers: list[DMSContainer] = []
         for class_ in self.information.classes:
             if class_.class_.versioned_id in classes_without_properties:
                 continue
             containers.append(
                 DMSContainer(
                     class_=class_.class_,
                     name=class_.name,
-                    container=ContainerEntity(prefix=class_.class_.prefix, suffix=class_.class_.suffix),
+                    container=class_.class_.as_container_entity(default_space),
                     description=class_.description,
                     constraint=[
-                        ContainerEntity(
-                            prefix=parent.prefix,
-                            suffix=parent.suffix,
-                        )
+                        parent.as_container_entity(default_space)
                         for parent in class_.parent or []
                         if parent.versioned_id not in classes_without_properties
                     ]
                     or None,
                 )
             )
 
@@ -449,59 +460,60 @@
             ),
             views=SheetList[DMSView](data=views),
             containers=SheetList[DMSContainer](data=containers),
             reference=self.information.reference and self.information.reference.as_dms_architect_rules(),  # type: ignore[arg-type]
         )
 
     @classmethod
-    def _as_dms_property(cls, prop: InformationProperty) -> "DMSProperty":
+    def _as_dms_property(cls, prop: InformationProperty, default_space: str, default_version: str) -> "DMSProperty":
         """This creates the first"""
 
         from ._dms_architect_rules import DMSProperty
 
         # returns property type, which can be ObjectProperty or DatatypeProperty
-        if isinstance(prop.value_type, XSDValueType):
-            value_type = cast(XSDValueType, prop.value_type).dms._type.casefold()  # type: ignore[attr-defined]
+        value_type: DataType | ViewEntity | ViewPropertyEntity | DMSUnknownEntity
+        if isinstance(prop.value_type, DataType):
+            value_type = prop.value_type
+        elif isinstance(prop.value_type, UnknownEntity):
+            value_type = DMSUnknownEntity()
         elif isinstance(prop.value_type, ClassEntity):
-            value_type = ViewPropEntity(
-                prefix=prop.value_type.prefix, suffix=prop.value_type.suffix, version=prop.value_type.version
-            )
+            value_type = prop.value_type.as_view_entity(default_space, default_version)
         else:
             raise ValueError(f"Unsupported value type: {prop.value_type.type_}")
 
         relation: Literal["direct", "multiedge"] | None = None
-        if isinstance(value_type, ViewPropEntity):
+        if isinstance(value_type, ViewEntity | ViewPropertyEntity):
             relation = "multiedge" if prop.is_list else "direct"
 
         container: ContainerEntity | None = None
         container_property: str | None = None
         is_list: bool | None = prop.is_list
         nullable: bool | None = not prop.is_mandatory
         if relation == "multiedge":
             is_list = None
             nullable = None
         elif relation == "direct":
             nullable = True
-            container, container_property = cls._get_container(prop)
+            container, container_property = cls._get_container(prop, default_space)
         else:
-            container, container_property = cls._get_container(prop)
+            container, container_property = cls._get_container(prop, default_space)
 
         return DMSProperty(
             class_=prop.class_,
             name=prop.name,
             property_=prop.property_,
             value_type=value_type,
             nullable=nullable,
             is_list=is_list,
             relation=relation,
             default=prop.default,
             reference=prop.reference,
             container=container,
             container_property=container_property,
-            view=ViewPropEntity(prefix=prop.class_.prefix, suffix=prop.class_.suffix, version=prop.class_.version),
+            view=prop.class_.as_view_entity(default_space, default_version),
             view_property=prop.property_,
         )
 
     @classmethod
     def _to_space(cls, prefix: str) -> str:
         """Ensures that the prefix comply with the CDF space regex"""
         prefix = re.sub(r"[^a-zA-Z0-9_-]", "_", prefix)
@@ -509,33 +521,28 @@
             prefix = f"a{prefix}"
         prefix = prefix[:43]
         if prefix[-1] == "_":
             prefix = f"{prefix[:-1]}1"
         return prefix
 
     @classmethod
-    def _get_container(cls, prop: InformationProperty) -> tuple[ContainerEntity, str]:
+    def _get_container(cls, prop: InformationProperty, default_space: str) -> tuple[ContainerEntity, str]:
         if isinstance(prop.reference, ReferenceEntity):
             return (
-                ContainerEntity(prefix=prop.reference.prefix, suffix=prop.reference.suffix),
+                prop.reference.as_container_entity(default_space),
                 prop.reference.property_ or prop.property_,
             )
         else:
-            return ContainerEntity(prefix=prop.class_.prefix, suffix=prop.class_.suffix), prop.property_
+            return prop.class_.as_container_entity(default_space), prop.property_
 
     @classmethod
     def _get_view_implements(cls, cls_: InformationClass, metadata: InformationMetadata) -> list[ViewEntity]:
         if isinstance(cls_.reference, ReferenceEntity) and cls_.reference.prefix != metadata.prefix:
             # We use the reference for implements if it is in a different namespace
             implements = [
-                ViewEntity(prefix=cls_.reference.prefix, suffix=cls_.reference.suffix, version=cls_.reference.version)
+                cls_.reference.as_view_entity(metadata.prefix, metadata.version),
             ]
         else:
             implements = []
 
-        implements.extend(
-            [
-                ViewEntity(prefix=parent.prefix, suffix=parent.suffix, version=parent.version)
-                for parent in cls_.parent or []
-            ]
-        )
+        implements.extend([parent.as_view_entity(metadata.prefix, metadata.version) for parent in cls_.parent or []])
         return implements
```

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/cdf.py` & `cognite_neat-0.75.8/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.75.8/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/exceptions.py` & `cognite_neat-0.75.8/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.75.8/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/text.py` & `cognite_neat-0.75.8/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/utils.py` & `cognite_neat-0.75.8/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/utils/xml.py` & `cognite_neat-0.75.8/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.75.8/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/base.py` & `cognite_neat-0.75.8/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.75.8/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.75.8/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/manager.py` & `cognite_neat-0.75.8/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.75.8/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.75.8/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/model.py` & `cognite_neat-0.75.8/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import ClassVar
 
 from cognite.client import CogniteClient
 
 from cognite.neat.rules import importers
 from cognite.neat.rules.issues.formatters import FORMATTER_BY_NAME
+from cognite.neat.rules.models.entities import DataModelEntity, DMSUnknownEntity
 from cognite.neat.rules.models.rules import RoleTypes
-from cognite.neat.rules.models.rules._types import DataModelEntity, Undefined
 from cognite.neat.workflows._exceptions import StepNotInitialized
 from cognite.neat.workflows.model import FlowMessage, StepExecutionStatus
 from cognite.neat.workflows.steps.data_contracts import MultiRuleData
 from cognite.neat.workflows.steps.step_model import Configurable, Step
 
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title()
 
@@ -203,16 +203,16 @@
             raise StepNotInitialized(type(self).__name__)
 
         datamodel_id_str = self.configs.get("Data model id")
         if datamodel_id_str is None:
             error_text = "Expected input payload to contain 'Data model id' key."
             return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
 
-        datamodel_entity = DataModelEntity.from_raw(datamodel_id_str)
-        if datamodel_entity.space is Undefined:
+        datamodel_entity = DataModelEntity.load(datamodel_id_str)
+        if isinstance(datamodel_entity, DMSUnknownEntity):
             error_text = (
                 f"Data model id should be in the format 'my_space:my_data_model(version=1)' "
                 f"or 'my_space:my_data_model', failed to parse space from {datamodel_id_str}"
             )
             return FlowMessage(error_text=error_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
 
         dms_importer = importers.DMSImporter.from_data_model_id(cdf_client, datamodel_entity.as_id())
```

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.75.8/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/tasks.py` & `cognite_neat-0.75.8/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/cognite/neat/workflows/triggers.py` & `cognite_neat-0.75.8/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.7/pyproject.toml` & `cognite_neat-0.75.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.75.7"
+version = "0.75.8"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.75.7/PKG-INFO` & `cognite_neat-0.75.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.75.7
+Version: 0.75.8
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

