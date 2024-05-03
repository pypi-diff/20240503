# Comparing `tmp/zettel_org-0.6.4.tar.gz` & `tmp/zettel_org-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.6.4.tar", last modified: Sat Apr 27 22:41:38 2024, max compression
+gzip compressed data, was "zettel_org-0.7.0.tar", last modified: Fri May  3 01:28:46 2024, max compression
```

## Comparing `zettel_org-0.6.4.tar` & `zettel_org-0.7.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-27 22:41:30.000000 zettel_org-0.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-27 22:41:30.000000 zettel_org-0.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-27 22:41:30.000000 zettel_org-0.6.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-27 22:41:30.000000 zettel_org-0.6.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-27 22:41:38.510029 zettel_org-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-27 22:41:30.000000 zettel_org-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.490029 zettel_org-0.6.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2663 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-27 22:41:30.000000 zettel_org-0.6.4/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 22:41:30.000000 zettel_org-0.6.4/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-27 22:41:30.000000 zettel_org-0.6.4/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.482029 zettel_org-0.6.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/examples/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_query/all_contexts.zoq
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 22:41:30.000000 zettel_org-0.6.4/examples/zorg_query/open_projects.zoq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-27 22:41:30.000000 zettel_org-0.6.4/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 22:41:30.000000 zettel_org-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-27 22:41:30.000000 zettel_org-0.6.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.494029 zettel_org-0.6.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-27 22:41:30.000000 zettel_org-0.6.4/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-27 22:41:38.510029 zettel_org-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-27 22:41:30.000000 zettel_org-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.482029 zettel_org-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:41:34.000000 zettel_org-0.6.4/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-27 22:41:38.000000 zettel_org-0.6.4/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.498029 zettel_org-0.6.4/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/messages/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/domain/models/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/_zorg_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/models/_zorg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   119519 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.502029 zettel_org-0.6.4/src/zorg/grammar/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.g4
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.interp
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQuery.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryListener.py
--rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/grammar/zorg_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/service/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_file_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/compiler/_query_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/file/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/file/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-27 22:41:30.000000 zettel_org-0.6.4/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-27 22:41:30.000000 zettel_org-0.6.4/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.506029 zettel_org-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    70292 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:41:38.510029 zettel_org-0.6.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-27 22:41:30.000000 zettel_org-0.6.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.234107 zettel_org-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.214107 zettel_org-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.214107 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.214107 zettel_org-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 01:28:35.000000 zettel_org-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-03 01:28:35.000000 zettel_org-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 01:28:35.000000 zettel_org-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-03 01:28:35.000000 zettel_org-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 01:28:35.000000 zettel_org-0.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-03 01:28:35.000000 zettel_org-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-05-03 01:28:46.234107 zettel_org-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-03 01:28:35.000000 zettel_org-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.214107 zettel_org-0.7.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2663 2024-05-03 01:28:35.000000 zettel_org-0.7.0/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-03 01:28:35.000000 zettel_org-0.7.0/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-03 01:28:35.000000 zettel_org-0.7.0/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-03 01:28:35.000000 zettel_org-0.7.0/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-03 01:28:35.000000 zettel_org-0.7.0/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 01:28:35.000000 zettel_org-0.7.0/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 01:28:35.000000 zettel_org-0.7.0/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.206107 zettel_org-0.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.218107 zettel_org-0.7.0/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/examples/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_query/all_contexts.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 01:28:35.000000 zettel_org-0.7.0/examples/zorg_query/open_projects.zoq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-03 01:28:35.000000 zettel_org-0.7.0/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-03 01:28:35.000000 zettel_org-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 01:28:35.000000 zettel_org-0.7.0/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-03 01:28:35.000000 zettel_org-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 01:28:35.000000 zettel_org-0.7.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-03 01:28:35.000000 zettel_org-0.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 01:28:35.000000 zettel_org-0.7.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-03 01:28:46.238107 zettel_org-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-03 01:28:35.000000 zettel_org-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.206107 zettel_org-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.234107 zettel_org-0.7.0/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 01:28:42.000000 zettel_org-0.7.0/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 01:28:46.000000 zettel_org-0.7.0/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.222107 zettel_org-0.7.0/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.226107 zettel_org-0.7.0/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.226107 zettel_org-0.7.0/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/messages/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.226107 zettel_org-0.7.0/src/zorg/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/models/_zorg_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/models/_zorg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.226107 zettel_org-0.7.0/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.226107 zettel_org-0.7.0/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119519 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/grammar/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQuery.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQuery.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQuery.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23293 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/grammar/zorg_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/service/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/compiler/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/compiler/_file_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/compiler/_query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/file/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/file/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.230107 zettel_org-0.7.0/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-03 01:28:35.000000 zettel_org-0.7.0/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-03 01:28:35.000000 zettel_org-0.7.0/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.234107 zettel_org-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.234107 zettel_org-0.7.0/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    71232 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 01:28:46.234107 zettel_org-0.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 01:28:35.000000 zettel_org-0.7.0/tox.ini
```

### Comparing `zettel_org-0.6.4/.cruft.json` & `zettel_org-0.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/.github/labels.yml` & `zettel_org-0.7.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/.github/workflows/ci.yml` & `zettel_org-0.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/.gitignore` & `zettel_org-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/.pylintrc` & `zettel_org-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/.readthedocs.yml` & `zettel_org-0.7.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/CHANGELOG.md` & `zettel_org-0.7.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.6.4...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.0...HEAD)
 
 No notable changes have been made.
 
 
+## [0.7.0](https://github.com/bbugyi200/zorg/compare/0.6.4...0.7.0) - 2024-05-02
+
+### Changed
+
+* *BREAKING CHANGE*: Expect final line of keep-alive file to be the full path
+  of the file in the currently focused buffer.
+
+
 ## [0.6.4](https://github.com/bbugyi200/zorg/compare/0.6.3...0.6.4) - 2024-04-27
 
 ### Changed
 
 * Add `zorg query` command that does nothing ATM.
 * Stop generating ZIDs which use any of the following characters based on
   similarity to digits OR because the lowercase letter hangs over an underline: `SQgipqy`
```

### Comparing `zettel_org-0.6.4/CONTRIBUTING.md` & `zettel_org-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/Dockerfile` & `zettel_org-0.7.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/Makefile` & `zettel_org-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/PKG-INFO` & `zettel_org-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.4
+Version: 0.7.0
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.6.4/README.md` & `zettel_org-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/bin/build_zorg_grammars` & `zettel_org-0.7.0/bin/build_zorg_grammars`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/bin/check_cc` & `zettel_org-0.7.0/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/bin/publish_docs` & `zettel_org-0.7.0/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/bin/quick-lints` & `zettel_org-0.7.0/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/bin/render_all_cogs` & `zettel_org-0.7.0/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/docs/Makefile` & `zettel_org-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/docs/make.bat` & `zettel_org-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/docs/source/conf.py` & `zettel_org-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/examples/zorg_file/20240323.zo` & `zettel_org-0.7.0/examples/zorg_file/20240323.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/examples/zorg_file/scrambled_prj_notes.zo` & `zettel_org-0.7.0/examples/zorg_file/scrambled_prj_notes.zo`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/lib/bugyi.sh` & `zettel_org-0.7.0/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/requirements-dev.in` & `zettel_org-0.7.0/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/requirements-dev.txt` & `zettel_org-0.7.0/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 docutils==0.20.1
     # via
     #   m2r2
     #   sphinx
     #   sphinx-rtd-theme
 exceptiongroup==1.2.1
     # via pytest
-filelock==3.13.4
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via -r requirements-dev.in
 freezegun==1.5.0
     # via -r requirements-dev.in
@@ -189,15 +189,15 @@
     # via flake8
 pygments==2.17.2
     # via
     #   rich
     #   sphinx
 pylint==3.1.0
     # via -r requirements-dev.in
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 pytest==7.4.4
     # via
     #   -r requirements-dev.in
     #   pytest-cov
