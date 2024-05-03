# Comparing `tmp/troi-29.0.tar.gz` & `tmp/troi-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troi-29.0.tar", last modified: Mon Apr 29 12:03:53 2024, max compression
+gzip compressed data, was "troi-3.0.tar", last modified: Fri May  3 11:21:41 2024, max compression
```

## Comparing `troi-29.0.tar` & `troi-3.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.787052 troi-29.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.759052 troi-29.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.763052 troi-29.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-29 12:03:22.000000 troi-29.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-29 12:03:22.000000 troi-29.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 12:03:22.000000 troi-29.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-29 12:03:22.000000 troi-29.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-29 12:03:22.000000 troi-29.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-29 12:03:53.787052 troi-29.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-29 12:03:22.000000 troi-29.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 12:03:22.000000 troi-29.0/config.py.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.763052 troi-29.0/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-29 12:03:22.000000 troi-29.0/docker/endless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 12:03:22.000000 troi-29.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-29 12:03:22.000000 troi-29.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-29 12:03:22.000000 troi-29.0/docs/dev/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/docs/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/listenbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-29 12:03:22.000000 troi-29.0/docs/elements/musicbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-29 12:03:22.000000 troi-29.0/docs/entities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-29 12:03:22.000000 troi-29.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 12:03:22.000000 troi-29.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-29 12:03:22.000000 troi-29.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-29 12:03:22.000000 troi-29.0/docs/lb_radio.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-04-29 12:03:22.000000 troi-29.0/docs/listenbrainz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 12:03:22.000000 troi-29.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-29 12:03:22.000000 troi-29.0/docs/patches.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 12:03:22.000000 troi-29.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-29 12:03:22.000000 troi-29.0/docs/troi-arguments.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-29 12:03:22.000000 troi-29.0/docs/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-29 12:03:22.000000 troi-29.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:03:53.787052 troi-29.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.767052 troi-29.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-29 12:03:22.000000 troi-29.0/tests/listenbrainz/test_recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-29 12:03:22.000000 troi-29.0/tests/listenbrainz/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-29 12:03:22.000000 troi-29.0/tests/musicbrainz/test_related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-29 12:03:22.000000 troi-29.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-29 12:03:22.000000 troi-29.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-04-29 12:03:22.000000 troi-29.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-29 12:03:22.000000 troi-29.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-29 12:03:22.000000 troi-29.0/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 12:03:22.000000 troi-29.0/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-29 12:03:22.000000 troi-29.0/tests/test_sorts.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-29 12:03:22.000000 troi-29.0/tests/test_tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 12:03:22.000000 troi-29.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 12:03:22.000000 troi-29.0/tests/tools/test_area_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.771052 troi-29.0/troi/
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-29 12:03:22.000000 troi-29.0/troi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-04-29 12:03:22.000000 troi-29.0/troi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.775052 troi-29.0/troi/content_resolver/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4411 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/artist_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9460 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/content_resolver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/database.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3647 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/duplicates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.775052 troi-29.0/troi/content_resolver/formats/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/flac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/m4a.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/mp3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/ogg_opus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      903 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/ogg_vorbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/tag_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/formats/wma.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/fuzzy_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2677 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/lb_radio.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/metadata_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/content_resolver/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/model/unresolved_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/py_sonic_fix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10148 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/subsonic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/tag_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/top_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/unresolved_recording.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-29 12:03:22.000000 troi-29.0/troi/content_resolver/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-29 12:03:22.000000 troi-29.0/troi/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-29 12:03:22.000000 troi-29.0/troi/external/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-29 12:03:22.000000 troi-29.0/troi/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/listens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/listenbrainz/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/unused/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/unused/dataset_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 12:03:22.000000 troi-29.0/troi/listenbrainz/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/local/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-29 12:03:22.000000 troi-29.0/troi/local/periodic_jams_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-29 12:03:22.000000 troi-29.0/troi/local/recording_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 12:03:22.000000 troi-29.0/troi/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-29 12:03:22.000000 troi-29.0/troi/loops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.779052 troi-29.0/troi/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/mbid_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-29 12:03:22.000000 troi-29.0/troi/musicbrainz/related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-29 12:03:22.000000 troi-29.0/troi/operations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6070 2024-04-29 12:03:22.000000 troi-29.0/troi/parse_prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8787 2024-04-29 12:03:22.000000 troi-29.0/troi/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/ai_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10520 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/lb_radio_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/artist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/blend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/country.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1544 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/recs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2850 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/lb_radio_classes/tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6880 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/periodic_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3116 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/periodic_jams_local.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/playlist_from_listenbrainz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/playlist_from_mbids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3881 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/recs_to_playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/patches/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/unused/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-04-29 12:03:22.000000 troi-29.0/troi/patches/unused/area_random_recordings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20763 2024-04-29 12:03:22.000000 troi-29.0/troi/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2747 2024-04-29 12:03:22.000000 troi-29.0/troi/plist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-04-29 12:03:22.000000 troi-29.0/troi/print_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-29 12:03:22.000000 troi-29.0/troi/recording_search_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-29 12:03:22.000000 troi-29.0/troi/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 12:03:22.000000 troi-29.0/troi/sorts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/area_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-29 12:03:22.000000 troi-29.0/troi/tools/spotify_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2912 2024-04-29 12:03:22.000000 troi-29.0/troi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:03:53.783052 troi-29.0/troi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 12:03:53.000000 troi-29.0/troi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.925858 troi-3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.897858 troi-3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.901858 troi-3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 11:21:04.000000 troi-3.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-03 11:21:04.000000 troi-3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 11:21:04.000000 troi-3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-03 11:21:04.000000 troi-3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-03 11:21:04.000000 troi-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-03 11:21:41.921858 troi-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-03 11:21:04.000000 troi-3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-03 11:21:04.000000 troi-3.0/config.py.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.901858 troi-3.0/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-05-03 11:21:04.000000 troi-3.0/docker/endless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 11:21:04.000000 troi-3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-03 11:21:04.000000 troi-3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 11:21:04.000000 troi-3.0/docs/dev/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/docs/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-03 11:21:04.000000 troi-3.0/docs/elements/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-03 11:21:04.000000 troi-3.0/docs/elements/listenbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 11:21:04.000000 troi-3.0/docs/elements/musicbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-03 11:21:04.000000 troi-3.0/docs/entities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-03 11:21:04.000000 troi-3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 11:21:04.000000 troi-3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-03 11:21:04.000000 troi-3.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-05-03 11:21:04.000000 troi-3.0/docs/lb_radio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-05-03 11:21:04.000000 troi-3.0/docs/listenbrainz-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-03 11:21:04.000000 troi-3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-03 11:21:04.000000 troi-3.0/docs/patches.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 11:21:04.000000 troi-3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 11:21:04.000000 troi-3.0/docs/troi-arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-03 11:21:04.000000 troi-3.0/docs/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-03 11:21:04.000000 troi-3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:21:41.925858 troi-3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/tests/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-03 11:21:04.000000 troi-3.0/tests/listenbrainz/test_recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-03 11:21:04.000000 troi-3.0/tests/listenbrainz/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.905858 troi-3.0/tests/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-03 11:21:04.000000 troi-3.0/tests/musicbrainz/test_mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-05-03 11:21:04.000000 troi-3.0/tests/musicbrainz/test_recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-03 11:21:04.000000 troi-3.0/tests/musicbrainz/test_related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-03 11:21:04.000000 troi-3.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-03 11:21:04.000000 troi-3.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-05-03 11:21:04.000000 troi-3.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-03 11:21:04.000000 troi-3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-05-03 11:21:04.000000 troi-3.0/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-03 11:21:04.000000 troi-3.0/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-03 11:21:04.000000 troi-3.0/tests/test_sorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 11:21:04.000000 troi-3.0/tests/test_tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 11:21:04.000000 troi-3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.909858 troi-3.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-03 11:21:04.000000 troi-3.0/tests/tools/test_area_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.909858 troi-3.0/troi/
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-05-03 11:21:04.000000 troi-3.0/troi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-05-03 11:21:04.000000 troi-3.0/troi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.913859 troi-3.0/troi/content_resolver/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4411 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/artist_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9460 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/content_resolver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/database.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3647 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/duplicates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.913859 troi-3.0/troi/content_resolver/formats/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/flac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/m4a.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/mp3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/ogg_opus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      903 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/ogg_vorbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/tag_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/formats/wma.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/fuzzy_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2677 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/lb_radio.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6220 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/metadata_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/content_resolver/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/model/unresolved_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/py_sonic_fix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10148 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/subsonic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/tag_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/top_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/unresolved_recording.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-05-03 11:21:04.000000 troi-3.0/troi/content_resolver/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-05-03 11:21:04.000000 troi-3.0/troi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-03 11:21:04.000000 troi-3.0/troi/external/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-05-03 11:21:04.000000 troi-3.0/troi/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/listens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/listenbrainz/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/unused/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/unused/dataset_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-03 11:21:04.000000 troi-3.0/troi/listenbrainz/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/local/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-05-03 11:21:04.000000 troi-3.0/troi/local/periodic_jams_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-03 11:21:04.000000 troi-3.0/troi/local/recording_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 11:21:04.000000 troi-3.0/troi/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-03 11:21:04.000000 troi-3.0/troi/loops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/mbid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-03 11:21:04.000000 troi-3.0/troi/musicbrainz/related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-03 11:21:04.000000 troi-3.0/troi/operations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6070 2024-05-03 11:21:04.000000 troi-3.0/troi/parse_prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8787 2024-05-03 11:21:04.000000 troi-3.0/troi/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.917858 troi-3.0/troi/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/ai_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10520 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.921858 troi-3.0/troi/patches/lb_radio_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/artist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/blend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/country.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1544 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/recs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2850 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4139 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/lb_radio_classes/tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6880 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/periodic_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3116 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/periodic_jams_local.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/playlist_from_listenbrainz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1183 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/playlist_from_mbids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3881 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/recs_to_playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.921858 troi-3.0/troi/patches/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/unused/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-05-03 11:21:04.000000 troi-3.0/troi/patches/unused/area_random_recordings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20763 2024-05-03 11:21:04.000000 troi-3.0/troi/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2747 2024-05-03 11:21:04.000000 troi-3.0/troi/plist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-05-03 11:21:04.000000 troi-3.0/troi/print_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-03 11:21:04.000000 troi-3.0/troi/recording_search_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-03 11:21:04.000000 troi-3.0/troi/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-03 11:21:04.000000 troi-3.0/troi/sorts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.921858 troi-3.0/troi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:04.000000 troi-3.0/troi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-03 11:21:04.000000 troi-3.0/troi/tools/area_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-03 11:21:04.000000 troi-3.0/troi/tools/spotify_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2912 2024-05-03 11:21:04.000000 troi-3.0/troi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:21:41.921858 troi-3.0/troi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 11:21:41.000000 troi-3.0/troi.egg-info/top_level.txt
```

### Comparing `troi-29.0/.github/workflows/cd.yml` & `troi-3.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `troi-29.0/.github/workflows/ci.yml` & `troi-3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `troi-29.0/LICENSE` & `troi-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troi-29.0/PKG-INFO` & `troi-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 29.0
+Version: 3.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-29.0/README.md` & `troi-3.0/README.md`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/Makefile` & `troi-3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/conf.py` & `troi-3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/dev/index.rst` & `troi-3.0/docs/dev/index.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/elements/index.rst` & `troi-3.0/docs/elements/index.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/elements/listenbrainz.rst` & `troi-3.0/docs/elements/listenbrainz.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/elements/musicbrainz.rst` & `troi-3.0/docs/elements/musicbrainz.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/entities.rst` & `troi-3.0/docs/entities.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/index.rst` & `troi-3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/installation.rst` & `troi-3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/introduction.rst` & `troi-3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/lb_radio.rst` & `troi-3.0/docs/lb_radio.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/listenbrainz-logo.svg` & `troi-3.0/docs/listenbrainz-logo.svg`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/make.bat` & `troi-3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/patches.rst` & `troi-3.0/docs/patches.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/troi-arguments.rst` & `troi-3.0/docs/troi-arguments.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/docs/user-guide.rst` & `troi-3.0/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `troi-29.0/pyproject.toml` & `troi-3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/listenbrainz/test_recs.py` & `troi-3.0/tests/listenbrainz/test_recs.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/listenbrainz/test_stats.py` & `troi-3.0/tests/listenbrainz/test_stats.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/musicbrainz/test_mbid_mapping.py` & `troi-3.0/tests/musicbrainz/test_mbid_mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     @unittest.mock.patch('requests.post', side_effect=mocked_requests_post)
     def test_read(self, req):
 
         e = troi.musicbrainz.mbid_mapping.MBIDMappingLookupElement()
 
         r = [ troi.Recording("trigger hippie", artist_credit=troi.ArtistCredit(name="morcheeba")) ]
         entities = e.read([r])
-        req.assert_called_with(e.SERVER_URL, json=[{'[artist_credit_name]': 'morcheeba', '[recording_name]': 'trigger hippie'}])
+        req.assert_called_with(e.SERVER_URL, json=[{'artist_credit_name': 'morcheeba', 'recording_name': 'trigger hippie'}])
 
         assert len(entities) == 1
         assert entities[0].artist_credit.artist_credit_id == 963
         assert entities[0].artist_credit.name == "Morcheeba"
         assert entities[0].artist_credit.artists[0].mbid == "067102ea-9519-4622-9077-57ca4164cfbb"
         assert entities[0].release.mbid == "9db51cd6-38f6-3b42-8ad5-559963d68f35"
         assert entities[0].release.name == "Who Can You Trust?"
```

