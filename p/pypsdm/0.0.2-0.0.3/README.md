# Comparing `tmp/pypsdm-0.0.2.tar.gz` & `tmp/pypsdm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypsdm-0.0.2.tar", max compression
+gzip compressed data, was "pypsdm-0.0.3.tar", max compression
```

## Comparing `pypsdm-0.0.2.tar` & `pypsdm-0.0.3.tar`

### file list

```diff
@@ -1,89 +1,96 @@
--rw-r--r--   0        0        0     1581 2023-10-19 09:20:19.144022 pypsdm-0.0.2/LICENSE
--rw-r--r--   0        0        0     2311 2024-02-12 08:45:11.949782 pypsdm-0.0.2/README.md
--rw-r--r--   0        0        0      840 2024-02-12 09:07:58.322007 pypsdm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.607595 pypsdm-0.0.2/pypsdm/__init__.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.607688 pypsdm-0.0.2/pypsdm/analysis/__init__.py
--rw-r--r--   0        0        0      625 2023-11-07 13:27:54.607779 pypsdm-0.0.2/pypsdm/analysis/calc.py
--rw-r--r--   0        0        0     1251 2023-11-07 13:27:54.607849 pypsdm-0.0.2/pypsdm/analysis/grid.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.607925 pypsdm-0.0.2/pypsdm/conversion/__init__.py
--rw-r--r--   0        0        0     3898 2023-11-07 13:27:54.608010 pypsdm-0.0.2/pypsdm/conversion/pandapower.py
--rw-r--r--   0        0        0        0 2024-01-29 11:16:26.885279 pypsdm-0.0.2/pypsdm/db/__init__.py
--rw-r--r--   0        0        0    15030 2024-02-09 17:06:31.257654 pypsdm-0.0.2/pypsdm/db/gwr.py
--rw-r--r--   0        0        0     3666 2024-01-29 11:20:20.779850 pypsdm-0.0.2/pypsdm/db/utils.py
--rw-r--r--   0        0        0      380 2023-11-07 13:27:54.608076 pypsdm-0.0.2/pypsdm/errors.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.608111 pypsdm-0.0.2/pypsdm/io/__init__.py
--rw-r--r--   0        0        0     5185 2023-11-23 15:34:12.046488 pypsdm-0.0.2/pypsdm/io/utils.py
--rw-r--r--   0        0        0      117 2023-11-07 13:27:54.608804 pypsdm-0.0.2/pypsdm/models/__init__.py
--rw-r--r--   0        0        0     4119 2024-01-31 13:41:24.874193 pypsdm-0.0.2/pypsdm/models/enums.py
--rw-r--r--   0        0        0     8183 2024-02-09 13:56:04.427869 pypsdm-0.0.2/pypsdm/models/gwr.py
--rw-r--r--   0        0        0      124 2024-01-30 11:04:59.372704 pypsdm-0.0.2/pypsdm/models/input/__init__.py
--rw-r--r--   0        0        0      147 2023-11-07 13:27:54.609653 pypsdm-0.0.2/pypsdm/models/input/connector/__init__.py
--rw-r--r--   0        0        0     2858 2024-02-07 13:06:19.306358 pypsdm-0.0.2/pypsdm/models/input/connector/connector.py
--rw-r--r--   0        0        0     1982 2024-02-07 13:06:20.470627 pypsdm-0.0.2/pypsdm/models/input/connector/lines.py
--rw-r--r--   0        0        0     1171 2024-02-07 13:07:18.344971 pypsdm-0.0.2/pypsdm/models/input/connector/switches.py
--rw-r--r--   0        0        0     2202 2024-02-07 13:06:54.776853 pypsdm-0.0.2/pypsdm/models/input/connector/transformer.py
--rw-r--r--   0        0        0      205 2023-11-07 13:27:54.610213 pypsdm-0.0.2/pypsdm/models/input/container/__init__.py
--rw-r--r--   0        0        0     6263 2024-02-07 13:22:21.160660 pypsdm-0.0.2/pypsdm/models/input/container/grid.py
--rw-r--r--   0        0        0     2017 2024-02-08 07:29:50.011476 pypsdm-0.0.2/pypsdm/models/input/container/mixins.py
--rw-r--r--   0        0        0     7150 2024-02-07 13:55:38.948889 pypsdm-0.0.2/pypsdm/models/input/container/participants.py
--rw-r--r--   0        0        0     5258 2024-02-07 12:54:25.825255 pypsdm-0.0.2/pypsdm/models/input/container/raw_grid.py
--rw-r--r--   0        0        0     9382 2023-11-07 13:34:13.925731 pypsdm-0.0.2/pypsdm/models/input/create/participants.py
--rw-r--r--   0        0        0     2118 2023-11-07 13:27:54.611921 pypsdm-0.0.2/pypsdm/models/input/create/poi.py
--rw-r--r--   0        0        0     1644 2023-11-07 13:27:54.611994 pypsdm-0.0.2/pypsdm/models/input/create/thermal.py
--rw-r--r--   0        0        0     3298 2023-11-07 13:27:54.612219 pypsdm-0.0.2/pypsdm/models/input/create/utils.py
--rw-r--r--   0        0        0    15814 2024-02-07 13:11:00.237198 pypsdm-0.0.2/pypsdm/models/input/entity.py
--rw-r--r--   0        0        0     2181 2023-11-07 13:27:54.612906 pypsdm-0.0.2/pypsdm/models/input/mixins.py
--rw-r--r--   0        0        0     1926 2024-02-07 13:02:55.568489 pypsdm-0.0.2/pypsdm/models/input/node.py
--rw-r--r--   0        0        0      646 2023-11-07 13:27:54.613418 pypsdm-0.0.2/pypsdm/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1346 2024-02-07 13:24:48.964845 pypsdm-0.0.2/pypsdm/models/input/participant/bm.py
--rw-r--r--   0        0        0     3109 2023-11-07 13:27:54.613907 pypsdm-0.0.2/pypsdm/models/input/participant/charging.py
--rw-r--r--   0        0        0      883 2024-02-07 13:23:33.290940 pypsdm-0.0.2/pypsdm/models/input/participant/em.py
--rw-r--r--   0        0        0     1985 2024-02-07 13:25:28.749295 pypsdm-0.0.2/pypsdm/models/input/participant/evcs.py
--rw-r--r--   0        0        0     1055 2024-02-07 13:25:18.404308 pypsdm-0.0.2/pypsdm/models/input/participant/evs.py
--rw-r--r--   0        0        0      590 2024-02-07 13:24:28.398160 pypsdm-0.0.2/pypsdm/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      905 2024-02-07 13:25:36.112208 pypsdm-0.0.2/pypsdm/models/input/participant/hp.py
--rw-r--r--   0        0        0     1086 2024-02-07 13:23:38.915309 pypsdm-0.0.2/pypsdm/models/input/participant/load.py
--rw-r--r--   0        0        0      722 2023-11-07 13:27:54.615371 pypsdm-0.0.2/pypsdm/models/input/participant/mixins.py
--rw-r--r--   0        0        0     1227 2024-02-07 13:30:29.926878 pypsdm-0.0.2/pypsdm/models/input/participant/participant.py
--rw-r--r--   0        0        0     1506 2024-02-07 13:24:41.491412 pypsdm-0.0.2/pypsdm/models/input/participant/pv.py
--rw-r--r--   0        0        0     1534 2024-02-07 13:31:50.446996 pypsdm-0.0.2/pypsdm/models/input/participant/storage.py
--rw-r--r--   0        0        0     1205 2024-02-07 13:24:59.331303 pypsdm-0.0.2/pypsdm/models/input/participant/wec.py
--rw-r--r--   0        0        0      165 2023-11-07 13:27:54.616200 pypsdm-0.0.2/pypsdm/models/input/thermal/__init__.py
--rw-r--r--   0        0        0      432 2023-11-07 13:27:54.616273 pypsdm-0.0.2/pypsdm/models/input/thermal/bus.py
--rw-r--r--   0        0        0      849 2023-11-07 13:27:54.616341 pypsdm-0.0.2/pypsdm/models/input/thermal/grid.py
--rw-r--r--   0        0        0     1186 2023-11-07 13:27:54.616395 pypsdm-0.0.2/pypsdm/models/input/thermal/house.py
--rw-r--r--   0        0        0     9691 2023-11-23 15:34:12.112731 pypsdm-0.0.2/pypsdm/models/primary_data.py
--rw-r--r--   0        0        0      172 2023-11-07 13:27:54.616748 pypsdm-0.0.2/pypsdm/models/result/__init__.py
--rw-r--r--   0        0        0      190 2023-11-07 13:27:54.616934 pypsdm-0.0.2/pypsdm/models/result/container/__init__.py
--rw-r--r--   0        0        0     4874 2024-02-09 12:00:32.412045 pypsdm-0.0.2/pypsdm/models/result/container/grid.py
--rw-r--r--   0        0        0    13875 2024-02-08 08:29:56.898494 pypsdm-0.0.2/pypsdm/models/result/container/participants.py
--rw-r--r--   0        0        0     6672 2024-02-08 07:48:25.846392 pypsdm-0.0.2/pypsdm/models/result/container/raw_grid.py
--rw-r--r--   0        0        0    11572 2024-02-08 12:12:40.224771 pypsdm-0.0.2/pypsdm/models/result/entity.py
--rw-r--r--   0        0        0      440 2023-11-07 13:27:54.617912 pypsdm-0.0.2/pypsdm/models/result/grid/__init__.py
--rw-r--r--   0        0        0     3028 2024-02-07 13:42:47.849509 pypsdm-0.0.2/pypsdm/models/result/grid/connector.py
--rw-r--r--   0        0        0     2698 2024-02-12 07:39:16.383782 pypsdm-0.0.2/pypsdm/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     3419 2024-02-07 13:27:23.205550 pypsdm-0.0.2/pypsdm/models/result/grid/node.py
--rw-r--r--   0        0        0     1849 2024-02-07 13:51:01.987939 pypsdm-0.0.2/pypsdm/models/result/grid/switch.py
--rw-r--r--   0        0        0     2613 2024-02-07 13:44:00.175312 pypsdm-0.0.2/pypsdm/models/result/grid/transformer.py
--rw-r--r--   0        0        0      165 2023-11-07 13:27:54.618384 pypsdm-0.0.2/pypsdm/models/result/participant/__init__.py
--rw-r--r--   0        0        0    12367 2024-02-09 10:23:45.755341 pypsdm-0.0.2/pypsdm/models/result/participant/dict.py
--rw-r--r--   0        0        0     3730 2024-02-08 08:31:28.612087 pypsdm-0.0.2/pypsdm/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     3714 2024-02-07 13:28:26.904434 pypsdm-0.0.2/pypsdm/models/result/participant/pq_dict.py
--rw-r--r--   0        0        0     6796 2024-02-07 13:49:19.764750 pypsdm-0.0.2/pypsdm/models/result/power.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.619101 pypsdm-0.0.2/pypsdm/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.619160 pypsdm-0.0.2/pypsdm/plots/common/__init__.py
--rw-r--r--   0        0        0     2885 2023-11-07 13:34:13.079443 pypsdm-0.0.2/pypsdm/plots/common/bar_plot.py
--rw-r--r--   0        0        0     1278 2023-11-07 13:27:54.619485 pypsdm-0.0.2/pypsdm/plots/common/line_plot.py
--rw-r--r--   0        0        0     1028 2024-02-09 10:46:58.271415 pypsdm-0.0.2/pypsdm/plots/common/style.py
--rw-r--r--   0        0        0     6089 2023-11-07 13:34:14.326652 pypsdm-0.0.2/pypsdm/plots/common/utils.py
--rw-r--r--   0        0        0     7362 2024-02-09 09:38:53.969629 pypsdm-0.0.2/pypsdm/plots/grid.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.619920 pypsdm-0.0.2/pypsdm/plots/results/__init__.py
--rw-r--r--   0        0        0     8653 2023-11-07 13:27:54.620068 pypsdm-0.0.2/pypsdm/plots/results/connector_plot.py
--rw-r--r--   0        0        0     3436 2024-02-09 10:50:03.771387 pypsdm-0.0.2/pypsdm/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1297 2023-11-07 13:27:54.620262 pypsdm-0.0.2/pypsdm/plots/results/nodes.py
--rw-r--r--   0        0        0    17671 2024-02-09 10:50:31.120756 pypsdm-0.0.2/pypsdm/plots/results/power_plot.py
--rw-r--r--   0        0        0     7865 2023-11-07 13:27:54.620719 pypsdm-0.0.2/pypsdm/plots/results/voltage_plot.py
--rw-r--r--   0        0        0        0 2023-11-07 13:27:54.620750 pypsdm-0.0.2/pypsdm/processing/__init__.py
--rw-r--r--   0        0        0     1788 2023-11-07 13:27:54.620964 pypsdm-0.0.2/pypsdm/processing/dataframe.py
--rw-r--r--   0        0        0     2228 2023-11-07 13:27:54.651747 pypsdm-0.0.2/pypsdm/processing/series.py
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 pypsdm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1581 2024-03-06 12:52:05.879858 pypsdm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2311 2024-03-06 12:52:05.880176 pypsdm-0.0.3/README.md
+-rw-r--r--   0        0        0      966 2024-04-30 11:24:32.720299 pypsdm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-03-11 07:48:22.849243 pypsdm-0.0.3/pypsdm/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.907560 pypsdm-0.0.3/pypsdm/analysis/__init__.py
+-rw-r--r--   0        0        0      625 2024-03-06 12:52:05.907864 pypsdm-0.0.3/pypsdm/analysis/calc.py
+-rw-r--r--   0        0        0     1251 2024-03-06 12:52:05.907951 pypsdm-0.0.3/pypsdm/analysis/grid.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.908006 pypsdm-0.0.3/pypsdm/conversion/__init__.py
+-rw-r--r--   0        0        0     3896 2024-04-30 11:24:32.722505 pypsdm-0.0.3/pypsdm/conversion/pandapower.py
+-rw-r--r--   0        0        0       51 2024-03-27 08:57:05.226610 pypsdm-0.0.3/pypsdm/db/__init__.py
+-rw-r--r--   0        0        0    20413 2024-04-30 11:24:32.722854 pypsdm-0.0.3/pypsdm/db/gwr.py
+-rw-r--r--   0        0        0     3666 2024-03-06 12:52:05.909289 pypsdm-0.0.3/pypsdm/db/utils.py
+-rw-r--r--   0        0        0      264 2024-04-10 12:33:59.411508 pypsdm-0.0.3/pypsdm/db/weather/__init__.py
+-rw-r--r--   0        0        0     2156 2024-05-02 08:01:33.666484 pypsdm-0.0.3/pypsdm/db/weather/models.py
+-rw-r--r--   0        0        0     4422 2024-05-02 08:44:37.455294 pypsdm-0.0.3/pypsdm/db/weather/proxy.py
+-rw-r--r--   0        0        0     5159 2024-05-02 08:01:33.667717 pypsdm-0.0.3/pypsdm/db/weather/utils.py
+-rw-r--r--   0        0        0      380 2024-03-06 12:52:05.909483 pypsdm-0.0.3/pypsdm/errors.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.909569 pypsdm-0.0.3/pypsdm/io/__init__.py
+-rw-r--r--   0        0        0     5159 2024-04-30 11:24:32.723327 pypsdm-0.0.3/pypsdm/io/utils.py
+-rw-r--r--   0        0        0      129 2024-05-03 10:30:22.510341 pypsdm-0.0.3/pypsdm/models/__init__.py
+-rw-r--r--   0        0        0     6445 2024-04-30 11:24:32.723752 pypsdm-0.0.3/pypsdm/models/enums.py
+-rw-r--r--   0        0        0     9540 2024-04-30 11:24:32.724448 pypsdm-0.0.3/pypsdm/models/gwr.py
+-rw-r--r--   0        0        0      124 2024-03-06 12:52:05.912269 pypsdm-0.0.3/pypsdm/models/input/__init__.py
+-rw-r--r--   0        0        0      147 2024-03-06 12:52:05.912770 pypsdm-0.0.3/pypsdm/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     2857 2024-03-06 12:52:05.913038 pypsdm-0.0.3/pypsdm/models/input/connector/connector.py
+-rw-r--r--   0        0        0     5182 2024-04-30 11:24:32.725026 pypsdm-0.0.3/pypsdm/models/input/connector/lines.py
+-rw-r--r--   0        0        0     1170 2024-03-06 12:52:05.913575 pypsdm-0.0.3/pypsdm/models/input/connector/switches.py
+-rw-r--r--   0        0        0     7064 2024-03-14 09:49:16.396511 pypsdm-0.0.3/pypsdm/models/input/connector/transformer.py
+-rw-r--r--   0        0        0      205 2024-03-06 12:52:05.914272 pypsdm-0.0.3/pypsdm/models/input/container/__init__.py
+-rw-r--r--   0        0        0     6662 2024-04-30 11:24:32.726089 pypsdm-0.0.3/pypsdm/models/input/container/grid.py
+-rw-r--r--   0        0        0     5192 2024-04-30 11:24:32.726393 pypsdm-0.0.3/pypsdm/models/input/container/mixins.py
+-rw-r--r--   0        0        0     8126 2024-04-30 11:24:32.726717 pypsdm-0.0.3/pypsdm/models/input/container/participants.py
+-rw-r--r--   0        0        0     6171 2024-04-30 11:24:32.727170 pypsdm-0.0.3/pypsdm/models/input/container/raw_grid.py
+-rw-r--r--   0        0        0        0 2024-03-11 07:48:22.850752 pypsdm-0.0.3/pypsdm/models/input/create/__init__.py
+-rw-r--r--   0        0        0    10607 2024-04-30 11:24:32.727504 pypsdm-0.0.3/pypsdm/models/input/create/participants.py
+-rw-r--r--   0        0        0     2118 2024-03-06 12:52:05.916072 pypsdm-0.0.3/pypsdm/models/input/create/poi.py
+-rw-r--r--   0        0        0     1644 2024-03-06 12:52:05.916356 pypsdm-0.0.3/pypsdm/models/input/create/thermal.py
+-rw-r--r--   0        0        0     3298 2024-03-06 12:52:05.916676 pypsdm-0.0.3/pypsdm/models/input/create/utils.py
+-rw-r--r--   0        0        0    16404 2024-04-30 11:24:32.727886 pypsdm-0.0.3/pypsdm/models/input/entity.py
+-rw-r--r--   0        0        0     2181 2024-03-06 12:52:05.917680 pypsdm-0.0.3/pypsdm/models/input/mixins.py
+-rw-r--r--   0        0        0     1926 2024-03-06 12:52:05.917898 pypsdm-0.0.3/pypsdm/models/input/node.py
+-rw-r--r--   0        0        0      646 2024-03-06 12:52:05.918346 pypsdm-0.0.3/pypsdm/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1350 2024-04-30 11:24:32.728243 pypsdm-0.0.3/pypsdm/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3109 2024-03-06 12:52:05.920087 pypsdm-0.0.3/pypsdm/models/input/participant/charging.py
+-rw-r--r--   0        0        0      887 2024-04-30 11:24:32.728565 pypsdm-0.0.3/pypsdm/models/input/participant/em.py
+-rw-r--r--   0        0        0     1989 2024-04-30 11:24:32.728855 pypsdm-0.0.3/pypsdm/models/input/participant/evcs.py
+-rw-r--r--   0        0        0     1085 2024-04-30 11:24:32.729041 pypsdm-0.0.3/pypsdm/models/input/participant/evs.py
+-rw-r--r--   0        0        0      594 2024-04-30 11:24:32.729246 pypsdm-0.0.3/pypsdm/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      909 2024-04-30 11:24:32.729443 pypsdm-0.0.3/pypsdm/models/input/participant/hp.py
+-rw-r--r--   0        0        0     1090 2024-04-30 11:24:32.729753 pypsdm-0.0.3/pypsdm/models/input/participant/load.py
+-rw-r--r--   0        0        0      722 2024-03-06 12:52:05.922777 pypsdm-0.0.3/pypsdm/models/input/participant/mixins.py
+-rw-r--r--   0        0        0     1243 2024-04-30 11:24:32.730225 pypsdm-0.0.3/pypsdm/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1510 2024-04-30 11:24:32.730754 pypsdm-0.0.3/pypsdm/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1538 2024-04-30 11:24:32.730945 pypsdm-0.0.3/pypsdm/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1209 2024-04-30 11:24:32.731119 pypsdm-0.0.3/pypsdm/models/input/participant/wec.py
+-rw-r--r--   0        0        0      165 2024-03-06 12:52:05.923553 pypsdm-0.0.3/pypsdm/models/input/thermal/__init__.py
+-rw-r--r--   0        0        0      432 2024-03-06 12:52:05.923789 pypsdm-0.0.3/pypsdm/models/input/thermal/bus.py
+-rw-r--r--   0        0        0      842 2024-04-30 11:24:32.731517 pypsdm-0.0.3/pypsdm/models/input/thermal/grid.py
+-rw-r--r--   0        0        0     1186 2024-03-06 12:52:05.923916 pypsdm-0.0.3/pypsdm/models/input/thermal/house.py
+-rw-r--r--   0        0        0    10132 2024-04-30 11:24:32.731839 pypsdm-0.0.3/pypsdm/models/primary_data.py
+-rw-r--r--   0        0        0       72 2024-04-30 11:24:32.732122 pypsdm-0.0.3/pypsdm/models/result/__init__.py
+-rw-r--r--   0        0        0      256 2024-04-30 11:24:32.732326 pypsdm-0.0.3/pypsdm/models/result/container/__init__.py
+-rw-r--r--   0        0        0     5648 2024-04-30 11:24:32.732679 pypsdm-0.0.3/pypsdm/models/result/container/grid.py
+-rw-r--r--   0        0        0     9371 2024-04-30 11:24:32.732929 pypsdm-0.0.3/pypsdm/models/result/container/participants.py
+-rw-r--r--   0        0        0     5272 2024-04-30 11:24:32.733174 pypsdm-0.0.3/pypsdm/models/result/container/raw_grid.py
+-rw-r--r--   0        0        0      440 2024-04-30 11:24:32.733506 pypsdm-0.0.3/pypsdm/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     3810 2024-04-30 11:24:32.734295 pypsdm-0.0.3/pypsdm/models/result/grid/connector.py
+-rw-r--r--   0        0        0     1062 2024-04-30 11:24:32.734631 pypsdm-0.0.3/pypsdm/models/result/grid/line.py
+-rw-r--r--   0        0        0      497 2024-04-30 11:24:32.735108 pypsdm-0.0.3/pypsdm/models/result/grid/node.py
+-rw-r--r--   0        0        0     1169 2024-04-30 11:24:32.735402 pypsdm-0.0.3/pypsdm/models/result/grid/switch.py
+-rw-r--r--   0        0        0     3360 2024-04-30 11:24:32.735752 pypsdm-0.0.3/pypsdm/models/result/grid/transformer.py
+-rw-r--r--   0        0        0      490 2024-04-30 11:24:32.735957 pypsdm-0.0.3/pypsdm/models/result/participant/__init__.py
+-rw-r--r--   0        0        0    11441 2024-05-02 08:01:33.668287 pypsdm-0.0.3/pypsdm/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3340 2024-04-30 11:24:32.736696 pypsdm-0.0.3/pypsdm/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0       41 2024-04-30 11:24:32.737085 pypsdm-0.0.3/pypsdm/models/ts/__init__.py
+-rw-r--r--   0        0        0    14808 2024-04-30 11:24:32.737378 pypsdm-0.0.3/pypsdm/models/ts/base.py
+-rw-r--r--   0        0        0     7532 2024-05-02 08:01:33.668625 pypsdm-0.0.3/pypsdm/models/ts/mixins.py
+-rw-r--r--   0        0        0     7239 2024-05-02 08:01:33.668941 pypsdm-0.0.3/pypsdm/models/ts/types.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.928010 pypsdm-0.0.3/pypsdm/plots/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.928084 pypsdm-0.0.3/pypsdm/plots/common/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-30 11:24:32.738402 pypsdm-0.0.3/pypsdm/plots/common/bar_plot.py
+-rw-r--r--   0        0        0     1488 2024-04-30 11:24:32.738641 pypsdm-0.0.3/pypsdm/plots/common/line_plot.py
+-rw-r--r--   0        0        0     1028 2024-03-06 12:52:05.928941 pypsdm-0.0.3/pypsdm/plots/common/style.py
+-rw-r--r--   0        0        0     6590 2024-04-30 11:24:32.739083 pypsdm-0.0.3/pypsdm/plots/common/utils.py
+-rw-r--r--   0        0        0     7412 2024-04-08 06:34:45.701529 pypsdm-0.0.3/pypsdm/plots/grid.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.929593 pypsdm-0.0.3/pypsdm/plots/results/__init__.py
+-rw-r--r--   0        0        0     7023 2024-04-30 11:24:32.739894 pypsdm-0.0.3/pypsdm/plots/results/connector.py
+-rw-r--r--   0        0        0     3795 2024-04-30 11:24:32.740031 pypsdm-0.0.3/pypsdm/plots/results/flex.py
+-rw-r--r--   0        0        0     1287 2024-04-30 11:24:32.740213 pypsdm-0.0.3/pypsdm/plots/results/nodes.py
+-rw-r--r--   0        0        0    20296 2024-04-30 11:24:32.740469 pypsdm-0.0.3/pypsdm/plots/results/power.py
+-rw-r--r--   0        0        0     8853 2024-04-30 11:24:32.740662 pypsdm-0.0.3/pypsdm/plots/results/voltage.py
+-rw-r--r--   0        0        0        0 2024-03-06 12:52:05.930749 pypsdm-0.0.3/pypsdm/processing/__init__.py
+-rw-r--r--   0        0        0     3063 2024-05-02 08:01:33.669204 pypsdm-0.0.3/pypsdm/processing/dataframe.py
+-rw-r--r--   0        0        0     3812 2024-04-30 11:24:32.741226 pypsdm-0.0.3/pypsdm/processing/numba.py
+-rw-r--r--   0        0        0     2609 2024-04-30 11:24:32.741618 pypsdm-0.0.3/pypsdm/processing/series.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 pypsdm-0.0.3/PKG-INFO
```

### Comparing `pypsdm-0.0.2/LICENSE` & `pypsdm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/README.md` & `pypsdm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pyproject.toml` & `pypsdm-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 [tool.poetry]
 name = "pypsdm"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.11, <3.12"
 pandas = ">1.2, <2.1"
 jupyter = "^1.0.0"
 matplotlib = "^3.6.0"