@@ -263,15 +263,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sqlalchemy==2.0.29
     # via sqlmodel
-sqlmodel==0.0.16
+sqlmodel==0.0.18
     # via
     #   -r requirements.in
     #   zettel-org
 structlog==24.1.0
     # via bolton-logrus
 syrupy==4.6.1
     # via -r requirements-dev.in
@@ -284,15 +284,14 @@
     #   black
     #   build
     #   coverage
     #   mypy
     #   pip-tools
     #   pydocstyle
     #   pylint
-    #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   sphinx
     #   tox
 tomlkit==0.12.4
     # via pylint
 tox==3.28.0
@@ -323,15 +322,15 @@
     #   typer
 urllib3==2.2.1
     # via requests
 vimala==0.2.0
     # via
     #   -r requirements.in
     #   zettel-org
-virtualenv==20.26.0
+virtualenv==20.26.1
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
```

### Comparing `zettel_org-0.6.4/requirements.txt` & `zettel_org-0.7.0/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     # via bolton-clack
 python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via bolton-clack
 sqlalchemy==2.0.29
     # via sqlmodel
-sqlmodel==0.0.16
+sqlmodel==0.0.18
     # via -r requirements.in
 structlog==24.1.0
     # via bolton-logrus
 tqdm==4.66.2
     # via -r requirements.in
 typing-extensions==4.11.0
     # via
```

### Comparing `zettel_org-0.6.4/setup.cfg` & `zettel_org-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 show_error_context = True
 warn_redundant_casts = True
 warn_return_any = True
 warn_unreachable = True
 warn_unused_configs = True
 warn_unused_ignores = True
 
-[mypy-zorg.service.compiler._file_compiler]
+[mypy-zorg.service.compiler._file_compiler,zorg.service.compiler._query_compiler]
 disallow_untyped_calls = False
 
 [mypy-zorg.grammar.*]
 follow_imports = silent
 
 [mypy-antlr4.*,pluggy.*,setuptools.*]
 ignore_missing_imports = True
