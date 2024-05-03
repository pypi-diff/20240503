# Comparing `tmp/therix-0.1.2.tar.gz` & `tmp/therix-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.2.tar", max compression
+gzip compressed data, was "therix-0.1.3.tar", max compression
```

## Comparing `therix-0.1.2.tar` & `therix-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,99 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.2/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-12 15:05:11.676463 therix-0.1.2/README.md
--rw-r--r--   0        0        0      841 2024-04-16 06:14:22.172351 therix-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.929969 therix-0.1.2/therix/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-12 14:54:15.930143 therix-0.1.2/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930181 therix-0.1.2/therix/core/__init__.py
--rw-r--r--   0        0        0     1571 2024-04-12 14:54:15.930332 therix-0.1.2/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 06:13:24.884093 therix-0.1.2/therix/core/data_sources.py
--rw-r--r--   0        0        0     1676 2024-04-16 06:13:24.884272 therix-0.1.2/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2381 2024-04-16 06:13:24.884478 therix-0.1.2/therix/core/inference_models.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.930720 therix-0.1.2/therix/core/output_source.py
--rw-r--r--   0        0        0     3422 2024-04-16 06:13:24.884674 therix-0.1.2/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-12 14:54:15.930956 therix-0.1.2/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      299 2024-04-16 06:13:24.884857 therix-0.1.2/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.931148 therix-0.1.2/therix/db/__init__.py
--rw-r--r--   0        0        0       83 2024-04-12 14:54:15.931283 therix-0.1.2/therix/db/base.py
--rw-r--r--   0        0        0     2936 2024-04-16 06:13:24.885055 therix-0.1.2/therix/db/db_manager.py
--rw-r--r--   0        0        0      410 2024-04-16 06:13:24.885241 therix-0.1.2/therix/db/session.py
--rw-r--r--   0        0        0      234 2024-04-12 14:54:15.931776 therix-0.1.2/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-12 14:54:15.931895 therix-0.1.2/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-12 14:54:15.932023 therix-0.1.2/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-12 14:54:15.932200 therix-0.1.2/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-12 14:54:15.932340 therix-0.1.2/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-12 14:54:15.932456 therix-0.1.2/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-12 14:54:15.932858 therix-0.1.2/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-12 14:54:15.933048 therix-0.1.2/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-12 14:54:15.933157 therix-0.1.2/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0     1411 2024-04-12 14:54:15.933315 therix-0.1.2/therix/docs/docs/intro.md
--rw-r--r--   0        0        0      180 2024-04-12 14:54:15.933452 therix-0.1.2/therix/docs/docs/tutorial-basics/_category_.json
--rw-r--r--   0        0        0     1078 2024-04-12 14:54:15.933560 therix-0.1.2/therix/docs/docs/tutorial-basics/congratulations.md
--rw-r--r--   0        0        0      886 2024-04-12 14:54:15.933661 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-blog-post.md
--rw-r--r--   0        0        0     1042 2024-04-12 14:54:15.933784 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-document.md
--rw-r--r--   0        0        0     1015 2024-04-12 14:54:15.933895 therix-0.1.2/therix/docs/docs/tutorial-basics/create-a-page.md
--rw-r--r--   0        0        0      702 2024-04-12 14:54:15.934002 therix-0.1.2/therix/docs/docs/tutorial-basics/deploy-your-site.md
--rw-r--r--   0        0        0     3006 2024-04-12 14:54:15.934112 therix-0.1.2/therix/docs/docs/tutorial-basics/markdown-features.mdx
--rw-r--r--   0        0        0       99 2024-04-12 14:54:15.934248 therix-0.1.2/therix/docs/docs/tutorial-extras/_category_.json
--rw-r--r--   0        0        0    25427 2024-04-12 14:54:15.934440 therix-0.1.2/therix/docs/docs/tutorial-extras/img/docsVersionDropdown.png
--rw-r--r--   0        0        0    27841 2024-04-12 14:54:15.934733 therix-0.1.2/therix/docs/docs/tutorial-extras/img/localeDropdown.png
--rw-r--r--   0        0        0     1232 2024-04-12 14:54:15.934904 therix-0.1.2/therix/docs/docs/tutorial-extras/manage-docs-versions.md
--rw-r--r--   0        0        0     1587 2024-04-12 14:54:15.935005 therix-0.1.2/therix/docs/docs/tutorial-extras/translate-your-site.md
--rw-r--r--   0        0        0     3605 2024-04-12 14:54:15.935114 therix-0.1.2/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0   573996 2024-04-12 14:54:15.936314 therix-0.1.2/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1061 2024-04-12 14:54:15.936493 therix-0.1.2/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-12 14:54:15.936597 therix-0.1.2/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-12 14:54:15.936828 therix-0.1.2/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2024-04-12 14:54:15.936929 therix-0.1.2/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2239 2024-04-12 14:54:15.937061 therix-0.1.2/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-12 14:54:15.937193 therix-0.1.2/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-12 14:54:15.937292 therix-0.1.2/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.937368 therix-0.1.2/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-12 14:54:15.937664 therix-0.1.2/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-12 14:54:15.937878 therix-0.1.2/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-12 14:54:15.938169 therix-0.1.2/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-12 14:54:15.938362 therix-0.1.2/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3626 2024-04-12 14:54:15.938464 therix-0.1.2/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      506 2024-04-12 14:54:15.938561 therix-0.1.2/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0     6438 2024-04-12 14:54:15.938694 therix-0.1.2/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0    31486 2024-04-12 14:54:15.938840 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-12 14:54:15.939041 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-12 14:54:15.939300 therix-0.1.2/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939374 therix-0.1.2/therix/entities/__init__.py
--rw-r--r--   0        0        0     2205 2024-04-12 14:54:15.939477 therix-0.1.2/therix/entities/models.py
--rw-r--r--   0        0        0        0 2024-04-12 14:54:15.939553 therix-0.1.2/therix/services/__init__.py
--rw-r--r--   0        0        0     3411 2024-04-16 06:13:24.885453 therix-0.1.2/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-12 14:54:15.939755 therix-0.1.2/therix/services/web_crawling.py
--rw-r--r--   0        0        0    10269 2024-04-16 06:13:24.885743 therix-0.1.2/therix/utils/rag.py
--rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 therix-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.3/README.md
+-rw-r--r--   0        0        0     1023 2024-05-03 13:10:49.072394 therix-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.3/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.3/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.3/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.3/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.3/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.3/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      838 2024-05-03 12:50:17.295642 therix-0.1.3/therix/alembic/versions/2024_05_03_1637-04b509a2f1cc_added_chat_history_fix.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.3/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.3/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.3/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.3/therix/core/__init__.py
+-rw-r--r--   0        0        0     2371 2024-05-03 05:53:02.645943 therix-0.1.3/therix/core/cache.py
+-rw-r--r--   0        0        0     1408 2024-05-03 12:50:17.295817 therix-0.1.3/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1649 2024-05-03 12:50:17.296463 therix-0.1.3/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.3/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.3/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2374 2024-05-03 13:10:49.072728 therix-0.1.3/therix/core/inference_models.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.3/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.3/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     5711 2024-05-03 12:50:17.297034 therix-0.1.3/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.3/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      248 2024-05-03 05:53:02.646834 therix-0.1.3/therix/core/response.py
+-rw-r--r--   0        0        0      588 2024-04-26 09:41:57.772788 therix-0.1.3/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.3/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.3/therix/db/__init__.py
+-rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.3/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.3/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.3/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.3/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.3/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.3/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.3/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.3/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.3/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.3/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.3/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.3/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.3/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.3/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.3/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.3/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     1460 2024-05-03 05:53:02.648669 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0       91 2024-05-03 05:53:02.648747 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0       97 2024-05-03 05:53:02.648823 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0       81 2024-05-03 05:53:02.649008 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/index.md
+-rw-r--r--   0        0        0       98 2024-05-03 05:53:02.649150 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0       78 2024-05-03 05:53:02.649233 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0       97 2024-05-03 05:53:02.648360 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.3/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0       67 2024-05-03 05:53:02.649417 therix-0.1.3/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.3/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.3/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.3/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0      435 2024-05-03 05:53:02.649793 therix-0.1.3/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.3/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.3/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.3/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.3/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.3/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.3/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.3/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.3/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     4371 2024-05-03 05:53:02.651405 therix-0.1.3/therix/docs/docs/use-cases/summarizer_doc.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.3/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.3/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.3/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.3/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.3/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.3/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.3/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.3/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.3/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.3/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.3/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.3/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.3/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.3/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.3/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.3/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.3/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.3/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.3/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.3/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.3/therix/entities/models.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.3/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.3/therix/services/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-26 09:41:57.774292 therix-0.1.3/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.3/therix/services/web_crawling.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.3/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    10397 2024-05-03 12:50:17.298312 therix-0.1.3/therix/utils/rag.py
+-rw-r--r--   0        0        0     4051 2024-04-26 09:41:57.774560 therix-0.1.3/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 therix-0.1.3/PKG-INFO
```

### Comparing `therix-0.1.2/LICENSE` & `therix-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/README.md` & `therix-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/pyproject.toml` & `therix-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.2"
+version = "0.1.3"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
+include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 wheel = "^0.43.0"
 alembic = "1.13.1"
 psycopg2-binary = "2.9.9"
 sqlalchemy = "2.0.28"