### Comparing `troi-29.0/tests/musicbrainz/test_recording_lookup.py` & `troi-3.0/tests/musicbrainz/test_recording_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/musicbrainz/test_related_artist_credits.py` & `troi-3.0/tests/musicbrainz/test_related_artist_credits.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_entities.py` & `troi-3.0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_filters.py` & `troi-3.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_operations.py` & `troi-3.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_parser.py` & `troi-3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_playlist.py` & `troi-3.0/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_plist.py` & `troi-3.0/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_sorts.py` & `troi-3.0/tests/test_sorts.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/test_tag_utils.py` & `troi-3.0/tests/test_tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/tests/tools/test_area_lookup.py` & `troi-3.0/tests/tools/test_area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/__init__.py` & `troi-3.0/troi/__init__.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/cli.py` & `troi-3.0/troi/cli.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/artist_search.py` & `troi-3.0/troi/content_resolver/artist_search.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/cli.py` & `troi-3.0/troi/content_resolver/cli.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/content_resolver.py` & `troi-3.0/troi/content_resolver/content_resolver.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/database.py` & `troi-3.0/troi/content_resolver/database.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/duplicates.py` & `troi-3.0/troi/content_resolver/duplicates.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/flac.py` & `troi-3.0/troi/content_resolver/formats/flac.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/m4a.py` & `troi-3.0/troi/content_resolver/formats/m4a.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/mp3.py` & `troi-3.0/troi/content_resolver/formats/mp3.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/ogg_opus.py` & `troi-3.0/troi/content_resolver/formats/ogg_opus.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/ogg_vorbis.py` & `troi-3.0/troi/content_resolver/formats/ogg_vorbis.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/tag_utils.py` & `troi-3.0/troi/content_resolver/formats/tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/formats/wma.py` & `troi-3.0/troi/content_resolver/formats/wma.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/fuzzy_index.py` & `troi-3.0/troi/content_resolver/fuzzy_index.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/lb_radio.py` & `troi-3.0/troi/content_resolver/lb_radio.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/metadata_lookup.py` & `troi-3.0/troi/content_resolver/metadata_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from collections import defaultdict, namedtuple
 import datetime
