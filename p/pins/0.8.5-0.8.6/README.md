# Comparing `tmp/pins-0.8.5.tar.gz` & `tmp/pins-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pins-0.8.5.tar", last modified: Tue Apr 16 23:17:09 2024, max compression
+gzip compressed data, was "pins-0.8.6.tar", last modified: Fri May  3 20:53:50 2024, max compression
```

## Comparing `pins-0.8.5.tar` & `pins-0.8.6.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.413551 pins-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-16 23:17:04.000000 pins-0.8.5/.env.dev
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-16 23:17:04.000000 pins-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 23:17:04.000000 pins-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-16 23:17:04.000000 pins-0.8.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 23:17:04.000000 pins-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-16 23:17:04.000000 pins-0.8.5/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 23:17:04.000000 pins-0.8.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-16 23:17:09.413551 pins-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 23:17:04.000000 pins-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 23:17:04.000000 pins-0.8.5/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/binder/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 23:17:04.000000 pins-0.8.5/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-16 23:17:04.000000 pins-0.8.5/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 23:17:04.000000 pins-0.8.5/binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 23:17:04.000000 pins-0.8.5/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-16 23:17:04.000000 pins-0.8.5/pins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 23:17:04.000000 pins-0.8.5/pins/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-04-16 23:17:04.000000 pins-0.8.5/pins/boards.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-16 23:17:04.000000 pins-0.8.5/pins/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-16 23:17:04.000000 pins-0.8.5/pins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-04-16 23:17:04.000000 pins-0.8.5/pins/constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/data/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-16 23:17:04.000000 pins-0.8.5/pins/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-16 23:17:04.000000 pins-0.8.5/pins/data/mtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-16 23:17:04.000000 pins-0.8.5/pins/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 23:17:04.000000 pins-0.8.5/pins/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-16 23:17:04.000000 pins-0.8.5/pins/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.397551 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-04-16 23:17:04.000000 pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/_snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
--rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.401551 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
--rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/example-bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/data_frame.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/example-bundle/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/_pins.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pin-board/x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pin-board/y/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.389551 pins-0.8.5/pins/tests/pins-compat/df_arrow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_rds/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-compat/df_unversioned/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-old-types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.393551 pins-0.8.5/pins/tests/pins-old-types/a-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/pins/tests/pins-old-types/a-table/v/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.csv
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.rds
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/pins-old-types/a-table/v/data.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21746 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_boards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_compat_old_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_rsconnect_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-16 23:17:04.000000 pins-0.8.5/pins/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-16 23:17:04.000000 pins-0.8.5/pins/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-16 23:17:04.000000 pins-0.8.5/pins/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/pins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 23:17:09.000000 pins-0.8.5/pins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 23:17:04.000000 pins-0.8.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.405551 pins-0.8.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-16 23:17:04.000000 pins-0.8.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 23:17:04.000000 pins-0.8.5/requirements/minimum.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/ci-compat-check/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/dump_py_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/dump_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/validate_py_to_r.R
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 23:17:04.000000 pins-0.8.5/script/ci-compat-check/validate_r_to_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 23:17:09.409551 pins-0.8.5/script/setup-rsconnect/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/add-users.sh
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/dump_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/rstudio-connect.gcfg
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 23:17:04.000000 pins-0.8.5/script/setup-rsconnect/users.txt
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_example_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_r_pins.R
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 23:17:04.000000 pins-0.8.5/script/stage_r_pins_old_types.R
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-16 23:17:09.413551 pins-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.779343 pins-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-03 20:53:46.000000 pins-0.8.6/.env.dev
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-03 20:53:46.000000 pins-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 20:53:46.000000 pins-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-03 20:53:46.000000 pins-0.8.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 20:53:46.000000 pins-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 20:53:46.000000 pins-0.8.6/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 20:53:46.000000 pins-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-03 20:53:46.000000 pins-0.8.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-03 20:53:50.779343 pins-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-03 20:53:46.000000 pins-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-03 20:53:46.000000 pins-0.8.6/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.759343 pins-0.8.6/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 20:53:46.000000 pins-0.8.6/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-03 20:53:46.000000 pins-0.8.6/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 20:53:46.000000 pins-0.8.6/binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-03 20:53:46.000000 pins-0.8.6/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.763343 pins-0.8.6/pins/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-03 20:53:46.000000 pins-0.8.6/pins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 20:53:46.000000 pins-0.8.6/pins/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-05-03 20:53:46.000000 pins-0.8.6/pins/boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-05-03 20:53:46.000000 pins-0.8.6/pins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-03 20:53:46.000000 pins-0.8.6/pins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-05-03 20:53:46.000000 pins-0.8.6/pins/constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.763343 pins-0.8.6/pins/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 20:53:46.000000 pins-0.8.6/pins/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-03 20:53:46.000000 pins-0.8.6/pins/data/mtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-03 20:53:46.000000 pins-0.8.6/pins/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 20:53:46.000000 pins-0.8.6/pins/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-05-03 20:53:46.000000 pins-0.8.6/pins/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.763343 pins-0.8.6/pins/rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.763343 pins-0.8.6/pins/rsconnect/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.763343 pins-0.8.6/pins/rsconnect/html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.767343 pins-0.8.6/pins/rsconnect/html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-05-03 20:53:46.000000 pins-0.8.6/pins/rsconnect/html/pagedtable-1.1/pagedtable.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.767343 pins-0.8.6/pins/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/_snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.767343 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/data.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.767343 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    31530 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css
+-rw-r--r--   0 runner    (1001) docker     (127)    34769 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/test_rsc_pin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/example-bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/example-bundle/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/example-bundle/data_frame.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/example-bundle/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/example-bundle/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pin-board/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/_pins.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pin-board/x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pin-board/x/20221215T180351Z-c3943/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/x/20221215T180351Z-c3943/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/x/20221215T180351Z-c3943/x.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pin-board/y/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pin-board/y/20221215T180357Z-9ae7a/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/y/20221215T180357Z-9ae7a/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/y/20221215T180357Z-9ae7a/y.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pin-board/y/20221215T180400Z-b81d5/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/y/20221215T180400Z-b81d5/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pin-board/y/20221215T180400Z-b81d5/y.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-compat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-compat/df_arrow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-compat/df_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163718Z-eceac/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_csv/20220214T163720Z-9bfad/df_csv.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-compat/df_rds/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.771344 pins-0.8.6/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_rds/20220214T163720Z-35b15/df_rds.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-compat/df_unversioned/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-compat/df_unversioned/20220214T163720Z-35b15/df_unversioned.rds
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-old-types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.755343 pins-0.8.6/pins/tests/pins-old-types/a-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/pins/tests/pins-old-types/a-table/v/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-old-types/a-table/v/data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-old-types/a-table/v/data.rds
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/pins-old-types/a-table/v/data.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21746 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_boards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_compat_old_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_rsconnect_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-03 20:53:46.000000 pins-0.8.6/pins/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-03 20:53:46.000000 pins-0.8.6/pins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-03 20:53:46.000000 pins-0.8.6/pins/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/pins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-03 20:53:50.000000 pins-0.8.6/pins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-03 20:53:50.000000 pins-0.8.6/pins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:53:50.000000 pins-0.8.6/pins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 20:53:50.000000 pins-0.8.6/pins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 20:53:50.000000 pins-0.8.6/pins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 20:53:46.000000 pins-0.8.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-03 20:53:46.000000 pins-0.8.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 20:53:46.000000 pins-0.8.6/requirements/minimum.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/script/ci-compat-check/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/dump_py_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/dump_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/validate_py_to_r.R
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 20:53:46.000000 pins-0.8.6/script/ci-compat-check/validate_r_to_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:53:50.775344 pins-0.8.6/script/setup-rsconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 20:53:46.000000 pins-0.8.6/script/setup-rsconnect/add-users.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-03 20:53:46.000000 pins-0.8.6/script/setup-rsconnect/dump_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 20:53:46.000000 pins-0.8.6/script/setup-rsconnect/rstudio-connect.gcfg
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 20:53:46.000000 pins-0.8.6/script/setup-rsconnect/users.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-03 20:53:46.000000 pins-0.8.6/script/stage_example_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-03 20:53:46.000000 pins-0.8.6/script/stage_r_pins.R
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 20:53:46.000000 pins-0.8.6/script/stage_r_pins_old_types.R
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-03 20:53:50.779343 pins-0.8.6/setup.cfg
```

### Comparing `pins-0.8.5/.env.dev` & `pins-0.8.6/.env.dev`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/.gitignore` & `pins-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/CONTRIBUTING.md` & `pins-0.8.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/LICENSE` & `pins-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/Makefile` & `pins-0.8.6/Makefile`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/PKG-INFO` & `pins-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.5
+Version: 0.8.6
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python
 Keywords: data,tidyverse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pins Version: 0.8.5 Summary: Publish data sets,