@@ -18,20 +19,27 @@
 tiktoken = "0.6.0"
 pypdf = "4.1.0"
 langfuse = "2.21.1"
 alembic-postgresql-enum = "1.1.2"
 greenlet = "^3.0.3"
 youtube-transcript-api = "^0.6.2"
 pytube = "^15.0.0"
+presidio-analyzer = "^2.2.354"
 bs4 = "^0.0.2"
 selenium = "^4.19.0"
 psycopg = {extras = ["binary", "pool"], version = "^3.1.18"}
 langchain-groq = "^0.1.0"
 boto3 = "^1.34.81"
+pylint = "^3.1.0"
+coverage = "^7.4.4"
+pytest-cov = "^5.0.0"
+langchain-postgres = "^0.0.3"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
-poetry-dotenv = "0.4.0"
+pytest = "^8.1.1"
+pytest-mock = "^3.14.0"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `therix-0.1.2/therix/core/JSONLoader.py` & `therix-0.1.3/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/core/constants.py` & `therix-0.1.3/therix/core/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,11 @@
     DATABASE = "DATABASE"
 
 
 class ChatMessage(Enum):
     CHAT_SAVED = "Message saved successfully!"
     CHAT_FAILED = "Error saving message"
     FAILED_TO_RETRIEVE = "Error retrieving message history"
+
+class PipelineTypeMaster(Enum):
+    RAG = 'RAG'
+    SUMMARIZER = 'SUMMARIZER'
```