-seaborn = "^0.12.1"
+seaborn = "0.13"
 plotly = "^5.6.0"
 requests = "^2.27.1"
 numpy = "^1.24.1"
 scipy = "^1.10.0"
 pyarrow = "^11.0.0"
 openpyxl = "^3.1.2"
-python-dotenv = "^1.0.0" # Can probably be removed in the future
+python-dotenv = "^1.0.0"                              # Can probably be removed in the future
 shapely = "^2.0.1"
 networkx = "^3.1"
-black = {extras = ["jupyter"], version = "~24.1.1"}
+black = { extras = ["jupyter"], version = "~24.1.1" }
+loguru = "^0.7.2"
+sqlmodel = "^0.0.14"
+pyhocon = "^0.3.60"
+psycopg2 = "^2.9.9"
+numba = "^0.59.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^6.0.0"
 flake8-black = "^0.3.6"
 flake8-isort = "^6.0.0"
 pre-commit = ">=2.21,<4.0"
 PyYAML = "^6.0"
 
 [tool.isort]
-profile= "black"
+profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pypsdm-0.0.2/pypsdm/analysis/calc.py` & `pypsdm-0.0.3/pypsdm/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/analysis/grid.py` & `pypsdm-0.0.3/pypsdm/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/conversion/pandapower.py` & `pypsdm-0.0.3/pypsdm/conversion/pandapower.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,52 +4,52 @@
 
 from pypsdm.models.enums import (
     EntitiesEnum,
     RawGridElementsEnum,
     SystemParticipantsEnum,
 )
 from pypsdm.models.result.grid.node import NodeResult, NodesResult
-from pypsdm.models.result.participant.pq_dict import PQResultDict
 from pypsdm.models.result.power import PQResult