+Metadata-Version: 2.1 Name: pins Version: 0.8.6 Summary: Publish data sets,
 models, and other python objects, making it easy to share them across projects
 and with your colleagues. Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python Keywords:
 data,tidyverse Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

### Comparing `pins-0.8.5/README.md` & `pins-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/README.qmd` & `pins-0.8.6/README.qmd`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/binder/requirements.txt` & `pins-0.8.6/binder/requirements.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/boards.py` & `pins-0.8.6/pins/boards.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/cache.py` & `pins-0.8.6/pins/cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/config.py` & `pins-0.8.6/pins/config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/constructors.py` & `pins-0.8.6/pins/constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/data/mtcars.csv` & `pins-0.8.6/pins/data/mtcars.csv`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/drivers.py` & `pins-0.8.6/pins/drivers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/meta.py` & `pins-0.8.6/pins/meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/api.py` & `pins-0.8.6/pins/rsconnect/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import os
 import requests
 import tempfile
-import json
 
 from dataclasses import dataclass
 from pathlib import Path
 from functools import partial
 from io import IOBase
 from urllib.parse import urlencode
 
@@ -200,15 +199,15 @@
             data = r.json()
             self._validate_json_response(data)
 
             # this should never be triggered
             raise ValueError(
                 "Unknown json returned by delete_content endpoint: %s" % data
             )