### Comparing `therix-0.1.2/therix/core/data_sources.py` & `therix-0.1.3/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/core/embedding_models.py` & `therix-0.1.3/therix/core/embedding_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/core/inference_models.py` & `therix-0.1.3/therix/core/inference_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,10 +63,10 @@
 class BedrockTextExpressV1(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(
             name=InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1, config=config
         )
 
 
-class BedrockTextExpressV1(InferenceModel):
+class BedrockLiteG1(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.BEDROCK_TEXT_LITE_G1, config=config)
```

### Comparing `therix-0.1.2/therix/core/pipeline_component.py` & `therix-0.1.3/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/db/db_manager.py` & `therix-0.1.3/therix/db/db_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,109 @@
-from sqlalchemy import create_engine, Engine, text
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.exc import SQLAlchemyError
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker, scoped_session
+from sqlalchemy.engine.url import URL
 from alembic.config import Config
 from alembic import command
+import threading
 import logging
 import os
 
-from therix.db.base import Base
+from therix.entities.models import Base
 
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class DatabaseManager:
-    """
-    Database manager / connection handler and session manager
-    """
-
     _instance = None
-    engine: Engine
-    session: sessionmaker
-    SQLALCHEMY_DATABASE_URL: str
+    _engine = None
+    _session_factory = None
 
-    def __new__(cls, *args, **kwargs):
+    def __new__(cls):
+        logger.debug("Checking instance...")
         if cls._instance is None:
-            cls._instance = super(DatabaseManager, cls).__new__(cls)
+            with threading.Lock():
+                if cls._instance is None:
+                    logger.debug("Creating new instance...")
+                    cls._instance = super(DatabaseManager, cls).__new__(cls)
+                    cls._engine = cls._create_engine()
+                    cls._session_factory = sessionmaker(
+                        bind=cls._engine, autoflush=False, autocommit=False
+                    )
+                    cls._setup_database()
         return cls._instance
 
-    def __init__(self):
-        """
-        Initializes the database by creating all defined tables
-        and running any pending migrations.
-        """
-        db_type = os.getenv("THERIX_DB_TYPE", "postgresql")
+    @classmethod
+    def get_session(cls):
+        if cls._session_factory is None:
+            raise Exception("DatabaseManager is not initialized properly.")
+        return scoped_session(cls._session_factory)
+
+    @classmethod
+    def _create_engine(cls):
+        db_url = cls._construct_db_url()
+        return create_engine(db_url)
+
+    @classmethod
+    def _construct_db_url(cls):
+        drivername = os.getenv("THERIX_DB_TYPE", "postgresql")
         username = os.getenv("THERIX_DB_USERNAME")
         password = os.getenv("THERIX_DB_PASSWORD")
         host = os.getenv("THERIX_DB_HOST")
         port = os.getenv("THERIX_DB_PORT")
         db_name = os.getenv("THERIX_DB_NAME")
-        try:
-            if not hasattr(self, "engine"):
-                if all(
-                    param is not None
-                    for param in [db_type, username, password, host, port, db_name]
-                ):
+        return URL.create(
+            drivername=drivername,
+            username=username,
+            password=password,
+            host=host,
+            port=port,
+            database=db_name,
+        ).render_as_string(hide_password=False)
+
+    @staticmethod
+    def _setup_database():
+        # Placeholder for database setup logic like migrations
+
+        Base.metadata.create_all(DatabaseManager._engine)
+        logger.info("Database tables created.")
+
+        alembic_cfg = DatabaseManager._get_alembic_config()
+        DatabaseManager._upgrade_database(alembic_cfg)
+
+    @staticmethod
+    def _get_alembic_config():
+        # Navigate up two levels from the current file location to find the Alembic directory.
+        base_dir = os.path.dirname(
+            os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+        )
+        alembic_config_path = os.path.join(base_dir, "therix/alembic.ini")
+        alembic_cfg = Config(alembic_config_path)
+        alembic_cfg.set_main_option(
+            "script_location", os.path.join(base_dir, "therix/alembic")
+        )
+        alembic_cfg.set_main_option(
+            "sqlalchemy.url", str(DatabaseManager._construct_db_url())
+        )
+        return alembic_cfg
 
-                    self.SQLALCHEMY_DATABASE_URL = (
-                        f"{db_type}://{username}:{password}@{host}:{port}/{db_name}"
-                    )
-                    self.engine = create_engine(self.SQLALCHEMY_DATABASE_URL)
-                    self.session = sessionmaker(bind=self.engine)
-                    self.session().execute(text("SELECT 1"))
-
-                    Base.metadata.create_all(self.engine)
-                    logger.info("All tables created successfully.")
-                    # Run Alembic migrations
-                    alembic_cfg = Config("alembic.ini")
-                    alembic_cfg.set_main_option(
-                        "sqlalchemy.url", self.SQLALCHEMY_DATABASE_URL
-                    )
-                    command.upgrade(alembic_cfg, "head")
-                    logger.info("All migrations executed successfully.")
-                    logger.info(
-                        "Database engine and session factory created successfully."
-                    )
-        except SQLAlchemyError as e:
-            logger.error(f"An error occurred while initializing the database: {e}")
+    @staticmethod
+    def _upgrade_database(alembic_cfg):
+        try:
+            # command.upgrade(alembic_cfg, "head")
+            # logger.info("Database upgraded successfully.")
+            pass
+        except Exception as e:
+            logger.error(f"An error occurred while upgrading the database: {e}")
             raise
 
-    def create_session(self):
-        return self.session()
+
+# Unit testing with pytest will be created next. This would involve testing these functionalities effectively.
 
 
 db_manager = DatabaseManager()
 # Example usage:
 # db_manager = DatabaseManager(
 #     "postgresql", "postgres", "password", "localhost", "5432", "coditas_dot_ai"
 # )
```

### Comparing `therix-0.1.2/therix/docs/README.md` & `therix-0.1.3/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.3/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.3/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.3/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/docusaurus.config.js` & `therix-0.1.3/therix/docs/docusaurus.config.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -7,29 +7,28 @@
 import {
     themes as prismThemes
 } from 'prism-react-renderer';
 
 /** @type {import('@docusaurus/types').Config} */
 const config = {
     title: 'Therix Ai',
-    tagline: 'Ai is cool',
+    tagline: 'Add AI to your product in minutes',
     favicon: 'img/favicon.ico',
 
     // Set the production url of your site here
-    url: 'https://your-docusaurus-site.example.com',
+    url: 'https://docs.therix.ai',
     // Set the /<baseUrl>/ pathname under which your site is served
     // For GitHub pages deployment, it is often '/<projectName>/'
     baseUrl: '/',
 
     // GitHub pages deployment config.
     // If you aren't using GitHub pages, you don't need these.
-    organizationName: 'Coditas', // Usually your GitHub org/user name.
+    organizationName: 'therix-ai', // Usually your GitHub org/user name.
     projectName: 'Therix', // Usually your repo name.
-
-    onBrokenLinks: 'throw',
+    onBrokenLinks: 'ignore',
     onBrokenMarkdownLinks: 'warn',
 
     // Even if you don't use internationalization, you can use this field to set
     // useful metadata like html lang. For example, if your site is Chinese, you
     // may want to replace "en" with "zh-Hans".
     i18n: {
         defaultLocale: 'en',
@@ -49,20 +48,20 @@
         ],
     ],
 
     themeConfig:
         /** @type {import('@docusaurus/preset-classic').ThemeConfig} */
         ({
             // Replace with your project's social card
-            image: 'img/icon.svg',
+            image: 'img/therix-logo.png',
             navbar: {
-                title: 'Therix.Ai',
+                title: '',
                 logo: {
-                    alt: 'My Site Logo',
-                    src: 'img/icon.svg',
+                    alt: 'Therix.ai',
+                    src: 'img/therix-logo.png',
                 },
                 items: [{
                         type: 'docSidebar',
                         sidebarId: 'defaultSidebar',
                         position: 'left',
                         label: 'Documentation',
                     },
@@ -76,15 +75,15 @@
             },
             footer: {
                 style: 'dark',
                 links: [{
                         title: 'Docs',
                         items: [{
                             label: 'Tutorial',
-                            to: '/docs/intro',
+                            to: '/introduction/getting-started',
                         }, ],
                     }, {
                         title: 'Community',
                         items: [{
                             label: 'Stack Overflow',
                             href: 'https://stackoverflow.com/questions/tagged/docusaurus',
                         }, {
@@ -105,17 +104,28 @@
                     //     {
                     //       label: 'GitHub',
                     //       href: 'https://github.com/coditas-llp/therix-core',
                     //     },
                     //   ],
                     // },
                 ],
-                copyright: `Copyright © ${new Date().getFullYear()} Coditas, Built with Docusaurus.`,
+                copyright: `Copyright © ${new Date().getFullYear()} therix.ai`,
             },
             prism: {
                 theme: prismThemes.github,
                 darkTheme: prismThemes.dracula,
             },
         }),
+
+    plugins: [
+        [
+            '@docusaurus/plugin-client-redirects', {
+                redirects: [{
+                    from: '/', // From the root
+                    to: '/introduction', // To your introduction page
+                }, ],
+            },
+        ],
+    ]
 };
 
 export default config;
```

### Comparing `therix-0.1.2/therix/docs/package-lock.json` & `therix-0.1.3/therix/docs/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998337821043911%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@docusaurus/plugin-client-redirects': '3.2.0'}}, "*

 * *               "'node_modules/@docusaurus/plugin-client-redirects': OrderedDict([('version', "*

 * *               "'3.2.0'), ('resolved', "*

 * *               "'https://registry.npmjs.org/@docusaurus/plugin-client-redirects/-/plugin-client-redirects-3.2.0.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-re5bgvYOgBHmevlI8HO3fZHL7mvX2lAULr4E89n/bQ5kgekLLhsaerWrAah22ZluMZyJC2439EGjR63E9Ba6KA=='), "*

 * *               […]*

```diff
@@ -1,14 +1,15 @@
 {
     "lockfileVersion": 3,
     "name": "my-website",
     "packages": {
         "": {
             "dependencies": {
                 "@docusaurus/core": "3.2.0",
+                "@docusaurus/plugin-client-redirects": "3.2.0",
                 "@docusaurus/preset-classic": "3.2.0",
                 "@mdx-js/react": "^3.0.0",
                 "clsx": "^2.0.0",
                 "prism-react-renderer": "^2.3.0",
                 "react": "^18.0.0",
                 "react-dom": "^18.0.0"
             },
@@ -2295,14 +2296,37 @@
             "peerDependencies": {
                 "react": "*",
                 "react-dom": "*"
             },
             "resolved": "https://registry.npmjs.org/@docusaurus/module-type-aliases/-/module-type-aliases-3.2.0.tgz",
             "version": "3.2.0"
         },
+        "node_modules/@docusaurus/plugin-client-redirects": {
+            "dependencies": {
+                "@docusaurus/core": "3.2.0",
+                "@docusaurus/logger": "3.2.0",
+                "@docusaurus/utils": "3.2.0",
+                "@docusaurus/utils-common": "3.2.0",
+                "@docusaurus/utils-validation": "3.2.0",
+                "eta": "^2.2.0",
+                "fs-extra": "^11.1.1",
+                "lodash": "^4.17.21",
+                "tslib": "^2.6.0"
+            },
+            "engines": {
+                "node": ">=18.0"
+            },
+            "integrity": "sha512-re5bgvYOgBHmevlI8HO3fZHL7mvX2lAULr4E89n/bQ5kgekLLhsaerWrAah22ZluMZyJC2439EGjR63E9Ba6KA==",
+            "peerDependencies": {
+                "react": "^18.0.0",
+                "react-dom": "^18.0.0"
+            },
+            "resolved": "https://registry.npmjs.org/@docusaurus/plugin-client-redirects/-/plugin-client-redirects-3.2.0.tgz",
+            "version": "3.2.0"
+        },
         "node_modules/@docusaurus/plugin-content-blog": {
             "dependencies": {
                 "@docusaurus/core": "3.2.0",
                 "@docusaurus/logger": "3.2.0",
                 "@docusaurus/mdx-loader": "3.2.0",
                 "@docusaurus/types": "3.2.0",
                 "@docusaurus/utils": "3.2.0",
@@ -6510,27 +6534,14 @@
             "version": "1.0.5"
         },
         "node_modules/fs.realpath": {
             "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "node_modules/fsevents": {
-            "engines": {
-                "node": "^8.16.0 || ^10.6.0 || >=11.0.0"
-            },
-            "hasInstallScript": true,
-            "integrity": "sha512-5xoDfX+fL7faATnagmWPpbFtwh/R77WmMMqqHGS65C3vvB0YHrgF+B1YmZ3441tMj5n63k0212XNoJwzlhffQw==",
-            "optional": true,
-            "os": [
-                "darwin"
-            ],
-            "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-2.3.3.tgz",
-            "version": "2.3.3"
-        },
         "node_modules/function-bind": {
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
             "integrity": "sha512-7XHNxH7qX9xG5mIwxkhumTox/MIRNcOgDrxWsMt2pAr23WHp6MrRlN7FBSFpCpr+oVO0F744iUgR82nJMfG2SA==",
             "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.2.tgz",
             "version": "1.1.2"
```

### Comparing `therix-0.1.2/therix/docs/package.json` & `therix-0.1.3/therix/docs/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9887152777777778%*

 * *Differences: {"'dependencies'": "{'@docusaurus/plugin-client-redirects': '3.2.0'}",*

 * * "'scripts'": "{'start': 'docusaurus start --port=3030 --host=0.0.0.0'}"}*

```diff
@@ -9,14 +9,15 @@
             ">0.5%",
             "not dead",
             "not op_mini all"
         ]
     },
     "dependencies": {
         "@docusaurus/core": "3.2.0",
+        "@docusaurus/plugin-client-redirects": "3.2.0",
         "@docusaurus/preset-classic": "3.2.0",
         "@mdx-js/react": "^3.0.0",
         "clsx": "^2.0.0",
         "prism-react-renderer": "^2.3.0",
         "react": "^18.0.0",
         "react-dom": "^18.0.0"
     },
@@ -31,14 +32,14 @@
     "private": true,
     "scripts": {
         "build": "docusaurus build",
         "clear": "docusaurus clear",
         "deploy": "docusaurus deploy",
         "docusaurus": "docusaurus",
         "serve": "docusaurus serve",
-        "start": "docusaurus start",
+        "start": "docusaurus start --port=3030 --host=0.0.0.0",
         "swizzle": "docusaurus swizzle",
         "write-heading-ids": "docusaurus write-heading-ids",
         "write-translations": "docusaurus write-translations"
     },
     "version": "0.0.0"
 }
```

### Comparing `therix-0.1.2/therix/docs/sidebars.js` & `therix-0.1.3/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.3/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/src/css/custom.css` & `therix-0.1.3/therix/docs/src/css/custom.css`

 * *Files 2% similar despite different names*

```diff
@@ -46,7 +46,12 @@
   --ifm-color-primary-darker: #1976d2; /* Adjusted darker primary color */
   --ifm-color-primary-darkest: #1565c0; /* Adjusted darkest primary color */
   --ifm-color-primary-light: #42a5f5; /* Adjusted light primary color */
   --ifm-color-primary-lighter: #64b5f6; /* Adjusted lighter primary color */
   --ifm-color-primary-lightest: #90caf9; /* Adjusted lightest primary color */
   --docusaurus-highlighted-code-line-bg: rgba(0, 0, 0, 0.3); /* Assuming you want to keep this as is */
 }
+
+
+.hidden {
+  display: none !important;
+  }
```

### Comparing `therix-0.1.2/therix/docs/static/img/coditas.png` & `therix-0.1.3/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.3/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.3/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/docusaurus.png` & `therix-0.1.3/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/entities/models.py` & `therix-0.1.3/therix/entities/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,86 @@
-from sqlalchemy import Column, String, Boolean, DateTime, ForeignKey, JSON, Enum
+import enum
+from sqlalchemy import Column, String, Boolean, DateTime, ForeignKey, JSON
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.orm import relationship
-from sqlalchemy.ext.declarative import declarative_base
 import uuid
-import enum
 
-# from db.base import Base
-Base = declarative_base()
+from sqlalchemy.orm import DeclarativeBase
+import sqlalchemy as sa
+
+from therix.core.constants import PipelineTypeMaster
+
+
+# Creating a base class
+class Base(DeclarativeBase):
+    pass
+
 
-# Define an ENUM for configuration types
 class ConfigType(enum.Enum):
     INPUT_SOURCE = "INPUT_SOURCE"
     EMBEDDING_MODEL = "EMBEDDING_MODEL"
     INFERENCE_MODEL = "INFERENCE_MODEL"
     OUTPUT_SOURCE = "OUTPUT_SOURCE"
     TRACE_DETAILS = "TRACE_DETAILS"
+    PII_FILTER = "PII_FILTER"
+    SUMMARIZER = "SUMMARIZER"
+    CACHE_CONFIG = "CACHE_CONFIG"
+
 
 class Pipeline(Base):
-    __tablename__ = 'pipelines'
+    __tablename__ = "pipelines"
 
-    id = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4, unique=True, nullable=False)
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
     name = Column(String, nullable=False)
-    status = Column(String, default='IN_DRAFT')  # Adjust default value as needed
+    type = Column(
+        sa.Enum(PipelineTypeMaster)
+    )
+    status = Column(String, default="IN_DRAFT")  # Adjust default value as needed
     is_deleted = Column(Boolean, default=False)
     deleted_at = Column(DateTime, nullable=True)
     custom_data = Column(JSON, default=dict)
 
     configurations = relationship("PipelineConfiguration", back_populates="pipeline")
     chat_history = relationship("ChatHistory", back_populates="pipeline")
 
 
 class PipelineConfiguration(Base):
-    __tablename__ = 'pipeline_configurations'
+    __tablename__ = "pipeline_configurations"
 
-    id = Column(UUID(as_uuid=True), primary_key=True, default=uuid.uuid4, unique=True, nullable=False)
-    pipeline_id = Column(UUID(as_uuid=True), ForeignKey('pipelines.id'))
-    config_type = Column(Enum(ConfigType)) 
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    pipeline_id = Column(UUID(as_uuid=True), ForeignKey("pipelines.id"))
+    config_type = Column(
+        sa.Enum(ConfigType, name="configtype", create_constraint=True), nullable=False
+    )
     name = Column(String, nullable=False)
     config = Column(JSON, default=dict)
     custom_data = Column(JSON, default=dict)
     pipeline = relationship("Pipeline", back_populates="configurations")
 
 
 class ChatHistory(Base):
-    __tablename__ = 'chat_history'
+    __tablename__ = "chat_history"
 
-    id = Column(UUID(as_uuid=True), primary_key=True,
-                default=uuid.uuid4, unique=True, nullable=False)
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
     message = Column(String, nullable=False)
-    message_role = Column(String, nullable=False)
-    user_id = Column(String, nullable=False)
-    pipeline_id = Column(UUID(as_uuid=True), ForeignKey(
-        'pipelines.id'))
+    message_role=Column(String, nullable=False)
+    pipeline_id = Column(UUID(as_uuid=True), ForeignKey("pipelines.id"))
     pipeline = relationship("Pipeline", back_populates="chat_history")
     session_id = Column(UUID(as_uuid=True), default=uuid.uuid4, nullable=False)
```

### Comparing `therix-0.1.2/therix/services/pipeline_service.py` & `therix-0.1.3/therix/services/pipeline_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from therix.utils.summarizer import summarizer
+from therix.utils.rag import chat, create_embeddings, get_loader, get_vectorstore
+from ..db.session import SessionLocal
+from ..entities.models import ConfigType, Pipeline, PipelineConfiguration
 import json
 import os
 import urllib
 from therix.services.web_crawling import crawl_website
+from therix.utils.pii_filter import pii_filter
 from therix.utils.rag import chat, create_embeddings, get_vectorstore
 from ..db.session import SessionLocal
-from ..entities.models import Pipeline, PipelineConfiguration
+from ..entities.models import ConfigType, Pipeline, PipelineConfiguration
 from therix.utils.rag import chat, create_embeddings, get_vectorstore
 
 
 class PipelineService:
     def __init__(self):
         self.db_session = SessionLocal()
 
@@ -75,19 +80,31 @@
             pipeline_id, "EMBEDDING_MODEL"
         )
         store = get_vectorstore(embedding_model[0], str(pipeline_id))
         retreiver = store.as_retriever()
         inference_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "INFERENCE_MODEL"
         )
-        return chat(
+        result = chat(
             question,
             retreiver,
             inference_model[0],
             embedding_model,
             session_id,
             pipeline_id,
             trace_details,
         )
-
+        pii_filter_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.PII_FILTER)
+        if pii_filter_config:
+            pii_filter_config = pii_filter_config[0].config
+            entities = pii_filter_config['entities']
+            return pii_filter(result,entities)
+        else:
+            return result
+
+    def invoke_summarizer_pipeline(self, pipeline_id, text, trace_details=None):
+        inference_model = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.INFERENCE_MODEL)
+        summarizer_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.SUMMARIZER)[0].config
+        return summarizer(summarizer_config,inference_model[0],text)
+    
     def __del__(self):
         self.db_session.close()