+from pypsdm.models.ts.types import ComplexPowerDict
 
 # These are just some early quite specific conversions. Additional ones will be added as needed.
 
 
 def pp_load_to_participants_result(
     pp_net_file: str,  # pp net xlsx export
     participant_p_file: str,  # pp time series p_mw export
     participant_q_file: str,  # pp time series q_mvar export
     psdm_load_file: str,  # psdm load csv input
     start: datetime,  # start of the time series simulation
     resolution: timedelta,  # resolution of the time series simulation
-) -> PQResultDict:
+) -> ComplexPowerDict:
     return _pp_to_psdm_result(
         entity_type=SystemParticipantsEnum.LOAD,
         pp_net_file=pp_net_file,
         pp_sheet_name="load",
         pp_attribute_a_file=participant_p_file,
         psdm_attribute_a_name="p",
         pp_attribute_b_file=participant_q_file,
         psdm_attribute_b_name="q",
         psdm_entity_input_file=psdm_load_file,
         start=start,
         resolution=resolution,
         res_entity_class=PQResult,
-        res_dict_class=PQResultDict,
+        res_dict_class=ComplexPowerDict,
     )
 
 
 def pp_node_to_nodes_result(
     pp_net_file: str,  # pp net xlsx export
     node_vm_file: str,  # pp time series vm_pu export
     node_va_file: str,  # pp time series va_degree export
     psdm_node_file: str,  # psdm node csv input
     start: datetime,  # start of the time series simulation
     resolution: timedelta,  # resolution of the time series simulation
-) -> PQResultDict:
+) -> ComplexPowerDict:
     return _pp_to_psdm_result(
         entity_type=RawGridElementsEnum.NODE,
         pp_net_file=pp_net_file,
         pp_sheet_name="bus",
         pp_attribute_a_file=node_vm_file,
         psdm_attribute_a_name="v_mag",
         pp_attribute_b_file=node_va_file,
```

### Comparing `pypsdm-0.0.2/pypsdm/db/gwr.py` & `pypsdm-0.0.3/pypsdm/db/gwr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import os
 import re
 import shutil
+from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
 
+from loguru import logger
+from pyhocon import ConfigFactory, ConfigTree, HOCONConverter
+
 from pypsdm.db.utils import PathManagerMixin
 from pypsdm.models.gwr import GridWithResults
-from pypsdm.models.input import GridContainer
-from pypsdm.models.result import GridResultContainer
+from pypsdm.models.input.container.grid import GridContainer
+from pypsdm.models.result.container.grid import GridResultContainer
 
 # Grid id naming strategy
 # [grid id]-v[version number]
 # e.g. my_grid-v1
 GRID_ID_REGEX = re.compile(r"(\w+)-v(\d+)")
 
 # Simulation result folder naming strategy
@@ -21,14 +25,15 @@
 RESULT_DATE_REGEX = re.compile(r"(\d{4}_\d{2}_\d{2})(?:-\d+)?")
 RESULT_SUFFIX_REGEX = re.compile(r"(?:-(.+))?")
 RESULT_ID_REGEX = re.compile(
     r"{}-({}){}".format(
         RESULT_DATE_REGEX.pattern, GRID_ID_REGEX.pattern, RESULT_SUFFIX_REGEX.pattern
     )
 )
+DB_ENV_VAR = "LOCAL_GWR_DB"
 
 
 @dataclass
 class LocalGwrDb(PathManagerMixin):
     """
     Local database that keeps track of grid models and and corresponding results.
     Offers methods to read grids, results as well as grid with results. Also
@@ -38,15 +43,27 @@
 
     Args:
         path (Path): Base path to database.
     """
 
     path: Path
 
-    def __init__(self, path: str | Path):
+    def __init__(self, path: str | Path | None = None):
+        if path is None:
+            path = os.environ.get(DB_ENV_VAR)
+            if path is None:
+                raise ValueError(
+                    f"Database path not specified. Set {DB_ENV_VAR} environment variable or pass path as argument."
+                )
+            if path.startswith("~"):
+                path = os.path.expanduser(path)
+            path = Path(path).absolute()
+        else:
+            if path.startswith("~"):
+                path = os.path.expanduser(path)
         self.path = Path(path) if isinstance(path, str) else path
 
     @property
     def grids_path(self) -> Path:
         return self.path.joinpath("grids")
 
     @property
@@ -162,22 +179,76 @@
                 if match:
                     _, grid_id, _ = match
                     if grid_id == grid_id:
                         filtered.append(res)
             results = filtered
         return results
 
+    def open_configs(self, grid_id: str):
+        path = self.get_grid_path(grid_id)
+        if path:
+            conf_path = path.joinpath("configs")
+            if conf_path.exists():
+                self.open_in_file_explorer()
+            else:
+                raise FileNotFoundError(
+                    f"No configs for {grid_id} exist in {conf_path}."
+                )
+        else:
+            raise FileNotFoundError(f"Grid with id {grid_id} does not exist.")
+
+    def copy_configs(
+        self,
+        grid_id: str,
+        target_grid_id: str,
+        adjust_grid_path: bool = True,
+        copy_slack_volt: bool = True,
+    ):
+        origin_grid_path = self.get_grid_path(grid_id)
+        if not origin_grid_path:
+            raise FileNotFoundError(f"Grid with id {grid_id} does not exist.")
+
+        origin_conf_path = origin_grid_path.joinpath("configs")
+        if not origin_conf_path.exists():
+            logger.debug(f"No configs for {grid_id} exist in {origin_conf_path}.")
+            return
+
+        target_grid_path = self.get_grid_path(target_grid_id)
+        if not target_grid_path:
+            raise FileNotFoundError(f"Grid with id {target_grid_id} does not exist.")
+        target_conf_path = target_grid_path.joinpath("configs")
+        target_conf_path.mkdir(exist_ok=True)
+
+        for file in os.listdir(origin_conf_path):
+            conf = ConfigFactory.parse_file(origin_conf_path.joinpath(file))
+            if adjust_grid_path:
+                conf = self.adjust_conf_path(conf, str(target_grid_path))
+            conf = HOCONConverter.to_hocon(conf)
+            with open(os.path.join(target_conf_path, file), "w") as f:
+                f.write(conf)
+
+        # temporary
+        if copy_slack_volt:
+            slack_v_path = origin_grid_path.joinpath("slack_volt.csv")
+            if slack_v_path.exists():
+                shutil.copy(slack_v_path, target_grid_path)
+
     def read_gwr_most_recent(self, grid_id) -> GridWithResults:
         """Read most recent GridWithResults."""
         result = self.list_results(grid_id)[0]
         return self.read_gwr(result)
 
     def read_gwr(self, res_id: str) -> GridWithResults:
         """Read GridWithResults."""
-        res_path = os.path.join(self.results_path, res_id, "rawOutputData")
+
+        raw_output_path = os.path.join(self.results_path, res_id, "rawOutputData")
+        if os.path.exists(raw_output_path):
+            res_path = raw_output_path
+        else:
+            res_path = os.path.join(self.results_path, res_id)
         res_id_match = self.match_res_id(res_id)
         if res_id_match:
             _, grid_id, _ = res_id_match
         else:
             raise ValueError(
                 f"Invalid res_id: {res_id}, expected format: {RESULT_ID_REGEX.pattern}"
             )
@@ -208,23 +279,21 @@
         grid_path = self.get_grid_path(identifier)
         if grid_path is None:
             raise FileNotFoundError(
                 f"Grid or result with id {identifier} does not exist in database."
             )
         return GridContainer.from_csv(
             str(grid_path),
-            delimiter=",",
         )
 
     def read_results(self, res_id: str):
         """Read results from res_id."""
         return GridResultContainer.from_csv(
             res_id,
             str(self.results_path.joinpath(res_id)),
-            delimiter=",",
         )
 
     def add_grid(
         self,
         grid: GridContainer,
         grid_id: str,
         include_primary_data: bool = True,
@@ -302,14 +371,54 @@
             raise FileExistsError(f"Grid with id {versioned_id} already exists.")
         if move:
             os.rename(grid_path, destination_dir)
         else:
             shutil.copytree(grid_path, destination_dir)
         return versioned_id
 
+    def add_results(
+        self,
+        results: GridResultContainer,
+        versioned_grid_id: str,
+        suffix: str | None = None,
+        date: datetime | None = None,
+    ):
+        """
+        Adds results to local "database".
+        NOTE: There needs to be a grid with the given versioned_grid_id in the database.
+
+        Args:
+            results (GridResultContainer): GridResultContainer instance.
+            versioned_grid_id (str): Versioned grid id.
+            date (datetime, optional): Date of results. Defaults to None.
+            move (bool, optional): Move results to database source path. Defaults to False.
+        """
+        versioned_grid_id_match = self.match_grid_id(versioned_grid_id)
+        if versioned_grid_id_match is None:
+            raise ValueError(
+                f"Invalid grid_id: {versioned_grid_id}, expected format: {GRID_ID_REGEX.pattern}"
+            )
+
+        # Check if corresponding grid exists
+        grid_path = self.grids_path.joinpath(versioned_grid_id)
+        if not grid_path.exists():
+            raise FileNotFoundError(
+                f"Grid with id {versioned_grid_id} does not exist. Please add grid first."
+            )
+
+        if not date:
+            date = datetime.now()
+
+        # Add result data
+        res_id = self.create_res_id(versioned_grid_id, date, suffix)
+        destination_dir = self.results_path.joinpath(res_id)
+        if destination_dir.exists():
+            raise FileExistsError(f"Results with id {res_id} already exists.")
+        results.to_csv(str(destination_dir), mkdirs=True)
+
     def add_results_from_path(
         self,
         results_path: str | Path,
         versioned_grid_id: str,
         suffix: str | None = None,
         date: datetime | None = None,
         move=False,
@@ -334,35 +443,33 @@
         # Check if corresponding grid exists
         grid_path = self.grids_path.joinpath(versioned_grid_id)
         if not grid_path.exists():
             raise FileNotFoundError(
                 f"Grid with id {versioned_grid_id} does not exist. Please add grid first."
             )
 
-        # Check if results are present where expected
-        raw_output_path = os.path.join(results_path, "rawOutputData")
-        if not os.path.exists(raw_output_path):
-            raise FileNotFoundError(f"Expected results at {raw_output_path}.")
-
         if not date:
             # Get date where result folder was created
-            raw_output_path_stat = os.stat(raw_output_path)
-            date = datetime.fromtimestamp(raw_output_path_stat.st_mtime)
+            result_path_stat = os.stat(results_path)
+            date = datetime.fromtimestamp(result_path_stat.st_mtime)
 
         # Add result data
         res_id = self.create_res_id(versioned_grid_id, date, suffix)
         destination_dir = self.results_path.joinpath(res_id)
         if destination_dir.exists():
             raise FileExistsError(f"Results with id {res_id} already exists.")
         if move:
             os.rename(results_path, destination_dir)
         else:
             shutil.copytree(results_path, destination_dir)
 
     def create_grid_id(self, grid_id: str) -> str:
+        match = self.match_grid_id(grid_id)
+        if match:
+            grid_id = match[0]
         grids = self.list_grids(grid_id)
         if grids:
             max_version = 1
             for grid in grids:
                 match = self.match_grid_id(grid)
                 if match:
                     _, version = match
@@ -405,7 +512,40 @@
             date = datetime.now()
         res_id = f"{date.strftime('%Y_%m_%d')}-{grid_id}"
         if suffix:
             res_id = res_id + f"-{suffix}"
         match = RESULT_ID_REGEX.match(res_id)
         assert match, f"Invalid res_id: {res_id}"
         return res_id
+
+    def adjust_conf_path(self, conf: ConfigTree, new_grid_path: str):
+        grid_paths_to_adjust = [
+            "simona.input.grid.datasource.csvParams.directoryPath",
+            "simona.input.primary.csvParams.directoryPath",
+        ]
+
+        updated = deepcopy(conf)
+        for p in grid_paths_to_adjust:
+            if p in conf:
+                updated.put(p, new_grid_path)
+            else:
+                raise ValueError(f"Path {p} not found in config.")
+
+        grid_id = Path(new_grid_path).name
+        res_id = self.create_res_id(grid_id)
+        output_conf = "simona.output.base.dir"
+
+        if output_conf in updated:
+            updated.put(output_conf, os.path.join(self.results_path, res_id))
+            updated.put("simona.output.base.addTimestampToOutputDir", "false")
+
+        updated.put("siona.simulationName", res_id)
+
+        slack_volt_src = "simona.input.grid.slackVoltageSource.directoryPath"
+        if slack_volt_src in conf:
+            sl_volt_path = conf.get(slack_volt_src)
+            if sl_volt_path:
+                file_name = Path(sl_volt_path).name
+                new_sl_volt_path = os.path.join(new_grid_path, file_name)
+                updated.put(slack_volt_src, new_sl_volt_path)
+
+        return updated
```

### Comparing `pypsdm-0.0.2/pypsdm/db/utils.py` & `pypsdm-0.0.3/pypsdm/db/utils.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/io/utils.py` & `pypsdm-0.0.3/pypsdm/io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         raise ValueError(f"Unexpected date time string: {zoned_date_time}")
     try:
         year = int(zoned_date_time[0:4])
         month = int(zoned_date_time[5:7])
         day = int(zoned_date_time[8:10])
         hour = int(zoned_date_time[11:13])
         minute = int(zoned_date_time[14:16])
-    except IndexError:
-        raise IOError(f"Could not parse time stamp: {zoned_date_time}")
+    except Exception:
+        return pd.to_datetime(zoned_date_time)
     return datetime(year=year, month=month, day=day, hour=hour, minute=minute)
 
 
 def csv_to_grpd_df(
     file_name: str, simulation_data_path: str, delimiter: str | None = None
 ) -> DataFrameGroupBy:
     """
```

### Comparing `pypsdm-0.0.2/pypsdm/models/enums.py` & `pypsdm-0.0.3/pypsdm/models/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+from __future__ import annotations
+
 from enum import Enum
-from typing import TypeVar
+from typing import TYPE_CHECKING, Type, TypeVar
+
+if TYPE_CHECKING:
+    from pypsdm.models.result.participant.dict import EntitiesResultDictMixin
+    from pypsdm.models.ts.base import TimeSeries
 
 
 class EntitiesEnum(Enum):
     def has_type(self):
         if self in {
             RawGridElementsEnum.LINE,
             RawGridElementsEnum.TRANSFORMER_2_W,
@@ -27,44 +33,97 @@
     def get_type_file_name(self):
         assert self.has_type() is True
         return self.value + "_type_input.csv"
 
     def get_plot_name(self):
         return self.value.replace("_", " ").title()
 
-    def get_result_type(self):
+    def get_result_type(self) -> type[TimeSeries]:
         # locally to avoid circular imports
-        from pypsdm.models.result.grid.connector import ConnectorResult
-        from pypsdm.models.result.grid.node import NodeResult
+        from pypsdm.models.result.grid.connector import ConnectorCurrent
         from pypsdm.models.result.grid.switch import SwitchResult
         from pypsdm.models.result.grid.transformer import Transformer2WResult
-        from pypsdm.models.result.power import PQResult, PQWithSocResult
+        from pypsdm.models.ts.types import (
+            ComplexPower,
+            ComplexPowerWithSoc,
+            ComplexVoltage,
+        )
 
         if isinstance(self, SystemParticipantsEnum):
             if self.has_soc():
-                return PQWithSocResult
+                return ComplexPowerWithSoc
             else:
-                return PQResult
+                return ComplexPower
         elif isinstance(self, RawGridElementsEnum):
             match self:
                 case RawGridElementsEnum.NODE:
-                    return NodeResult
+                    return ComplexVoltage
                 case RawGridElementsEnum.TRANSFORMER_2_W:
                     return Transformer2WResult
                 case RawGridElementsEnum.LINE:
-                    return ConnectorResult
+                    return ConnectorCurrent
                 case RawGridElementsEnum.SWITCH:
                     return SwitchResult
                 case _:
                     raise NotImplementedError(
                         f"Result type {self} not implemented yet!"
                     )
         else:
             raise ValueError(f"Entity type {self} not supported!")
 
+    def get_result_dict_type(self) -> Type["EntitiesResultDictMixin"]:
+        from pypsdm.models.result.grid.line import LinesResult
+        from pypsdm.models.result.grid.node import NodesResult
+        from pypsdm.models.result.grid.switch import SwitchesResult
+        from pypsdm.models.result.grid.transformer import Transformers2WResult
+        from pypsdm.models.result.participant.dict import (
+            EmsResult,
+            EvcsResult,
+            EvsResult,
+            FixedFeedInsResult,
+            HpsResult,
+            LoadsResult,
+            PvsResult,
+            StoragesResult,
+            WecsResult,
+        )
+        from pypsdm.models.result.participant.flex_options import FlexOptionsDict
+
+        match self:
+            case RawGridElementsEnum.NODE:
+                return NodesResult
+            case RawGridElementsEnum.LINE:
+                return LinesResult
+            case RawGridElementsEnum.TRANSFORMER_2_W:
+                return Transformers2WResult
+            case RawGridElementsEnum.SWITCH:
+                return SwitchesResult
+            case SystemParticipantsEnum.ELECTRIC_VEHICLE:
+                return EvsResult
+            case SystemParticipantsEnum.EV_CHARGING_STATION:
+                return EvcsResult
+            case SystemParticipantsEnum.FIXED_FEED_IN:
+                return FixedFeedInsResult
+            case SystemParticipantsEnum.LOAD:
+                return LoadsResult
+            case SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT:
+                return PvsResult
+            case SystemParticipantsEnum.WIND_ENERGY_CONVERTER:
+                return WecsResult
+            case SystemParticipantsEnum.STORAGE:
+                return StoragesResult
+            case SystemParticipantsEnum.ENERGY_MANAGEMENT:
+                return EmsResult
+            case SystemParticipantsEnum.HEAT_PUMP:
+                return HpsResult
+            case SystemParticipantsEnum.FLEX_OPTIONS:
+                return FlexOptionsDict
+            case sp:
+                raise NotImplementedError(f"No result dict type for {sp}")
+
 
 EntityEnumType = TypeVar("EntityEnumType", bound=EntitiesEnum)
 
 
 class SystemParticipantsEnum(EntitiesEnum):
     BIOMASS_PLANT = "bm"
     COMBINED_HEAT_AND_POWER = "chp"
@@ -79,15 +138,15 @@
     HEAT_PUMP = "hp"
     FLEX_OPTIONS = "flex_options"
     PRIMARY_DATA = "primary_data"
     PARTICIPANTS_SUM = "participants_sum"
 
     @staticmethod
     def values():
-        return [participant for participant in SystemParticipantsEnum]
+        return [participant for participant in EntitiesEnum]
 
     def has_soc(self):
         return self in {
             SystemParticipantsEnum.ELECTRIC_VEHICLE,
             SystemParticipantsEnum.STORAGE,
         }
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/connector/connector.py` & `pypsdm-0.0.3/pypsdm/models/input/connector/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pypsdm.models.input.node import Nodes
 
 ConnectorType = TypeVar("ConnectorType", bound="Connector")
 
 
 @dataclass(frozen=True)
 class Connector(Entities, ABC):
-
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @property
     def node_a(self):
         return self.data["node_a"]
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/connector/switches.py` & `pypsdm-0.0.3/pypsdm/models/input/connector/switches.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from pypsdm.models.enums import EntitiesEnum, RawGridElementsEnum
 from pypsdm.models.input.connector.connector import Connector
 
 
 @dataclass(frozen=True)
 class Switches(Connector):
-
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @property
     def closed(self):
         return self.data["closed"]
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/connector/transformer.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/evcs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,76 @@
 from dataclasses import dataclass
+from enum import Enum
+from string import Template
 
-from pypsdm.models.enums import RawGridElementsEnum
-from pypsdm.models.input.connector.connector import Connector
-from pypsdm.models.input.mixins import HasTypeMixin
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
+from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
-class Transformers2W(HasTypeMixin, Connector):
+class EvChargingStations(SystemParticipants):
     def __eq__(self, other: object) -> bool:
-        return Connector.__eq__(self, other)
+        return super().__eq__(other)
 
-    @property
-    def type_id(self):
-        return self.data["type_id"]
-
-    @property
-    def tap_pos(self):
-        return self.data["tap_pos"]
-
-    @property
-    def auto_tap(self):
-        return self.data["auto_tap"]
-
-    @property
-    def r_sc(self):
-        return self.data["r_sc"]
-
-    @property
-    def x_sc(self):
-        return self.data["x_sc"]
-
-    @property
-    def g_m(self):
-        return self.data["g_m"]
-
-    @property
-    def b_m(self):
-        return self.data["b_m"]
-
-    @property
-    def s_rated(self):
-        return self.data["s_rated"]
-
-    @property
-    def v_rated_a(self):
-        return self.data["v_rated_a"]
-
-    @property
-    def v_rated_b(self):
-        return self.data["v_rated_b"]
+    @staticmethod
+    def get_enum() -> EntitiesEnum:
+        return SystemParticipantsEnum.EV_CHARGING_STATION
 
     @property
-    def d_v(self):
-        return self.data["d_v"]
+    def charging_points(self):
+        return self.data["charging_points"]
 
     @property
-    def d_phi(self):
-        return self.data["d_phi"]
+    def location_type(self):
+        return self.data["location_type"]
 
     @property
-    def tap_side(self):
-        return self.data["tap_side"]
+    def electric_current_type(self):
+        return self.data["type"]
 
     @property
-    def tap_neutr(self):
-        return self.data["tap_neutr"]
+    def v2g_support(self):
+        return self.data["v2g_support"]
 
     @property
-    def tap_min(self):
-        return self.data["tap_min"]
+    def cos_phi_rated(self):
+        return self.data["cos_phi_rated"]
 
-    @property
-    def tap_max(self):
-        return self.data["tap_max"]
+    def get_public_evcs(self):
+        return self.data[
+            self.location_type.isin(
+                [EvcsLocationType.CUSTOMER_PARKING.value, EvcsLocationType.WORK.value]
+            )
+        ]
 
-    @staticmethod
-    def get_enum() -> RawGridElementsEnum:
-        return RawGridElementsEnum.TRANSFORMER_2_W
+    def get_home_evcs(self):
+        return self.data[self.location_type.isin([EvcsLocationType.HOME.value])]
 
     @staticmethod
-    def entity_attributes() -> list[str]:
-        return Connector.attributes() + [
-            "tap_pos",
-            "auto_tap",
+    def attributes() -> list[str]:
+        return SystemParticipants.attributes() + [
+            "charging_points",
+            "location_type",
+            "type",
+            "v2g_support",
+            "cos_phi_rated",
         ]
 
     @staticmethod
-    def type_attributes() -> list[str]:
-        return HasTypeMixin.type_attributes() + [
-            "r_sc",
-            "x_sc",
-            "g_m",
-            "b_m",
-            "s_rated",
-            "v_rated_a",
-            "v_rated_b",
-            "d_v",
-            "d_phi",
-            "tap_side",
-            "tap_neutr",
-            "tap_min",
-            "tap_max",
+    def additional_attributes() -> list[str]:
+        return SystemParticipants.additional_attributes() + [
+            "power",
+            "current_type",
+            "synonymous_ids",
         ]
+
+
+class EvcsLocationType(Enum):
+    HOME = "HOME"
+    WORK = "WORK"
+    CUSTOMER_PARKING = "CUSTOMER_PARKING"
+    STREET = "STREET"
+    CHARGING_HUB_TOWN = "CHARGING_HUB_TOWN"
+    CHARGING_HUB_HIGHWAY = "CHARGING_HUB_HIGHWAY"
+
+
+evcs_type = Template("$id($s_rated|$current_type)")
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/container/grid.py` & `pypsdm-0.0.3/pypsdm/models/input/container/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
+from pypsdm.models.enums import (
+    EntitiesEnum,
+    RawGridElementsEnum,
+    SystemParticipantsEnum,
+)
 from pypsdm.models.input.container.mixins import ContainerMixin
 from pypsdm.models.input.container.participants import SystemParticipantsContainer
 from pypsdm.models.input.container.raw_grid import RawGridContainer
+from pypsdm.models.ts.types import ComplexPower
 
 if TYPE_CHECKING:
     from pypsdm.models.primary_data import PrimaryData
 
 
 @dataclass(frozen=True)
 class GridContainer(ContainerMixin):
@@ -91,25 +97,23 @@
             [self.raw_grid, self.participants, self.primary_data]
             if include_primary_data
             else [self.raw_grid, self.participants]
         )
         return grid if include_empty else [g for g in grid if g]
 
     def get_nodal_primary_data(self):
-        from pypsdm.models.result.power import PQResult
-
         time_series = []
         nodal_primary_data = dict()
         for node, participants_container in self.node_participants_map.items():
             participants_uuids = participants_container.uuids().tolist()
             node_primary_data = self.primary_data.get_for_participants(
                 participants_uuids
             )
             time_series.extend(node_primary_data)
-            node_primary_data_agg = PQResult.sum(node_primary_data)
+            node_primary_data_agg = ComplexPower.sum(node_primary_data)
             nodal_primary_data[node] = node_primary_data_agg
         return nodal_primary_data
 
     def get_nodal_sp_count_and_power(self):
         data = {}
         for node_uuid, sps in self.node_participants_map.items():
             nodal_data = {}
@@ -121,14 +125,21 @@
                 if hasattr(sp, "s_rated"):
                     s_rated = round(sp.s_rated.sum(), 2)
                     data_str += f", Rated Power: {s_rated} kw"
                 nodal_data[sp_id] = data_str
             data[node_uuid] = nodal_data
         return data
 
+    def get_with_enum(self, enum: EntitiesEnum):
+        if isinstance(enum, RawGridElementsEnum):
+            return self.raw_grid.get_with_enum(enum)
+        if isinstance(enum, SystemParticipantsEnum):
+            return self.participants.get_with_enum(enum)
+        raise ValueError(f"Unretrievable enum {enum}")
+
     def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
         return GridContainer(
             raw_grid=self.raw_grid,
             participants=self.participants,
             primary_data=self.primary_data.filter_by_date_time(time),
             node_participants_map=self.node_participants_map,
         )
@@ -175,16 +186,16 @@
         raw_grid = RawGridContainer.from_csv(path, delimiter)
         participants = SystemParticipantsContainer.from_csv(path, delimiter)
         node_participants_map = participants.build_node_participants_map(raw_grid.nodes)
         primary_data = PrimaryData.from_csv(path, primary_data_delimiter)
         return cls(raw_grid, participants, primary_data, node_participants_map)
 
     @classmethod
-    def create_empty(cls):
+    def empty(cls):
         from pypsdm.models.primary_data import PrimaryData
 
         return cls(
-            raw_grid=RawGridContainer.create_empty(),
-            participants=SystemParticipantsContainer.create_empty(),
+            raw_grid=RawGridContainer.empty(),
+            participants=SystemParticipantsContainer.empty(),
             primary_data=PrimaryData.create_empty(),
             node_participants_map=dict(),
         )
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/container/participants.py` & `pypsdm-0.0.3/pypsdm/models/input/container/participants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Union
 
 import pandas as pd
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.container.mixins import ContainerMixin
 from pypsdm.models.input.node import Nodes
 from pypsdm.models.input.participant.bm import BiomassPlants
 from pypsdm.models.input.participant.em import EnergyManagementSystems
 from pypsdm.models.input.participant.evcs import EvChargingStations
 from pypsdm.models.input.participant.evs import ElectricVehicles
 from pypsdm.models.input.participant.fixed_feed_in import FixedFeedIns
@@ -76,15 +76,15 @@
             wecs,
             storages,
             evs,
             evcs,
             hps,
         )
 
-    def get_participants(self, sp_type: SystemParticipantsEnum):
+    def get_with_enum(self, sp_type: EntitiesEnum):
         if sp_type == SystemParticipantsEnum.ENERGY_MANAGEMENT:
             return self.ems
         elif sp_type == SystemParticipantsEnum.LOAD:
             return self.loads
         elif sp_type == SystemParticipantsEnum.BIOMASS_PLANT:
             return self.biomass_plants
         elif sp_type == SystemParticipantsEnum.FIXED_FEED_IN:
@@ -149,39 +149,66 @@
             self.hps.subset(uuids, intersection=True),
         )
 
     @staticmethod
     def from_csv(
         path: str, delimiter: str | None = None
     ) -> "SystemParticipantsContainer":
-        loads = Loads.from_csv(path, delimiter)
-        fixed_feed_ins = FixedFeedIns.from_csv(path, delimiter)
-        pvs = PhotovoltaicPowerPlants.from_csv(path, delimiter)
-        biomass_plants = BiomassPlants.from_csv(path, delimiter)
-        wecs = WindEnergyConverters.from_csv(path, delimiter)
-        storages = Storages.from_csv(path, delimiter)
-        ems = EnergyManagementSystems.from_csv(path, delimiter)
-        evs = ElectricVehicles.from_csv(path, delimiter)
-        evcs = EvChargingStations.from_csv(path, delimiter)
-        hps = HeatPumps.from_csv(path, delimiter)
+        loads = Loads.from_csv(path, delimiter, must_exist=False)
+        fixed_feed_ins = FixedFeedIns.from_csv(path, delimiter, must_exist=False)
+        pvs = PhotovoltaicPowerPlants.from_csv(path, delimiter, must_exist=False)
+        biomass_plants = BiomassPlants.from_csv(path, delimiter, must_exist=False)
+        wecs = WindEnergyConverters.from_csv(path, delimiter, must_exist=False)
+        storages = Storages.from_csv(path, delimiter, must_exist=False)
+        ems = EnergyManagementSystems.from_csv(path, delimiter, must_exist=False)
+        evs = ElectricVehicles.from_csv(path, delimiter, must_exist=False)
+        evcs = EvChargingStations.from_csv(path, delimiter, must_exist=False)
+        hps = HeatPumps.from_csv(path, delimiter, must_exist=False)
         return SystemParticipantsContainer(
             ems,
             loads,
             fixed_feed_ins,
             pvs,
             biomass_plants,
             wecs,
             storages,
             evs,
             evcs,
             hps,
         )
 
     @classmethod
-    def create_empty(cls):
+    def create(
+        cls,
+        ems=EnergyManagementSystems.create_empty(),
+        loads=Loads.create_empty(),
+        fixed_feed_ins=FixedFeedIns.create_empty(),
+        pvs=PhotovoltaicPowerPlants.create_empty(),
+        bms=BiomassPlants.create_empty(),
+        wecs=WindEnergyConverters.create_empty(),
+        storages=Storages.create_empty(),
+        evs=ElectricVehicles.create_empty(),
+        evcs=EvChargingStations.create_empty(),
+        hps=HeatPumps.create_empty(),
+    ):
+        return cls(
+            ems=ems,
+            loads=loads,
+            fixed_feed_ins=fixed_feed_ins,
+            pvs=pvs,
+            biomass_plants=bms,
+            wecs=wecs,
+            storages=storages,
+            evs=evs,
+            evcs=evcs,
+            hps=hps,
+        )
+
+    @classmethod
+    def empty(cls):
         return cls(
             EnergyManagementSystems.create_empty(),
             Loads.create_empty(),
             FixedFeedIns.create_empty(),
             PhotovoltaicPowerPlants.create_empty(),
             BiomassPlants.create_empty(),
             WindEnergyConverters.create_empty(),
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/container/raw_grid.py` & `pypsdm-0.0.3/pypsdm/models/input/container/raw_grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from typing import Union
 
 from networkx import Graph
 
+from pypsdm.models.enums import RawGridElementsEnum
 from pypsdm.models.input.connector.lines import Lines
 from pypsdm.models.input.connector.switches import Switches
 from pypsdm.models.input.connector.transformer import Transformers2W
 from pypsdm.models.input.container.mixins import ContainerMixin
 from pypsdm.models.input.entity import Entities
 from pypsdm.models.input.node import Nodes
 
@@ -62,14 +63,27 @@
         graph = self.build_networkx_graph()
         branches = self._find_branches(graph, slack_connected_node)
         branches = [[slack_connected_node] + branch for branch in branches]
         if as_graphs:
             return [graph.subgraph(branch).copy() for branch in branches]
         return branches
 
+    def get_with_enum(self, enum: RawGridElementsEnum):
+        match enum:
+            case RawGridElementsEnum.NODE:
+                return self.nodes
+            case RawGridElementsEnum.LINE:
+                return self.lines
+            case RawGridElementsEnum.TRANSFORMER_2_W:
+                return self.transformers_2_w
+            case RawGridElementsEnum.SWITCH:
+                return self.switches
+            case _:
+                raise ValueError(f"Unknown enum {enum}")
+
     def build_networkx_graph(self, include_transformer: bool = False) -> Graph:
         graph = Graph()
         closed_switches = self.switches.get_closed()
         line_data_dicts = self.lines.data.apply(
             lambda row: {"weight": row["length"]}, axis=1
         )
 
@@ -86,14 +100,20 @@
         return RawGridContainer(
             self.nodes.filter_by_nodes(nodes),
             self.lines.filter_by_nodes(nodes, both_in_nodes=True),
             self.transformers_2_w.filter_by_nodes(nodes, both_in_nodes=False),
             self.switches.filter_by_nodes(nodes, both_in_nodes=True),
         )
 
+    def admittance_matrix(self, uuid_to_idx: dict):
+        """TODO: `parallelDevices` not yet considered."""
+        lines_admittance = self.lines.admittance_matrix(uuid_to_idx)
+        transformers_admittance = self.transformers_2_w.admittance_matrix(uuid_to_idx)
+        return lines_admittance + transformers_admittance
+
     @staticmethod
     def _find_branches(G: Graph, start_node):
         visited = set()
         visited.add(start_node)
         branches = []
 
         def dfs(node, path):
@@ -111,25 +131,25 @@
                 branches.append(path)
 
         return branches
 
     @classmethod
     def from_csv(cls, path: str, delimiter: str | None = None) -> "RawGridContainer":
         nodes = Nodes.from_csv(path, delimiter)
-        lines = Lines.from_csv(path, delimiter)
-        transformers_2_w = Transformers2W.from_csv(path, delimiter)
-        switches = Switches.from_csv(path, delimiter)
+        lines = Lines.from_csv(path, delimiter, must_exist=False)
+        transformers_2_w = Transformers2W.from_csv(path, delimiter, must_exist=False)
+        switches = Switches.from_csv(path, delimiter, must_exist=False)
         return cls(
             nodes=nodes,
             lines=lines,
             transformers_2_w=transformers_2_w,
             switches=switches,
         )
 
     @classmethod
-    def create_empty(cls):
+    def empty(cls):
         return cls(
             nodes=Nodes.create_empty(),
             lines=Lines.create_empty(),
             transformers_2_w=Transformers2W.create_empty(),
             switches=Switches.create_empty(),
         )
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/create/participants.py` & `pypsdm-0.0.3/pypsdm/models/input/create/participants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import random
 from uuid import uuid4
 
 import pandas as pd
 
-from pypsdm.models.enums import ElectricCurrentType, SystemParticipantsEnum
+from pypsdm.models.enums import ElectricCurrentType, EntitiesEnum
 from pypsdm.models.input.create.utils import create_data
 from pypsdm.models.input.participant import evcs
 from pypsdm.models.input.participant.em import EnergyManagementSystems
 from pypsdm.models.input.participant.evcs import EvChargingStations
 from pypsdm.models.input.participant.evs import ElectricVehicles
+from pypsdm.models.input.participant.fixed_feed_in import FixedFeedIns
 from pypsdm.models.input.participant.hp import HeatPumps
 from pypsdm.models.input.participant.load import Loads
 from pypsdm.models.input.participant.pv import PhotovoltaicPowerPlants
 from pypsdm.models.input.participant.storage import Storages
 
 
 def fixed_q_characteristics(cos_phi):
@@ -61,14 +63,31 @@
             "k_t": k_t,
             "market_reaction": market_reaction,
             "cos_phi_rated": cos_phi_rated,
         }
     ).rename(uuid)
 
 
+def sample_azimuth():
+    # Values from BW Speichermonitoring study
+    x = random.random()
+    if 0 <= x < 0.38:
+        return 0
+    elif 0.38 <= x < 0.5:
+        return 90
+    elif 0.5 <= x < 0.62:
+        return -90
+    elif 0.62 <= x < 0.81:
+        return 45
+    elif 0.81 <= x < 0.95:
+        return -45
+    else:
+        return sample_azimuth()
+
+
 def create_storages(data_dict):
     return Storages(create_data(data_dict, create_storages_data))
 
 
 def create_storages_data(
     id,
     node,
@@ -177,15 +196,15 @@
 
 
 def create_ev_charging_stations(data_dict):
     return EvChargingStations(
         create_data(
             data_dict,
             create_ev_charging_stations_data,
-            entity_preprocessing=SystemParticipantsEnum.EV_CHARGING_STATION,
+            entity_preprocessing=EntitiesEnum.EV_CHARGING_STATION,
         )
     )
 
 
 def create_ev_charging_stations_data(
     id,
     node,
@@ -347,7 +366,40 @@
     ).rename(uuid)
 
 
 def create_energy_management_systems(data_dict):
     return EnergyManagementSystems(
         create_data(data_dict, create_energy_management_systems_data)
     )
+
+
+def create_fixed_feed_ins(data_dict):
+    return FixedFeedIns(create_data(data_dict, create_fixed_feed_in_data))
+
+
+def create_fixed_feed_in_data(
+    id,
+    node,
+    s_rated,
+    cos_phi_rated,
+    q_characteristics=None,
+    uuid=None,
+    operates_from=None,
+    operates_until=None,
+    operator=None,
+):
+    if not uuid:
+        uuid = str(uuid4())
+    if not q_characteristics:
+        q_characteristics = fixed_q_characteristics(0.9)
+    return pd.Series(
+        {
+            "id": id,
+            "node": node,
+            "s_rated": s_rated,
+            "cos_phi_rated": cos_phi_rated,
+            "q_characteristics": q_characteristics,
+            "operates_from": operates_from,
+            "operates_until": operates_until,
+            "operator": operator,
+        }
+    ).rename(uuid)
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/create/poi.py` & `pypsdm-0.0.3/pypsdm/models/input/create/poi.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/create/thermal.py` & `pypsdm-0.0.3/pypsdm/models/input/create/thermal.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/create/utils.py` & `pypsdm-0.0.3/pypsdm/models/input/create/utils.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/entity.py` & `pypsdm-0.0.3/pypsdm/models/input/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import copy
 import json
-import logging
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, replace
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Self, Tuple, Type, TypeVar, Union
 
 import pandas as pd
+from loguru import logger
 from pandas import DataFrame, Series
 
 from pypsdm.errors import ComparisonError
 from pypsdm.io import utils
 from pypsdm.io.utils import bool_converter, df_to_csv, read_csv
 from pypsdm.models.enums import (
     EntitiesEnum,
     RawGridElementsEnum,
     SystemParticipantsEnum,
 )
+from pypsdm.models.ts.base import EntityKey
 from pypsdm.processing.dataframe import compare_dfs
 
 if TYPE_CHECKING:
     from pypsdm.models.input.node import Nodes
 
 pd.set_option("mode.copy_on_write", True)
 EntityType = TypeVar("EntityType", bound="Entities")
@@ -75,15 +76,15 @@
         if not isinstance(other, type(self)):
             raise TypeError(
                 f"The two Entities instances must be of the same type. Received {type(self)} and {type(other)}"
             )
 
         columns_diff = set(self.data.columns).symmetric_difference(other.data.columns)
         if len(columns_diff) > 0 and columns_diff.issubset(self.attributes()):
-            logging.warning(
+            logger.warning(
                 "The two Entities instances have different columns: %s", columns_diff
             )
         return type(self)(pd.concat([self.data, other.data]))
 
     def __sub__(self: EntityType, other: Union[EntityType, List[str]]) -> EntityType:
         """
         Subtacts the entities with the given uuids from the Entities instance.
@@ -105,14 +106,27 @@
         if not set(indices_to_remove).issubset(self.data.index):
             raise ValueError(
                 f"All indices to remove must exist in the current Entities instance: {set(indices_to_remove) - set(self.data.index)}"
             )
 
         return type(self)(self.data.drop(indices_to_remove))
 
+    def __getitem__(self, get: str) -> pd.Series:
+        try:
+            return self.data.loc[get]
+        except KeyError:
+            subset = self.subset_id(get)
+            if len(subset) == 1:
+                return subset.data.iloc[0]
+            if len(subset) > 1:
+                raise KeyError(
+                    "Multiple entities with the same id found. Please use the uuids instead."
+                )
+            raise KeyError(f"Entity with id {get} not found.")
+
     @property
     def uuid(self) -> Series:
         """
         Returns: The uuids of the entities.
         """
         return self.data.index.to_series()
 
@@ -146,15 +160,14 @@
 
     @property
     @abstractmethod
     def node(self) -> Series:
         """
         Returns: The nodes to which the entities are connected.
         """
-        pass
 
     def get(self, uuid: str) -> Series:
         """
         Returns the entity information of the entitiy with the given uuid.
 
         Args:
             uuid: The uuid of the entity.
@@ -162,33 +175,33 @@
         Returns:
             Row (Series) of the corresponding entity information.
         """
         return self.data.loc[uuid]
 
     def subset(
         self: EntityType,
-        uuids: Union[list[str], Series, set[str], str],
+        uuids,
         intersection: bool = False,
     ) -> EntityType:
         """
         Creates a subset of the Entities instance with the given uuids. By default it expects all uuids to be
         contained within the Entities. If intersection is set to True, it returns the Entities subset of uuids which are
         present in the Entities instance.
 
         Args:
             uuids: The uuids to subset.
 
         Returns:
             A new instance with the subset of entities.
         """
-        if isinstance(uuids, str):
+        if isinstance(uuids, str | EntityKey):
             uuids = [uuids]
         if intersection:
-            intersection = list(set(self.uuid) & set(uuids))
-            return type(self)(self.data.loc[intersection])
+            keys = list(set(self.uuid) & set(uuids))
+            return type(self)(self.data.loc[keys])
         if isinstance(uuids, set):
             uuids = list(uuids)
         try:
             return type(self)(self.data.loc[uuids])
         except KeyError as e:
             not_found = set(uuids) - set(self.data.index)
             raise KeyError(
@@ -263,15 +276,15 @@
         if isinstance(self, HasTypeMixin):
             HasTypeMixin.to_csv(self, path, mkdirs, delimiter)
         else:
             if self.additional_attributes():
                 additional_attributes = set(self.additional_attributes())
                 additional_not_in_data = additional_attributes - set(data.columns)
                 if additional_not_in_data:
-                    logging.warning(
+                    logger.warning(
                         f"The following additional attributese were not found in the data: \n"
                         f"{additional_not_in_data}.\n"
                         "This might be due to not using the Entities.preprocessing() method "
                         "when building the data."
                     )
                     additional_attributes = (
                         additional_attributes - additional_not_in_data
@@ -325,57 +338,63 @@
         Returns:
             The copy of the current Entities instance.
         """
         to_copy = copy.deepcopy(self) if deep else self
         return replace(to_copy, **changes)
 
     @classmethod
-    def from_csv(cls: Type[Self], path: str, delimiter: str | None = None) -> Self:
+    def from_csv(
+        cls: Type[Self],
+        path: str,
+        delimiter: str | None = None,
+        must_exist: bool = True,
+    ) -> Self:
         """
         Reads the entity data from a csv file.
 
         Args:
             path: The path to the csv file.
             delimiter: The delimiter of the csv file.
+            must_exist: Wether or not exception is thrown if file does not exist.
 
         Returns:
            The corresponding entities object.
         """
-        return cls._from_csv(path, cls.get_enum(), delimiter)
+        return cls._from_csv(path, cls.get_enum(), delimiter, must_exist)
 
     @classmethod
     def _from_csv(
-        cls: Type[Self], path: str, entity: EntitiesEnum, delimiter: str | None = None
+        cls: Type[Self],
+        path: str,
+        entity: EntitiesEnum,
+        delimiter: str | None = None,
+        must_exist: bool = True,
     ) -> Self:
         file_path = utils.get_file_path(path, entity.get_csv_input_file_name())
         if os.path.exists(file_path):
             return cls(Entities._data_from_csv(entity, path, delimiter))
         else:
-            logging.debug(
-                "There is no file named: "
-                + str(file_path)
-                + ". No "
-                + entity.value
-                + " entities are loaded."
-            )
-            return cls.create_empty()
+            if must_exist:
+                raise FileNotFoundError(f"File {file_path} does not exist.")
+            else:
+                return cls.create_empty()
 
     @classmethod
     def _data_from_csv(
         cls, entity: EntitiesEnum, path: str | Path, delimiter: str | None = None
     ) -> DataFrame:
         data = read_csv(path, entity.get_csv_input_file_name(), delimiter)
 
         bool_cols = cls.bool_attributes()
         for col in bool_cols:
             try:
                 data[col] = data[col].apply(lambda x: bool_converter(x))
                 data[col] = data[col].astype(bool)
             except ValueError as e:
-                logging.error(
+                logger.error(
                     f"Could not convert column {col} to bool. "
                     f"Please check the values in the csv file. "
                     f"Error: {e}"
                 )
 
         if entity.has_type():
             # TODO: Capture nonexistent type
@@ -397,15 +416,15 @@
                 "Column 'uuid' not found. This might be due to wrong csv delimiter!", e
             )
 
     @staticmethod
     def preprocessing(entity: EntitiesEnum, data: DataFrame) -> DataFrame:
         """
         We perform some data transformations on the data wich make them easier to handle.
-        Additional columns we add are droppen when persisting the data.
+        Additional columns we add are dropped when persisting the data.
         """
 
         # special data transformations
         match entity:
             # for raw grid elements
             # ---------------------
             case RawGridElementsEnum.NODE:
@@ -443,15 +462,14 @@
 
     @staticmethod
     @abstractmethod
     def get_enum() -> EntitiesEnum:
         """
         Returns the corresponding entity enum value.
         """
-        pass
 
     @classmethod
     def attributes(cls) -> list[str]:
         """
         Method that should hold all attributes field (transformed to snake_case and case-sensitive)
         of the corresponding PSDM entity
         :return:
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/mixins.py` & `pypsdm-0.0.3/pypsdm/models/input/mixins.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/node.py` & `pypsdm-0.0.3/pypsdm/models/input/node.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/__init__.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/bm.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/bm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.mixins import SpTypeMixin
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class BiomassPlants(SpTypeMixin, SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.BIOMASS_PLANT
 
     @property
     def market_reaction(self):
         return self.data["market_reaction"]
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/charging.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/charging.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/em.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/wec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from dataclasses import dataclass
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
+from pypsdm.models.input.participant.mixins import SpTypeMixin
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
-class EnergyManagementSystems(SystemParticipants):
+class WindEnergyConverters(SpTypeMixin, SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
-        return SystemParticipantsEnum.ENERGY_MANAGEMENT
+    def get_enum() -> EntitiesEnum:
+        return SystemParticipantsEnum.WIND_ENERGY_CONVERTER
 
     @property
-    def connected_assets(self):
-        return self.data["connected_assets"]
+    def market_reaction(self):
+        return self.data["market_reaction"]
 
     @property
-    def control_strategy(self):
-        return self.data["control_strategy"]
+    def eta_conv(self):
+        return self.data["eta_conv"]
 
-    def uuid_to_connected_assets(self):
-        return self.connected_assets.to_dict()
+    @property
+    def rotor_area(self):
+        return self.data["rotor_area"]
+
+    @property
+    def hub_height(self):
+        return self.data["hub_height"]
+
+    @staticmethod
+    def entity_attributes() -> list[str]:
+        return SystemParticipants.attributes() + ["market_reaction"]
 
     @staticmethod
-    def attributes():
-        return SystemParticipants.attributes() + [
-            "connected_assets",
-            "control_strategy",
+    def type_attributes() -> list[str]:
+        return SpTypeMixin.type_attributes() + [
+            "cp_characteristic",
+            "eta_conv",
+            "rotor_area",
+            "hub_height",
         ]
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/evs.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/evs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.mixins import SpTypeMixin
 from pypsdm.models.input.participant.participant import SystemParticipantsWithCapacity
 
 
 @dataclass(frozen=True)
 class ElectricVehicles(SpTypeMixin, SystemParticipantsWithCapacity):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.ELECTRIC_VEHICLE
 
     @staticmethod
     def capacity_attribute() -> str:
         return "e_storage"
 
     @property
@@ -29,10 +29,11 @@
     @staticmethod
     def entity_attributes() -> list[str]:
         return SystemParticipantsWithCapacity.attributes()
 
     @staticmethod
     def type_attributes() -> list[str]:
         return SpTypeMixin.type_attributes() + [
+            "s_rated_dc",
             "e_storage",
             "e_cons",
         ]
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/fixed_feed_in.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/fixed_feed_in.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class FixedFeedIns(SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.FIXED_FEED_IN
 
     @property
     def s_rated(self):
         return self.data["s_rated"]
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/hp.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/hp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.mixins import SpTypeMixin
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class HeatPumps(SpTypeMixin, SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.HEAT_PUMP
 
     @property
     def thermal_bus(self):
         return self.data["thermal_bus"]
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/load.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 from typing import List
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class Loads(SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.LOAD
 
     @property
     def s_rated(self):
         return self.data["s_rated"]
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/mixins.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/mixins.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/participant.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,25 @@
     def insert_node_id_columns(self, nodes: Nodes) -> None:
         index_to_id = nodes.id.to_dict()
 
         if "node_id" not in self.data.columns:
             self.data.insert(self.data.columns.get_loc("node") + 1, "node_id", None)
         self.data["node_id"] = self.node.map(index_to_id)
 
-    @staticmethod
-    def attributes():
+    @classmethod
+    def attributes(cls):
         return Entities.attributes() + ["node", "q_characteristics"]
 
 
 @dataclass(frozen=True)
 class SystemParticipantsWithCapacity(SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
+    @property
     def capacity(self):
         return self.data[self.capacity_attribute()]
 
     @staticmethod
     @abstractmethod
     def capacity_attribute() -> str:
         raise NotImplementedError
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/pv.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/pv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 from typing import List
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.participant import SystemParticipants
 
 
 @dataclass(frozen=True)
 class PhotovoltaicPowerPlants(SystemParticipants):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT
 
     @property
     def s_rated(self):
         return self.data["s_rated"]
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/participant/storage.py` & `pypsdm-0.0.3/pypsdm/models/input/participant/storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pandas import Series
 
-from pypsdm.models.enums import SystemParticipantsEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.participant.mixins import SpTypeMixin
 from pypsdm.models.input.participant.participant import SystemParticipantsWithCapacity
 
 
 class Storages(SpTypeMixin, SystemParticipantsWithCapacity):
     def __eq__(self, other: object) -> bool:
         return SystemParticipantsWithCapacity.__eq__(self, other)
 
     @staticmethod
-    def get_enum() -> SystemParticipantsEnum:
+    def get_enum() -> EntitiesEnum:
         return SystemParticipantsEnum.STORAGE
 
     @staticmethod
     def capacity_attribute() -> str:
         return "e_storage"
 
     @property
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/thermal/grid.py` & `pypsdm-0.0.3/pypsdm/models/input/thermal/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     @classmethod
     def from_csv(cls, path: str, delimiter: str):
         busses = ThermalBus.from_csv(path, delimiter)
         houses = ThermalHouse.from_csv(path, delimiter)
         return cls(busses, houses)
 
     @classmethod
-    def create_empty(cls):
+    def empty(cls):
         return cls(ThermalBus.create_empty(), ThermalHouse.create_empty())
```

### Comparing `pypsdm-0.0.2/pypsdm/models/input/thermal/house.py` & `pypsdm-0.0.3/pypsdm/models/input/thermal/house.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/models/primary_data.py` & `pypsdm-0.0.3/pypsdm/models/primary_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,154 @@
 import concurrent.futures
 import copy
-import logging
 import os
 import re
 import uuid
 from dataclasses import dataclass
 from datetime import datetime
 from functools import partial
 from pathlib import Path
 from typing import Union
 
 import pandas as pd
+from loguru import logger
 from pandas import Series
 
 from pypsdm.errors import ComparisonError
 from pypsdm.io import utils
 from pypsdm.io.utils import df_to_csv, to_date_time
-from pypsdm.models.enums import SystemParticipantsEnum, TimeSeriesEnum
-from pypsdm.models.result.participant.pq_dict import PQResultDict
-from pypsdm.models.result.power import PQResult
+from pypsdm.models.enums import TimeSeriesEnum
+from pypsdm.models.ts.types import ComplexPower, ComplexPowerDict
+
+
+@dataclass(frozen=True)
+class TimeSeriesKey:
+    ts_uuid: str
+    ts_type: TimeSeriesEnum | None
+
+    def __eq__(self, other):
+        return self.ts_uuid == other.ts_uuid
+
+    def __hash__(self):
+        return hash(self.ts_uuid)
 
 
 @dataclass
 class PrimaryData:
     # ts_uuid -> ts
-    time_series: "PQResultDict"
+    time_series: ComplexPowerDict[TimeSeriesKey]
     # participant_uuid -> ts_uuid
     participant_mapping: dict[str, str]
 
+    def __init__(
+        self, time_series: "ComplexPowerDict", participant_mapping: dict[str, str]
+    ):
+        self.time_series = time_series
+        self.participant_mapping = participant_mapping
+
     def __eq__(self, other):
         try:
             self.compare(other)
             return True
         except ComparisonError:
             return False
 
     def __len__(self):
         return len(self.time_series)
 
     def __contains__(self, uuid):
         return uuid in self.time_series or uuid in self.participant_mapping
 
-    def __getitem__(self, get):
+    def __getitem__(self, get: str | TimeSeriesKey) -> ComplexPower:
         match get:
             case str():
+                get_key = TimeSeriesKey(get, None)
                 if get in self.participant_mapping:
-                    return self.time_series[self.participant_mapping[get]]
-                elif get in self.time_series:
-                    return self.time_series[get]
+                    ts_uuid = self.participant_mapping[get]
+                    key = TimeSeriesKey(ts_uuid, None)
+                    return self.time_series[key]
+                elif get_key in self.time_series:
+                    return self.time_series[get_key]
                 else:
                     raise KeyError(
                         f"{get} neither a valid time series nor a participant uuid."
                     )
-            case slice():
-                start, stop, step = get.start, get.stop, get.step
-                if step is not None:
-                    logging.warning("Step is not supported for slicing. Ignoring it.")
-                if not (isinstance(start, datetime) and isinstance(stop, datetime)):
-                    raise ValueError("Only datetime slicing is supported")
-                return self.filter_for_time_interval(start, stop)
+            case TimeSeriesKey():
+                return self.time_series[get]
             case _:
                 raise ValueError(
-                    "Only get by uuid or datetime slice for filtering is supported."
+                    "Only str uuid of either time series or participant or TimeSeriesKey of time series are allowed as key for PrimaryData."
                 )
 
-    @property
-    def p(self):
-        return self.time_series.p
-
-    @property
-    def q(self):
-        return self.time_series.q
+    def p(self, ffill=True):
+        return self.time_series.p(ffill)
+
+    def q(self, ffill=True):
+        return self.time_series.q(ffill)
 
     def p_sum(self) -> Series:
         return self.time_series.p_sum()
 
     def q_sum(self):
         return self.time_series.q_sum()
 
-    def sum(self) -> PQResult:
+    def sum(self) -> ComplexPower:
         return self.time_series.sum()
 
-    def get_for_participants(self, participants) -> list[PQResult]:
+    def get_for_participants(self, participants) -> list[ComplexPower]:
         time_series = []
         for participant in participants:
             ts = self.get_for_participant(participant)
             if ts:
                 time_series.append(ts)
         return time_series
 
     def filter_by_participants(
         self, participants: list[str], skip_missing: bool = False
     ):
         if skip_missing:
             participants = [p for p in participants if p in self.participant_mapping]
         try:
             pm = {p: self.participant_mapping[p] for p in participants}
-            ts = {ts_uuid: self.time_series[ts_uuid] for ts_uuid in pm.values()}
+            ts = ComplexPowerDict({ts_uuid: self[ts_uuid] for ts_uuid in pm.values()})  # type: ignore
             return PrimaryData(ts, pm)
         except KeyError as e:
             missing_key = e.args[0]
             raise KeyError(
                 f"Participant with uuid: {missing_key} has no associated primary data."
             ) from e
 
-    def get_for_participant(self, participant: str) -> PQResult | None:
+    def get_for_participant(self, participant: str) -> ComplexPower | None:
         ts_uuid = self.participant_mapping.get(participant)
         if ts_uuid:
-            return self.time_series.entities[ts_uuid]
+            return self[ts_uuid]  # type: ignore
         else:
             return None
 
     def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
-        """
-        Filters the result by the given datetime or list of datetimes.
-        :param time: the time or list of times to filter by
-        :return: a new result containing only the given time or times
-        """
         ts = self.time_series.filter_by_date_time(time)
         return PrimaryData(ts, self.participant_mapping)
 
-    def filter_for_time_interval(self, start: datetime, end: datetime):
-        ts = self.time_series.filter_for_time_interval(start, end)
+    def interval(self, start: datetime, end: datetime):
+        ts = self.time_series.interval(start, end)
         return PrimaryData(ts, self.participant_mapping)
 
     def to_csv(self, path: str, mkdirs=False, delimiter=","):
         write_ts = partial(PrimaryData._write_ts_df, path, mkdirs, delimiter)
+
         with concurrent.futures.ProcessPoolExecutor() as executor:
-            executor.map(write_ts, list(self.time_series.entities.values()))
+            futures = [
+                executor.submit(write_ts, ts, key)
+                for key, ts in list(self.time_series.items())
+            ]
+
+            for future in concurrent.futures.as_completed(futures):
+                maybe_exception = future.result()
+                if isinstance(maybe_exception, Exception):
+                    raise maybe_exception
 
         # write mapping data
         index = [str(uuid.uuid4()) for _ in range(len(self.participant_mapping))]
         mapping_data = pd.DataFrame(
             {
                 "participant": self.participant_mapping.keys(),
                 "time_series": self.participant_mapping.values(),
@@ -144,32 +161,42 @@
             path,
             "time_series_mapping.csv",
             delimiter=delimiter,
             index_label="uuid",
         )
 
     @staticmethod
-    def _write_ts_df(path: str, mkdirs: bool, delimiter: str, ts: PQResult):
-        data = copy.deepcopy(ts.data)
-        if not isinstance(ts.entity_type, TimeSeriesEnum):
-            raise ValueError(
-                f"Expected entity type to be TypeSeriesEnum but is {ts.entity_type}. Can not determine file name."
+    def _write_ts_df(
+        path: str,
+        mkdirs: bool,
+        delimiter: str,
+        ts: ComplexPower,
+        key: TimeSeriesKey,
+    ) -> None | Exception:
+        try:
+            data = copy.deepcopy(ts.data)
+            if not isinstance(key.ts_type, TimeSeriesEnum):
+                raise ValueError(
+                    f"Expected entity type to be TypeSeriesEnum but is {key.ts_type}. Can not determine file name."
+                )
+            ts_name = key.ts_type.get_csv_input_file_name(key.ts_uuid)
+            data["uuid"] = [str(uuid.uuid4()) for _ in range(len(ts))]
+            data["time"] = data.index
+            data.set_index("uuid", inplace=True)
+            df_to_csv(
+                data,
+                path,
+                ts_name,
+                mkdirs=mkdirs,
+                delimiter=delimiter,
+                index_label="uuid",
             )
-        ts_name = ts.entity_type.get_csv_input_file_name(ts.input_model)
-        data["uuid"] = [str(uuid.uuid4()) for _ in range(len(ts))]
-        data["time"] = data.index
-        data.set_index("uuid", inplace=True)
-        df_to_csv(
-            data,
-            path,
-            ts_name,
-            mkdirs=mkdirs,
-            delimiter=delimiter,
-            index_label="uuid",
-        )
+            return None
+        except Exception as e:
+            return e
 
     def compare(self, other):
         if not isinstance(other, type(self)):
             raise ComparisonError(
                 f"Type of self {type(self)} != type of other {type(other)}"
             )
 
@@ -200,15 +227,15 @@
         if errors:
             raise ComparisonError(
                 f"Found Differences in {type(self)} comparison: ", differences=errors
             )
 
     @classmethod
     def from_csv(cls, path: str | Path, delimiter: str | None = None):
-        from pypsdm.models.result.participant.pq_dict import PQResultDict
+        from pypsdm.models.ts.types import ComplexPowerDict
 
         # get all files that start with "its_"
         path = Path(path).resolve()
         ts_files = [file for file in os.listdir(path) if file.startswith("its_p")]
 
         time_series_dict = {}
 
@@ -224,27 +251,26 @@
             pa_read_time_series = partial(
                 PrimaryData._read_pd_time_series, path, delimiter=delimiter
             )
 
             # TODO: Only parallel reading if a lot of ts files
             with concurrent.futures.ProcessPoolExecutor() as executor:
                 time_series = executor.map(pa_read_time_series, ts_files)
-                for ts in time_series:
-                    time_series_dict[ts.name] = ts
+                for ts_key, ts in time_series:
+                    time_series_dict[ts_key] = ts
 
-            time_series = PQResultDict(
-                SystemParticipantsEnum.PRIMARY_DATA, time_series_dict
-            )
+            time_series = ComplexPowerDict(time_series_dict)
 
             return PrimaryData(time_series, participant_mapping)
 
         else:
-            logging.debug(f"No primary data in path {path}")
+            logger.debug(f"No primary data in path {path}")
             return PrimaryData(
-                PQResultDict.create_empty(SystemParticipantsEnum.PRIMARY_DATA), dict()
+                ComplexPowerDict.empty(),
+                dict(),
             )
 
     @staticmethod
     def _read_pd_time_series(
         dir_path: Path | str, ts_file: str, delimiter: str | None = None
     ):
         ts_types = "|".join([e.value for e in TimeSeriesEnum])
@@ -258,19 +284,17 @@
             data = utils.read_csv(dir_path, ts_file, delimiter, index_col="uuid")
             data["time"] = data["time"].apply(
                 lambda date_string: to_date_time(date_string)
             )
             data = data.set_index("time", drop=True)
             if "q" not in data.columns:
                 data["q"] = 0
-            return PQResult(TimeSeriesEnum(ts_type), ts_uuid, ts_uuid, data)
+            return TimeSeriesKey(ts_uuid, TimeSeriesEnum(ts_type)), ComplexPower(data)
 
         else:
             raise IOError(
                 f"Could not read time series with name {ts_file}. Expected format: e.g. its_p_5022a70e-a58f-4bac-b8ec-1c62376c216b.csv"
             )
 
     @classmethod
     def create_empty(cls):
-        return cls(
-            PQResultDict.create_empty(SystemParticipantsEnum.PRIMARY_DATA), dict()
-        )
+        return cls(ComplexPowerDict.empty(), dict())
```

### Comparing `pypsdm-0.0.2/pypsdm/models/result/container/grid.py` & `pypsdm-0.0.3/pypsdm/models/result/container/grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from __future__ import annotations
+
+import os
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 from pypsdm.io.utils import check_filter
-from pypsdm.models.input.container.grid import GridContainer
 from pypsdm.models.input.container.mixins import ContainerMixin
-from pypsdm.models.result.container.participants import ParticipantsResultContainer
+from pypsdm.models.result.container.participants import (
+    SystemParticipantsResultContainer,
+)
 from pypsdm.models.result.container.raw_grid import RawGridResultContainer
 
+if TYPE_CHECKING:
+    from pypsdm.models.input.container.grid import GridContainer
+
 
 @dataclass(frozen=True)
 class GridResultContainer(ContainerMixin):
     raw_grid: RawGridResultContainer
-    participants: ParticipantsResultContainer
+    participants: SystemParticipantsResultContainer
 
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     @property
     def nodes(self):
         return self.raw_grid.nodes
@@ -70,41 +77,41 @@
         return self.participants.hps
 
     @property
     def flex(self):
         return self.participants.flex
 
     def __len__(self):
-        return +len(self.raw_grid) + len(self.participants)
+        return len(self.raw_grid) + len(self.participants)
 
-    # TODO: implement slicing
-    def __getitem__(self, slice_val):
-        raise NotImplementedError
+    def __getitem__(self, slice_val: slice) -> "GridResultContainer":
+        if not isinstance(slice_val, slice):
+            raise ValueError("Only datetime slicing is supported!")
+        start, stop, _ = slice_val.start, slice_val.stop, slice_val.step
+        if not (isinstance(start, datetime) and isinstance(stop, datetime)):
+            raise ValueError("Only datetime slicing is supported")
+        return self.interval(start, stop)
 
     def to_list(self, include_empty: bool = False) -> list:
         res = [
-            self.nodes,
             self.raw_grid,
             self.participants,
         ]
         return res if include_empty else [r for r in res if r]
 
-    def uuids(self) -> set[str]:
-        return set(self.nodes.entities.keys())
-
     def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
         return GridResultContainer(
             self.raw_grid.filter_by_date_time(time),
             self.participants.filter_by_date_time(time),
         )
 
-    def filter_for_time_interval(self, start: datetime, end: datetime):
+    def interval(self, start: datetime, end: datetime):
         return GridResultContainer(
-            self.raw_grid.filter_for_time_interval(start, end),
-            self.participants.filter_for_time_interval(start, end),
+            self.raw_grid.interval(start, end),
+            self.participants.interval(start, end),
         )
 
     def concat(self, other: "GridResultContainer", deep: bool = True, keep="last"):
         """
         Concatenates the data of the two containers, which means concatenating
         the data of their entities.
 
@@ -129,35 +136,48 @@
         simulation_data_path: str,
         delimiter: str | None = None,
         simulation_end: Optional[datetime] = None,
         grid_container: Optional[GridContainer] = None,
         filter_start: Optional[datetime] = None,
         filter_end: Optional[datetime] = None,
     ):
+        res_files = [
+            f for f in os.listdir(simulation_data_path) if f.endswith("_res.csv")
+        ]
+        if len(res_files) == 0:
+            raise FileNotFoundError(
+                f"No simulation results found in '{simulation_data_path}'."
+            )
+
         check_filter(filter_start, filter_end)
 
         raw_grid = RawGridResultContainer.from_csv(
             simulation_data_path,
             delimiter=delimiter,
             simulation_end=simulation_end,
             grid_container=grid_container,
             filter_start=filter_start,
             filter_end=filter_end,
         )
 
-        participants = ParticipantsResultContainer.from_csv(
+        if simulation_end is None:
+            if not len(raw_grid.nodes) == 0:
+                sample_res = raw_grid.nodes[list(raw_grid.nodes.keys())[0]]
+                simulation_end = sample_res.data.index.max()  # type: ignore
+
+        participants = SystemParticipantsResultContainer.from_csv(
             simulation_data_path,
-            simulation_end,  # type: ignore
+            simulation_end,
             grid_container=grid_container,
             filter_start=filter_start,
             filter_end=filter_end,
             delimiter=delimiter,
         )
 
         return cls(raw_grid, participants)
 
     @classmethod
-    def create_empty(cls):
+    def empty(cls):
         return cls(
-            raw_grid=RawGridResultContainer.create_empty(),
-            participants=ParticipantsResultContainer.create_empty(),
+            raw_grid=RawGridResultContainer.empty(),
+            participants=SystemParticipantsResultContainer.empty(),
         )
```

### Comparing `pypsdm-0.0.2/pypsdm/models/result/grid/switch.py` & `pypsdm-0.0.3/pypsdm/models/result/grid/switch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional, Type
 
-import pandas as pd
 from pandas import DataFrame
 
 from pypsdm.models.enums import RawGridElementsEnum
-from pypsdm.models.input.entity import Entities
-from pypsdm.models.result.entity import ResultEntities
-from pypsdm.models.result.participant.dict import ResultDict, ResultDictType
+from pypsdm.models.result.participant.dict import EntitiesResultDictMixin
+from pypsdm.models.ts.base import (
+    EntityKey,
+    TimeSeries,
+    TimeSeriesDict,
+    TimeSeriesDictMixin,
+)
 
 
-@dataclass(frozen=True)
-class SwitchResult(ResultEntities):
+@dataclass
+class SwitchResult(TimeSeries):
+    def __init__(self, data: DataFrame, end: datetime | None = None):
+        super().__init__(data, end)
+
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     def __add__(self, _):
         return NotImplemented
 
     @property
@@ -24,45 +29,21 @@
         return self.data["closed"]
 
     @staticmethod
     def attributes() -> list[str]:
         return ["closed"]
 
 
-@dataclass(frozen=True)
-class SwitchesResult(ResultDict):
-    entities: dict[str, SwitchResult]
-
+class SwitchesResult(
+    TimeSeriesDict[EntityKey, SwitchResult],
+    TimeSeriesDictMixin,
+    EntitiesResultDictMixin,
+):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
-    @property
     def closed(self) -> DataFrame:
-        if not self.entities:
-            return pd.DataFrame()
-        return pd.concat(
-            [
-                switch_res.closed.rename(switch_res.input_model)
-                for switch_res in self.entities.values()
-            ],
-            axis=1,
-        )
+        return self.attr_df("closed")
 
     @classmethod
-    def from_csv(
-        cls: Type[ResultDictType],
-        simulation_data_path: str,
-        delimiter: str | None = None,
-        simulation_end: Optional[datetime] = None,
-        input_entities: Optional[Entities] = None,
-        filter_start: Optional[datetime] = None,
-        filter_end: Optional[datetime] = None,
-    ) -> ResultDictType:
-        return super().from_csv(
-            RawGridElementsEnum.SWITCH,
-            simulation_data_path,
-            delimiter,
-            simulation_end,
-            input_entities,
-            filter_start,
-            filter_end,
-        )
+    def entity_type(cls) -> RawGridElementsEnum:
+        return RawGridElementsEnum.SWITCH
```

### Comparing `pypsdm-0.0.2/pypsdm/models/result/participant/dict.py` & `pypsdm-0.0.3/pypsdm/models/result/participant/dict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,348 +1,339 @@
-import logging
+from __future__ import annotations
+
 import os
 import uuid
-from abc import ABC
-from dataclasses import dataclass
+from abc import abstractmethod
 from datetime import datetime
-from pathlib import Path
-from typing import Dict, Generic, Optional, Self, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Self, Tuple, Type
 
-from pandas import DataFrame
-from pandas.core.groupby.generic import DataFrameGroupBy
+import pandas as pd
+from loguru import logger
 
-from pypsdm.errors import ComparisonError
 from pypsdm.io.utils import check_filter, csv_to_grpd_df, get_file_path, to_date_time
-from pypsdm.models.enums import EntitiesEnum
+from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
 from pypsdm.models.input.entity import Entities
-from pypsdm.models.result.entity import ResultEntities
-from pypsdm.processing.dataframe import join_dataframes
-
-ResultDictType = TypeVar("ResultDictType", bound="ResultDict")
-T = TypeVar("T", bound=ResultEntities)
+from pypsdm.models.ts.base import EntityKey, TimeSeries
+from pypsdm.models.ts.types import (
+    ComplexPower,
+    ComplexPowerDict,
+    ComplexPowerWithSoc,
+    ComplexPowerWithSocDict,
+)
+
+if TYPE_CHECKING:
+    from pypsdm.models.input.container.grid import GridContainer
 
 
-@dataclass(frozen=True)
-class ResultDict(Generic[T], ABC):
-    entity_type: EntitiesEnum
-    entities: Dict[str, T]
-
-    def __eq__(self, other):
-        if not isinstance(other, type(self)):
-            return False
-        if self.entity_type != other.entity_type:
-            return False
-        for key, res in self.entities.items():
-            if key not in other.entities:
-                return False
-            if res != other.entities[key]:
-                return False
-        return True
-
-    def __len__(self):
-        return len(self.entities)
-
-    def __contains__(self, uuid):
-        return uuid in self.entities
-
-    def __getitem__(self, get) -> T:
-        match get:
-            case str():
-                return self.entities[get]
-            case slice():
-                raise ValueError(
-                    "If you want to filter by time interval use filter_for_time_interval method instead."
-                )
-            case _:
-                raise ValueError("Only get by uuid is supported.")
-
-    def __add__(self: ResultDictType, other: ResultDictType):
-        """
-        Add two ResultDicts together. The entity types must be the same.
-
-        BEWARE: The underlying data will NOT be copied. That means changing items in the returned ResultDict will also
-        change the items in the original ResultDicts and vice versa.
-
-        Args:
-            other: The ResultDict to add to this ResultDict
-
-        Returns:
-            A new ResultDict containing the entities of both ResultDicts.
-        """
-        if not isinstance(other, type(self)):
-            raise TypeError(f"Cannot add {type(self)} and {type(other)}")
-        if self.entity_type != other.entity_type:
-            raise TypeError(
-                f"Cannot add {type(self)} and {type(other)}. Entities are of different entity types"
-            )
-        return type(self)(self.entity_type, {**self.entities, **other.entities})
-
-    def __sub__(self: ResultDictType, other: ResultDictType):
-        """
-        Creates a new dict with the elements of self minus all keys of other. The entity types must be the same.
-
-        BEWARE: Returns a shallow copy of the data, the underlying data will NOT be copied.
-
-        Args:
-            other: The ResultDict to subtract from this ResultDict
-
-        """
-        if not isinstance(other, type(self)):
-            raise TypeError(f"Cannot subtract {type(self)} and {type(other)}")
-        if self.entity_type != other.entity_type:
-            raise TypeError(
-                f"Cannot subtract {type(self)} and {type(other)}. Entities are of different entity types"
-            )
-        keys = self.entities.keys() - other.entities.keys()
-        return type(self)(self.entity_type, {key: self.entities[key] for key in keys})
+class EntitiesResultDictMixin:
+    def uuids(self) -> set[str]:
+        return {key.uuid for key in self.keys()}  # type: ignore
 
-    def __iter__(self):
-        return self.entities.__iter__()
+    @classmethod
+    @abstractmethod
+    def entity_type(cls) -> EntitiesEnum:
+        raise NotImplementedError
 
-    def keys(self):
-        return self.entities.keys()
+    @classmethod
+    def result_type(cls) -> Type[TimeSeries]:
+        return cls.entity_type().get_result_type()
 
-    def values(self):
-        return self.entities.values()
-
-    def to_list(self):
-        return list(self.entities.values())
-
-    def items(self):
-        return self.entities.items()
-
-    def uuids(self):
-        return list(self.entities.keys())
-
-    def results(self):
-        return list(self.entities.values())
-
-    # noinspection PyArgumentList
-    def subset(self, uuids):
-        matched_participants = {
-            uuid: self.entities[uuid] for uuid in self.entities.keys() & uuids
-        }
-
-        return type(self)(self.entity_type, matched_participants)
-
-    def subset_split(self, uuids: list[str]):
-        """
-        Returns a results result containing the given uuids and a results result containing the remaining uuids.
-        :param uuids: the uuids with which to split the result
-        :return:
-        """
-
-        rmd_uuids = self.entities.keys() - uuids
-        return self.subset(uuids), self.subset(rmd_uuids)
-
-    def filter_by_date_time(self, time: Union[datetime, list[datetime]]):
-        """
-        Filters the result by the given datetime or list of datetimes.
-        :param time: the time or list of times to filter by
-        :return: a new result containing only the given time or times
-        """
-        return type(self)(
-            self.entity_type,
-            {uuid: result[time] for uuid, result in self.entities.items()},
-        )
+    @classmethod
+    def from_csv(
+        cls,
+        simulation_data_path: str,
+        delimiter: str | None = None,
+        simulation_end: datetime | None = None,
+        input_entities: Entities | None = None,
+        filter_start: datetime | None = None,
+        filter_end: datetime | None = None,
+        must_exist: bool = True,
+    ) -> Self:
+        check_filter(filter_start, filter_end)
 
-    # noinspection PyArgumentList
-    def filter_for_time_interval(self, start: datetime, end: datetime):
-        return type(self)(
-            self.entity_type,
-            {
-                uuid: result.filter_for_time_interval(start, end)
-                for uuid, result in self.entities.items()
-            },
-        )
+        file_name = cls.entity_type().get_csv_result_file_name()
+        path = get_file_path(simulation_data_path, file_name)
+        if path.exists():
+            grpd_df = csv_to_grpd_df(file_name, simulation_data_path, delimiter)
+        else:
+            if must_exist:
+                raise FileNotFoundError(f"File {path} does not exist")
+            else:
+                return cls.empty()  # type: ignore
 
-    def uuid_to_id_map(self) -> dict[str, Optional[str]]:
-        return {uuid: result.name for uuid, result in self.entities.items()}
+        if len(grpd_df) == 0:
+            return cls.empty()  # type: ignore
 
-    def compare(self, other):
-        if not isinstance(other, type(self)):
-            raise ComparisonError(
-                f"Type of self {type(self)} != type of other {type(other)}",
-                differences=[],
-            )
-        differences = []
-        if self.entity_type != other.entity_type:
-            differences.append(f"Entity type {self.entity_type} != {other.entity_type}")
-        for key, entity in self.entities.items():
-            if key not in other.entities:
-                differences.append(f"Entity {key} not in other")
-            else:
-                try:
-                    entity.compare(other.entities[key])
-                except ComparisonError as e:
-                    differences.extend(e.differences)
-        if differences:
-            raise ComparisonError(
-                f"Comparison of {type(self)} failed", differences=differences
-            )
+        if simulation_end is None:
+            simulation_end = to_date_time(grpd_df["time"].max().max())  # type: ignore
 
-    def concat(
-        self: ResultDictType, other: ResultDictType, deep: bool = True, keep="last"
-    ):
-        """
-        Concatenates the data of the two ResultDicts, which means concatenating
-        the data of their entities.
-
-        NOTE: This only makes sense if the entities indexes are continuous. Given
-        that we deal with discrete event data that means that the last state of self
-        is valid until the first state of other. Which would probably not be what
-        you want in case the results are separated by a year.
-
-        Args:
-            other: The other ResultEntities object to concatenate with.
-            deep: Whether to do a deep copy of the data.
-            keep: How to handle duplicate indexes. "last" by default.
-        """
-        if not isinstance(other, type(self)):
-            raise TypeError(f"Cannot concatenate {type(self)} and {type(other)}")
-        if self.entity_type != other.entity_type:
-            raise TypeError(
-                f"Cannot add {type(self)} and {type(other)}. Entities are of different entity types"
-            )
+        ts_dict = {}
+        for key, grp in grpd_df:
+            name = None
+            if input_entities:
+                if key in input_entities:  # type: ignore
+                    name = input_entities[key].id  # type: ignore
+                else:
+                    logger.warning("Entity {} not in input entities".format(key))
+            entity_key = EntityKey(key, name)  # type: ignore
+            grp.drop(columns=["input_model"], inplace=True)
+            ts = cls.result_type()(grp, simulation_end)
+            ts_dict[entity_key] = ts
 
-        if not set(self.entities.keys()) == set(other.entities.keys()):
-            raise ValueError(
-                "ResultDicts need to contain the same entities to be concatenated"
-            )
-        concat_entities = {}
-        for key, entity in self.entities.items():
-            concat_entities[key] = entity.concat(
-                other.entities[key], deep=deep, keep=keep
-            )
-        return type(self)(self.entity_type, concat_entities)
+        res = cls(ts_dict)
+        return (
+            res
+            if not filter_start
+            else res.filter_for_time_interval(filter_start, filter_end)  # type: ignore
+        )
 
     def to_csv(
         self,
         path: str,
         delimiter=",",
         mkdirs=False,
-        resample_rate: Optional[str] = None,
+        resample_rate: str | None = None,
     ):
         if mkdirs:
             os.makedirs(path, exist_ok=True)
 
-        file_name = self.entity_type.get_csv_result_file_name()
+        file_name = self.entity_type().get_csv_result_file_name()
 
-        def prepare_data(data: DataFrame, input_model: str):
+        def prepare_data(data: pd.DataFrame, input_model: str):
             data = data.copy()
             data = (
                 data.resample("60s").ffill().resample(resample_rate).mean()
                 if resample_rate
                 else data
             )
             data["uuid"] = data.apply(lambda _: str(uuid.uuid4()), axis=1)
             data["input_model"] = input_model
             data.index.name = "time"
             return data
 
         dfs = [
-            prepare_data(participant.data, input_model)
-            for input_model, participant in self.entities.items()
+            prepare_data(participant.data, entity_key.uuid)
+            for entity_key, participant in self.items()  # type: ignore
         ]
-        df = join_dataframes(dfs)
+        df = pd.concat(dfs)
         df.to_csv(os.path.join(path, file_name), sep=delimiter, index=True)
 
-    @classmethod
-    def from_csv(
-        cls: Type[ResultDictType],
-        entity_type: EntitiesEnum,
+    @staticmethod
+    def from_csv_for_entity(
         simulation_data_path: str,
+        simulation_end: datetime | None,
+        grid_container: GridContainer | None,
+        entity: EntitiesEnum,
         delimiter: str | None = None,
-        simulation_end: Optional[datetime] = None,
-        input_entities: Optional[Entities] = None,
-        filter_start: Optional[datetime] = None,
-        filter_end: Optional[datetime] = None,
-    ) -> ResultDictType:
-        check_filter(filter_start, filter_end)
-        grpd_df = ResultDict.get_grpd_df(
-            entity_type,
-            simulation_data_path,
-            delimiter,
-        )
-        if not grpd_df:
-            logging.debug("There are no " + str(cls))
-            return cls.create_empty(entity_type)
-        if simulation_end is None:
-            simulation_end = to_date_time(grpd_df["time"].max().max())
-        entities = dict(
-            grpd_df.apply(
-                lambda grp: ResultDict.build_for_entity(
-                    entity_type,
-                    grp.name,  # type: ignore
-                    grp.drop(columns=["input_model"]),
-                    simulation_end,
-                    input_entities=input_entities,
-                )
-            )
-        )
-        res = cls(
-            entity_type,
-            entities,
-        )
-        return (
-            res
-            if not filter_start
-            else res.filter_for_time_interval(filter_start, filter_end)
-        )
+    ) -> "EntitiesResultDictMixin" | Tuple[Exception, EntitiesEnum]:
+        try:
+            if grid_container:
+                input_entities = grid_container.get_with_enum(entity)
+            else:
+                input_entities = None
+            dict_type = entity.get_result_dict_type()
+            return dict_type.from_csv(
+                simulation_data_path,
+                delimiter=delimiter,
+                simulation_end=simulation_end,
+                input_entities=input_entities,
+                must_exist=False,
+            )
+
+        except Exception as e:
+            return (e, entity)
+
+
+class EmsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPower]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPower):
+                raise ValueError(f"Time series {value} is not of type ComplexPower")
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
 
     @classmethod
-    def create_empty(cls: Type[Self], entity_type: EntitiesEnum) -> Self:
-        return cls(entity_type, dict())
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.ENERGY_MANAGEMENT
 
-    @staticmethod
-    def build_for_entity(
-        entity_type: EntitiesEnum,
-        input_model: str,
-        data: DataFrame,
-        simulation_end: datetime,
-        input_entities: Optional[Entities],
-    ) -> ResultEntities:
-        name = None
-        if input_entities is not None:
-            if input_model not in input_entities.id.index:
-                logging.debug(
-                    f"Input model {input_model} of type {entity_type} not found in input entities. It seems like the wrong input_entities have been passed. Not assigning a name to the result."
-                )
-            else:
-                name = input_entities.id.loc[input_model]
 
-        return entity_type.get_result_type().build(
-            entity_type, input_model, data, simulation_end, name=name
-        )
+class LoadsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPower]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPower):
+                raise ValueError(f"Time series {value} is not of type ComplexPower")
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
 
-    @staticmethod
-    def get_grpd_df(
-        entity_type: EntitiesEnum,
-        simulation_data_path: str,
-        delimiter: str | None = None,
-    ) -> Optional[DataFrameGroupBy]:
-        file_name = entity_type.get_csv_result_file_name()
-        path = get_file_path(simulation_data_path, file_name)
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
 
-        if not path.exists():
-            logging.info(
-                "No results built for {} since {} does not exist".format(
-                    file_name, str(path)
-                )
-            )
-            return None
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.LOAD
 
-        return csv_to_grpd_df(file_name, simulation_data_path, delimiter)
 
-    @staticmethod
-    def safe_get_path(entity_type: EntitiesEnum, data_path: str) -> Optional[Path]:
-        file_name = entity_type.get_csv_result_file_name()
-        path = get_file_path(data_path, file_name)
-        if path.exists():
-            return path
+class FixedFeedInsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPower]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPower):
+                raise ValueError(f"Time series {value} is not of type ComplexPower")
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
         else:
-            logging.info(
-                "No results built for {} since {} does not exist".format(
-                    file_name, str(path)
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.FIXED_FEED_IN
+
+
+class PvsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPower]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPower):
+                raise ValueError(f"Time series {value} is not of type ComplexPower")
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.PHOTOVOLTAIC_POWER_PLANT
+
+
+class WecsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPower]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPower):
+                raise ValueError(f"Time series {value} is not of type ComplexPower")
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.WIND_ENERGY_CONVERTER
+
+
+class StoragesResult(ComplexPowerWithSocDict[EntityKey], EntitiesResultDictMixin):
+    def __init__(self, data: dict[EntityKey, ComplexPowerWithSoc]):
+        for key, value in data.items():
+            if not isinstance(key, EntityKey):
+                raise ValueError(f"Key {key} is not of type EntityKey")
+            if not isinstance(value, ComplexPowerWithSoc):
+                raise ValueError(
+                    f"Time series {value} is not of type ComplexPowerWithSoc"
                 )
-            )
-            return None
+        super().__init__(data)
+
+    def __getitem__(self, key: str | EntityKey) -> ComplexPowerWithSoc:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.STORAGE
+
+
+class EvcsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __getitem__(self, key: str | EntityKey) -> ComplexPower:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.EV_CHARGING_STATION
+
+
+class EvsResult(ComplexPowerWithSocDict[EntityKey], EntitiesResultDictMixin):
+    def __getitem__(self, key: str | EntityKey) -> ComplexPowerWithSoc:
+        if isinstance(key, str):
+            key = EntityKey(key)
+        else:
+            key = key
+        return super().__getitem__(key)
+
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.ELECTRIC_VEHICLE
+
+
+class HpsResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.HEAT_PUMP
+
+
+class FlexResult(ComplexPowerDict[EntityKey], EntitiesResultDictMixin):
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    @classmethod
+    def entity_type(cls) -> EntitiesEnum:
+        return SystemParticipantsEnum.FLEX_OPTIONS
```

### Comparing `pypsdm-0.0.2/pypsdm/models/result/participant/flex_options.py` & `pypsdm-0.0.3/pypsdm/models/result/participant/flex_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 from dataclasses import dataclass
-from typing import Dict, List
+from datetime import datetime
+from functools import reduce
+from typing import List, Self, Sequence
 
 import pandas as pd
 from pandas import DataFrame, Series
 
 from pypsdm.models.enums import SystemParticipantsEnum
-from pypsdm.models.result.entity import ResultEntities
-from pypsdm.models.result.participant.dict import ResultDict
-from pypsdm.models.result.power import PQResult
-from pypsdm.processing.series import add_series, hourly_mean_resample
+from pypsdm.models.result.participant.dict import EntitiesResultDictMixin
+from pypsdm.models.ts.base import EntityKey, TimeSeries, TimeSeriesDict
+from pypsdm.models.ts.types import ComplexPower
+from pypsdm.processing.dataframe import add_df
+from pypsdm.processing.series import hourly_mean_resample
 
 
-@dataclass(frozen=True)
-class FlexOptionResult(ResultEntities):
+@dataclass
+class FlexOption(TimeSeries):
+
+    def __init__(self, data: pd.DataFrame, end: datetime | None = None):
+        super().__init__(data, end)
+
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
-    def __add__(self, other: "FlexOptionResult"):
-        p_ref_sum = add_series(self.p_ref(), other.p_ref(), "p_ref")
-        p_min_sum = add_series(self.p_min(), other.p_min(), "p_min")
-        p_max_sum = add_series(self.p_max(), other.p_max(), "p_max")
-        summed_data = p_ref_sum.to_frame().join([p_min_sum, p_max_sum])
-        return FlexOptionResult(
-            self.entity_type,
-            "FlexResult - Sum",
-            "FlexResult - Sum",
-            summed_data,
+    def __add__(self, other: "FlexOption"):
+        data = add_df(self.data, other.data)
+        return FlexOption(
+            data,
         )
 
-    @staticmethod
-    def attributes() -> List[str]:
-        return ["p_max", "p_min", "p_ref"]
-
     def p_max(self):
         return self.data["p_max"]
 
     def p_min(self):
         return self.data["p_min"]
 
     def p_ref(self):
         return self.data["p_ref"]
 
-    def p_max_as_pq(self, sp_type: SystemParticipantsEnum) -> PQResult:
-        return self._p_to_pq_res(sp_type, self.p_max())
+    def p_max_as_power(self) -> ComplexPower:
+        return self._p_to_pq_res(self.p_max())
 
-    def p_ref_as_pq(self, sp_type: SystemParticipantsEnum) -> PQResult:
-        return self._p_to_pq_res(sp_type, self.p_ref())
+    def p_ref_as_power(self) -> ComplexPower:
+        return self._p_to_pq_res(self.p_ref())
 
-    def p_min_as_pq(self, sp_type: SystemParticipantsEnum):
-        return self._p_to_pq_res(sp_type, self.p_min())
+    def p_min_as_pq(self) -> ComplexPower:
+        return self._p_to_pq_res(self.p_min())
 
-    def _p_to_pq_res(
-        self, sp_type: SystemParticipantsEnum, p_series: Series
-    ) -> PQResult:
+    def _p_to_pq_res(self, p_series: Series) -> ComplexPower:
         data = p_series.rename("p").to_frame()
         data["q"] = 0
-        return PQResult(sp_type, "flex-signal", "flex-signal", data)
+        return ComplexPower(data)
 
     def hourly_resample(self):
         updated_data = self.data.apply(lambda x: hourly_mean_resample(x))
-        return FlexOptionResult(
-            self.entity_type, self.input_model, self.name, updated_data
-        )
+        return FlexOption(updated_data)  # type: ignore
 
-    def add_series(self, series: Series) -> "FlexOptionResult":
-        updated_data = self.data.apply(
-            lambda p_flex: add_series(p_flex, series, p_flex.name), axis=0
-        )
-        return FlexOptionResult(
-            self.entity_type, self.input_model, self.name, updated_data
-        )
+    @staticmethod
+    def attributes() -> List[str]:
+        return ["p_max", "p_min", "p_ref"]
+
+    @classmethod
+    # TODO: find a way for parallel calculation
+    def sum(cls, results: Sequence[Self]) -> "FlexOption":
+        if len(results) == 0:
+            return cls.empty()
+        if len(results) == 1:
+            return results[0]
+        return reduce(lambda a, b: a + b, results)
 
 
-@dataclass(frozen=True)
-class FlexOptionsResult(ResultDict):
-    entities: Dict[str, FlexOptionResult]
+class FlexOptionsDict(TimeSeriesDict[EntityKey, FlexOption], EntitiesResultDictMixin):
 
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
     def to_df(self) -> DataFrame:
         return pd.concat(
-            [f.data for f in self.entities.values()],
-            keys=self.entities.keys(),
+            [f.data for f in self.values()],
+            keys=self.keys(),
             axis=1,
         ).ffill()
 
-    def to_multi_index_df(
-        self, participants_res  # type hinting leads to circular import
-    ) -> DataFrame:
+    def to_multi_index_df(self, participants_res) -> DataFrame:
         flex_midfs = {}
         for res in participants_res.to_list():
             uuids = res.participants.keys()
             flex_res = self.subset(uuids)
             if flex_res:
                 flex_dfs = []
                 participant_uuids = []
                 [
                     (participant_uuids.append(uuid), flex_dfs.append(flex.data))
-                    for uuid, flex in flex_res.entities.items()
+                    for uuid, flex in flex_res.items()
                 ]
                 flex_midf = pd.concat(flex_dfs, keys=participant_uuids, axis=1)
                 flex_midfs[res.entity_type.value] = flex_midf
         return pd.concat(flex_midfs.values(), keys=(flex_midfs.keys()), axis=1).ffill()
 
-    def sum(self) -> FlexOptionResult:
-        return FlexOptionResult.sum(list(self.entities.values()))
+    def sum(self) -> FlexOption:
+        return FlexOption.sum(list(self.values()))
+
+    @classmethod
+    def entity_type(cls):
+        return SystemParticipantsEnum.FLEX_OPTIONS
```

### Comparing `pypsdm-0.0.2/pypsdm/models/result/power.py` & `pypsdm-0.0.3/pypsdm/models/ts/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,233 @@
-import dataclasses
-import os
-import re
-from dataclasses import dataclass
+from __future__ import annotations
+
 from functools import reduce
-from pathlib import Path
-from typing import List, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, List, Self, Sequence, Union
+
+from pandas import DataFrame
 
-import numpy as np
-import pandas as pd
-from pandas import Series
-
-from pypsdm.models.enums import EntitiesEnum, SystemParticipantsEnum
-from pypsdm.models.result.entity import ResultEntities
-from pypsdm.processing.dataframe import divide_positive_negative
-from pypsdm.processing.series import (
-    add_series,
-    duration_weighted_sum,
-    hourly_mean_resample,
-    load_and_generation,
+from pypsdm.models.ts.base import K, TimeSeries, TimeSeriesDict
+from pypsdm.models.ts.mixins import (
+    ComplexCurrentMixin,
+    ComplexPowerDictMixin,
+    ComplexPowerMixin,
+    ComplexVoltageDictMixin,
+    ComplexVoltageMixin,
+    SocDictMixin,
+    SocMixin,
+    WeatherDataDictMixin,
+    WeatherDataMixin,
 )
+from pypsdm.processing.dataframe import add_df
+from pypsdm.processing.series import Tuple, add_series
+
+if TYPE_CHECKING:
+    from pypsdm.db.weather.models import WeatherValue
 
 
-@dataclass(frozen=True)
-class PQResult(ResultEntities):
+class ComplexPower(TimeSeries, ComplexPowerMixin):
     def __eq__(self, other: object) -> bool:
         return super().__eq__(other)
 
-    def __add__(self, other: "PQResult"):
-        p_sum = add_series(self.p, other.p, "p")
-        q_sum = add_series(self.q, other.q, "q")
-        summed_data = p_sum.to_frame().join(q_sum)
-        return PQResult(
-            (
-                self.entity_type
-                if self.entity_type == other.entity_type
-                else SystemParticipantsEnum.PARTICIPANTS_SUM
-            ),
-            "PQResult - Sum",
-            "PQResult - Sum",
-            summed_data,
-        )
+    def __add__(self, other: Self) -> "ComplexPower":
+        if isinstance(other, ComplexPower):
+            self_data = self.data[ComplexPower.attributes()]
+            other_data = other.data[ComplexPower.attributes()]
+            data = add_df(self_data, other_data)
+            return ComplexPower(data)
+        else:
+            raise ValueError(
+                f"Addition with type {type(other)} not or not yet supported"
+            )
 
-    def __sub__(self, other: "PQResult"):
+    def __sub__(self, other: Self):
         return self + (other * -1)
 
     def __mul__(self, other: Union[float, int]):
         if isinstance(other, float) or isinstance(other, int):
             updated_data = self.data * other
-            return PQResult(self.entity_type, self.input_model, self.name, updated_data)
+            return ComplexPower(updated_data)
         else:
             raise ValueError(
                 f"Multiplication with type {type(other)} not or not yet supported"
             )
 
     # commutative multiplication (a*b=b*a)
     __rmul__ = __mul__
 
-    @property
-    def p(self):
-        return self.data["p"]
-
-    @property
-    def q(self):
-        return self.data["q"]
-
-    def complex_power(self):
-        return self.p + 1j * self.q
-
-    def angle(self):
-        return self.complex_power().apply(lambda x: np.angle(x, deg=True))
-
-    def energy(self) -> float:
-        return duration_weighted_sum(self.p)
-
-    def load_and_generation(self) -> Tuple[float, float]:
-        return load_and_generation(self.p)
-
-    def divide_load_generation(self):
-        load, generation = divide_positive_negative(self.data)
-        return dataclasses.replace(self, data=load), dataclasses.replace(
-            self, data=generation
-        )
-
-    def full_load_hours(self, device_power_kw, period="Y"):
-        """
-        Calculates the full load hours for the given period.
-
-        Args:
-            device_power_mw: The power of the device in MW
-            period: The period to calculate the full load hours for. Default is year.
-                    Use to_period() aliases, like Y for year, M for month, D for day, etc.
-                    (https://pandas.pydata.org/docs/user_guide/timeseries.html#timeseries-period-aliases)
-
-        Returns:
-            A series with the full load hours within the determined periods.
-        """
-        return self.p.groupby(self.p.index.to_period(period)).apply(
-            lambda series: duration_weighted_sum(series.abs())
-        ) / (
-            device_power_kw / 1000
-        )  # convert to MW since results are in MW
-
-    def annual_duration_series(self, drop_index=True):
-        return (
-            hourly_mean_resample(self.p)
-            .sort_values(ascending=False)
-            .reset_index(drop=drop_index)  # type: ignore
-        )
-
-    def hourly_resample(self):
-        updated_data = self.data.apply(lambda col: hourly_mean_resample(col), axis=0)
-        return PQResult(self.entity_type, self.input_model, self.name, updated_data)
-
-    def to_csv(self, path: str, file_name: str | None = None, delimiter: str = ","):
-        if not isinstance(path, str):
-            path = str(path)
-        file_name = file_name if file_name else self.get_default_output_name()
-        self.data.to_csv(
-            os.path.join(path, file_name), sep=delimiter, index_label="time"
-        )
-
-    def get_default_output_name(self) -> str:
-        return self.input_model + "_" + self.entity_type.get_csv_result_file_name()
-
-    @classmethod
-    def from_csv(
-        cls, file_path: str | Path, sp_type: EntitiesEnum, name: str | None = None
-    ):
-        file_path = Path(file_path).resolve()
-        data = pd.read_csv(file_path)
-        data["time"] = pd.to_datetime(data["time"])
-        data = data.set_index("time", drop=True)
-        file_name = os.path.basename(file_path)
-        is_default_file_name = re.match(
-            f"{sp_type.get_csv_result_file_name()}_.*", file_name
-        )
-        input_model = file_name.split("_")[-1] if is_default_file_name else file_name
-        return cls(sp_type, name if name else input_model, input_model, data)
-
     @classmethod
-    # todo: find a way for parallel calculation
-    def sum(cls, results: Sequence["PQResult"]) -> "PQResult":
+    def sum(cls, results: Sequence[Self]) -> "ComplexPower":
         if len(results) == 0:
-            return PQResult.create_empty(
-                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
-            )
+            return cls.empty()
         if len(results) == 1:
             return results[0]
         return reduce(lambda a, b: a + b, results)
 
     @staticmethod
     def attributes() -> List[str]:
         return ["p", "q"]
 
 
-@dataclass(frozen=True)
-class PQWithSocResult(PQResult):
-    def __eq__(self, other: object) -> bool:
-        return super().__eq__(other)
+class ComplexPowerDict(TimeSeriesDict[K, ComplexPower], ComplexPowerDictMixin):
+    def sum(self) -> ComplexPower:
+        return ComplexPower.sum(list(self.values()))
+
+    def load_and_generation(self) -> Tuple[float, float]:
+        return self.sum().load_and_generation_energy()
+
+
+@ComplexPower.register
+class ComplexPowerWithSoc(TimeSeries, ComplexPowerMixin, SocMixin):
+    def as_complex_power(self) -> ComplexPower:
+        return ComplexPower(self.data.drop(columns=["soc"]))
 
     def add_with_soc(
-        self, this_capacity: float, other: "PQWithSocResult", other_capacity: float
-    ):
-        p_sum = add_series(self.p, other.p, "p")
-        q_sum = add_series(self.q, other.q, "q")
+        self, this_capacity: float, other: "ComplexPowerWithSoc", other_capacity: float
+    ) -> Self:
+        data = add_df(self.data.drop(columns=["soc"]), other.data.drop(columns=["soc"]))
         total_capacity = this_capacity + other_capacity
         soc = add_series(
             self.soc * this_capacity / total_capacity,
             other.soc * other_capacity / total_capacity,
             "soc",
         )
-        summed_data = p_sum.to_frame().join([q_sum, soc])
-        return PQWithSocResult(
-            self.entity_type,
-            "PQResult - Sum",
-            "PQResult - Sum",
-            summed_data,
+        data["soc"] = soc
+        return self.__class__(
+            data,
         )
 
     @staticmethod
-    # todo: find a way for parallel calculation
     def sum_with_soc(
-        results: list[Tuple[float, "PQWithSocResult"]]
-    ) -> "PQWithSocResult":
+        results: list[Tuple[float, "ComplexPowerWithSoc"]],
+    ) -> "ComplexPowerWithSoc":
         if len(results) == 0:
-            return PQWithSocResult.create_empty(
-                SystemParticipantsEnum.PARTICIPANTS_SUM, "", ""
-            )
+            return ComplexPowerWithSoc.empty()
         if len(results) == 1:
             return results[0][1]
         this_capacity, agg = results[0]
         for other_capacity, result in results[1::]:
             agg = agg.add_with_soc(this_capacity, result, other_capacity)
         return agg
 
-    @property
-    def soc(self) -> Series:
-        return self.data["soc"]
+    @staticmethod
+    def attributes() -> List[str]:
+        return ["p", "q", "soc"]
+
+
+@ComplexPowerDict.register
+class ComplexPowerWithSocDict(
+    TimeSeriesDict[K, ComplexPowerWithSoc], ComplexPowerDictMixin, SocDictMixin
+):
+    def sum(self) -> ComplexPower:
+        return ComplexPower.sum([v.as_complex_power() for v in self.values()])
+
+    def sum_with_soc(self, capacities: dict[K, float]) -> ComplexPowerWithSoc:
+        if not self:
+            return ComplexPowerWithSoc.empty()
+        capacity_participant = []
+        for key, res in self.items():
+            capacity = capacities[key]
+            capacity_participant.append((capacity, res))
+        return ComplexPowerWithSoc.sum_with_soc(capacity_participant)
+
+
+class ComplexCurrent(TimeSeries, ComplexCurrentMixin):
+    @staticmethod
+    def attributes() -> list[str]:
+        return ["i_mag", "i_ang"]
+
+
+class ComplexCurrentDict(TimeSeriesDict[K, ComplexCurrent]):
+    pass
+
+
+class ComplexVoltage(TimeSeries, ComplexVoltageMixin):
+    @staticmethod
+    def attributes() -> list[str]:
+        return ["v_mag", "v_ang"]
+
+
+class ComplexVoltageDict(TimeSeriesDict[K, ComplexVoltage], ComplexVoltageDictMixin):
+    pass
+
+
+@ComplexVoltage.register
+class ComplexVoltagePower(ComplexVoltage, ComplexPower):
+    def __init__(self, data):
+        super().__init__(data)
+
+    def __add__(self, other: Self):
+        raise NotImplementedError
+
+    def __eq__(self, other: object):
+        return super().__eq__(other)
+
+    def as_complex_voltage(self):
+        return ComplexVoltage(self.data[ComplexVoltage.attributes()])
+
+    def as_complex_power(self):
+        return ComplexPower(self.data[ComplexPower.attributes()])
+
+
+@ComplexVoltageDict.register
+class ComplexVoltagePowerDict(
+    TimeSeriesDict[K, ComplexVoltagePower],
+    ComplexVoltageDictMixin,
+    ComplexPowerDictMixin,
+):
+    def __eq__(self, other: object) -> bool:
+        return super().__eq__(other)
+
+    def complex_power_sum(self) -> ComplexPower:
+        return ComplexPower.sum(list(self.values()))
+
+
+class CoordinateWeather(TimeSeries, WeatherDataMixin):
+
+    def __add__(self, other) -> Self:
+        return self.__class__(add_df(self.data, other.data))
+
+    def __mul__(self, other: float | int) -> Self:
+        return self.__class__(self.data * other)
+
+    __rmul__ = __mul__
+
+    @classmethod
+    def from_value_list(cls, values: list[WeatherValue]):
+        df = cls.df_from_value_list(values)
+        if df["coordinate_id"].nunique() > 1:
+            raise ValueError("Multiple coordinate ids in weather data")
+        df.drop(columns=["coordinate_id"], inplace=True)
+        return cls(df)
+
+    @staticmethod
+    def df_from_value_list(values: list[WeatherValue]):
+        from pypsdm.db.weather.models import WeatherValue
+
+        value_dicts = [value.model_dump() for value in values]
+        df = DataFrame(value_dicts, columns=WeatherValue.__table__.columns.keys())
+        df.rename(columns=WeatherValue.name_mapping(), inplace=True)
+        df.set_index("time", inplace=True, drop=True)
+        return df
 
     @staticmethod
     def attributes() -> List[str]:
-        return ["p", "q", "capacity"]
+        return [
+            "diffuse_irradiance",
+            "direct_irradiance",
+            "temperature",
+            "wind_velocity_u",
+            "wind_velocity_v",
+        ]
+
+
+class WeatherDict(TimeSeriesDict[int, CoordinateWeather], WeatherDataDictMixin):
+
+    @classmethod
+    def from_value_list(cls, values: list[WeatherValue]):
+        df = CoordinateWeather.df_from_value_list(values)
+        grps = df.groupby("coordinate_id")
+        dct = {}
+        for coord_id, grp in grps:
+            grp = grp.drop(columns=["coordinate_id"])
+            dct[coord_id] = CoordinateWeather(grp)
+        return cls(dct)
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/common/bar_plot.py` & `pypsdm-0.0.3/pypsdm/plots/common/bar_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 from matplotlib.ticker import FuncFormatter
 
-from pypsdm.models.result.container.participants import ParticipantsResultContainer
-from pypsdm.models.result.power import PQResult
+from pypsdm.models.enums import EntitiesEnum
+from pypsdm.models.result.container.participants import (
+    SystemParticipantsResultContainer,
+)
+from pypsdm.models.ts.types import ComplexPower
 from pypsdm.plots.common.utils import (
     FIGSIZE,
     FIGSIZE_WIDE,
     LOAD_COLOR,
     PV_COLOR,
     TITLE_FONT_SIZE,
     get_label_and_color,
 )
 
 sns.set_style("whitegrid")
 
 
-def plot_full_load_hours(res: PQResult, device_power_kw, period="M", title=None):
+def plot_full_load_hours(
+    res: ComplexPower,
+    device_power_kw,
+    entity_type: None | EntitiesEnum = None,
+    period="M",
+    title=None,
+):
+    """
+    Plots full load hours of the system in each period (e.g. Y, M, D for year, month, day).
+    """
     if not title:
-        name = res.name if res.name else res.input_model
-        title = f"Full load hours: {name}"
+        title = "Full load hours"
 
     full_load_hours = res.full_load_hours(device_power_kw, period=period)
     fig, ax = plt.subplots(figsize=FIGSIZE_WIDE)
-    _, color = get_label_and_color(res.entity_type)
+    _, color = get_label_and_color(entity_type)
     ax.bar([x for x in range(len(full_load_hours))], full_load_hours, color=color)
 
     # Set x-tick labels
     ax.set_xticks(range(len(full_load_hours)))
     ax.set_xticklabels(
         full_load_hours.index.astype(str), rotation=45, ha="right"
     )  # Rotate labels for better visibility
@@ -36,15 +47,18 @@
     ax.set_xlabel("Period")
 
     ax.set_title(title, fontsize=TITLE_FONT_SIZE, pad=15)
     plt.show()
     return fig, ax
 
 
-def plot_load_and_generation(participant_res: ParticipantsResultContainer):
+def plot_load_and_generation(participant_res: SystemParticipantsResultContainer):
+    """
+    Plots the energy consumption and generation of each participant type.
+    """
     lg_dict = participant_res.load_and_generation_energies()
     keys = []
     load = []
     generation = []
     for key, load_generation in lg_dict.items():
         keys.append(key)
         load.append(load_generation[0])
@@ -57,31 +71,28 @@
 
     bars_generation = axs[0].barh(
         keys,
         generation,
         align="center",
         color=PV_COLOR,
         edgecolor=PV_COLOR,
-        alpha=0.7,
         zorder=10,
     )
     axs[0].set_title("Generation", fontsize=TITLE_FONT_SIZE, pad=15)
     axs[0].set_xlim(left=-x_lim)
     axs[0].bar_label(
         bars_generation,
         padding=4,
         labels=[f"{x:,.0f}" for x in bars_generation.datavalues],
     )
     axs[0].get_xaxis().set_major_formatter(
         FuncFormatter(lambda x, p: format(int(x), ","))
     )
 
-    bars_load = axs[1].barh(
-        keys, load, align="center", color=LOAD_COLOR, alpha=0.7, zorder=10
-    )
+    bars_load = axs[1].barh(keys, load, align="center", color=LOAD_COLOR, zorder=10)
     axs[1].bar_label(
         bars_load, padding=4, labels=[f"{x:,.0f}" for x in bars_load.datavalues]
     )
     axs[1].set_title("Load", fontsize=TITLE_FONT_SIZE, pad=15)
     axs[1].set_xlim(right=x_lim)
     axs[1].get_xaxis().set_major_formatter(
         FuncFormatter(lambda x, p: format(int(x), ","))
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/common/line_plot.py` & `pypsdm-0.0.3/pypsdm/plots/common/line_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import logging
+from typing import Literal
 
+from loguru import logger
 from matplotlib.axes import Axes
 from pandas import Series
 
 from pypsdm.models.enums import EntitiesEnum
 from pypsdm.plots.common.utils import (
     FILL_ALPHA,
     add_to_kwargs_if_not_exist,
@@ -12,30 +13,33 @@
     set_date_format_and_label,
 )
 
 
 def ax_plot_time_series(
     ax: Axes,
     res: Series,
-    entity_type: EntitiesEnum,
-    resolution: str,
+    entity_type: EntitiesEnum | None = None,
     hourly_mean: bool = False,
     fill_from_index=False,
     fill_between=None,
     set_x_label: bool = True,
+    resolution: Literal["d", "w", "m", "y"] | None = None,
     **kwargs,
 ):
     args = get_label_and_color_dict(entity_type)
     kwargs = add_to_kwargs_if_not_exist(kwargs, args)
     if set_x_label:
-        set_date_format_and_label(ax, resolution)
+        if resolution is None:
+            set_date_format_and_label(ax, res.index)  # type: ignore
+        else:
+            set_date_format_and_label(ax, resolution)
     try:
         res = plot_resample(res, hourly_mean)
     except TypeError as e:
-        logging.warn(
+        logger.warning(
             f"Could not resample time series. Plotting without resampling. Error: {e}"
         )
     ax.plot(res, **kwargs)
     if fill_from_index:
         ax.fill_between(res.index, res, alpha=FILL_ALPHA, color=kwargs["color"])
     elif fill_between is not None:
         ax.fill_between(
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/common/style.py` & `pypsdm-0.0.3/pypsdm/plots/common/style.py`

 * *Files identical despite different names*

### Comparing `pypsdm-0.0.2/pypsdm/plots/common/utils.py` & `pypsdm-0.0.3/pypsdm/plots/common/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os.path
-from typing import Dict, NewType, Sequence, Tuple
+from typing import Dict, Literal, NewType, Sequence, Tuple
 
+import pandas as pd
 import seaborn as sns
 from matplotlib import dates as mdates
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from pandas import Series
 
 from pypsdm.models.enums import (
@@ -44,15 +45,15 @@
 RESIDUAL_LOAD_COLOR = LIGHT_BLUE
 UNKNOWN_COLOR = GREY
 FLEX_MAX = BLUE
 FLEX_MIN = GREEN
 FLEX_REF = YELLOW
 
 
-def get_label_and_color(sp_type: EntitiesEnum) -> Tuple[str, RGB]:
+def get_label_and_color(sp_type: EntitiesEnum | None) -> Tuple[str, RGB]:
     match sp_type:
         case RawGridElementsEnum.NODE:
             return "Node", NODE_COLOR
         case RawGridElementsEnum.TRANSFORMER_2_W:
             return "Transformer", TRANSFORMER_COLOR
         case RawGridElementsEnum.LINE:
             return "Line", LINE_COLOR
@@ -71,20 +72,20 @@
         case SystemParticipantsEnum.ENERGY_MANAGEMENT:
             return "Energy Management", LOAD_COLOR
         case SystemParticipantsEnum.PARTICIPANTS_SUM:
             return "Participants Sum", LOAD_COLOR
         case SystemParticipantsEnum.PRIMARY_DATA:
             return "Primary Data", LOAD_COLOR
         case _:
-            return sp_type.value, UNKNOWN_COLOR
+            return "", BLUE
 
 
-def get_label_and_color_dict(sp_type: EntitiesEnum):
+def get_label_and_color_dict(sp_type: EntitiesEnum | None):
     label, color = get_label_and_color(sp_type)
-    return {"label": label, "color": color}
+    return {"label": label, "color": color} if label else {"color": color}
 
 
 # === FIGURE DEFAULTS ===
 
 FIGSIZE = (12, 4)
 FIGSIZE_WIDE = (15, 4)
 SUBPLOTS_PADDING = 10
@@ -98,30 +99,34 @@
 TITLE_PAD = 15
 LABEL_PAD = 10
 
 # === SHADING ===
 
 FILL_ALPHA = 0.2
 
+Resolution = Literal["d", "w", "m", "y"]
+
 
 def save_fig(figure: Figure, path: str, file_name: str, format="svg"):
     figure.savefig(os.path.join(path, file_name), bbox_inches="tight", format=format)
 
 
 def plot_resample(res: Series, hourly_mean: bool):
     return (
         res.resample("60S").ffill()
         if not hourly_mean
         # todo: check the resample 60s
         else hourly_mean_resample(res).resample("60S").ffill()
     )
 
 
-def set_date_format_and_label(ax: Axes, resolution: str):
+def set_date_format_and_label(ax: Axes, resolution: str | pd.DatetimeIndex):
     possible_resolutions = set(["d", "w", "m", "y"])
+    if isinstance(resolution, pd.DatetimeIndex):
+        resolution = determine_resolution(resolution)
     if resolution not in possible_resolutions:
         raise ValueError(
             f"Invalid resolution: '{resolution}' (possible: {possible_resolutions}"
         )
     date_format, x_label = _date_format_and_x_label(resolution)
     ax.set_xlabel(x_label)
     if resolution == "y":
@@ -131,14 +136,27 @@
     if resolution == "m":
         locator = mdates.WeekdayLocator()
         ax.get_xaxis().set_major_locator(locator)
     ax.xaxis.set_major_formatter(mdates.DateFormatter(date_format))
     ax.xaxis.set_minor_formatter(mdates.DateFormatter(date_format))
 
 
+def determine_resolution(ts_index: pd.DatetimeIndex) -> str:
+    total_days = (ts_index.max() - ts_index.min()).days
+
+    if total_days <= 1:
+        return "d"
+    elif total_days <= 7:
+        return "w"
+    elif total_days <= 30:
+        return "m"
+    else:
+        return "y"
+
+
 def _date_format_and_x_label(resolution: str) -> Tuple[str, str]:
     if resolution == "d":
         return "%H:%M", "Time in h"
     elif resolution == "w":
         return "%a", "Day of Week"
     elif resolution == "m":
         return "%x", "Day of Month"
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/grid.py` & `pypsdm-0.0.3/pypsdm/plots/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
             raise ValueError(
                 f"Node with uuid: {node_data.name} not found in node_hover_data"
             )
 
         return (
             node_data["id"]
             + "<br>"
+            + node_data.name
+            + "<br>"
             + "<br>".join(
                 [
                     f"{key}={value}"
                     for key, value in node_hover_data[node_data.name].items()
                 ]
             )
         )
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/results/connector_plot.py` & `pypsdm-0.0.3/pypsdm/plots/results/connector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,325 +1,254 @@
-import logging
-from typing import Optional, Union
+from typing import Literal, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.axes import Axes
 
+from pypsdm.models.enums import EntitiesEnum, RawGridElementsEnum
 from pypsdm.models.gwr import GridWithResults
-from pypsdm.models.input.connector.lines import Lines
-from pypsdm.models.result.grid.connector import ConnectorResult
+from pypsdm.models.result.grid.connector import ConnectorCurrent
 from pypsdm.models.result.grid.transformer import Transformer2WResult
+from pypsdm.models.ts.base import EntityKey
 from pypsdm.plots.common.line_plot import ax_plot_time_series
 from pypsdm.plots.common.utils import (
     BLUE,
     FIGSIZE,
-    ax_plot_secondary_axis,
+    Resolution,
     set_subplot_title,
     set_suptitle,
     set_title,
 )
 
 
 def plot_transformer_s(
+    trafo_key: str | EntityKey,
     res: Transformer2WResult,
-    side: str,
     gwr: GridWithResults,
-    resolution: str,
+    side: Literal["hv", "lv"] = "hv",
     include_utilisation: bool = True,
-    show_util_grid_lines: bool = False,
     title: Optional[str] = None,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
-    transformer_name = res.name if res.name else res.input_model
-    if title is None:
-        title = f"Rated Power Transformer: {transformer_name}"
+    if isinstance(trafo_key, EntityKey):
+        name = trafo_key.id
+    else:
+        name = trafo_key
+    title = f"Rated Power Transformer: {name}"
     if include_utilisation:
         width, height = FIGSIZE
         fig, axs = plt.subplots(2, 1, figsize=(width, height * 2), sharex=False)
         ax_plot_transformer_s(
             axs[0],
+            trafo_key,
             res,
-            side,
             gwr,
-            resolution,
+            side=side,
             fill_from_index=fill_from_index,
             fill_between=fill_between,
             set_x_label=set_x_label,
+            resolution=resolution,
             **kwargs,
         )
         set_subplot_title(axs[0], "Rated Power Magnitude")
         ax_plot_transformer_utilization(
             axs[1],
+            trafo_key,
             res,
-            side,
             gwr,
-            resolution,
+            side=side,
             fill_from_index=fill_from_index,
             fill_between=fill_between,
             set_x_label=False,
             color=BLUE,
+            resolution=resolution,
             **kwargs,
         )
         set_subplot_title(axs[1], "Transformer Utilization")
         fig.suptitle(title, fontsize=16)
         fig.subplots_adjust(hspace=0.4)
         return fig, axs
     else:
         fig, ax = plt.subplots(figsize=FIGSIZE)
         ax_plot_transformer_s(
             ax,
+            trafo_key,
             res,
-            side,
             gwr,
-            resolution,
+            sides=side,
             fill_from_index=fill_from_index,
             fill_between=fill_between,
             set_x_label=set_x_label,
+            resolution=resolution,
             **kwargs,
         )
         set_suptitle(fig, title)
         return fig, ax
 
 
 def ax_plot_transformer_s(
     ax: Axes,
+    trafo_key: str | EntityKey,
     res: Transformer2WResult,
-    side: str,
     gwr: GridWithResults,
-    resolution: str,
+    side: Literal["hv", "lv"],
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     if len(res.i_a_mag) == 0:
         raise ValueError("Transformer current time series is empty. No data to plot")
 
-    rated_power = res.calc_apparent_power_gwr(gwr, side).apply(lambda x: np.real(x))
+    rated_power = res.apparent_power(trafo_key, gwr, side).apply(lambda x: np.real(x))
     ax_plot_time_series(
         ax,
         rated_power,
-        res.entity_type,
-        resolution,
+        entity_type=RawGridElementsEnum.TRANSFORMER_2_W,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Rated Power in kVA")
 
 
 def ax_plot_transformer_utilization(
     ax: Axes,
+    trafo_key: str | EntityKey,
     res: Transformer2WResult,
-    side: str,
     gwr: GridWithResults,
-    resolution: str,
+    side: Literal["hv", "lv"] = "hv",
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     ax_plot_time_series(
         ax,
-        res.calc_transformer_utilisation(gwr, side),
-        res.entity_type,
-        resolution,
+        res.utilisation(trafo_key, gwr, side),
+        entity_type=RawGridElementsEnum.TRANSFORMER_2_W,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Transformer Utilization")
 
 
-def plot_line_current(
-    res: ConnectorResult,
-    side: str,
-    resolution: str,
-    include_utilisation: bool = False,
-    i_max_src: Optional[Union[float, Lines]] = None,
-    title: Optional[str] = None,
-    fill_from_index: bool = False,
-    fill_between=None,
-    set_x_label=True,
-    **kwargs,
-):
-    line_name = res.name if res.name else res.input_model
-    if title is None:
-        title = f"Current Magnitude Line: {line_name}"
-    fig, ax = plt.subplots(figsize=FIGSIZE)
-    ax_plot_line_current(
-        ax,
-        res,
-        side,
-        resolution,
-        i_max_src=i_max_src,
-        include_utilisation=include_utilisation,
-        fill_from_index=fill_from_index,
-        fill_between=fill_between,
-        set_x_label=set_x_label,
-        **kwargs,
-    )
-    ax.set_ylabel("Current in Ampere")
-    set_title(ax, title)
-    return fig, ax
-
-
-def ax_plot_line_current(
-    ax: Axes,
-    res: ConnectorResult,
-    side: str,
-    resolution: str,
-    include_utilisation: bool = True,
-    i_max_src: Optional[Union[float, Lines]] = None,
-    fill_from_index: bool = False,
-    fill_between=None,
-    set_x_label=True,
-    **kwargs,
-):
-    if len(res.i_a_mag) == 0:
-        raise ValueError("Line current time series is empty. No data to plot")
-
-    current = get_connector_current(side, res)
-
-    ax = ax_plot_time_series(
-        ax,
-        current,
-        res.entity_type,
-        resolution,
-        fill_from_index=fill_from_index,
-        fill_between=fill_between,
-        set_x_label=set_x_label,
-        **kwargs,
-    )
-    ax.set_ylabel("Current Magnitude in Ampere")
-
-    if include_utilisation:
-        if i_max_src is None:
-            logging.warning("No i_max_src provided. Cannot plot utilisation")
-            return
-        if isinstance(i_max_src, float) or isinstance(i_max_src, int):
-            line_i_max = i_max_src
-        elif isinstance(i_max_src, Lines):
-            line_i_max = i_max_src.subset(res.input_model).i_max.iloc[0]
-        else:
-            raise ValueError(
-                f"i_max_src should be either float or Lines, got {type(i_max_src)}"
-            )
-        utilisation = current / line_i_max
-        ax_plot_secondary_axis(
-            ax, utilisation, "Line Utilisation", show_secondary_grid_lines=True
-        )
-
-
 def plot_connector_current(
-    res: ConnectorResult,
-    side: str,
-    resolution: str,
+    res: ConnectorCurrent,
+    key: str | EntityKey | None = None,
+    side: Literal["a", "b"] = "a",
     title: Optional[str] = None,
+    entity_type: EntitiesEnum | None = None,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
-    connector_type = res.entity_type.get_plot_name()
-    connector_name = res.name if res.name else res.input_model
     if title is None:
-        title = f"Current Magnitude {connector_type}: {connector_name}"
+        if key is not None:
+            title = (
+                f"Current Magnitude: {key.id if isinstance(key, EntityKey) else key}"
+            )
+        else:
+            title = "Current Magnitude"
     fig, ax = plt.subplots(figsize=FIGSIZE)
     ax_plot_connector_current(
         ax,
         res,
-        side,
-        resolution,
+        side=side,
+        entity_type=entity_type,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Current in Ampere")
     set_title(ax, title)
     return fig, ax
 
 
 def ax_plot_connector_current(
     ax: Axes,
-    res: ConnectorResult,
-    side: str,
-    resolution: str,
+    res: ConnectorCurrent,
+    side: Literal["a", "b"] = "a",
+    entity_type: EntitiesEnum | None = None,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
-    connector_type = res.entity_type.get_plot_name()
     if len(res.i_a_mag) == 0:
-        raise ValueError(
-            f"{connector_type} current time series is empty. No data to plot"
-        )
+        raise ValueError("Connector current time series is empty. No data to plot")
 
     current = get_connector_current(side, res)
 
     ax = ax_plot_time_series(
         ax,
         current,
-        res.entity_type,
-        resolution,
+        entity_type=entity_type,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Current Magnitude in Ampere")
 
 
 def ax_plot_connector_angle(
     ax: Axes,
-    res: ConnectorResult,
-    side: str,
-    resolution: str,
+    res: ConnectorCurrent,
+    side: Literal["a", "b"] = "a",
+    entity_type: EntitiesEnum | None = None,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
-    connector_type = res.entity_type.get_plot_name()
     if len(res.i_a_mag) == 0:
-        raise ValueError(
-            f"{connector_type} angle time series is empty. No data to plot"
-        )
+        raise ValueError("Angle time series is empty. No data to plot")
 
     angle = get_connector_angle(side, res)
 
     ax = ax_plot_time_series(
         ax,
         angle,
-        res.entity_type,
-        resolution,
+        entity_type=entity_type,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
 
 
-def get_connector_current(side: str, res: ConnectorResult):
+def get_connector_current(side: Literal["a", "b"], res: ConnectorCurrent):
     if side == "a":
         return res.i_a_mag
     elif side == "b":
         return res.i_b_mag
     else:
         raise ValueError('Side should be either "a" for node a or "b" for node b')
 
 
-def get_connector_angle(side: str, res: ConnectorResult):
+def get_connector_angle(side: str, res: ConnectorCurrent):
     if side == "a":
         return res.i_a_ang
     elif side == "b":
         return res.i_b_ang
     else:
         raise ValueError('Side should be either "a" for node a or "b" for node b')
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/results/flex_plot.py` & `pypsdm-0.0.3/pypsdm/plots/results/flex.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,108 @@
 from functools import partial
 
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 
 from pypsdm.models.enums import SystemParticipantsEnum
-from pypsdm.models.result.container.participants import ParticipantsResultContainer
-from pypsdm.models.result.participant.flex_options import FlexOptionResult
-from pypsdm.models.result.power import PQResult
+from pypsdm.models.result.container.participants import (
+    SystemParticipantsResultContainer,
+)
+from pypsdm.models.result.participant.flex_options import FlexOption
+from pypsdm.models.ts.types import ComplexPower
 from pypsdm.plots.common.line_plot import ax_plot_time_series
 from pypsdm.plots.common.utils import (
     FIGSIZE,
     FLEX_MAX,
     FLEX_MIN,
     FLEX_REF,
     ORANGE,
+    Resolution,
     set_title,
 )
-from pypsdm.plots.results.power_plot import ax_plot_active_power
+from pypsdm.plots.results.power import ax_plot_active_power
 
 
 def plot_all_participants_flex_range(
-    participants_res_container: ParticipantsResultContainer,
-    resolution: str,
+    participants_res_container: SystemParticipantsResultContainer,
     title: str = "Participants Flex Range",
     hourly_mean: bool = False,
     include_actual_res=False,
+    resolution: Resolution | None = None,
 ):
-    em_res_list = [
-        res
-        for res in participants_res_container.to_list(
-            include_em=False, include_flex=False, include_empty=False
-        )
-        if res.entity_type != SystemParticipantsEnum.LOAD
-    ]
-    plot_count = len(em_res_list)
+
+    em_res_dict = {}
+    for entity_type, participant_res in participants_res_container.to_dict().items():
+        if not participant_res:
+            continue
+        if entity_type not in {
+            SystemParticipantsEnum.LOAD,
+            SystemParticipantsEnum.ENERGY_MANAGEMENT,
+            SystemParticipantsEnum.FLEX_OPTIONS,
+        }:
+            em_res_dict[entity_type] = participant_res
+    plot_count = len(em_res_dict)
 
     fig, axs = plt.subplots(plot_count, 1, figsize=(10, 11), sharex=True, sharey=False)
     fig.suptitle(title)
     plt.subplots_adjust(hspace=0.5)
 
-    for idx, participant_res in enumerate(em_res_list):
+    for idx, (entity_type, participant_res) in enumerate(em_res_dict.items()):
         participant_flex = participants_res_container.flex.subset(
-            participant_res.entities.keys()
+            participant_res.keys()
         )
         if participant_flex:
             flex_sum = participant_flex.sum()
             axs[idx].set_title(f"{participant_res.entity_type.get_plot_name()}")
-            ax_plot_flex_range(axs[idx], flex_sum, "d", hourly_mean=hourly_mean)
+            ax_plot_flex_range(
+                axs[idx], flex_sum, hourly_mean=hourly_mean, resolution=resolution
+            )
         if include_actual_res:
             ax_plot_active_power(
                 axs[idx],
                 participant_res.sum() * 1e3,
-                resolution,
                 hourly_mean=hourly_mean,
                 color=ORANGE,
                 label="p_actual",
+                resolution=resolution,
             )
         axs[idx].legend()
         axs[idx].set_ylabel("Power in kW")
 
     return fig, axs
 
 
 def plot_flex_range(
-    flex_option: FlexOptionResult,
+    flex_option: FlexOption,
     title: str,
-    resolution: str,
     hourly_mean: bool,
-    actual_res: PQResult | None = None,
+    actual_res: ComplexPower | None = None,
+    resolution: Resolution | None = None,
 ):
     figure, ax = plt.subplots(figsize=FIGSIZE)
     # plt.tight_layout()
-    ax_plot_flex_range(ax, flex_option, resolution, hourly_mean, actual_res)
+    ax_plot_flex_range(ax, flex_option, hourly_mean, actual_res, resolution=resolution)
     title = title if title else "Flex Options"
 
     set_title(ax, title)
     return figure, ax
 
 
 def ax_plot_flex_range(
     ax: Axes,
-    flex_option: FlexOptionResult,
-    resolution: str,
+    flex_option: FlexOption,
     hourly_mean: bool,
-    actual_res: PQResult | None = None,
+    actual_res: ComplexPower | None = None,
+    resolution: Resolution | None = None,
 ):
     p_ref = flex_option.p_ref() * 1e3
     plot_func = partial(
         ax_plot_time_series,
         ax=ax,
-        type=SystemParticipantsEnum.FLEX_OPTIONS,
+        entity_type=SystemParticipantsEnum.FLEX_OPTIONS,
         resolution=resolution,
         hourly_mean=hourly_mean,
     )
 
     plot_func(
         res=flex_option.p_max() * 1e3,
         label="p_max",
@@ -108,16 +117,16 @@
     )
     plot_func(res=p_ref, label="p_ref", color=FLEX_REF)
 
     if actual_res:
         ax_plot_active_power(
             ax,
             actual_res,
-            resolution,
             hourly_mean=hourly_mean,
             color=ORANGE,
             label="p_actual",
+            resolution=resolution,
         )
 
     ax.set_ylabel("Power in kW")
 
     ax.legend()
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/results/nodes.py` & `pypsdm-0.0.3/pypsdm/plots/results/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 
 from pypsdm.models.gwr import GridWithResults
 from pypsdm.plots.common.utils import FIGSIZE
-from pypsdm.plots.results.power_plot import ax_plot_nodal_ps_violin
-from pypsdm.plots.results.voltage_plot import ax_plot_v_mags_violin
+from pypsdm.plots.results.power import ax_plot_nodal_ps_violin
+from pypsdm.plots.results.voltage import ax_plot_v_mags_violin
 
 
 def voltage_power_along_branches_violin(gwr: GridWithResults):
     branches = gwr.grid.raw_grid.get_branches()
-    nodes_res = gwr.build_enhanced_nodes_result()
+    nodes_res = gwr.build_extended_nodes_result()
     width, height = FIGSIZE
     height = height * len(branches) * 2
     fig = plt.figure(figsize=(width, height))
     outer_grid = gridspec.GridSpec(len(branches), 1, wspace=0.2, hspace=0.3)
     inner_grids = []
     for i, branch in enumerate(branches):
         inner_grid = gridspec.GridSpecFromSubplotSpec(
```

### Comparing `pypsdm-0.0.2/pypsdm/plots/results/voltage_plot.py` & `pypsdm-0.0.3/pypsdm/plots/results/voltage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import math
 from datetime import datetime
-from typing import Optional, Union
+from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
-from pypsdm.models.result.grid.enhanced_node import EnhancedNodesResult
-from pypsdm.models.result.grid.node import NodeResult, NodesResult
+from pypsdm.models.enums import RawGridElementsEnum
+from pypsdm.models.ts.base import EntityKey
+from pypsdm.models.ts.mixins import ComplexVoltageDictMixin
+from pypsdm.models.ts.types import (
+    ComplexVoltage,
+    ComplexVoltageDict,
+    ComplexVoltagePowerDict,
+)
 from pypsdm.plots.common.line_plot import ax_plot_time_series
 from pypsdm.plots.common.utils import (
-    COLOR_PALETTE,
     FIGSIZE,
     LABEL_PAD,
+    Resolution,
     set_subplot_title,
+    set_suptitle,
     set_title,
     set_xlabels_rotated,
     set_ylabel,
 )
 
 
 def plot_all_v_mag_branch_violin(
-    nodes_res: Union[NodesResult, EnhancedNodesResult],
+    nodes_res: ComplexVoltageDictMixin,
     branches: list[list[str]],
+    title: str | None = None,
+    **kwargs,
 ):
     """
     Plots violin plots for all nodes across all branches.
     Branches of the grid can be retrieved by raw_grid.get_branches()
 
     Args:
         gwr: GridWithResults object
@@ -37,82 +46,99 @@
         fig, axes
     """
     width, height = FIGSIZE
     height = height * len(branches)
     fig, axes = plt.subplots(nrows=len(branches), figsize=(width, height))
     for i, branch in enumerate(branches):
         axs = axes[i] if len(branches) > 1 else axes
-        ax_plot_v_mags_violin(axs, nodes_res, branch)  # type: ignore
-        set_subplot_title(axs, f"Voltages along Branch {i+1}")
+        ax_plot_v_mags_violin(axs, nodes_res, branch, **kwargs)  # type: ignore
+        if len(branches) > 1:
+            set_subplot_title(axs, f"Voltages along Branch {i+1}")
+
+    if not title:
+        title = "Voltage Magnitudes along Branches"
+    set_suptitle(fig, title)
     plt.tight_layout()
+    plt.grid(True)
 
     return fig, axes
 
 
 def plot_v_mags_violin(
-    nodes_res: Union[NodesResult, EnhancedNodesResult],
-    nodes: Optional[list[str]] = None,
+    nodes_res: ComplexVoltageDict,
+    nodes: list[str] | None = None,
+    title: str | None = None,
+    **kwargs,
 ):
     """
     Plots violin plots for all given nodes .
 
     Args:
-        nodes_res: NodesResult or EnhancedNodesResult object
+        nodes_res: NodesResult or ExtendedNodesResult object
         nodes: Optional list of node uuids that should be plotted. Order is preserved.
 
     Returns:
         fig, ax
     """
     fig, ax = plt.subplots(figsize=FIGSIZE)
-    ax_plot_v_mags_violin(ax, nodes_res, nodes)
-    set_title(ax, "Voltage Magnitudes along Branch")
+    ax_plot_v_mags_violin(ax, nodes_res, nodes, **kwargs)
+
+    if not title:
+        title = "Voltage Magnitudes"
+    set_title(ax, title)
     return fig, ax
 
 
 def ax_plot_v_mags_violin(
     ax: Axes,
-    nodes_res: Union[NodesResult, EnhancedNodesResult],
+    nodes_res: ComplexVoltageDict,
     nodes: Optional[list[str]],  # branches can be found by GridContainer.get_branches()
+    **kwargs,
 ):
     """
     Plots violin plots for given nodes. If no nodes are passed all nodes are plotted.
 
     Args:
         ax: Axes object
-        nodes_res: NodesResult or EnhancedNodesResult object
+        nodes_res: NodesResult or ExtendedNodesResult object
         nodes: Optional list of node uuids that should be plotted. Order is preserved.
     """
 
     if nodes:
         # get v_mag in listed sequence
-        v_mag = nodes_res.subset(nodes).v_mag.reindex(columns=nodes)
+        v_mag = nodes_res.subset(nodes).v_mag(favor_ids=False).reindex(columns=nodes)
+        uuid_id_map = {k.uuid: k.id for k in nodes_res.keys()}
+        v_mag.columns = [uuid_id_map[col] for col in v_mag.columns]
     else:
-        v_mag = nodes_res.v_mag
+        v_mag = nodes_res.v_mag()
+
+    data = []
+    for col in v_mag.columns:
+        data.append(v_mag[col].dropna().values)
 
-    sns.violinplot(v_mag, showmedians=True, ax=ax, linewidth=0.5, palette=COLOR_PALETTE)
+    ax.violinplot(data, **kwargs)
 
     # set labels
-    uuid_to_id = nodes_res.uuid_to_id_map()
-    x_labels = v_mag.columns.map(lambda uuid: uuid_to_id[uuid])
+    x_labels = v_mag.columns
     set_xlabels_rotated(ax, list(x_labels), ha="right")
     set_ylabel(ax, "Voltage magnitude in pu")
     _ = ax.set_xticklabels(x_labels, rotation=45, ha="right")
 
 
 def plot_v_mag_branch(
-    nodes_res: Union[NodesResult, EnhancedNodesResult],
+    nodes_res: ComplexVoltageDict,
     branch: list[str],  # branches can be found by GridContainer.get_branches()
     time: datetime,
     in_kw: bool = False,
 ):
     """
     Plots voltage magnitudes of nodes along the given branch.
 
     Args:
-        nodes_res: NodesResult or EnhancedNodesResult object
+        nodes_res: NodesResult or ExtendedNodesResult object
         branch: list of node uuids that form the branch
         time: datetime for which the voltage magnitudes should be plotted
         in_kw: if True, power is plotted in kW instead of MW
 
     Returns:
         fig, ax
     """
@@ -120,33 +146,33 @@
     ax_plot_v_mag_branch(ax, nodes_res, branch, time, fig=fig, in_kw=in_kw)
     set_title(ax, "Voltage Magnitudes along Branch")
     return fig, ax
 
 
 def ax_plot_v_mag_branch(
     ax: Axes,
-    nodes_res: Union[NodesResult, EnhancedNodesResult],
+    nodes_res: ComplexVoltageDict,
     branch: list[str],
     time: datetime,
     fig: Optional[Figure] = None,  # used to plot colorbar
     in_kw: bool = False,
 ):
     """
     Plots voltage magnitudes of nodes along the given branch.
 
     Args:
         ax: Axes object
-        nodes_res: NodesResult or EnhancedNodesResult object
+        nodes_res: NodesResult or ExtendedNodesResult object
         branch: list of node uuids that form the branch
         time: datetime for which the voltage magnitudes should be plotted
         fig: Optional Figure object which is used to plot the colorbar
         in_kw: if True, power is plotted in kW instead of MW
     """
 
-    with_power = isinstance(nodes_res, EnhancedNodesResult)
+    with_power = isinstance(nodes_res, ComplexVoltagePowerDict)
 
     v_mags = []
     x_ticks = []
     p_s = []
 
     for node in branch:
         node_res = nodes_res[node]
@@ -176,106 +202,116 @@
         if fig:
             cbar = fig.colorbar(sc, ax=ax)
             unit = "kW" if in_kw else "MW"
             cbar.set_label(f"Nodal Power in {unit}", labelpad=LABEL_PAD)
 
 
 def plot_v_mag(
-    res: NodeResult,
-    resolution: str,
+    res: ComplexVoltage,
+    name: EntityKey | str | None = None,
     title: Optional[str] = None,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     if title is None:
-        title = f"Voltage Magnitude at Node: {res.name}"
+        if name:
+            name = name if isinstance(name, str) else name.id
+            title = f"Voltage Magnitude at Node: {name}"
+        else:
+            title = "Voltage Magnitude"
     fig, ax = plt.subplots(figsize=FIGSIZE)
     ax_plot_node_v_mag(
         ax,
         res,
-        resolution,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     set_title(ax, title)
     return fig, ax
 
 
 def plot_v_ang(
-    res: NodeResult,
-    resolution: str,
+    res: ComplexVoltage,
+    name: EntityKey | str | None = None,
     title: Optional[str] = None,
     hourly_mean: bool = False,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     if title is None:
-        title = f"Voltage Angle at Node: {res.name}"
+        if name:
+            name = name if isinstance(name, str) else name.id
+            title = f"Voltage Magnitude at Node: {name}"
+        else:
+            title = "Voltage Magnitude"
     fig, ax = plt.subplots(figsize=FIGSIZE)
     ax_plot_node_v_ang(
         ax,
         res,
-        resolution,
         hourly_mean=hourly_mean,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     set_title(ax, title)
     return fig, ax
 
 
 def ax_plot_node_v_mag(
     ax: Axes,
-    res: NodeResult,
-    resolution: str,
+    res: ComplexVoltage,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     if len(res.v_mag) == 0:
         raise ValueError("Voltage magnitude time series is empty. No data to plot")
 
     ax = ax_plot_time_series(
         ax,
         res.v_mag,
-        res.entity_type,
-        resolution,
+        entity_type=RawGridElementsEnum.NODE,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Voltage Magnitude in p.u.")
 
 
 def ax_plot_node_v_ang(
     ax: Axes,
-    res: NodeResult,
-    resolution: str,
+    res: ComplexVoltage,
     fill_from_index: bool = False,
     fill_between=None,
     set_x_label=True,
+    resolution: Resolution | None = None,
     **kwargs,
 ):
     if len(res.v_ang) == 0:
         raise ValueError("Voltage angle time series is empty. No data to plot")
 
     ax = ax_plot_time_series(
         ax,
         res.v_ang,
-        res.entity_type,
-        resolution,
+        entity_type=RawGridElementsEnum.NODE,
         fill_from_index=fill_from_index,
         fill_between=fill_between,
         set_x_label=set_x_label,
+        resolution=resolution,
         **kwargs,
     )
     ax.set_ylabel("Voltage Angle in deg")
```

### Comparing `pypsdm-0.0.2/pypsdm/processing/series.py` & `pypsdm-0.0.3/pypsdm/processing/series.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Tuple
 
 import pandas as pd
 from pandas import DataFrame, Series
 
+from pypsdm.processing.numba import add_array
+
 
 def duration_weighted_series(series: Series):
     series.sort_index(inplace=True)
     values = series[:-1].reset_index(drop=True)
     time = (
         (series.index[1::] - series.index[:-1])
         .to_series()
@@ -20,26 +22,30 @@
     if len(weighted_series) == 0:
         return 0.0
     return (weighted_series["values"] * weighted_series["time"]).sum()
 
 
 def duration_weighted_sum(series: Series) -> float:
     weighted_series = duration_weighted_series(series)
-
     return weighted_series_sum(weighted_series)
 
 
-def add_series(this: Series, that: Series, name: str) -> Series:
-    # todo: Is there a more performant implementation?
+def add_series(a: pd.Series, b: pd.Series, name: str | None = None):
+    if not a.index.is_monotonic_increasing:
+        a.sort_index(inplace=True)
+    if not b.index.is_monotonic_increasing:
+        b.sort_index(inplace=True)
+    index = a.index.union(b.index)
+    values = add_array(
+        index.to_numpy(), a.index.to_numpy(), b.index.to_numpy(), a.values, b.values  # type: ignore
+    )
     return (
-        this.to_frame()
-        .join(that.rename("other"), how="outer")
-        .fillna(method="ffill")
-        .sum(axis=1)
-        .rename(name)
+        pd.Series(values, index=index)
+        if name is None
+        else pd.Series(values, index=index, name=name)
     )
 
 
 def join_series(series: list[Series]) -> DataFrame:
     first_series = series[0]
     df = first_series.rename(first_series.name).to_frame()
     for series in series[1:]:
@@ -47,15 +53,18 @@
     return df
 
 
 def hourly_mean_resample(series: Series) -> Series:
     return series.resample("60s").ffill().resample("1h").mean()
 
 
-def load_and_generation(p_ts: Series) -> Tuple[float, float]:
+def pos_and_neg_area(p_ts: Series) -> Tuple[float, float]:
+    """
+    Calculate the positive and negative area under the curve of a time series.
+    """
     weighted_series = duration_weighted_series(p_ts)
     load_filter = weighted_series["values"] > 0
     weighted_load = weighted_series[load_filter]
     weighted_generation = weighted_series[~load_filter]
     return (
         weighted_series_sum(weighted_load),
         weighted_series_sum(weighted_generation),
```

### Comparing `pypsdm-0.0.2/PKG-INFO` & `pypsdm-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: pypsdm
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
 Requires-Python: >3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: black[jupyter] (>=24.1.1,<24.2.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>1.2,<2.1)
 Requires-Dist: plotly (>=5.6.0,<6.0.0)
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: pyhocon (>=0.3.60,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: seaborn (==0.13)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
+Requires-Dist: sqlmodel (>=0.0.14,<0.0.15)
 Description-Content-Type: text/markdown
 
 # pypsdm
 
 pypsdm aims to make power system model analysis a breeze. It is based upon the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel). 
 
 Its main functionalities include:
```