-        except json.JSONDecodeError:
+        except requests.JSONDecodeError:
             # fallback to at least raising status errors
             r.raise_for_status()
 
     def query_v1(self, route, method="GET", return_request=False, **kwargs):
         endpoint = f"{self.base_v1_url}/{route}"
 
         return self._raw_query(endpoint, method, return_request, **kwargs)
@@ -233,15 +232,15 @@
             # the API can return http error codes AND codes in a json payload.
             # to handle this, we prefer the json error codes, but fallback to
             # checking for an HTTP error is no valid json was given.
             try:
                 data = r.json()
                 self._validate_json_response(data)
                 return data
-            except json.JSONDecodeError:
+            except requests.JSONDecodeError:
                 r.raise_for_status()
 
     def walk_paginated_offsets(self, f_query, endpoint, method, params=None, **kwargs):
         if params is None:
             params = {}
 
         all_results = []
```

### Comparing `pins-0.8.5/pins/rsconnect/fs.py` & `pins-0.8.6/pins/rsconnect/fs.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/highlight.js` & `pins-0.8.6/pins/rsconnect/html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.6/pins/rsconnect/html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/html/index.html` & `pins-0.8.6/pins/rsconnect/html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.css` & `pins-0.8.6/pins/rsconnect/html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/rsconnect/html/pagedtable-1.1/pagedtable.js` & `pins-0.8.6/pins/rsconnect/html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js` & `pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/highlight.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css` & `pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/highlight.js-9.15.9/qtcreator_light.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html` & `pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/index.html`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css` & `pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.css`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js` & `pins-0.8.6/pins/tests/_snapshots/test_board_pin_write_rsc_index_html/pagedtable-1.1/pagedtable.js`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/conftest.py` & `pins-0.8.6/pins/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/helpers.py` & `pins-0.8.6/pins/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow` & `pins-0.8.6/pins/tests/pins-compat/df_arrow/20220214T163720Z-ad0c1/df_arrow.arrow`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_boards.py` & `pins-0.8.6/pins/tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_cache.py` & `pins-0.8.6/pins/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_compat.py` & `pins-0.8.6/pins/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_config.py` & `pins-0.8.6/pins/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_constructors.py` & `pins-0.8.6/pins/tests/test_constructors.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_drivers.py` & `pins-0.8.6/pins/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_meta.py` & `pins-0.8.6/pins/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_rsconnect_api.py` & `pins-0.8.6/pins/tests/test_rsconnect_api.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/tests/test_versions.py` & `pins-0.8.6/pins/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/utils.py` & `pins-0.8.6/pins/utils.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins/versions.py` & `pins-0.8.6/pins/versions.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/pins.egg-info/PKG-INFO` & `pins-0.8.6/pins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pins
-Version: 0.8.5
+Version: 0.8.6
 Summary: Publish data sets, models, and other python objects, making it easy to share them across projects and with your colleagues.
 Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman
 Author-email: isabel.zimmerman@posit.co
 License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python
 Keywords: data,tidyverse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pins Version: 0.8.5 Summary: Publish data sets,
+Metadata-Version: 2.1 Name: pins Version: 0.8.6 Summary: Publish data sets,
 models, and other python objects, making it easy to share them across projects
 and with your colleagues. Home-page: https://github.com/rstudio/pins-python
 Author: Isabel Zimmerman Author-email: isabel.zimmerman@posit.co License: MIT
 Project-URL: Documentation, https://rstudio.github.io/pins-python Keywords:
 data,tidyverse Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

### Comparing `pins-0.8.5/pins.egg-info/SOURCES.txt` & `pins-0.8.6/pins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/requirements/dev.txt` & `pins-0.8.6/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/script/stage_example_bundle.py` & `pins-0.8.6/script/stage_example_bundle.py`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/script/stage_r_pins.R` & `pins-0.8.6/script/stage_r_pins.R`

 * *Files identical despite different names*

### Comparing `pins-0.8.5/setup.cfg` & `pins-0.8.6/setup.cfg`

 * *Files identical despite different names*