```

### Comparing `zettel_org-0.6.4/setup.py` & `zettel_org-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.6.4"}
+USE_SCM_VERSION = {"fallback_version": "0.7.0"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.6.4/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.7.0/src/zettel_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.6.4
+Version: 0.7.0
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `zettel_org-0.6.4/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.7.0/src/zettel_org.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/config.py` & `zettel_org-0.7.0/src/zorg/app/config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/__init__.py` & `zettel_org-0.7.0/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/_run_action.py` & `zettel_org-0.7.0/src/zorg/app/runners/_run_action.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.7.0/src/zorg/app/runners/_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/_run_db.py` & `zettel_org-0.7.0/src/zorg/app/runners/_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.7.0/src/zorg/app/runners/_run_edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     zo_paths = prepend_zdir(cfg.zettel_dir, zo_paths)
     for zo_path in zo_paths:
         init_from_template(cfg.zettel_dir, cfg.template_pattern_map, zo_path)
 
     messagebus.handle(
         [
             commands.EditCommand(
-                zettel_dir=cfg.zettel_dir,
-                paths=zo_paths,
                 keep_alive_file=cfg.keep_alive_file,
+                paths=zo_paths,
+                verbose=cfg.verbose,
                 vim_commands=cfg.vim_commands,
+                zettel_dir=cfg.zettel_dir,
             ),
         ],
         SQLSession(cfg.zettel_dir, cfg.database_url),
     )
     return 0
```

### Comparing `zettel_org-0.6.4/src/zorg/app/runners/_run_template.py` & `zettel_org-0.7.0/src/zorg/app/runners/_run_template.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/domain/messages/commands.py` & `zettel_org-0.7.0/src/zorg/domain/messages/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 @dataclass(frozen=True)
 class EditCommand(Command):
     """Command to open one or more zorg files using an editor."""
 
     paths: list[Path]
     keep_alive_file: Path
     vim_commands: list[str]
+    verbose: int = 0
 
 
 @dataclass(frozen=True)
 class CreateDBCommand(Command):
     """Command to (re)create zorg's database from scratch."""
```

### Comparing `zettel_org-0.6.4/src/zorg/domain/messages/events.py` & `zettel_org-0.7.0/src/zorg/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/domain/models/_zorg_file.py` & `zettel_org-0.7.0/src/zorg/domain/models/_zorg_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """This file contains Zorg's domain model classes."""
 
 from dataclasses import dataclass, field
 import datetime as dt
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 
-from ..types import TodoPriorityType, TodoStatus
+from ..types import NoteStatus, TodoPriorityType
 
 
 if TYPE_CHECKING:
     from ..messages.events import Event
 
 
 @dataclass(frozen=True)
 class TodoPayload:
     """Extra fields that are added to ZorgNotes that are todos."""
 
     priority: TodoPriorityType = "C"
-    status: TodoStatus = TodoStatus.OPEN
+    status: NoteStatus = NoteStatus.OPEN_TODO
 
 
 @dataclass
 class ZorgNote:
     """A Zorg note."""
 
     body: str
```

### Comparing `zettel_org-0.6.4/src/zorg/domain/models/_zorg_query.py` & `zettel_org-0.7.0/src/zorg/domain/models/_zorg_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dataclasses import dataclass, field
 import datetime as dt
 from typing import Iterable, Optional
 
 from ..types import (
     DescOperator,
+    NoteStatus,
     PropertyOperator,
     PropertyValueType,
     Select,
     TodoPriorityType,
 )
 
 
@@ -40,35 +41,46 @@
     end: Optional[dt.date] = None
 
 
 @dataclass
 class WhereAndFilter:
     """Tag used to filter ZorgNotes."""
 
+    allowed_note_statuses: set[NoteStatus] = field(default_factory=set)
     areas: list[str] = field(default_factory=list)
     contexts: list[str] = field(default_factory=list)
     create_date_ranges: list[DateRange] = field(default_factory=list)
     desc_filters: list[DescFilter] = field(default_factory=list)
-    done: Optional[bool] = None
     modify_date_ranges: list[DateRange] = field(default_factory=list)
     or_filters: list["WhereOrFilter"] = field(default_factory=list)
     people: list[str] = field(default_factory=list)
     property_filters: list[PropertyFilter] = field(default_factory=list)
     priorities: list[TodoPriorityType] = field(default_factory=list)
     projects: list[str] = field(default_factory=list)
 
+    def __repr__(self) -> str:
+        """String representation that only shows fields if they are set."""
+        dict_repr = ", ".join(
+            f"{k}={v!r}"
+            for k, v in filter(
+                lambda item: bool(item[1]), self.__dict__.items()
+            )
+        )
+
+        return f"{self.__class__.__name__}({dict_repr})"
+
 
 @dataclass(frozen=True)
 class WhereOrFilter:
     """A collection of `WhereAndFilter`s that have been ORed together."""
 
-    and_queries: Iterable[WhereAndFilter]
+    and_filters: Iterable[WhereAndFilter]
 
 
-@dataclass(frozen=True)
+@dataclass
 class ZorgQuery:
     """A zorg query that uses SWOG syntax.
 
     (S)ELECT
     (W)HERE
     (O)RDER BY
     (G)ROUP BY
```

### Comparing `zettel_org-0.6.4/src/zorg/domain/types.py` & `zettel_org-0.7.0/src/zorg/domain/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,22 +51,23 @@
     "Z",
 ]
 TemplatePatternMapType = Mapping[Pattern, Path]
 VarMapType = Mapping[str, Any]
 TodoStatusPrefixChar = Literal["o", "x", "~", "<", ">"]
 
 
-class TodoStatus(enum.Enum):
-    """Zorg todo status."""
+class NoteStatus(enum.Enum):
+    """Zorg note status."""
 
-    OPEN = enum.auto()  # o
-    CLOSED = enum.auto()  # x
-    CANCELED = enum.auto()  # ~
-    BLOCKED = enum.auto()  # <
-    PARENT = enum.auto()  # >
+    BASIC = enum.auto()  # -
+    OPEN_TODO = enum.auto()  # o
+    CLOSED_TODO = enum.auto()  # x
+    CANCELED_TODO = enum.auto()  # ~
+    BLOCKED_TODO = enum.auto()  # <
+    PARENT_TODO = enum.auto()  # >
 
 
 class CreateEngineType(Protocol):
     """The type of a `db.create_engine()` callable."""
 
     def __call__(self, url: str, /, **kwargs: Any) -> Engine:
         """The function's call signature."""
@@ -78,15 +79,19 @@
     CONTAINS = enum.auto()
     NOT_CONTAINS = enum.auto()
 
 
 class Select(enum.Enum):
     """A zorg query (S)ELECT."""
 
+    AREAS = enum.auto()
+    CONTEXTS = enum.auto()
+    FILES = enum.auto()
     NOTES = enum.auto()
+    PEOPLE = enum.auto()
     PROJECTS = enum.auto()
 
 
 class PropertyOperator(enum.Enum):
     """Used to determine what kind of metatag constraint has been specified."""
 
     # exists / not exists
```

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.g4` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.g4`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFile.tokens` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.7.0/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp` & `zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp`

 * *Files 23% similar despite different names*

```diff
@@ -2,55 +2,70 @@
 null
 'S'
 'W'
 'O'
 'G'
 'file'
 'note'
-'@'
-'#'
+null
+' '
 '+'
+'@'
 '%'
+'#'
+'-'
 'o'
-null
-' '
+'x'
+'<'
+'>'
+'~'
 
 token symbolic names:
 null
 null
 null
 null
 null
 null
 null
-null
-null
-null
-null
-null
 NL
 SPACE
+PLUS
+AT_SIGN
+PERCENT
+HASH
+DASH
+LOWER_O
+LOWER_X
+LANGLE
+RANGLE
+TILDE
 
 rule names:
 T__0
 T__1
 T__2
 T__3
 T__4
 T__5
-T__6
-T__7
-T__8
-T__9
-T__10
 NL
 SPACE
+PLUS
+AT_SIGN
+PERCENT
+HASH
+DASH
+LOWER_O
+LOWER_X
+LANGLE
+RANGLE
+TILDE
 
 channel names:
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[4, 0, 13, 62, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 11, 3, 11, 57, 8, 11, 1, 11, 1, 11, 1, 12, 1, 12, 0, 0, 13, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 1, 0, 0, 62, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 1, 27, 1, 0, 0, 0, 3, 29, 1, 0, 0, 0, 5, 31, 1, 0, 0, 0, 7, 33, 1, 0, 0, 0, 9, 35, 1, 0, 0, 0, 11, 40, 1, 0, 0, 0, 13, 45, 1, 0, 0, 0, 15, 47, 1, 0, 0, 0, 17, 49, 1, 0, 0, 0, 19, 51, 1, 0, 0, 0, 21, 53, 1, 0, 0, 0, 23, 56, 1, 0, 0, 0, 25, 60, 1, 0, 0, 0, 27, 28, 5, 83, 0, 0, 28, 2, 1, 0, 0, 0, 29, 30, 5, 87, 0, 0, 30, 4, 1, 0, 0, 0, 31, 32, 5, 79, 0, 0, 32, 6, 1, 0, 0, 0, 33, 34, 5, 71, 0, 0, 34, 8, 1, 0, 0, 0, 35, 36, 5, 102, 0, 0, 36, 37, 5, 105, 0, 0, 37, 38, 5, 108, 0, 0, 38, 39, 5, 101, 0, 0, 39, 10, 1, 0, 0, 0, 40, 41, 5, 110, 0, 0, 41, 42, 5, 111, 0, 0, 42, 43, 5, 116, 0, 0, 43, 44, 5, 101, 0, 0, 44, 12, 1, 0, 0, 0, 45, 46, 5, 64, 0, 0, 46, 14, 1, 0, 0, 0, 47, 48, 5, 35, 0, 0, 48, 16, 1, 0, 0, 0, 49, 50, 5, 43, 0, 0, 50, 18, 1, 0, 0, 0, 51, 52, 5, 37, 0, 0, 52, 20, 1, 0, 0, 0, 53, 54, 5, 111, 0, 0, 54, 22, 1, 0, 0, 0, 55, 57, 5, 13, 0, 0, 56, 55, 1, 0, 0, 0, 56, 57, 1, 0, 0, 0, 57, 58, 1, 0, 0, 0, 58, 59, 5, 10, 0, 0, 59, 24, 1, 0, 0, 0, 60, 61, 5, 32, 0, 0, 61, 26, 1, 0, 0, 0, 2, 0, 56, 0]
+[4, 0, 18, 82, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 57, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 11, 1, 11, 1, 12, 1, 12, 1, 13, 1, 13, 1, 14, 1, 14, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 0, 0, 18, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 1, 0, 0, 82, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 1, 37, 1, 0, 0, 0, 3, 39, 1, 0, 0, 0, 5, 41, 1, 0, 0, 0, 7, 43, 1, 0, 0, 0, 9, 45, 1, 0, 0, 0, 11, 50, 1, 0, 0, 0, 13, 56, 1, 0, 0, 0, 15, 60, 1, 0, 0, 0, 17, 62, 1, 0, 0, 0, 19, 64, 1, 0, 0, 0, 21, 66, 1, 0, 0, 0, 23, 68, 1, 0, 0, 0, 25, 70, 1, 0, 0, 0, 27, 72, 1, 0, 0, 0, 29, 74, 1, 0, 0, 0, 31, 76, 1, 0, 0, 0, 33, 78, 1, 0, 0, 0, 35, 80, 1, 0, 0, 0, 37, 38, 5, 83, 0, 0, 38, 2, 1, 0, 0, 0, 39, 40, 5, 87, 0, 0, 40, 4, 1, 0, 0, 0, 41, 42, 5, 79, 0, 0, 42, 6, 1, 0, 0, 0, 43, 44, 5, 71, 0, 0, 44, 8, 1, 0, 0, 0, 45, 46, 5, 102, 0, 0, 46, 47, 5, 105, 0, 0, 47, 48, 5, 108, 0, 0, 48, 49, 5, 101, 0, 0, 49, 10, 1, 0, 0, 0, 50, 51, 5, 110, 0, 0, 51, 52, 5, 111, 0, 0, 52, 53, 5, 116, 0, 0, 53, 54, 5, 101, 0, 0, 54, 12, 1, 0, 0, 0, 55, 57, 5, 13, 0, 0, 56, 55, 1, 0, 0, 0, 56, 57, 1, 0, 0, 0, 57, 58, 1, 0, 0, 0, 58, 59, 5, 10, 0, 0, 59, 14, 1, 0, 0, 0, 60, 61, 5, 32, 0, 0, 61, 16, 1, 0, 0, 0, 62, 63, 5, 43, 0, 0, 63, 18, 1, 0, 0, 0, 64, 65, 5, 64, 0, 0, 65, 20, 1, 0, 0, 0, 66, 67, 5, 37, 0, 0, 67, 22, 1, 0, 0, 0, 68, 69, 5, 35, 0, 0, 69, 24, 1, 0, 0, 0, 70, 71, 5, 45, 0, 0, 71, 26, 1, 0, 0, 0, 72, 73, 5, 111, 0, 0, 73, 28, 1, 0, 0, 0, 74, 75, 5, 120, 0, 0, 75, 30, 1, 0, 0, 0, 76, 77, 5, 60, 0, 0, 77, 32, 1, 0, 0, 0, 78, 79, 5, 62, 0, 0, 79, 34, 1, 0, 0, 0, 80, 81, 5, 126, 0, 0, 81, 36, 1, 0, 0, 0, 2, 0, 56, 0]
```

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryListener.py` & `zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryListener.py`

 * *Files 16% similar despite different names*

```diff
@@ -94,9 +94,27 @@
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#where_body.
     def exitWhere_body(self, ctx:ZorgQueryParser.Where_bodyContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgQueryParser#note_status.
+    def enterNote_status(self, ctx:ZorgQueryParser.Note_statusContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#note_status.
+    def exitNote_status(self, ctx:ZorgQueryParser.Note_statusContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#note_status_char.
+    def enterNote_status_char(self, ctx:ZorgQueryParser.Note_status_charContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#note_status_char.
+    def exitNote_status_char(self, ctx:ZorgQueryParser.Note_status_charContext):
+        pass
+
+
 
 del ZorgQueryParser
```

### Comparing `zettel_org-0.6.4/src/zorg/grammar/zorg_query/ZorgQueryParser.py` & `zettel_org-0.7.0/src/zorg/grammar/zorg_query/ZorgQueryParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,80 +6,92 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,13,60,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
-        6,2,7,7,7,2,8,7,8,2,9,7,9,1,0,1,0,1,0,1,1,1,1,3,1,26,8,1,1,2,1,2,
-        1,2,3,2,31,8,2,1,2,1,2,1,2,3,2,36,8,2,1,2,1,2,3,2,40,8,2,1,3,1,3,
-        1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,
-        1,9,0,0,10,0,2,4,6,8,10,12,14,16,18,0,1,1,0,5,10,53,0,20,1,0,0,0,
-        2,25,1,0,0,0,4,30,1,0,0,0,6,41,1,0,0,0,8,43,1,0,0,0,10,47,1,0,0,
-        0,12,51,1,0,0,0,14,53,1,0,0,0,16,55,1,0,0,0,18,57,1,0,0,0,20,21,
-        3,2,1,0,21,22,5,12,0,0,22,1,1,0,0,0,23,26,3,4,2,0,24,26,3,6,3,0,
-        25,23,1,0,0,0,25,24,1,0,0,0,26,3,1,0,0,0,27,28,3,8,4,0,28,29,5,13,
-        0,0,29,31,1,0,0,0,30,27,1,0,0,0,30,31,1,0,0,0,31,32,1,0,0,0,32,35,
-        3,10,5,0,33,34,5,13,0,0,34,36,3,12,6,0,35,33,1,0,0,0,35,36,1,0,0,
-        0,36,39,1,0,0,0,37,38,5,13,0,0,38,40,3,14,7,0,39,37,1,0,0,0,39,40,
-        1,0,0,0,40,5,1,0,0,0,41,42,3,8,4,0,42,7,1,0,0,0,43,44,5,1,0,0,44,
-        45,5,13,0,0,45,46,3,16,8,0,46,9,1,0,0,0,47,48,5,2,0,0,48,49,5,13,
-        0,0,49,50,3,18,9,0,50,11,1,0,0,0,51,52,5,3,0,0,52,13,1,0,0,0,53,
-        54,5,4,0,0,54,15,1,0,0,0,55,56,7,0,0,0,56,17,1,0,0,0,57,58,5,11,
-        0,0,58,19,1,0,0,0,4,25,30,35,39
+        4,1,18,72,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,1,0,1,0,3,0,27,8,0,
+        1,1,1,1,3,1,31,8,1,1,2,1,2,1,2,3,2,36,8,2,1,2,1,2,1,2,3,2,41,8,2,
+        1,2,1,2,3,2,45,8,2,1,3,1,3,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,6,1,
+        6,1,7,1,7,1,8,1,8,1,9,1,9,1,10,4,10,66,8,10,11,10,12,10,67,1,11,
+        1,11,1,11,0,0,12,0,2,4,6,8,10,12,14,16,18,20,22,0,2,2,0,5,6,9,12,
+        1,0,13,18,65,0,24,1,0,0,0,2,30,1,0,0,0,4,35,1,0,0,0,6,46,1,0,0,0,
+        8,48,1,0,0,0,10,52,1,0,0,0,12,56,1,0,0,0,14,58,1,0,0,0,16,60,1,0,
+        0,0,18,62,1,0,0,0,20,65,1,0,0,0,22,69,1,0,0,0,24,26,3,2,1,0,25,27,
+        5,7,0,0,26,25,1,0,0,0,26,27,1,0,0,0,27,1,1,0,0,0,28,31,3,4,2,0,29,
+        31,3,6,3,0,30,28,1,0,0,0,30,29,1,0,0,0,31,3,1,0,0,0,32,33,3,8,4,
+        0,33,34,5,8,0,0,34,36,1,0,0,0,35,32,1,0,0,0,35,36,1,0,0,0,36,37,
+        1,0,0,0,37,40,3,10,5,0,38,39,5,8,0,0,39,41,3,12,6,0,40,38,1,0,0,
+        0,40,41,1,0,0,0,41,44,1,0,0,0,42,43,5,8,0,0,43,45,3,14,7,0,44,42,
+        1,0,0,0,44,45,1,0,0,0,45,5,1,0,0,0,46,47,3,8,4,0,47,7,1,0,0,0,48,
+        49,5,1,0,0,49,50,5,8,0,0,50,51,3,16,8,0,51,9,1,0,0,0,52,53,5,2,0,
+        0,53,54,5,8,0,0,54,55,3,18,9,0,55,11,1,0,0,0,56,57,5,3,0,0,57,13,
+        1,0,0,0,58,59,5,4,0,0,59,15,1,0,0,0,60,61,7,0,0,0,61,17,1,0,0,0,
+        62,63,3,20,10,0,63,19,1,0,0,0,64,66,3,22,11,0,65,64,1,0,0,0,66,67,
+        1,0,0,0,67,65,1,0,0,0,67,68,1,0,0,0,68,21,1,0,0,0,69,70,7,1,0,0,
+        70,23,1,0,0,0,6,26,30,35,40,44,67
     ]
 
 class ZorgQueryParser ( Parser ):
 
     grammarFileName = "ZorgQuery.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
     literalNames = [ "<INVALID>", "'S'", "'W'", "'O'", "'G'", "'file'", 
-                     "'note'", "'@'", "'#'", "'+'", "'%'", "'o'", "<INVALID>", 
-                     "' '" ]
+                     "'note'", "<INVALID>", "' '", "'+'", "'@'", "'%'", 
+                     "'#'", "'-'", "'o'", "'x'", "'<'", "'>'", "'~'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                      "NL", "SPACE" ]
+                      "<INVALID>", "<INVALID>", "<INVALID>", "NL", "SPACE", 
+                      "PLUS", "AT_SIGN", "PERCENT", "HASH", "DASH", "LOWER_O", 
+                      "LOWER_X", "LANGLE", "RANGLE", "TILDE" ]
 
     RULE_prog = 0
     RULE_query = 1
     RULE_where_query = 2
     RULE_select_query = 3
     RULE_select = 4
     RULE_where = 5
     RULE_order_by = 6
     RULE_group_by = 7
     RULE_select_body = 8
     RULE_where_body = 9
