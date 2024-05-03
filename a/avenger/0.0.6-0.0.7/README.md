# Comparing `tmp/avenger-0.0.6.tar.gz` & `tmp/avenger-0.0.7.tar.gz`

## Comparing `avenger-0.0.6.tar` & `avenger-0.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0      501       20      533 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/Cargo.toml
--rw-r--r--   0      501       20      129 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/README.md
--rw-r--r--   0      501       20      735 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/error.rs
--rw-r--r--   0      501       20       51 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/lib.rs
--rw-r--r--   0      501       20     3689 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/arc.rs
--rw-r--r--   0      501       20     2414 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/area.rs
--rw-r--r--   0      501       20     4672 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/group.rs
--rw-r--r--   0      501       20     3031 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/image.rs
--rw-r--r--   0      501       20     1634 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/line.rs
--rw-r--r--   0      501       20     1329 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/mark.rs
--rw-r--r--   0      501       20      187 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/mod.rs
--rw-r--r--   0      501       20     2882 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/path.rs
--rw-r--r--   0      501       20     3831 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/rect.rs
--rw-r--r--   0      501       20     2873 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/rule.rs
--rw-r--r--   0      501       20    10808 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/symbol.rs
--rw-r--r--   0      501       20     5005 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/text.rs
--rw-r--r--   0      501       20     1551 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/trail.rs
--rw-r--r--   0      501       20     3215 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/marks/value.rs
--rw-r--r--   0      501       20      249 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/src/scene_graph.rs
--rw-r--r--   0      501       20       89 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/tests/test_scene_graph.rs
--rw-r--r--   0      501       20     1101 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/Cargo.toml
--rw-r--r--   0      501       20      109 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/README.md
--rw-r--r--   0      501       20     1490 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/error.rs
--rw-r--r--   0      501       20      757 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/image/mod.rs
--rw-r--r--   0      501       20     1504 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/image/reqwest_fetcher.rs
--rw-r--r--   0      501       20     1724 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/image/svg.rs
--rw-r--r--   0      501       20      131 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/lib.rs
--rw-r--r--   0      501       20     5495 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/arc.rs
--rw-r--r--   0      501       20     4361 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/area.rs
--rw-r--r--   0      501       20     6737 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/group.rs
--rw-r--r--   0      501       20     3759 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/image.rs
--rw-r--r--   0      501       20     3215 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/line.rs
--rw-r--r--   0      501       20     1522 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/mark.rs
--rw-r--r--   0      501       20      203 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/mod.rs
--rw-r--r--   0      501       20     5626 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/path.rs
--rw-r--r--   0      501       20     4307 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/rect.rs
--rw-r--r--   0      501       20     4382 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/rule.rs
--rw-r--r--   0      501       20     5019 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/shape.rs
--rw-r--r--   0      501       20     8093 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/symbol.rs
--rw-r--r--   0      501       20     6400 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/text.rs
--rw-r--r--   0      501       20     2795 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/trail.rs
--rw-r--r--   0      501       20     6163 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/marks/values.rs
--rw-r--r--   0      501       20      749 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/src/scene_graph.rs
--rw-r--r--   0      501       20      757 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-vega/tests/test_parsing.rs
--rw-r--r--   0      501       20     1485 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/Cargo.toml
--rw-r--r--   0      501       20       78 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/README.md
--rw-r--r--   0      501       20    28421 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/canvas.rs
--rw-r--r--   0      501       20     1800 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/error.rs
--rw-r--r--   0      501       20     6818 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/html_canvas.rs
--rw-r--r--   0      501       20      273 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/lib.rs
--rw-r--r--   0      501       20    11018 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/cosmic.rs
--rw-r--r--   0      501       20     6491 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/gradient.rs
--rw-r--r--   0      501       20     4996 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/image.rs
--rw-r--r--   0      501       20    12845 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/instanced_mark.rs
--rw-r--r--   0      501       20      151 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/mod.rs
--rw-r--r--   0      501       20    83346 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/multi.rs
--rw-r--r--   0      501       20     8946 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/multi.wgsl
--rw-r--r--   0      501       20     8759 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/symbol.rs
--rw-r--r--   0      501       20     3130 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/symbol.wgsl
--rw-r--r--   0      501       20    15441 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/marks/text.rs
--rw-r--r--   0      501       20     1329 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/src/util.rs
--rw-r--r--   0      501       20    10704 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-wgpu/tests/test_image_baselines.rs
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.6/avenger-python/Cargo.toml
--rw-r--r--   0      501       20     1453 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-python/LICENSE
--rw-r--r--   0      501       20     2375 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-python/README.md
--rw-r--r--   0      501       20      172 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-python/avenger/__init__.py
--rw-r--r--   0      501       20     3643 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-python/avenger/altair_utils.py
--rw-r--r--   0      501       20     2547 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger-python/src/lib.rs
--rw-r--r--   0      501       20   195804 2024-05-01 12:38:09.000000 avenger-0.0.6/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.6/Cargo.toml
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 avenger-0.0.6/pyproject.toml
--rw-r--r--   0      501       20      172 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/__init__.py
--rw-r--r--   0      501       20     3643 2024-05-01 12:38:09.000000 avenger-0.0.6/avenger/altair_utils.py
--rw-r--r--   0      501       20     2375 2024-05-01 12:38:09.000000 avenger-0.0.6/README.md
--rw-r--r--   0      501       20     1453 2024-05-01 12:38:09.000000 avenger-0.0.6/LICENSE
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.6/PKG-INFO
+-rw-r--r--   0      501       20     1510 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/Cargo.toml
+-rw-r--r--   0      501       20       78 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/README.md
+-rw-r--r--   0      501       20    28421 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/canvas.rs
+-rw-r--r--   0      501       20     1800 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/error.rs
+-rw-r--r--   0      501       20     6818 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/html_canvas.rs
+-rw-r--r--   0      501       20      273 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/lib.rs
+-rw-r--r--   0      501       20    11018 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/cosmic.rs
+-rw-r--r--   0      501       20     6491 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/gradient.rs
+-rw-r--r--   0      501       20     4996 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/image.rs
+-rw-r--r--   0      501       20    12845 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/instanced_mark.rs
+-rw-r--r--   0      501       20      151 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/mod.rs
+-rw-r--r--   0      501       20    83346 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/multi.rs
+-rw-r--r--   0      501       20     8946 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/multi.wgsl
+-rw-r--r--   0      501       20     8759 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/symbol.rs
+-rw-r--r--   0      501       20     3130 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/symbol.wgsl
+-rw-r--r--   0      501       20    15441 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/text.rs
+-rw-r--r--   0      501       20     1329 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/util.rs
+-rw-r--r--   0      501       20    10704 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/tests/test_image_baselines.rs
+-rw-r--r--   0      501       20      533 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/Cargo.toml
+-rw-r--r--   0      501       20      129 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/README.md
+-rw-r--r--   0      501       20      735 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/error.rs
+-rw-r--r--   0      501       20       51 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/lib.rs
+-rw-r--r--   0      501       20     3689 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/arc.rs
+-rw-r--r--   0      501       20     2414 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/area.rs
+-rw-r--r--   0      501       20     4672 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/group.rs
+-rw-r--r--   0      501       20     3031 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/image.rs
+-rw-r--r--   0      501       20     1634 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/line.rs
+-rw-r--r--   0      501       20     1329 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/mark.rs
+-rw-r--r--   0      501       20      187 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/mod.rs
+-rw-r--r--   0      501       20     2882 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/path.rs
+-rw-r--r--   0      501       20     3831 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/rect.rs
+-rw-r--r--   0      501       20     2873 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/rule.rs
+-rw-r--r--   0      501       20    10808 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/symbol.rs
+-rw-r--r--   0      501       20     5005 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/text.rs
+-rw-r--r--   0      501       20     1551 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/trail.rs
+-rw-r--r--   0      501       20     3215 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/value.rs
+-rw-r--r--   0      501       20      249 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/scene_graph.rs
+-rw-r--r--   0      501       20       89 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/tests/test_scene_graph.rs
+-rw-r--r--   0      501       20     1101 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/Cargo.toml
+-rw-r--r--   0      501       20      109 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/README.md
+-rw-r--r--   0      501       20     1490 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/error.rs
+-rw-r--r--   0      501       20      757 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/mod.rs
+-rw-r--r--   0      501       20     1504 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/reqwest_fetcher.rs
+-rw-r--r--   0      501       20     1724 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/svg.rs
+-rw-r--r--   0      501       20      131 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/lib.rs
+-rw-r--r--   0      501       20     5495 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/arc.rs
+-rw-r--r--   0      501       20     4361 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/area.rs
+-rw-r--r--   0      501       20     6737 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/group.rs
+-rw-r--r--   0      501       20     3759 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/image.rs
+-rw-r--r--   0      501       20     3215 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/line.rs
+-rw-r--r--   0      501       20     1522 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/mark.rs
+-rw-r--r--   0      501       20      203 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/mod.rs
+-rw-r--r--   0      501       20     5626 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/path.rs
+-rw-r--r--   0      501       20     4307 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/rect.rs
+-rw-r--r--   0      501       20     4382 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/rule.rs
+-rw-r--r--   0      501       20     5019 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/shape.rs
+-rw-r--r--   0      501       20     8093 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/symbol.rs
+-rw-r--r--   0      501       20     6400 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/text.rs
+-rw-r--r--   0      501       20     2795 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/trail.rs
+-rw-r--r--   0      501       20     6163 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/values.rs
+-rw-r--r--   0      501       20      749 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/scene_graph.rs
+-rw-r--r--   0      501       20      757 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/tests/test_parsing.rs
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.7/avenger-python/Cargo.toml
+-rw-r--r--   0      501       20     1453 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/LICENSE
+-rw-r--r--   0      501       20     2375 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/README.md
+-rw-r--r--   0      501       20      172 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/avenger/__init__.py
+-rw-r--r--   0      501       20     3643 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2547 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/src/lib.rs
+-rw-r--r--   0      501       20   195804 2024-05-03 19:02:42.000000 avenger-0.0.7/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.7/Cargo.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 avenger-0.0.7/pyproject.toml
+-rw-r--r--   0      501       20      172 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger/__init__.py
+-rw-r--r--   0      501       20     3643 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2375 2024-05-03 19:02:42.000000 avenger-0.0.7/README.md
+-rw-r--r--   0      501       20     1453 2024-05-03 19:02:42.000000 avenger-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.7/PKG-INFO
```

### Comparing `avenger-0.0.6/avenger/Cargo.toml` & `avenger-0.0.7/avenger/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 description = "A visualization engine and renderer"
 license = "BSD-3-Clause"
 
 [dependencies.thiserror]
 workspace = true