```

### Comparing `therix-0.1.2/therix/services/web_crawling.py` & `therix-0.1.3/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.2/therix/utils/rag.py` & `therix-0.1.3/therix/utils/rag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import json
 from operator import itemgetter
 from pathlib import Path
+from urllib import response
 from langchain.docstore.document import Document
 from langchain_community.document_loaders import TextLoader, PyPDFLoader
 from langchain_community.vectorstores.pgvector import PGVector
 from langchain_openai import OpenAIEmbeddings, ChatOpenAI
 from langchain_openai import AzureOpenAI
 from langchain_groq import ChatGroq
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
-from langchain_community.document_loaders import YoutubeLoader
-from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+from langchain_community.document_loaders.youtube import YoutubeLoader
+from langchain_core.prompts import ChatPromptTemplate
 from langchain_openai import AzureOpenAIEmbeddings
-
 from therix.core.JSONLoader import JSONLoader
-from langchain_community.embeddings import BedrockEmbeddings
+from langchain_community.embeddings.bedrock import BedrockEmbeddings
 import boto3
 from langchain_community.llms import Bedrock
+from therix.core.chat_history.base_chat_history import TherixChatMessageHistory
 from therix.core.constants import (
     DataSourceMaster,
     EmbeddingModelMaster,
     InferenceModelMaster,
 )
 from therix.db.session import SQLALCHEMY_DATABASE_URL
 from langfuse.callback import CallbackHandler
 from langchain_core.prompts import PromptTemplate
 from langchain_community.vectorstores.pgvector import PGVector