+    RULE_note_status = 10
+    RULE_note_status_char = 11
 
     ruleNames =  [ "prog", "query", "where_query", "select_query", "select", 
-                   "where", "order_by", "group_by", "select_body", "where_body" ]
+                   "where", "order_by", "group_by", "select_body", "where_body", 
+                   "note_status", "note_status_char" ]
 
     EOF = Token.EOF
     T__0=1
     T__1=2
     T__2=3
     T__3=4
     T__4=5
     T__5=6
-    T__6=7
-    T__7=8
-    T__8=9
-    T__9=10
-    T__10=11
-    NL=12
-    SPACE=13
+    NL=7
+    SPACE=8
+    PLUS=9
+    AT_SIGN=10
+    PERCENT=11
+    HASH=12
+    DASH=13
+    LOWER_O=14
+    LOWER_X=15
+    LANGLE=16
+    RANGLE=17
+    TILDE=18
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -114,20 +126,27 @@
 
 
 
     def prog(self):
 
         localctx = ZorgQueryParser.ProgContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_prog)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 20
+            self.state = 24
             self.query()
-            self.state = 21
-            self.match(ZorgQueryParser.NL)
+            self.state = 26
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==7:
+                self.state = 25
+                self.match(ZorgQueryParser.NL)
+
+
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -163,26 +182,26 @@
 
 
     def query(self):
 
         localctx = ZorgQueryParser.QueryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_query)
         try:
-            self.state = 25
+            self.state = 30
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,0,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,1,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 23
+                self.state = 28
                 self.where_query()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 24
+                self.state = 29
                 self.select_query()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -238,43 +257,43 @@
     def where_query(self):
 
         localctx = ZorgQueryParser.Where_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_where_query)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 30
+            self.state = 35
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==1:
-                self.state = 27
+                self.state = 32
                 self.select()
-                self.state = 28
+                self.state = 33
                 self.match(ZorgQueryParser.SPACE)
 
 
-            self.state = 32
+            self.state = 37
             self.where()
-            self.state = 35
+            self.state = 40
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,2,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,3,self._ctx)
             if la_ == 1:
-                self.state = 33
+                self.state = 38
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 34
+                self.state = 39
                 self.order_by()
 
 
-            self.state = 39
+            self.state = 44
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==13:
-                self.state = 37
+            if _la==8:
+                self.state = 42
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 38
+                self.state = 43
                 self.group_by()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -310,15 +329,15 @@
 
     def select_query(self):
 
         localctx = ZorgQueryParser.Select_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_select_query)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 41
+            self.state = 46
             self.select()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -355,19 +374,19 @@
 
     def select(self):
 
         localctx = ZorgQueryParser.SelectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_select)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 43
+            self.state = 48
             self.match(ZorgQueryParser.T__0)
-            self.state = 44
+            self.state = 49
             self.match(ZorgQueryParser.SPACE)
-            self.state = 45
+            self.state = 50
             self.select_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -404,19 +423,19 @@
 
     def where(self):
 
         localctx = ZorgQueryParser.WhereContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_where)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 47
+            self.state = 52
             self.match(ZorgQueryParser.T__1)
-            self.state = 48
+            self.state = 53
             self.match(ZorgQueryParser.SPACE)
-            self.state = 49
+            self.state = 54
             self.where_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -447,15 +466,15 @@
 
     def order_by(self):
 
         localctx = ZorgQueryParser.Order_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_order_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 51
+            self.state = 56
             self.match(ZorgQueryParser.T__2)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -486,15 +505,15 @@
 
     def group_by(self):
 
         localctx = ZorgQueryParser.Group_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 14, self.RULE_group_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 53
+            self.state = 58
             self.match(ZorgQueryParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -504,14 +523,25 @@
     class Select_bodyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
+        def AT_SIGN(self):
+            return self.getToken(ZorgQueryParser.AT_SIGN, 0)
+
+        def HASH(self):
+            return self.getToken(ZorgQueryParser.HASH, 0)
+
+        def PLUS(self):
+            return self.getToken(ZorgQueryParser.PLUS, 0)
+
+        def PERCENT(self):
+            return self.getToken(ZorgQueryParser.PERCENT, 0)
 
         def getRuleIndex(self):
             return ZorgQueryParser.RULE_select_body
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSelect_body" ):
                 listener.enterSelect_body(self)
@@ -526,17 +556,17 @@
     def select_body(self):
 
         localctx = ZorgQueryParser.Select_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 16, self.RULE_select_body)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 55
+            self.state = 60
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 2016) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 7776) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -549,14 +579,17 @@
     class Where_bodyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
+        def note_status(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Note_statusContext,0)
+
 
         def getRuleIndex(self):
             return ZorgQueryParser.RULE_where_body
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterWhere_body" ):
                 listener.enterWhere_body(self)
@@ -570,16 +603,134 @@
 
     def where_body(self):
 
         localctx = ZorgQueryParser.Where_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 18, self.RULE_where_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 57
-            self.match(ZorgQueryParser.T__10)
+            self.state = 62
+            self.note_status()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Note_statusContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def note_status_char(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgQueryParser.Note_status_charContext)
+            else:
+                return self.getTypedRuleContext(ZorgQueryParser.Note_status_charContext,i)
+
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_note_status
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterNote_status" ):
+                listener.enterNote_status(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitNote_status" ):
+                listener.exitNote_status(self)
+
+
+
+
+    def note_status(self):
+
+        localctx = ZorgQueryParser.Note_statusContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 20, self.RULE_note_status)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 65 
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while True:
+                self.state = 64
+                self.note_status_char()
+                self.state = 67 
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 516096) != 0)):
+                    break
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Note_status_charContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def DASH(self):
+            return self.getToken(ZorgQueryParser.DASH, 0)
+
+        def LOWER_O(self):
+            return self.getToken(ZorgQueryParser.LOWER_O, 0)
+
+        def LOWER_X(self):
+            return self.getToken(ZorgQueryParser.LOWER_X, 0)
+
+        def TILDE(self):
+            return self.getToken(ZorgQueryParser.TILDE, 0)
+
+        def LANGLE(self):
+            return self.getToken(ZorgQueryParser.LANGLE, 0)
+
+        def RANGLE(self):
+            return self.getToken(ZorgQueryParser.RANGLE, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_note_status_char
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterNote_status_char" ):
+                listener.enterNote_status_char(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitNote_status_char" ):
+                listener.exitNote_status_char(self)
+
+
+
+
+    def note_status_char(self):
+
+        localctx = ZorgQueryParser.Note_status_charContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 22, self.RULE_note_status_char)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 69
+            _la = self._input.LA(1)
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 516096) != 0)):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `zettel_org-0.6.4/src/zorg/service/common.py` & `zettel_org-0.7.0/src/zorg/service/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/service/compiler/_api.py` & `zettel_org-0.7.0/src/zorg/service/compiler/_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from pathlib import Path
 
 import antlr4
 
 from ...domain.models import ZorgFile, ZorgQuery
 from ...grammar.zorg_file.ZorgFileLexer import ZorgFileLexer
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
+from ...grammar.zorg_query.ZorgQueryLexer import ZorgQueryLexer
+from ...grammar.zorg_query.ZorgQueryParser import ZorgQueryParser
 from ._file_compiler import ErrorManager, ZorgFileCompiler
+from ._query_compiler import ZorgQueryCompiler
 
 
 def walk_zorg_file(
     zdir: Path, zo_path_part: Path, verbose: bool = False
 ) -> ZorgFile:
     """Create a new ZorgFileCompiler and walk through notes in {zorg_file}."""
     zo_path = (
@@ -30,10 +33,18 @@
     compiler = ZorgFileCompiler(zorg_file, error_manager)
     walker = antlr4.ParseTreeWalker()
     walker.walk(compiler, tree)
     return zorg_file
 
 
 def compile_zorg_query(query: str) -> ZorgQuery:
-    """Create a new ZorgQueryCompiler and use it to compile {query}."""
-    del query
-    return ZorgQuery()
+    """Constructs a new ZorgQuery using {query}."""
+    stream = antlr4.InputStream(query)
+    lexer = ZorgQueryLexer(stream)
+    tokens = antlr4.CommonTokenStream(lexer)
+    parser = ZorgQueryParser(tokens)
+    tree = parser.prog()  # type: ignore[no-untyped-call]
+    zorg_query = ZorgQuery()
+    compiler = ZorgQueryCompiler(zorg_query)
+    walker = antlr4.ParseTreeWalker()
+    walker.walk(compiler, tree)
+    return zorg_query
```

