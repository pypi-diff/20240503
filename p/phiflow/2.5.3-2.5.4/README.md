# Comparing `tmp/phiflow-2.5.3.tar.gz` & `tmp/phiflow-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\phiflow-2.5.3.tar", last modified: Sun Nov 26 12:17:02 2023, max compression
+gzip compressed data, was "dist\phiflow-2.5.4.tar", last modified: Fri May  3 11:59:59 2024, max compression
```

## Comparing `phiflow-2.5.3.tar` & `phiflow-2.5.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.234617 phiflow-2.5.3/
--rw-rw-rw-   0        0        0       95 2022-04-20 10:42:57.000000 phiflow-2.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2505 2023-11-26 12:17:02.234617 phiflow-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     8724 2023-11-26 12:16:26.000000 phiflow-2.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.757184 phiflow-2.5.3/phi/
--rw-rw-rw-   0        0        0        5 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/VERSION
--rw-rw-rw-   0        0        0     2019 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/__init__.py
--rw-rw-rw-   0        0        0     1390 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/_troubleshoot.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.834254 phiflow-2.5.3/phi/field/
--rw-rw-rw-   0        0        0     2408 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/__init__.py
--rw-rw-rw-   0        0        0     2503 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_angular_velocity.py
--rw-rw-rw-   0        0        0     3559 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_embed.py
--rw-rw-rw-   0        0        0    19915 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/field/_field.py
--rw-rw-rw-   0        0        0     5139 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_field_io.py
--rw-rw-rw-   0        0        0    42366 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_field_math.py
--rw-rw-rw-   0        0        0    33850 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/field/_grid.py
--rw-rw-rw-   0        0        0     1588 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_mask.py
--rw-rw-rw-   0        0        0     4956 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_mesh.py
--rw-rw-rw-   0        0        0     2839 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_noise.py
--rw-rw-rw-   0        0        0    12591 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/field/_point_cloud.py
--rw-rw-rw-   0        0        0    22014 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/field/_scene.py
--rw-rw-rw-   0        0        0     1559 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/flow.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.900314 phiflow-2.5.3/phi/geom/
--rw-rw-rw-   0        0        0      567 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/__init__.py
--rw-rw-rw-   0        0        0    21650 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_box.py
--rw-rw-rw-   0        0        0    19955 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_geom.py
--rw-rw-rw-   0        0        0    10187 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_poly_surface.py
--rw-rw-rw-   0        0        0     4464 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_sphere.py
--rw-rw-rw-   0        0        0     3945 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_stack.py
--rw-rw-rw-   0        0        0     7619 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_transform.py
--rw-rw-rw-   0        0        0     3474 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/geom/_union.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.915327 phiflow-2.5.3/phi/jax/
--rw-rw-rw-   0        0        0      327 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/jax/__init__.py
--rw-rw-rw-   0        0        0      907 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/jax/flow.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.929339 phiflow-2.5.3/phi/jax/stax/
--rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/jax/stax/__init__.py
--rw-rw-rw-   0        0        0      797 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/jax/stax/flow.py
--rw-rw-rw-   0        0        0      335 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/jax/stax/nets.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.934345 phiflow-2.5.3/phi/math/
--rw-rw-rw-   0        0        0      361 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/math/__init__.py
--rw-rw-rw-   0        0        0      123 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/math/backend.py
--rw-rw-rw-   0        0        0      150 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/math/extrapolation.py
--rw-rw-rw-   0        0        0      126 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/math/magic.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.961369 phiflow-2.5.3/phi/physics/
--rw-rw-rw-   0        0        0      480 2023-02-26 20:09:34.000000 phiflow-2.5.3/phi/physics/__init__.py
--rw-rw-rw-   0        0        0    18296 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/physics/_boundaries.py
--rw-rw-rw-   0        0        0     8611 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/physics/advect.py
--rw-rw-rw-   0        0        0     5387 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/physics/diffuse.py
--rw-rw-rw-   0        0        0    15607 2023-11-26 12:16:26.000000 phiflow-2.5.3/phi/physics/fluid.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:01.983390 phiflow-2.5.3/phi/tf/
--rw-rw-rw-   0        0        0      368 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/tf/__init__.py
--rw-rw-rw-   0        0        0     1170 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/tf/flow.py
--rw-rw-rw-   0        0        0      338 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/tf/nets.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.002406 phiflow-2.5.3/phi/torch/
--rw-rw-rw-   0        0        0      349 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/torch/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/torch/flow.py
--rw-rw-rw-   0        0        0      332 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/torch/nets.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.064463 phiflow-2.5.3/phi/vis/
--rw-rw-rw-   0        0        0     1150 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.095491 phiflow-2.5.3/phi/vis/_console/
--rw-rw-rw-   0        0        0       36 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_console/__init__.py
--rw-rw-rw-   0        0        0     6865 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_console/_console_gui.py
--rw-rw-rw-   0        0        0     3144 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_console/_console_plot.py
--rw-rw-rw-   0        0        0     2360 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_console/_console_util.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.191578 phiflow-2.5.3/phi/vis/_dash/
--rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/__init__.py
--rw-rw-rw-   0        0        0    21721 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_dash/_plotly_plots.py
--rw-rw-rw-   0        0        0     7826 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/board.py
--rw-rw-rw-   0        0        0     4218 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_dash/colormaps.py
--rw-rw-rw-   0        0        0     2954 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/dash_app.py
--rw-rw-rw-   0        0        0     7104 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_dash/dash_gui.py
--rw-rw-rw-   0        0        0     2075 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/info.py
--rw-rw-rw-   0        0        0     1228 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/log.py
--rw-rw-rw-   0        0        0     5359 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_dash/model_controls.py
--rw-rw-rw-   0        0        0     3493 2023-04-20 17:29:41.000000 phiflow-2.5.3/phi/vis/_dash/player_controls.py
--rw-rw-rw-   0        0        0     2710 2023-02-26 20:09:34.000000 phiflow-2.5.3/phi/vis/_dash/viewer.py
--rw-rw-rw-   0        0        0     5892 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_dash/viewsettings.py
--rw-rw-rw-   0        0        0     2291 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_io.py
--rw-rw-rw-   0        0        0     3371 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_log.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.215599 phiflow-2.5.3/phi/vis/_matplotlib/
--rw-rw-rw-   0        0        0      108 2023-02-26 20:09:34.000000 phiflow-2.5.3/phi/vis/_matplotlib/__init__.py
--rw-rw-rw-   0        0        0    36276 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_matplotlib/_matplotlib_plots.py
--rw-rw-rw-   0        0        0     7572 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_matplotlib/_scalars.py
--rw-rw-rw-   0        0        0     1558 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_plot_util.py
--rw-rw-rw-   0        0        0     7184 2022-04-20 10:42:57.000000 phiflow-2.5.3/phi/vis/_user_namespace.py
--rw-rw-rw-   0        0        0    10708 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_viewer.py
--rw-rw-rw-   0        0        0    30805 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_vis.py
--rw-rw-rw-   0        0        0    18977 2023-08-30 13:48:12.000000 phiflow-2.5.3/phi/vis/_vis_base.py
-drwxrwxrwx   0        0        0        0 2023-11-26 12:17:02.233617 phiflow-2.5.3/phiflow.egg-info/
--rw-rw-rw-   0        0        0     2505 2023-11-26 12:17:01.000000 phiflow-2.5.3/phiflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1806 2023-11-26 12:17:01.000000 phiflow-2.5.3/phiflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-26 12:17:01.000000 phiflow-2.5.3/phiflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-11-26 12:17:01.000000 phiflow-2.5.3/phiflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-11-26 12:17:01.000000 phiflow-2.5.3/phiflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-11-26 12:17:02.236619 phiflow-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2068 2023-11-26 12:16:26.000000 phiflow-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:59.020045 phiflow-2.5.4/
+-rw-rw-rw-   0        0        0       95 2022-04-20 10:42:57.000000 phiflow-2.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2505 2024-05-03 11:59:59.020045 phiflow-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8724 2023-11-26 12:16:26.000000 phiflow-2.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.925960 phiflow-2.5.4/phi/
+-rw-rw-rw-   0        0        0        5 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/VERSION
+-rw-rw-rw-   0        0        0     2019 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/_troubleshoot.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.938971 phiflow-2.5.4/phi/field/
+-rw-rw-rw-   0        0        0     2408 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/__init__.py
+-rw-rw-rw-   0        0        0     2503 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_angular_velocity.py
+-rw-rw-rw-   0        0        0     3559 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_embed.py
+-rw-rw-rw-   0        0        0    19915 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/field/_field.py
+-rw-rw-rw-   0        0        0     5139 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_field_io.py
+-rw-rw-rw-   0        0        0    42366 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_field_math.py
+-rw-rw-rw-   0        0        0    33850 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/field/_grid.py
+-rw-rw-rw-   0        0        0     1588 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_mask.py
+-rw-rw-rw-   0        0        0     4956 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_mesh.py
+-rw-rw-rw-   0        0        0     2839 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/field/_noise.py
+-rw-rw-rw-   0        0        0    12622 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/field/_point_cloud.py
+-rw-rw-rw-   0        0        0    21938 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/field/_scene.py
+-rw-rw-rw-   0        0        0     1559 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/flow.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.947979 phiflow-2.5.4/phi/geom/
+-rw-rw-rw-   0        0        0      567 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/__init__.py
+-rw-rw-rw-   0        0        0    21650 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/_box.py
+-rw-rw-rw-   0        0        0    19955 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/_geom.py
+-rw-rw-rw-   0        0        0    10187 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/_poly_surface.py
+-rw-rw-rw-   0        0        0     4532 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/geom/_sphere.py
+-rw-rw-rw-   0        0        0     3936 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/geom/_stack.py
+-rw-rw-rw-   0        0        0     7619 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/_transform.py
+-rw-rw-rw-   0        0        0     3474 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/geom/_union.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.949983 phiflow-2.5.4/phi/jax/
+-rw-rw-rw-   0        0        0      327 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/jax/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/jax/flow.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.951984 phiflow-2.5.4/phi/jax/stax/
+-rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/jax/stax/__init__.py
+-rw-rw-rw-   0        0        0      797 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/jax/stax/flow.py
+-rw-rw-rw-   0        0        0      335 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/jax/stax/nets.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.955988 phiflow-2.5.4/phi/math/
+-rw-rw-rw-   0        0        0      361 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/math/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/math/backend.py
+-rw-rw-rw-   0        0        0      150 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/math/extrapolation.py
+-rw-rw-rw-   0        0        0      126 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/math/magic.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.960991 phiflow-2.5.4/phi/physics/
+-rw-rw-rw-   0        0        0      480 2023-02-26 20:09:34.000000 phiflow-2.5.4/phi/physics/__init__.py
+-rw-rw-rw-   0        0        0    18296 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/physics/_boundaries.py
+-rw-rw-rw-   0        0        0     8611 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/physics/advect.py
+-rw-rw-rw-   0        0        0     5387 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/physics/diffuse.py
+-rw-rw-rw-   0        0        0    15607 2023-11-26 12:16:26.000000 phiflow-2.5.4/phi/physics/fluid.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.962994 phiflow-2.5.4/phi/tf/
+-rw-rw-rw-   0        0        0      368 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/tf/__init__.py
+-rw-rw-rw-   0        0        0     1170 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/tf/flow.py
+-rw-rw-rw-   0        0        0      338 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/tf/nets.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.965996 phiflow-2.5.4/phi/torch/
+-rw-rw-rw-   0        0        0      349 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/torch/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/torch/flow.py
+-rw-rw-rw-   0        0        0      332 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/torch/nets.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.974003 phiflow-2.5.4/phi/vis/
+-rw-rw-rw-   0        0        0     1150 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.979007 phiflow-2.5.4/phi/vis/_console/
+-rw-rw-rw-   0        0        0       36 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_console/__init__.py
+-rw-rw-rw-   0        0        0     6865 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_console/_console_gui.py
+-rw-rw-rw-   0        0        0     3144 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_console/_console_plot.py
+-rw-rw-rw-   0        0        0     2360 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_console/_console_util.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.991019 phiflow-2.5.4/phi/vis/_dash/
+-rw-rw-rw-   0        0        0        0 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/__init__.py
+-rw-rw-rw-   0        0        0    21721 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_dash/_plotly_plots.py
+-rw-rw-rw-   0        0        0     7826 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/board.py
+-rw-rw-rw-   0        0        0     4218 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_dash/colormaps.py
+-rw-rw-rw-   0        0        0     2954 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/dash_app.py
+-rw-rw-rw-   0        0        0     7104 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_dash/dash_gui.py
+-rw-rw-rw-   0        0        0     2075 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/info.py
+-rw-rw-rw-   0        0        0     1228 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/log.py
+-rw-rw-rw-   0        0        0     5359 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_dash/model_controls.py
+-rw-rw-rw-   0        0        0     3493 2023-04-20 17:29:41.000000 phiflow-2.5.4/phi/vis/_dash/player_controls.py
+-rw-rw-rw-   0        0        0     2710 2023-02-26 20:09:34.000000 phiflow-2.5.4/phi/vis/_dash/viewer.py
+-rw-rw-rw-   0        0        0     5892 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_dash/viewsettings.py
+-rw-rw-rw-   0        0        0     2291 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_io.py
+-rw-rw-rw-   0        0        0     3371 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_log.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:58.994021 phiflow-2.5.4/phi/vis/_matplotlib/
+-rw-rw-rw-   0        0        0      108 2023-02-26 20:09:34.000000 phiflow-2.5.4/phi/vis/_matplotlib/__init__.py
+-rw-rw-rw-   0        0        0    36276 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_matplotlib/_matplotlib_plots.py
+-rw-rw-rw-   0        0        0     7572 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_matplotlib/_scalars.py
+-rw-rw-rw-   0        0        0     1558 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_plot_util.py
+-rw-rw-rw-   0        0        0     7184 2022-04-20 10:42:57.000000 phiflow-2.5.4/phi/vis/_user_namespace.py
+-rw-rw-rw-   0        0        0    10708 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_viewer.py
+-rw-rw-rw-   0        0        0    30760 2024-05-03 11:59:29.000000 phiflow-2.5.4/phi/vis/_vis.py
+-rw-rw-rw-   0        0        0    18977 2023-08-30 13:48:12.000000 phiflow-2.5.4/phi/vis/_vis_base.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:59:59.019045 phiflow-2.5.4/phiflow.egg-info/
+-rw-rw-rw-   0        0        0     2505 2024-05-03 11:59:58.000000 phiflow-2.5.4/phiflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2024-05-03 11:59:58.000000 phiflow-2.5.4/phiflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 11:59:58.000000 phiflow-2.5.4/phiflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-03 11:59:58.000000 phiflow-2.5.4/phiflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-03 11:59:58.000000 phiflow-2.5.4/phiflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-03 11:59:59.022047 phiflow-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-03 11:59:29.000000 phiflow-2.5.4/setup.py
```

### Comparing `phiflow-2.5.3/PKG-INFO` & `phiflow-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phiflow
-Version: 2.5.3
+Version: 2.5.4
 Summary: Differentiable PDE solving framework for machine learning
 Home-page: https://github.com/tum-pbs/PhiFlow
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.5.3.tar.gz
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.5.4.tar.gz
 Description: # PhiFlow
         
         [**Homepage**](https://github.com/tum-pbs/PhiFlow)
         &nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
         &nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
         &nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
         &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
```

### Comparing `phiflow-2.5.3/README.md` & `phiflow-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/__init__.py` & `phiflow-2.5.4/phi/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/_troubleshoot.py` & `phiflow-2.5.4/phi/_troubleshoot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/__init__.py` & `phiflow-2.5.4/phi/field/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_angular_velocity.py` & `phiflow-2.5.4/phi/field/_angular_velocity.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_embed.py` & `phiflow-2.5.4/phi/field/_embed.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_field.py` & `phiflow-2.5.4/phi/field/_field.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_field_io.py` & `phiflow-2.5.4/phi/field/_field_io.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_field_math.py` & `phiflow-2.5.4/phi/field/_field_math.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_grid.py` & `phiflow-2.5.4/phi/field/_grid.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     def with_extrapolation(self, extrapolation: Extrapolation):
         return type(self)(self.values, extrapolation=extrapolation, bounds=self.bounds)
 
     def with_bounds(self, bounds: Box):
         return type(self)(self.values, extrapolation=self.extrapolation, bounds=bounds)
 
     def __value_attrs__(self):
-        return '_values', '_extrapolation'
+        return '_values',
 
     def __variable_attrs__(self):
-        return '_values',
+        return '_values', '_extrapolation'
 
     def __expand__(self, dims: Shape, **kwargs) -> 'Grid':
         return self.with_values(math.expand(self.values, dims, **kwargs))
 
     def __replace_dims__(self, dims: Tuple[str, ...], new_dims: Shape, **kwargs) -> 'Grid':
         for dim in dims:
             if dim in self._resolution:
```

### Comparing `phiflow-2.5.3/phi/field/_mask.py` & `phiflow-2.5.4/phi/field/_mask.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_mesh.py` & `phiflow-2.5.4/phi/field/_mesh.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_noise.py` & `phiflow-2.5.4/phi/field/_noise.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/field/_point_cloud.py` & `phiflow-2.5.4/phi/field/_point_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     def with_extrapolation(self, extrapolation: Extrapolation):
         return PointCloud(elements=self.elements, values=self.values, extrapolation=extrapolation, add_overlapping=self._add_overlapping, bounds=self._bounds)
 
     def with_bounds(self, bounds: Box):
         return PointCloud(elements=self.elements, values=self.values, extrapolation=self.extrapolation, add_overlapping=self._add_overlapping, bounds=bounds)
 
     def __value_attrs__(self):
-        return '_values', '_extrapolation'
+        return '_values', '_extrapolation', '_elements'
 
     def __variable_attrs__(self):
-        return '_values', '_elements'
+        return '_values', '_elements', '_extrapolation'
 
     def __expand__(self, dims: Shape, **kwargs) -> 'PointCloud':
         return self.with_values(expand(self.values, dims, **kwargs))
 
     def __replace_dims__(self, dims: Tuple[str, ...], new_dims: Shape, **kwargs) -> 'PointCloud':
         elements = math.rename_dims(self.elements, dims, new_dims)
         values = math.rename_dims(self.values, dims, new_dims)
```

### Comparing `phiflow-2.5.3/phi/field/_scene.py` & `phiflow-2.5.4/phi/field/_scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             return scenes[id]
         if id is None:
             paths = directory
         else:
             id = math.wrap(id)
             paths = math.map(lambda d, i: join(d, f"sim_{i:06d}"), directory, id)
         # test all exist
-        for path in math.flatten(paths, flatten_batch=True):
+        for path in math.flatten(wrap(paths), flatten_batch=True):
             if not isdir(path):
                 raise IOError(f"There is no scene at '{path}'")
         return Scene(paths)
 
     def subpath(self, name: str, create=False, create_parent=False) -> Union[str, tuple]:
         """
         Resolves the relative path `name` with this `Scene` as the root folder.
@@ -237,18 +237,15 @@
             if create_parent and not isdir(os.path.dirname(path)):
                 os.makedirs(os.path.dirname(path))
             if create and not isdir(path):
                 os.mkdir(path)
             return path
 
         result = math.map(single_subpath, self._paths)
-        if result.rank == 0:
-            return result.native()
-        else:
-            return result
+        return result
 
     def _init_properties(self):
         if self._properties is not None:
             return
 
         def read_json(path: str) -> dict:
             json_file = join(path, "description.json")
```

### Comparing `phiflow-2.5.3/phi/flow.py` & `phiflow-2.5.4/phi/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/__init__.py` & `phiflow-2.5.4/phi/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/_box.py` & `phiflow-2.5.4/phi/geom/_box.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/_geom.py` & `phiflow-2.5.4/phi/geom/_geom.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/_poly_surface.py` & `phiflow-2.5.4/phi/geom/_poly_surface.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/_sphere.py` & `phiflow-2.5.4/phi/geom/_sphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
     def scaled(self, factor: Union[float, Tensor]) -> 'Geometry':
         return Sphere(self.center, self.radius * factor)
 
     def __variable_attrs__(self):
         return '_center', '_radius'
 
+    def __value_attrs__(self):
+        return '_center', '_radius'
+
     def __getitem__(self, item):
         item = slicing_dict(self, item)
         return Sphere(self._center[_keep_vector(item)], self._radius[item])
 
     def push(self, positions: Tensor, outward: bool = True, shift_amount: float = 0) -> Tensor:
         raise NotImplementedError()
```

### Comparing `phiflow-2.5.3/phi/geom/_transform.py` & `phiflow-2.5.4/phi/geom/_transform.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/geom/_union.py` & `phiflow-2.5.4/phi/geom/_union.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/jax/flow.py` & `phiflow-2.5.4/phi/jax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/jax/stax/flow.py` & `phiflow-2.5.4/phi/jax/stax/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/physics/_boundaries.py` & `phiflow-2.5.4/phi/physics/_boundaries.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/physics/advect.py` & `phiflow-2.5.4/phi/physics/advect.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/physics/diffuse.py` & `phiflow-2.5.4/phi/physics/diffuse.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/physics/fluid.py` & `phiflow-2.5.4/phi/physics/fluid.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/tf/flow.py` & `phiflow-2.5.4/phi/tf/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/torch/flow.py` & `phiflow-2.5.4/phi/torch/flow.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/__init__.py` & `phiflow-2.5.4/phi/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_console/_console_gui.py` & `phiflow-2.5.4/phi/vis/_console/_console_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_console/_console_plot.py` & `phiflow-2.5.4/phi/vis/_console/_console_plot.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_console/_console_util.py` & `phiflow-2.5.4/phi/vis/_console/_console_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/_plotly_plots.py` & `phiflow-2.5.4/phi/vis/_dash/_plotly_plots.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/board.py` & `phiflow-2.5.4/phi/vis/_dash/board.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/colormaps.py` & `phiflow-2.5.4/phi/vis/_dash/colormaps.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/dash_app.py` & `phiflow-2.5.4/phi/vis/_dash/dash_app.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/dash_gui.py` & `phiflow-2.5.4/phi/vis/_dash/dash_gui.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/info.py` & `phiflow-2.5.4/phi/vis/_dash/info.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/log.py` & `phiflow-2.5.4/phi/vis/_dash/log.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/model_controls.py` & `phiflow-2.5.4/phi/vis/_dash/model_controls.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/player_controls.py` & `phiflow-2.5.4/phi/vis/_dash/player_controls.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/viewer.py` & `phiflow-2.5.4/phi/vis/_dash/viewer.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_dash/viewsettings.py` & `phiflow-2.5.4/phi/vis/_dash/viewsettings.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_io.py` & `phiflow-2.5.4/phi/vis/_io.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_log.py` & `phiflow-2.5.4/phi/vis/_log.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_matplotlib/_matplotlib_plots.py` & `phiflow-2.5.4/phi/vis/_matplotlib/_matplotlib_plots.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_matplotlib/_scalars.py` & `phiflow-2.5.4/phi/vis/_matplotlib/_scalars.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_plot_util.py` & `phiflow-2.5.4/phi/vis/_plot_util.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_user_namespace.py` & `phiflow-2.5.4/phi/vis/_user_namespace.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_viewer.py` & `phiflow-2.5.4/phi/vis/_viewer.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phi/vis/_vis.py` & `phiflow-2.5.4/phi/vis/_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,36 +433,36 @@
     data = layout_pytree_node(data, wrap_leaf=False)
     if isinstance(data, Tensor) and data.dtype.kind == object:  # layout
         rows, cols = 0, 0
         non_reduced = math.EMPTY_SHAPE
         dim0 = reduced = data.shape[0]
         if dim0.only(overlay):
             for overlay_index in dim0.only(overlay).meshgrid(names=True):  # overlay these fields
-                e_rows, e_cols, d_non_reduced, d_reduced = layout_sub_figures(data[overlay_index].native(), row_dims, col_dims, animate, overlay, offset_row, offset_col, positioning, indices, {**base_index, **overlay_index})
+                e_rows, e_cols, d_non_reduced, d_reduced = layout_sub_figures(data[overlay_index], row_dims, col_dims, animate, overlay, offset_row, offset_col, positioning, indices, {**base_index, **overlay_index})
                 rows = max(rows, e_rows)
                 cols = max(cols, e_cols)
                 non_reduced &= d_non_reduced
                 reduced = merge_shapes(reduced, d_reduced, allow_varying_sizes=True)
         elif dim0.only(animate):
-            data = math.stack(data.native(), dim0)
+            data = math.stack(data, dim0)
             return layout_sub_figures(data, row_dims, col_dims, animate, overlay, offset_row, offset_col, positioning, indices, base_index)
         else:
             elements = unstack(data, dim0)
             for item_name, e in zip(dim0.get_item_names(dim0.name) or range(dim0.size), elements):
                 index = dict(base_index, **{dim0.name: item_name})
                 if dim0.only(row_dims):
-                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e.native(), row_dims, col_dims, animate, overlay, offset_row + rows, offset_col, positioning, indices, index)
+                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e, row_dims, col_dims, animate, overlay, offset_row + rows, offset_col, positioning, indices, index)
                     rows += e_rows
                     cols = max(cols, e_cols)
                 elif dim0.only(col_dims):
-                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e.native(), row_dims, col_dims, animate, overlay, offset_row, offset_col + cols, positioning, indices, index)
+                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e, row_dims, col_dims, animate, overlay, offset_row, offset_col + cols, positioning, indices, index)
                     cols += e_cols
                     rows = max(rows, e_rows)
                 else:
-                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e.native(), row_dims, col_dims, animate, overlay, offset_row, offset_col, positioning, indices, index)
+                    e_rows, e_cols, e_non_reduced, e_reduced = layout_sub_figures(e, row_dims, col_dims, animate, overlay, offset_row, offset_col, positioning, indices, index)
                     cols = max(cols, e_cols)
                     rows = max(rows, e_rows)
                 non_reduced &= e_non_reduced
                 reduced = merge_shapes(reduced, e_reduced, allow_varying_sizes=True)
         return rows, cols, non_reduced, reduced
     else:
         data = to_field(data)
```

### Comparing `phiflow-2.5.3/phi/vis/_vis_base.py` & `phiflow-2.5.4/phi/vis/_vis_base.py`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/phiflow.egg-info/PKG-INFO` & `phiflow-2.5.4/phiflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phiflow
-Version: 2.5.3
+Version: 2.5.4
 Summary: Differentiable PDE solving framework for machine learning
 Home-page: https://github.com/tum-pbs/PhiFlow
 Author: Philipp Holl
 Author-email: philipp.holl@tum.de
 License: MIT
-Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.5.3.tar.gz
+Download-URL: https://github.com/tum-pbs/PhiFlow/archive/2.5.4.tar.gz
 Description: # PhiFlow
         
         [**Homepage**](https://github.com/tum-pbs/PhiFlow)
         &nbsp;&nbsp;&nbsp; [**Documentation**](https://tum-pbs.github.io/PhiFlow/)
         &nbsp;&nbsp;&nbsp; [**API**](https://tum-pbs.github.io/PhiFlow/phi)
         &nbsp;&nbsp;&nbsp; [**Demos**](https://github.com/tum-pbs/PhiFlow/tree/master/demos)
         &nbsp;&nbsp;&nbsp; [<img src="https://www.tensorflow.org/images/colab_logo_32px.png" height=16> **Fluids Tutorial**](https://colab.research.google.com/github/tum-pbs/PhiFlow/blob/develop/docs/Fluids_Tutorial.ipynb#offline=true&sandboxMode=true)
```

### Comparing `phiflow-2.5.3/phiflow.egg-info/SOURCES.txt` & `phiflow-2.5.4/phiflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiflow-2.5.3/setup.py` & `phiflow-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     keywords=['Differentiable', 'Simulation', 'Fluid', 'Machine Learning', 'Deep Learning'],
     license='MIT',
     author='Philipp Holl',
     author_email='philipp.holl@tum.de',
     url='https://github.com/tum-pbs/PhiFlow',
     include_package_data=True,
     install_requires=[
-        'phiml==1.2.1',
+        'phiml==1.5.1',
         'matplotlib>=3.5.0',  # also required by dash for color maps
         'packaging',
     ],
     # Optional packages:  dash + plotly (included in dash)
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