```

### Comparing `avenger-0.0.6/avenger/src/error.rs` & `avenger-0.0.7/avenger/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/arc.rs` & `avenger-0.0.7/avenger/src/marks/arc.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/area.rs` & `avenger-0.0.7/avenger/src/marks/area.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/group.rs` & `avenger-0.0.7/avenger/src/marks/group.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/image.rs` & `avenger-0.0.7/avenger/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/line.rs` & `avenger-0.0.7/avenger/src/marks/line.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/mark.rs` & `avenger-0.0.7/avenger/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/path.rs` & `avenger-0.0.7/avenger/src/marks/path.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/rect.rs` & `avenger-0.0.7/avenger/src/marks/rect.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/rule.rs` & `avenger-0.0.7/avenger/src/marks/rule.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/symbol.rs` & `avenger-0.0.7/avenger/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/text.rs` & `avenger-0.0.7/avenger/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/trail.rs` & `avenger-0.0.7/avenger/src/marks/trail.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger/src/marks/value.rs` & `avenger-0.0.7/avenger/src/marks/value.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/Cargo.toml` & `avenger-0.0.7/avenger-vega/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-vega"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 description = "Utilities for importing Vega scenegraphs into Avenger"
 license = "BSD-3-Clause"
 
 [features]
 image-request = [ "reqwest",]
 svg = [ "resvg", "usvg", "tiny-skia",]