### Comparing `zettel_org-0.6.4/src/zorg/service/compiler/_file_compiler.py` & `zettel_org-0.7.0/src/zorg/service/compiler/_file_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import antlr4
 from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
 from typist import assert_never
 
 from ...domain.models import TodoPayload, ZorgFile, ZorgNote
-from ...domain.types import TodoPriorityType, TodoStatus, TodoStatusPrefixChar
+from ...domain.types import NoteStatus, TodoPriorityType, TodoStatusPrefixChar
 from ...grammar.zorg_file.ZorgFileListener import ZorgFileListener
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
 
 _LOGGER = Logger(__name__)
@@ -191,37 +191,38 @@
         self._s.in_note = True
         self._s.parent_id = None
         del ctx
 
     def enterTodo_prefix(
         self, ctx: ZorgFileParser.Todo_prefixContext
     ) -> None:  # noqa: D102
-        status = TodoStatus.OPEN
+        status = NoteStatus.OPEN_TODO
         if self._s.in_note:
             ch: TodoStatusPrefixChar = ctx.getText()[0]
             if ch == "o":
-                status = TodoStatus.OPEN
+                status = NoteStatus.OPEN_TODO
             elif ch == "x":
-                status = TodoStatus.CLOSED
+                status = NoteStatus.CLOSED_TODO
             elif ch == "~":
-                status = TodoStatus.CANCELED
+                status = NoteStatus.CANCELED_TODO
             elif ch == "<":
-                status = TodoStatus.BLOCKED
+                status = NoteStatus.BLOCKED_TODO
             elif ch == ">":
-                status = TodoStatus.PARENT
+                status = NoteStatus.PARENT_TODO
             else:
                 assert_never(ch)
 
             self._s.todo_status = status
 
     def enterZid(self, ctx: ZorgFileParser.ZidContext) -> None:  # noqa: D102