-from langchain.memory import PostgresChatMessageHistory
 from langchain.prompts import PromptTemplate
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import get_buffer_string
 from langchain_core.prompts import format_document
 from langchain_core.runnables import RunnableParallel
@@ -198,18 +198,19 @@
             secret_key=trace_details["secret_key"],
             public_key=trace_details["public_key"],
             host=trace_details["host"],
             trace_name=trace_details["identifier"],
         )
         chain_callbacks.append(langfuse_handler)
 
-    history = PostgresChatMessageHistory(
-        connection_string=SQLALCHEMY_DATABASE_URL,
+    history = TherixChatMessageHistory(
+        str(session_id),
+        str(pipeline_id),
+        SQLALCHEMY_DATABASE_URL,
         table_name="chat_history",
-        session_id=str(session_id),
     )
     chat_history = history.messages
 
     template = """Answer the question based only on the following context:
                      {context}
 
                     Question: {question}
@@ -244,11 +245,13 @@
         "context": itemgetter("standalone_question") | retriever | _combine_documents,
         "question": lambda x: x["standalone_question"],
     }
     conversational_qa_chain = _inputs | _context | ANSWER_PROMPT | model
     result = conversational_qa_chain.invoke(
         {"question": question, "chat_history": chat_history}
     )
-
-    history.add_user_message(question)
-    history.add_ai_message(result)
-    return json.loads(result.json())["content"]
+    
+    response=json.loads(result.json())["content"]
+    
+    history.add_message("user",question,pipeline_id,session_id)
+    history.add_message("system",response,pipeline_id,session_id)
+    return response
```

### Comparing `therix-0.1.2/PKG-INFO` & `therix-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.2
+Version: 0.1.3
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (==1.13.1)
 Requires-Dist: alembic-postgresql-enum (==1.1.2)
 Requires-Dist: boto3 (>=1.34.81,<2.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
+Requires-Dist: coverage (>=7.4.4,<8.0.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: langchain (==0.1.13)
 Requires-Dist: langchain-groq (>=0.1.0,<0.2.0)
 Requires-Dist: langchain-openai (==0.1.1)
+Requires-Dist: langchain-postgres (>=0.0.3,<0.0.4)
 Requires-Dist: langfuse (==2.21.1)
 Requires-Dist: pgvector (==0.2.5)
+Requires-Dist: presidio-analyzer (>=2.2.354,<3.0.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: psycopg[binary,pool] (>=3.1.18,<4.0.0)
+Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pypdf (==4.1.0)
+Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: selenium (>=4.19.0,<5.0.0)
 Requires-Dist: sqlalchemy (==2.0.28)
 Requires-Dist: tiktoken (==0.6.0)
 Requires-Dist: wheel (>=0.43.0,<0.44.0)
 Requires-Dist: youtube-transcript-api (>=0.6.2,<0.7.0)
 Description-Content-Type: text/markdown
```