@@ -29,15 +29,15 @@
 workspace = true
 
 [dependencies.tracing]
 workspace = true
 
 [dependencies.avenger]
 path = "../avenger"
-version = "0.0.6"
+version = "0.0.7"
 
 [dependencies.thiserror]
 workspace = true
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.6/avenger-vega/src/error.rs` & `avenger-0.0.7/avenger-vega/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/image/mod.rs` & `avenger-0.0.7/avenger-vega/src/image/mod.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/image/reqwest_fetcher.rs` & `avenger-0.0.7/avenger-vega/src/image/reqwest_fetcher.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/image/svg.rs` & `avenger-0.0.7/avenger-vega/src/image/svg.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/arc.rs` & `avenger-0.0.7/avenger-vega/src/marks/arc.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/area.rs` & `avenger-0.0.7/avenger-vega/src/marks/area.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/group.rs` & `avenger-0.0.7/avenger-vega/src/marks/group.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/image.rs` & `avenger-0.0.7/avenger-vega/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/line.rs` & `avenger-0.0.7/avenger-vega/src/marks/line.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/mark.rs` & `avenger-0.0.7/avenger-vega/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/path.rs` & `avenger-0.0.7/avenger-vega/src/marks/path.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/rect.rs` & `avenger-0.0.7/avenger-vega/src/marks/rect.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/rule.rs` & `avenger-0.0.7/avenger-vega/src/marks/rule.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/shape.rs` & `avenger-0.0.7/avenger-vega/src/marks/shape.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/symbol.rs` & `avenger-0.0.7/avenger-vega/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/text.rs` & `avenger-0.0.7/avenger-vega/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/trail.rs` & `avenger-0.0.7/avenger-vega/src/marks/trail.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/marks/values.rs` & `avenger-0.0.7/avenger-vega/src/marks/values.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/src/scene_graph.rs` & `avenger-0.0.7/avenger-vega/src/scene_graph.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-vega/tests/test_parsing.rs` & `avenger-0.0.7/avenger-vega/tests/test_parsing.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/Cargo.toml` & `avenger-0.0.7/avenger-wgpu/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-wgpu"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 description = "WGPU rendering engine for the Avenger visualization framework"
 license = "BSD-3-Clause"
 
 [lib]
 crate-type = [ "cdylib", "rlib",]
 