-        zid = ctx.getText()
-        self._s.zid = zid
-        zorg_id_date = f"20{zid.split('#')[0]}"
-        self._s.note_date = dt.datetime.strptime(zorg_id_date, "%Y%m%d")
+        if self._s.in_note and self._s.ids_in_note == 0:
+            zid = ctx.getText()
+            self._s.zid = zid
+            zorg_id_date = f"20{zid.split('#')[0]}"
+            self._s.note_date = dt.datetime.strptime(zorg_id_date, "%Y%m%d")
 
     def exitBase_todo(
         self, ctx: ZorgFileParser.Base_todoContext
     ) -> None:  # noqa: D102
         self._s.in_note = False
         kwargs = self._get_note_kwargs(
             ctx,
@@ -244,15 +245,15 @@
             self.zorg_file.has_errors = True
         else:
             todo = ZorgNote(id_note_body.getText(), **kwargs)
             self.zorg_file.notes.append(todo)
 
         # Reset todo priority and status back to defaults.
         self._s.todo_priority = "C"
-        self._s.todo_status = TodoStatus.OPEN
+        self._s.todo_status = NoteStatus.OPEN_TODO
 
     def exitH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = False
 
@@ -470,15 +471,15 @@
     h1_date: Optional[dt.date] = None
     h2_date: Optional[dt.date] = None
     h3_date: Optional[dt.date] = None
     h4_date: Optional[dt.date] = None
     note_date: Optional[dt.date] = None
 
     todo_priority: TodoPriorityType = "C"
-    todo_status: TodoStatus = TodoStatus.OPEN
+    todo_status: NoteStatus = NoteStatus.OPEN_TODO
 
     @property
     def areas(self) -> list[str]:
         """Area tags that are currently in-scope."""
         return self._get_current_tags("areas")
 
     @property
```

### Comparing `zettel_org-0.6.4/src/zorg/service/file_groups.py` & `zettel_org-0.7.0/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/service/handlers.py` & `zettel_org-0.7.0/src/zorg/service/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Zorg's event and command handlers live here."""
 
+from functools import partial
 import hashlib
 import json
 from pathlib import Path
 import sys
 from typing import Iterable, Iterator
 
 from logrus import Logger
@@ -30,50 +31,65 @@
     session.add_message(events.EditorClosedEvent(edit_cmd=cmd))
 
 
 def check_keep_alive_file(
     event: events.EditorClosedEvent, session: SQLSession
 ) -> None:
     """Check if the 'keep alive' file exists and, if so, reopens the editor."""
-    if not event.edit_cmd.keep_alive_file.exists():
+    keep_alive_file = event.edit_cmd.keep_alive_file
+    if not keep_alive_file.exists():
         logger.debug(
             "No keep alive file found.",
-            keep_alive_file=event.edit_cmd.keep_alive_file,
+            keep_alive_file=keep_alive_file,
         )
         return
 
-    if event.edit_cmd.keep_alive_file.stat().st_size == 0:
+    zdir = event.edit_cmd.zettel_dir
+    prepend_zdir = partial(common.prepend_zdir, zdir)
+    vim_commands = list(event.edit_cmd.vim_commands)
+    if keep_alive_file.stat().st_size == 0:
         logger.debug(
             "Empty keep alive file found.",
-            keep_alive_file=event.edit_cmd.keep_alive_file,
+            keep_alive_file=keep_alive_file,
         )
         paths = event.edit_cmd.paths
     else:
-        new_paths = common.prepend_zdir(
-            event.edit_cmd.zettel_dir,
-            [
-                Path(p.strip())
-                for p in event.edit_cmd.keep_alive_file.read_text().split()
-            ],
-        )
+        keep_alive_lines = list(keep_alive_file.read_text().split())
+        focused_filename = keep_alive_lines.pop()
+        vim_commands = [
+            cmd for cmd in vim_commands if not cmd.startswith("edit")
+        ]
+        vim_commands.append(f"edit {focused_filename}")
+        new_paths = prepend_zdir([Path(p.strip()) for p in keep_alive_lines])
         logger.debug(
             "Editing files specified in the keep alive file.",
-            keep_alive_file=event.edit_cmd.keep_alive_file,
+            keep_alive_file=keep_alive_file,
             old_paths=event.edit_cmd.paths,
             new_paths=new_paths,
         )
         paths = new_paths
 
-    event.edit_cmd.keep_alive_file.unlink()
+    verbose = event.edit_cmd.verbose
+    if verbose <= 1:
+        logger.debug(
+            "Unlinking keep-alive file", keep_alive_file=keep_alive_file
+        )
+        keep_alive_file.unlink()
+    else:
+        logger.debug(
+            "We are NOT deleting the keep-alive file",
+            keep_alive_file=keep_alive_file,
+        )
     session.add_last_message(
         commands.EditCommand(
-            zettel_dir=event.edit_cmd.zettel_dir,
+            zettel_dir=zdir,
             paths=paths,
-            keep_alive_file=event.edit_cmd.keep_alive_file,
-            vim_commands=event.edit_cmd.vim_commands,
+            keep_alive_file=keep_alive_file,
+            verbose=verbose,
+            vim_commands=vim_commands,
         )
     )
 
 
 def create_database(
     cmd: commands.CreateDBCommand, session: SQLSession
 ) -> None:
```

### Comparing `zettel_org-0.6.4/src/zorg/service/messagebus.py` & `zettel_org-0.7.0/src/zorg/service/messagebus.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/service/templates.py` & `zettel_org-0.7.0/src/zorg/service/templates.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/service/zid_manager.py` & `zettel_org-0.7.0/src/zorg/service/zid_manager.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/storage/sql/converters.py` & `zettel_org-0.7.0/src/zorg/storage/sql/converters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,75 @@
 """Contains logic to convert domain models to/from SQL models."""
 
 from collections import defaultdict
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Any
+from typing import Any, Callable, Optional
 
-from sqlmodel import Session, select
+import metaman
+from sqlmodel import Session, or_, select
+from sqlmodel.sql.expression import ColumnElement, SelectOfScalar
 
 from . import models as sql
-from ...domain.models import ZorgFile, ZorgNote
-from ...domain.types import EntityConverter
+from ...domain.models import WhereAndFilter, WhereOrFilter, ZorgFile, ZorgNote
+from ...domain.types import EntityConverter, NoteStatus
 from ...service import common
 
 
+_SONConverterParser = Callable[["_SONConverter"], ColumnElement]
+# the @_son_converter_parser decorator should be used to mark a _SONConverter
+# parser method
+_SON_CONVERTER_PARSERS: list[_SONConverterParser] = []
+_son_converter_parser = metaman.register_function_factory(
+    _SON_CONVERTER_PARSERS
+)
+
+
+def to_select_of_note(
+    or_filter: Optional[WhereOrFilter],
+) -> SelectOfScalar[sql.ZorgNote]:
+    """Converts a WhereOrFilter to a SQL SELECT that will fetch ZorgNotes."""
+    if or_filter is None or not or_filter.and_filters:
+        return select(sql.ZorgNote)
+
+    return select(sql.ZorgNote).where(
+        or_(*[
+            _SONConverter(and_filter).to_note_clause()
+            for and_filter in or_filter.and_filters
+        ])
+    )
+
+
+@dataclass(frozen=True)
+class _SONConverter:
+    """Converts a WhereAndFilter to a ColumnElement."""
+
+    and_filter: WhereAndFilter
+
+    def to_note_clause(self) -> ColumnElement:
+        """Constructs a SQL statement from the provided WhereAndFilter."""
+        where = or_(*[parse(self) for parse in _SON_CONVERTER_PARSERS])
+        return where
+
+    @_son_converter_parser
+    def note_status(self) -> ColumnElement:
+        """Converter for done status (e.g. '-' or 'ox~<>')."""
+        return or_(*[
+            sql.ZorgNote.todo_status == _to_todo_status(note_status)
+            for note_status in self.and_filter.allowed_note_statuses
+        ])
+
+
+def _to_todo_status(note_status: NoteStatus) -> Optional[NoteStatus]:
+    if note_status is NoteStatus.BASIC:
+        return None
+    else:
+        return note_status
+
+
 class ZorgFileConverter(EntityConverter[ZorgFile, sql.ZorgFile]):
     """Converts ZorgFile domain entities to/from ZorgFile sqlmodels."""
 
     def __init__(self, zdir: Path, session: Session) -> None:
         self._zdir = zdir
         self._note_converter = ZorgNoteConverter(session)
         self._all_sql_notes: list[sql.ZorgNote] = []
```

### Comparing `zettel_org-0.6.4/src/zorg/storage/sql/engine.py` & `zettel_org-0.7.0/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/src/zorg/storage/sql/models.py` & `zettel_org-0.7.0/src/zorg/storage/sql/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # WARNING: Don't bother importing __future__.annotations in this module!
 import datetime as dt
 from typing import List, Optional
 
 from sqlmodel import Field, Relationship, SQLModel, String
 from sqlmodel.sql.expression import Select, SelectOfScalar
 
-from ...domain.types import TodoStatus
+from ...domain.types import NoteStatus
 
 
 # HACK: see https://github.com/tiangolo/sqlmodel/issues/189
 Select.inherit_cache = True
 SelectOfScalar.inherit_cache = True
 
 
@@ -118,15 +118,15 @@
 
     # TODO(bugyi): Make zid required to persist to DB.
     # TODO(bugyi): Make zid unique.
     zid: Optional[str] = Field(default=None)
 
     create_date: dt.date = Field(default_factory=dt.date.today)
     todo_priority: Optional[str] = None
-    todo_status: Optional[TodoStatus] = None
+    todo_status: Optional[NoteStatus] = None
 
     # relationships
     zorg_file: ZorgFile = Relationship(
         back_populates="notes", link_model=ZorgFileLink
     )
     contexts: List["Context"] = Relationship(
         back_populates="notes", link_model=ContextLink
```

### Comparing `zettel_org-0.6.4/src/zorg/storage/sql/repo.py` & `zettel_org-0.7.0/src/zorg/storage/sql/repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """Contains the Repo class."""
 
+# pylint: disable=unsubscriptable-object
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Optional
 
 from eris import ErisResult, Err, Ok
 from logrus import Logger
-from potoroo import QueryRepo
 from sqlmodel import Session, select
 
 from . import models as sql
 from ...domain.messages.events import NewZorgNotesEvent
-from ...domain.models import ZorgFile, ZorgQuery
+from ...domain.models import WhereOrFilter, ZorgFile, ZorgNote
 from ...service.zid_manager import ZIDManager
-from .converters import ZorgFileConverter
+from .converters import ZorgFileConverter, ZorgNoteConverter, to_select_of_note
 
 
 logger = Logger(__name__)
 
 
-class SQLRepo(QueryRepo[str, ZorgFile, ZorgQuery]):
+class SQLRepo:
     """Repo that stores zorg notes in sqlite database."""
 
     def __init__(
         self,
         zettel_dir: Path,
         session: Session,
     ) -> None:
         self._zettel_dir = zettel_dir
         self._session = session
         self._converter = ZorgFileConverter(zettel_dir, session)
+        self._note_converter = ZorgNoteConverter(session)
 
         self.seen: list[ZorgFile] = []
 
     def add(
         self, zorg_file: ZorgFile, /, *, key: str = None
     ) -> ErisResult[str]:
         """Adds a new file to the DB.
@@ -106,20 +108,22 @@
         if sql_zorg_file:
             zorg_file = self._converter.to_entity(sql_zorg_file)
             self._seen_zorg_file(zorg_file)
             return Ok(zorg_file)
         else:
             return Ok(None)
 
-    def get_by_query(self, query: ZorgQuery) -> ErisResult[list[ZorgFile]]:
+    def get_by_query(
+        self, query: Optional[WhereOrFilter]
+    ) -> ErisResult[list[ZorgNote]]:
         """Get file(s) from DB by using a query."""
-        del query
-        result: list[ZorgFile] = []
-        for zorg_file in result:
-            self._seen_zorg_file(zorg_file)
+        select_of_note = to_select_of_note(query)
+        result: list[ZorgNote] = []
+        for sql_note in self._session.exec(select_of_note):
+            result.append(self._note_converter.to_entity(sql_note))
         return Ok(result)
 
     def all(self) -> ErisResult[list[ZorgFile]]:
         """Returns all zorg notes contained in the underlying SQL database."""
         stmt = select(sql.ZorgFile)
         result: list[ZorgFile] = []
         for sql_zorg_file in self._session.exec(stmt).all():
```

### Comparing `zettel_org-0.6.4/src/zorg/storage/sql/session.py` & `zettel_org-0.7.0/src/zorg/storage/sql/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 
 from functools import partial
 from pathlib import Path
 from types import TracebackType
 from typing import Iterator, Type
 
 from logrus import Logger
-from potoroo import UnitOfWork
 from sqlmodel import Session
 
 from ...domain.messages import Message
 from ...domain.types import CreateEngineType
 from .engine import create_cached_engine
 from .repo import SQLRepo
 
 
 logger = Logger(__name__)
 
 
-class SQLSession(UnitOfWork[SQLRepo]):
+class SQLSession:
     """Unit-of-work pattern used to manage transactions on zorg's SQL DB.
 
     TODO: Document __init__() params here.
     """
 
     def __init__(
         self,
```

### Comparing `zettel_org-0.6.4/targets.mk` & `zettel_org-0.7.0/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/__snapshots__/test_run_compile.ambr` & `zettel_org-0.7.0/tests/__snapshots__/test_run_compile.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-links]
   '''
   {'notes': [{'areas': [],
@@ -343,14 +344,28 @@
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
               'todo_payload': None,
+              'zid': None},
+             {'areas': [],
+              'body': 'Some note that references an old 200101#12 ZID.',
+              'child_note_ids': [],
+              'contexts': [],
+              'create_date': FakeDate(2000, 1, 3),
+              'links': [],
+              'next_note_id': None,
+              'parent_note_id': None,
+              'people': [],
+              'prev_note_id': None,
+              'projects': [],
+              'properties': {},
+              'todo_payload': None,
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-multiblocks]
   '''
   {'notes': [{'areas': [],
@@ -361,29 +376,31 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' Another related todo',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'A note about life...',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -403,15 +420,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'With a note',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -534,43 +552,46 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'A', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'A',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Medium Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'B', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'B',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': ' 2024-03-13 Low Priority TODO',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDatetime(2024, 3, 13, 0, 0),
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-property]
   '''
   {'notes': [{'areas': [],
@@ -595,15 +616,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {'due': '2024-03-13', 'p': '1'},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None}]}
   
   '''
 # ---
 # name: test_compile[YAMLConfigFile-scrambled_prj_notes]
   '''
   {'notes': [{'areas': [],
@@ -1557,15 +1579,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {'due': '2024-03-30', 'p': '1'},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'Todo subnote A',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1744,15 +1767,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'A note on the second section.',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1800,15 +1824,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'This is inside of h4_section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
@@ -1870,15 +1895,16 @@
               'links': [],
               'next_note_id': None,
               'parent_note_id': None,
               'people': [],
               'prev_note_id': None,
               'projects': [],
               'properties': {},
-              'todo_payload': {'priority': 'C', 'status': <TodoStatus.OPEN: 1>},
+              'todo_payload': {'priority': 'C',
+                               'status': <NoteStatus.OPEN_TODO: 2>},
               'zid': None},
              {'areas': [],
               'body': 'This is the final section!',
               'child_note_ids': [],
               'contexts': [],
               'create_date': FakeDate(2000, 1, 3),
               'links': [],
```

### Comparing `zettel_org-0.6.4/tests/__snapshots__/test_run_db.ambr` & `zettel_org-0.7.0/tests/__snapshots__/test_run_db.ambr`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     '2030-12-31',
   ])
 # ---
 # name: test_run_db_create__file_count[YAMLConfigFile]
   10
 # ---
 # name: test_run_db_create__note_count[YAMLConfigFile]
-  134
+  135
 # ---
 # name: test_run_db_create__people[YAMLConfigFile]
   list([
     'clyzajrm',
     'pig',
   ])
 # ---
@@ -102,15 +102,15 @@
     'A',
     'B',
     'C',
   ])
 # ---
 # name: test_run_db_create__todo_statuses[YAMLConfigFile]
   list([
-    'OPEN',
+    'OPEN_TODO',
   ])
 # ---
 # name: test_run_db_create__zids[YAMLConfigFile]
   list([
     '000103#00',
     '000103#01',
     '000103#02',
@@ -216,14 +216,15 @@
     '000103#20',
     '000103#21',
     '000103#22',
     '000103#23',
     '000103#24',
     '000103#25',
     '000103#26',
+    '000103#27',
     '240313#00',
     '240313#01',
     '240313#02',
     '240323#00',
     '240323#01',
     '240323#02',
     '240323#03',
```

### Comparing `zettel_org-0.6.4/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.7.0/tests/__snapshots__/test_run_edit.ambr`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   # 2000-01-03.Mon
   #
   # ^ = [[2000/20000103]]
   # < = [[2000/20000102_day]]
   # > = [[2000/20000104_day]]
   # @ = [[day_log.zot]]
   
-  o 000103#27 #gtd pomodoro
+  o 000103#28 #gtd pomodoro
     * Google Calendar (bbugyi@google + bryanbugyi34@gmail)
     * Process yesterday's bujo log (e.g. close events, add missing pomodoros, rollover goals)
     * Copy any important gchat convos from yesterday into chat/*.txt
     * Check today's tickler file: [[tick_03]]
     * Fill out yesterday's habit tracker: [[2000/20000102_habit]]
     * go/g3co
     * Review Google Keep Inbox
@@ -69,7 +69,22 @@
   # @ = [[done_log.zot]]
   #
   # 0 = [[2000/20000103_day]]
   
   
   '''
 # ---
+# name: test_whenKeepAliveFileContainsPaths_useThosePathsOnRestart[YAMLConfigFile]
+  list([
+    list([
+      'vim',
+      '<TMP>/org/foobar.zo',
+    ]),
+    list([
+      'vim',
+      '<TMP>/org/baz.zo',
+      '<TMP>/org/buz.zo',
+      '-c',
+      'edit buz.zo',
+    ]),
+  ])
+# ---
```

### Comparing `zettel_org-0.6.4/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.7.0/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/common.py` & `zettel_org-0.7.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/conftest.py` & `zettel_org-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/data/day_log.zot` & `zettel_org-0.7.0/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/data/done_log.zot` & `zettel_org-0.7.0/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/data/habit_log.zot` & `zettel_org-0.7.0/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_config.py` & `zettel_org-0.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_file_groups.py` & `zettel_org-0.7.0/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_run_action_open.py` & `zettel_org-0.7.0/tests/test_run_action_open.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_run_compile.py` & `zettel_org-0.7.0/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_run_db.py` & `zettel_org-0.7.0/tests/test_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.6.4/tests/test_run_edit.py` & `zettel_org-0.7.0/tests/test_run_edit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests the zorg project's 'edit' CLI command."""
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
-from unittest.mock import Mock, call
+from unittest.mock import Mock
 
 from syrupy.assertion import SnapshotAssertion as Snapshot
 
 from . import common as c
 
 
 def test_edit_day_logs(
@@ -86,45 +86,30 @@
         timeout=None,
     )
     assert vim_proc_mock.call_count == 2
     assert not keep_alive_file.exists()
 
 
 def test_whenKeepAliveFileContainsPaths_useThosePathsOnRestart(
-    main: c.MainType, vim_proc_mock: Mock, tmp_path: Path
+    main: c.MainType, vim_proc_mock: Mock, tmp_path: Path, snapshot: Snapshot
 ) -> None:
     """Test that we can use the keep alive file to change our vim file args."""
     zettel_dir = tmp_path / "org"
 
     keep_alive_file = tmp_path / "zorg_keep_alive"
-    keep_alive_file.write_text("baz.zo buz.zo")
+    keep_alive_file.write_text("baz.zo buz.zo buz.zo")
     exit_code = main(
         "--dir",
         str(zettel_dir),
         "edit",
         "foobar.zo",
         keep_alive_file=keep_alive_file,
     )
 
     assert exit_code == 0
-    vim_proc_mock.assert_has_calls([
-        call(
-            ["vim", str(zettel_dir / "foobar.zo")],
-            stdout=None,
-            stderr=None,
-            timeout=None,
-        ),
-        call().unwrap(),
-        call(
-            [
-                "vim",
-                str(zettel_dir / "baz.zo"),
-                str(zettel_dir / "buz.zo"),
-            ],
-            stdout=None,
-            stderr=None,
-            timeout=None,
-        ),
-        call().unwrap(),
-    ])
+    assert [
+        [cmd_part.replace(str(tmp_path), "<TMP>") for cmd_part in call.args[0]]
+        for call in vim_proc_mock.mock_calls
+        if call.args
+    ] == snapshot
     assert vim_proc_mock.call_count == 2
     assert not keep_alive_file.exists()
```

### Comparing `zettel_org-0.6.4/tests/test_run_template.py` & `zettel_org-0.7.0/tests/test_run_template.py`

 * *Files identical despite different names*