+from time import sleep
 
 import requests
 from tqdm import tqdm
 
 from troi.content_resolver.model.database import db
 from troi.content_resolver.model.recording import Recording, RecordingMetadata
 from troi.content_resolver.model.tag import RecordingTag
@@ -61,15 +62,15 @@
             popularity and tags into the DB for the given chunk of recordings.
         """
 
         args = []
         mbid_to_recording = {}
         for rec in recordings:
             mbid_to_recording[rec.mbid] = rec
-            args.append({"[recording_mbid]": rec.mbid})
+            args.append({"recording_mbid": rec.mbid})
 
         while True:
             r = requests.post("https://labs.api.listenbrainz.org/bulk-tag-lookup/json", json=args)
             if r.status_code == 429:
                 sleep(2)
                 continue
```

### Comparing `troi-29.0/troi/content_resolver/model/recording.py` & `troi-3.0/troi/content_resolver/model/recording.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/model/tag.py` & `troi-3.0/troi/content_resolver/model/tag.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/model/unresolved_recording.py` & `troi-3.0/troi/content_resolver/model/unresolved_recording.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/playlist.py` & `troi-3.0/troi/content_resolver/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/py_sonic_fix.py` & `troi-3.0/troi/content_resolver/py_sonic_fix.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/subsonic.py` & `troi-3.0/troi/content_resolver/subsonic.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/tag_search.py` & `troi-3.0/troi/content_resolver/tag_search.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/top_tags.py` & `troi-3.0/troi/content_resolver/top_tags.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/unresolved_recording.py` & `troi-3.0/troi/content_resolver/unresolved_recording.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/content_resolver/utils.py` & `troi-3.0/troi/content_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/core.py` & `troi-3.0/troi/core.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/external/gpt.py` & `troi-3.0/troi/external/gpt.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/filters.py` & `troi-3.0/troi/filters.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/feedback.py` & `troi-3.0/troi/listenbrainz/feedback.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/listens.py` & `troi-3.0/troi/listenbrainz/listens.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/recs.py` & `troi-3.0/troi/listenbrainz/recs.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/stats.py` & `troi-3.0/troi/listenbrainz/stats.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/unused/dataset_fetcher.py` & `troi-3.0/troi/listenbrainz/unused/dataset_fetcher.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/listenbrainz/user.py` & `troi-3.0/troi/listenbrainz/user.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/local/periodic_jams_local.py` & `troi-3.0/troi/local/periodic_jams_local.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/local/recording_resolver.py` & `troi-3.0/troi/local/recording_resolver.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/loops.py` & `troi-3.0/troi/loops.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/musicbrainz/mbid_mapping.py` & `troi-3.0/troi/musicbrainz/mbid_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return [Recording]
 
     def read(self, inputs):
 
         params = []
         for r in inputs[0]:
             if r.artist_credit is not None and r.name is not None:
-                params.append({"[artist_credit_name]": r.artist_credit.name, "[recording_name]": r.name})
+                params.append({"artist_credit_name": r.artist_credit.name, "recording_name": r.name})
 
         if not params:
             return []
 
         r = requests.post(self.SERVER_URL, json=params)
         if r.status_code != 200:
             raise PipelineError("Cannot fetch MBID mapping rows from ListenBrainz: HTTP code %d (%s)" % (r.status_code, r.text))
```

### Comparing `troi-29.0/troi/musicbrainz/mbid_reader.py` & `troi-3.0/troi/musicbrainz/mbid_reader.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/musicbrainz/recording.py` & `troi-3.0/troi/musicbrainz/recording.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/musicbrainz/recording_lookup.py` & `troi-3.0/troi/musicbrainz/recording_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/musicbrainz/related_artist_credits.py` & `troi-3.0/troi/musicbrainz/related_artist_credits.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/operations.py` & `troi-3.0/troi/operations.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/parse_prompt.py` & `troi-3.0/troi/parse_prompt.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patch.py` & `troi-3.0/troi/patch.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/ai_jams.py` & `troi-3.0/troi/patches/ai_jams.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio.py` & `troi-3.0/troi/patches/lb_radio.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/artist.py` & `troi-3.0/troi/patches/lb_radio_classes/artist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/blend.py` & `troi-3.0/troi/patches/lb_radio_classes/blend.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/collection.py` & `troi-3.0/troi/patches/lb_radio_classes/collection.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/country.py` & `troi-3.0/troi/patches/lb_radio_classes/country.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/playlist.py` & `troi-3.0/troi/patches/lb_radio_classes/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/recs.py` & `troi-3.0/troi/patches/lb_radio_classes/recs.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/stats.py` & `troi-3.0/troi/patches/lb_radio_classes/stats.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/lb_radio_classes/tag.py` & `troi-3.0/troi/patches/lb_radio_classes/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from time import sleep
+
 import troi
 from random import randint, shuffle
 
 import requests
 
 from troi import Recording
 from troi.plist import plist
@@ -31,15 +33,15 @@
 
     def fetch_similar_tags(self, tag):
         """
             Fetch similar tags from LB
         """
 
         while True:
-            r = requests.post( "https://labs.api.listenbrainz.org/tag-similarity/json", json=[{ "tag": tag }])
+            r = requests.post("https://labs.api.listenbrainz.org/tag-similarity/json", json=[{"tag": tag}])
             if r.status_code == 429:
                 sleep(2)
                 continue
 
             if r.status_code == 404:
                 return plist()
```

### Comparing `troi-29.0/troi/patches/periodic_jams.py` & `troi-3.0/troi/patches/periodic_jams.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/periodic_jams_local.py` & `troi-3.0/troi/patches/periodic_jams_local.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/playlist_from_listenbrainz.py` & `troi-3.0/troi/patches/playlist_from_listenbrainz.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/playlist_from_mbids.py` & `troi-3.0/troi/patches/playlist_from_mbids.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/recs_to_playlist.py` & `troi-3.0/troi/patches/recs_to_playlist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/patches/unused/area_random_recordings.py` & `troi-3.0/troi/patches/unused/area_random_recordings.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/playlist.py` & `troi-3.0/troi/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/plist.py` & `troi-3.0/troi/plist.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/print_recording.py` & `troi-3.0/troi/print_recording.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/recording_search_service.py` & `troi-3.0/troi/recording_search_service.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/service.py` & `troi-3.0/troi/service.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/sorts.py` & `troi-3.0/troi/sorts.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/tools/area_lookup.py` & `troi-3.0/troi/tools/area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/tools/spotify_lookup.py` & `troi-3.0/troi/tools/spotify_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi/utils.py` & `troi-3.0/troi/utils.py`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi.egg-info/PKG-INFO` & `troi-3.0/troi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 29.0
+Version: 3.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-29.0/troi.egg-info/SOURCES.txt` & `troi-3.0/troi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `troi-29.0/troi.egg-info/requires.txt` & `troi-3.0/troi.egg-info/requires.txt`

 * *Files identical despite different names*