@@ -29,15 +29,15 @@
 
 [dev-dependencies]
 dssim = "3.2.4"
 rstest = "0.18.2"
 
 [dependencies.avenger]
 path = "../avenger"
-version = "0.0.6"
+version = "0.0.7"
 
 [dependencies.rayon]
 workspace = true
 optional = true
 
 [dependencies.tracing]
 workspace = true
@@ -63,18 +63,19 @@
 
 [dependencies.lyon]
 workspace = true
 
 [dev-dependencies.avenger-vega]
 path = "../avenger-vega"
 features = [ "image-request", "svg",]
-version = "0.0.6"
+version = "0.0.7"
 
 [dev-dependencies.serde_json]
 version = "1.0.111"
 
 [target."cfg(target_arch = \"wasm32\")".dependencies.wgpu]
 version = "0.19.3"
+default-features = false
 
 [target."cfg(target_arch = \"wasm32\")".dependencies.web-sys]
 version = "0.3.67"
 features = [ "Document", "Window", "Element", "HtmlCanvasElement",]
```

### Comparing `avenger-0.0.6/avenger-wgpu/src/canvas.rs` & `avenger-0.0.7/avenger-wgpu/src/canvas.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/error.rs` & `avenger-0.0.7/avenger-wgpu/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/html_canvas.rs` & `avenger-0.0.7/avenger-wgpu/src/html_canvas.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/cosmic.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/cosmic.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/gradient.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/gradient.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/image.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/instanced_mark.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/instanced_mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/multi.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/multi.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/multi.wgsl` & `avenger-0.0.7/avenger-wgpu/src/marks/multi.wgsl`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/symbol.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/symbol.wgsl` & `avenger-0.0.7/avenger-wgpu/src/marks/symbol.wgsl`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/marks/text.rs` & `avenger-0.0.7/avenger-wgpu/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/src/util.rs` & `avenger-0.0.7/avenger-wgpu/src/util.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-wgpu/tests/test_image_baselines.rs` & `avenger-0.0.7/avenger-wgpu/tests/test_image_baselines.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-python/Cargo.toml` & `avenger-0.0.7/avenger-python/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-python"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 license = "BSD-3-Clause"
 description = "Python API to Avenger visualization framework"
 publish = false
 
 [lib]
 name = "avenger"
@@ -13,25 +13,25 @@
 [dependencies]
 pythonize = "0.20.0"
 pollster = "0.3"
 
 [dependencies.avenger]
 path = "../avenger"
 features = [ "pyo3",]
-version = "0.0.6"
+version = "0.0.7"
 
 [dependencies.avenger-vega]
 path = "../avenger-vega"
 features = [ "pyo3",]
-version = "0.0.6"
+version = "0.0.7"
 
 [dependencies.avenger-wgpu]
 path = "../avenger-wgpu"
 features = [ "pyo3",]
-version = "0.0.6"
+version = "0.0.7"
 
 [dependencies.pyo3]
 workspace = true
 features = [ "extension-module", "abi3-py38",]
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.6/avenger-python/LICENSE` & `avenger-0.0.7/avenger-python/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-python/README.md` & `avenger-0.0.7/avenger-python/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-python/avenger/altair_utils.py` & `avenger-0.0.7/avenger-python/avenger/altair_utils.py`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/avenger-python/src/lib.rs` & `avenger-0.0.7/avenger-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/Cargo.lock` & `avenger-0.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -321,29 +321,29 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "avenger"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "image",
  "lyon_extra",
  "lyon_path",
  "pyo3",
  "rayon",
  "serde",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "avenger-python"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "avenger",
  "avenger-vega",
  "avenger-wgpu",
  "image",
  "lazy_static",
  "pollster",
@@ -352,15 +352,15 @@
  "serde",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "avenger-vega"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "avenger",
  "cfg-if",
  "csscolorparser",
  "image",
  "lazy_static",
  "lyon_extra",
@@ -374,15 +374,15 @@
  "tiny-skia",
  "tracing",
  "usvg 0.38.0",
 ]
 
 [[package]]
 name = "avenger-vega-renderer"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "avenger",
  "avenger-vega",
  "avenger-wgpu",
  "console_error_panic_hook",
  "csscolorparser",
  "gloo-utils",
@@ -398,24 +398,24 @@
  "wasm-bindgen-futures",
  "web-sys",
  "wgpu",
 ]
 
 [[package]]
 name = "avenger-vega-test-data"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "pollster",
  "serde_json",
  "vl-convert-rs",
 ]
 
 [[package]]
 name = "avenger-wgpu"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "avenger",
  "avenger-vega",
  "bytemuck",
  "cfg-if",
  "cgmath",
  "colorgrad",
```

### Comparing `avenger-0.0.6/avenger/altair_utils.py` & `avenger-0.0.7/avenger/altair_utils.py`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/README.md` & `avenger-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/LICENSE` & `avenger-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.6/PKG-INFO` & `avenger-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avenger
-Version: 0.0.6
+Version: 0.0.7
 License-File: LICENSE
 Summary: A Visualization Engine and Renderer
 License: BSD-3-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Avenger: A visualization engine and renderer
 Avenger is an early stage prototype of a new foundational rendering library for information visualization (InfoVis) systems. Avenger defines a 2D scenegraph representation tailored to the needs of InfoVis systems. To start with, the initial application of Avenger is to serve as an alternative, GPU accelerated, rendering backend for Vega visualizations.
```

