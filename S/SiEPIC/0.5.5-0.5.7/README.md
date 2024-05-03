# Comparing `tmp/SiEPIC-0.5.5.tar.gz` & `tmp/siepic-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiEPIC-0.5.5.tar", last modified: Sun Feb 11 09:39:42 2024, max compression
+gzip compressed data, was "siepic-0.5.7.tar", last modified: Fri May  3 05:30:51 2024, max compression
```

## Comparing `SiEPIC-0.5.5.tar` & `siepic-0.5.7.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.413486 SiEPIC-0.5.5/
--rw-r--r--   0 lukasc     (501) staff       (20)     3206 2024-02-11 09:39:42.413265 SiEPIC-0.5.5/PKG-INFO
--rw-r--r--   0 lukasc     (501) staff       (20)     2626 2023-11-19 05:49:17.000000 SiEPIC-0.5.5/README.md
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.372606 SiEPIC-0.5.5/SiEPIC/
--rw-r--r--   0 lukasc     (501) staff       (20)     1125 2024-02-11 06:44:50.000000 SiEPIC-0.5.5/SiEPIC/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3785 2023-11-23 04:21:18.000000 SiEPIC-0.5.5/SiEPIC/_globals.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7575 2021-11-05 09:08:30.000000 SiEPIC-0.5.5/SiEPIC/calibre_temp.py
--rw-r--r--   0 lukasc     (501) staff       (20)    26548 2023-11-20 06:01:24.000000 SiEPIC-0.5.5/SiEPIC/core.py
--rw-r--r--   0 lukasc     (501) staff       (20)      154 2021-11-05 09:08:30.000000 SiEPIC-0.5.5/SiEPIC/example_gr.py
--rwxr-xr-x   0 lukasc     (501) staff       (20)       63 2021-11-05 09:08:30.000000 SiEPIC-0.5.5/SiEPIC/examples.py
--rw-r--r--   0 lukasc     (501) staff       (20)    79760 2023-11-20 06:13:54.000000 SiEPIC-0.5.5/SiEPIC/extend.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11536 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/github.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3364 2023-11-23 04:14:23.000000 SiEPIC-0.5.5/SiEPIC/install.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.376216 SiEPIC-0.5.5/SiEPIC/lumerical/
--rw-r--r--   0 lukasc     (501) staff       (20)     9113 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/lumerical/ApodizedContraDC.py
--rwxr-xr-x   0 lukasc     (501) staff       (20)      364 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/lumerical/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    16928 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/lumerical/contraDirectionalCoupler.py
--rw-r--r--   0 lukasc     (501) staff       (20)    44944 2023-11-05 07:52:40.000000 SiEPIC-0.5.5/SiEPIC/lumerical/fdtd.py
--rw-r--r--   0 lukasc     (501) staff       (20)    45741 2023-11-08 07:52:02.000000 SiEPIC-0.5.5/SiEPIC/lumerical/interconnect.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7495 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/lumerical/load_lumapi.py
--rw-r--r--   0 lukasc     (501) staff       (20)    10177 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/lumerical/mode.py
--rwxr-xr-x   0 lukasc     (501) staff       (20)    24849 2023-11-05 07:53:36.000000 SiEPIC-0.5.5/SiEPIC/metal_menu_helper.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2644 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/netlist.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.377833 SiEPIC-0.5.5/SiEPIC/opics/
--rw-r--r--   0 lukasc     (501) staff       (20)     1601 2023-05-15 15:42:21.000000 SiEPIC-0.5.5/SiEPIC/opics/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11358 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/components.py
--rw-r--r--   0 lukasc     (501) staff       (20)       88 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/globals.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.378169 SiEPIC-0.5.5/SiEPIC/opics/libraries/
--rw-r--r--   0 lukasc     (501) staff       (20)      928 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/libraries/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4429 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/libraries/catalogue_mgmt.py
--rw-r--r--   0 lukasc     (501) staff       (20)    16360 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/network.py
--rw-r--r--   0 lukasc     (501) staff       (20)     8013 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics/sparam_ops.py
--rw-r--r--   0 lukasc     (501) staff       (20)    18967 2024-01-12 22:31:03.000000 SiEPIC-0.5.5/SiEPIC/opics/utils.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4115 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/opics_netlist_sim.py
--rw-r--r--   0 lukasc     (501) staff       (20)   175162 2024-02-11 07:04:22.000000 SiEPIC-0.5.5/SiEPIC/scripts.py
--rw-r--r--   0 lukasc     (501) staff       (20)     8091 2023-11-14 05:40:49.000000 SiEPIC-0.5.5/SiEPIC/setup.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.378366 SiEPIC-0.5.5/SiEPIC/simulation/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/__init__.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.379064 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.379620 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/Tutorial/
--rw-r--r--   0 lukasc     (501) staff       (20)     5979 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/Tutorial/examples.py
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)      607 2023-09-21 06:34:40.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contraDC_klayout_gui.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.380749 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/
--rw-r--r--   0 lukasc     (501) staff       (20)    39156 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/ContraDC.py
--rw-r--r--   0 lukasc     (501) staff       (20)       16 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3981 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/lumerical_tools.py
--rw-r--r--   0 lukasc     (501) staff       (20)      226 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/modules.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2582 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/utils.py
--rw-r--r--   0 lukasc     (501) staff       (20)    19881 2023-09-21 06:34:40.000000 SiEPIC-0.5.5/SiEPIC/simulation/contraDC/klayout_gui.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.381670 SiEPIC-0.5.5/SiEPIC/tidy3d/
--rw-r--r--   0 lukasc     (501) staff       (20)     1566 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/lint.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1914 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/make_script.py
--rw-r--r--   0 lukasc     (501) staff       (20)      276 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/schema.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2119 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/setup.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.381981 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/
--rw-r--r--   0 lukasc     (501) staff       (20)       34 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/__init__.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.383504 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     9050 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4760 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2684 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1491 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7026 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_web.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.388780 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7912 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_IO.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1359 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_apodization.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3312 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_base.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7018 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_boundaries.py
--rw-r--r--   0 lukasc     (501) staff       (20)    10420 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_custom.py
--rw-r--r--   0 lukasc     (501) staff       (20)    10793 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_field_projection.py
--rw-r--r--   0 lukasc     (501) staff       (20)    17440 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_geometry.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11141 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_grid.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2438 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_grid_spec.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7926 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_medium.py
--rw-r--r--   0 lukasc     (501) staff       (20)    22200 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 lukasc     (501) staff       (20)      837 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_mode.py
--rw-r--r--   0 lukasc     (501) staff       (20)    10667 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_monitor.py
--rw-r--r--   0 lukasc     (501) staff       (20)    19473 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_sidewall.py
--rw-r--r--   0 lukasc     (501) staff       (20)    34997 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_simulation.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7581 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_source.py
--rw-r--r--   0 lukasc     (501) staff       (20)      692 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_types.py
--rw-r--r--   0 lukasc     (501) staff       (20)      229 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_viz.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.389574 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     9196 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_data_arrays.py
--rw-r--r--   0 lukasc     (501) staff       (20)    19312 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_monitor_data.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11662 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.390983 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1044 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_config.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1487 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_log.py
--rw-r--r--   0 lukasc     (501) staff       (20)      509 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_main.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1067 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_make_script.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1986 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_material_library.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.392492 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    24776 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11953 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2529 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 lukasc     (501) staff       (20)     6094 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 lukasc     (501) staff       (20)     6190 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7434 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_resonance_finder.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.393579 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)      287 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/mock_web.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4168 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_auth.py
--rw-r--r--   0 lukasc     (501) staff       (20)      563 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_cli.py
--rw-r--r--   0 lukasc     (501) staff       (20)      133 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_task.py
--rw-r--r--   0 lukasc     (501) staff       (20)     5152 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_webapi.py
--rw-r--r--   0 lukasc     (501) staff       (20)    13532 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tests/utils.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.395262 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/
--rw-r--r--   0 lukasc     (501) staff       (20)     5013 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2860 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/__main__.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.398415 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3113 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/apodization.py
--rw-r--r--   0 lukasc     (501) staff       (20)    22482 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/base.py
--rw-r--r--   0 lukasc     (501) staff       (20)    25014 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/boundary.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.399428 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    13000 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/data_array.py
--rw-r--r--   0 lukasc     (501) staff       (20)    13720 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/dataset.py
--rw-r--r--   0 lukasc     (501) staff       (20)    69817 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 lukasc     (501) staff       (20)    19852 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/sim_data.py
--rw-r--r--   0 lukasc     (501) staff       (20)    35105 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/field_projection.py
--rw-r--r--   0 lukasc     (501) staff       (20)   129452 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/geometry.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.400152 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    14523 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/grid.py
--rw-r--r--   0 lukasc     (501) staff       (20)    22210 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 lukasc     (501) staff       (20)    47226 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/mesher.py
--rw-r--r--   0 lukasc     (501) staff       (20)    37971 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/medium.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4988 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/mode.py
--rw-r--r--   0 lukasc     (501) staff       (20)    29696 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/monitor.py
--rw-r--r--   0 lukasc     (501) staff       (20)    90768 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/simulation.py
--rw-r--r--   0 lukasc     (501) staff       (20)    30929 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/source.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4737 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/structure.py
--rw-r--r--   0 lukasc     (501) staff       (20)     5135 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/types.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7626 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/validators.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7374 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/viz.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1091 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/config.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1258 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/constants.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3642 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/log.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.400829 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    57477 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/material_library.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7867 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/material_reference.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.401158 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/
--rw-r--r--   0 lukasc     (501) staff       (20)      598 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.401741 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/
--rw-r--r--   0 lukasc     (501) staff       (20)      878 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.403102 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 lukasc     (501) staff       (20)      507 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2244 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.403988 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     7349 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1005 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 lukasc     (501) staff       (20)    12129 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4667 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 lukasc     (501) staff       (20)    17964 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 lukasc     (501) staff       (20)    12660 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 lukasc     (501) staff       (20)    12597 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3508 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2900 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 lukasc     (501) staff       (20)      157 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/log.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11774 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.404524 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    23656 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 lukasc     (501) staff       (20)    12374 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.405563 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/
--rw-r--r--   0 lukasc     (501) staff       (20)      135 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     5726 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 lukasc     (501) staff       (20)    22687 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 lukasc     (501) staff       (20)    20820 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4370 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.405782 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/optimize/
--rw-r--r--   0 lukasc     (501) staff       (20)      347 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/optimize/device_optimizer.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.406144 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/polyslab/
--rw-r--r--   0 lukasc     (501) staff       (20)       63 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    11049 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.406515 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/resonance/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    17709 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.406838 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/smatrix/
--rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)    16023 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/smatrix/smatrix.py
--rw-r--r--   0 lukasc     (501) staff       (20)    10860 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/updater.py
--rw-r--r--   0 lukasc     (501) staff       (20)       94 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/version.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.408654 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/
--rw-r--r--   0 lukasc     (501) staff       (20)      406 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     5800 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/asynchronous.py
--rw-r--r--   0 lukasc     (501) staff       (20)     6333 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/auth.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.409023 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/cli/
--rw-r--r--   0 lukasc     (501) staff       (20)       62 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/cli/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1773 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/cli/app.py
--rw-r--r--   0 lukasc     (501) staff       (20)     2550 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/config.py
--rw-r--r--   0 lukasc     (501) staff       (20)    17294 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/container.py
--rw-r--r--   0 lukasc     (501) staff       (20)     3747 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/httputils.py
--rw-r--r--   0 lukasc     (501) staff       (20)     8201 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/s3utils.py
--rw-r--r--   0 lukasc     (501) staff       (20)     1860 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/task.py
--rw-r--r--   0 lukasc     (501) staff       (20)    23092 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/webapi.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.412621 SiEPIC-0.5.5/SiEPIC/utils/
--rw-r--r--   0 lukasc     (501) staff       (20)    54896 2023-12-10 07:59:54.000000 SiEPIC-0.5.5/SiEPIC/utils/__init__.py
--rw-r--r--   0 lukasc     (501) staff       (20)     8844 2023-11-23 23:41:23.000000 SiEPIC-0.5.5/SiEPIC/utils/components.py
--rw-r--r--   0 lukasc     (501) staff       (20)    16889 2023-11-05 08:53:36.000000 SiEPIC-0.5.5/SiEPIC/utils/crossings.py
--rw-r--r--   0 lukasc     (501) staff       (20)    14965 2023-11-15 07:37:45.000000 SiEPIC-0.5.5/SiEPIC/utils/geometry.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4024 2023-11-19 08:17:27.000000 SiEPIC-0.5.5/SiEPIC/utils/klive.py
--rw-r--r--   0 lukasc     (501) staff       (20)    52209 2024-02-11 06:11:00.000000 SiEPIC-0.5.5/SiEPIC/utils/layout.py
--rw-r--r--   0 lukasc     (501) staff       (20)     4926 2023-03-31 03:57:33.000000 SiEPIC-0.5.5/SiEPIC/utils/sampling.py
--rw-r--r--   0 lukasc     (501) staff       (20)    36065 2023-11-20 20:55:07.000000 SiEPIC-0.5.5/SiEPIC/verification.py
-drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-02-11 09:39:42.412969 SiEPIC-0.5.5/SiEPIC.egg-info/
--rw-r--r--   0 lukasc     (501) staff       (20)     3206 2024-02-11 09:39:42.000000 SiEPIC-0.5.5/SiEPIC.egg-info/PKG-INFO
--rw-r--r--   0 lukasc     (501) staff       (20)     7762 2024-02-11 09:39:42.000000 SiEPIC-0.5.5/SiEPIC.egg-info/SOURCES.txt
--rw-r--r--   0 lukasc     (501) staff       (20)        1 2024-02-11 09:39:42.000000 SiEPIC-0.5.5/SiEPIC.egg-info/dependency_links.txt
--rw-r--r--   0 lukasc     (501) staff       (20)       12 2024-02-11 09:39:42.000000 SiEPIC-0.5.5/SiEPIC.egg-info/requires.txt
--rw-r--r--   0 lukasc     (501) staff       (20)        7 2024-02-11 09:39:42.000000 SiEPIC-0.5.5/SiEPIC.egg-info/top_level.txt
--rw-r--r--   0 lukasc     (501) staff       (20)      583 2024-02-11 06:44:50.000000 SiEPIC-0.5.5/pyproject.toml
--rw-r--r--   0 lukasc     (501) staff       (20)       38 2024-02-11 09:39:42.413543 SiEPIC-0.5.5/setup.cfg
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.831630 siepic-0.5.7/
+-rw-r--r--   0 lukasc     (501) staff       (20)     3228 2024-05-03 05:30:51.831375 siepic-0.5.7/PKG-INFO
+-rw-r--r--   0 lukasc     (501) staff       (20)     2626 2023-11-19 05:49:17.000000 siepic-0.5.7/README.md
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.789329 siepic-0.5.7/SiEPIC/
+-rw-r--r--   0 lukasc     (501) staff       (20)     1125 2024-05-03 05:29:23.000000 siepic-0.5.7/SiEPIC/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3785 2023-11-23 04:21:18.000000 siepic-0.5.7/SiEPIC/_globals.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7575 2021-11-05 09:08:30.000000 siepic-0.5.7/SiEPIC/calibre_temp.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    26548 2023-11-20 06:01:24.000000 siepic-0.5.7/SiEPIC/core.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      154 2021-11-05 09:08:30.000000 siepic-0.5.7/SiEPIC/example_gr.py
+-rwxr-xr-x   0 lukasc     (501) staff       (20)       63 2021-11-05 09:08:30.000000 siepic-0.5.7/SiEPIC/examples.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    80609 2024-03-23 23:13:53.000000 siepic-0.5.7/SiEPIC/extend.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11536 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/github.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3364 2023-11-23 04:14:23.000000 siepic-0.5.7/SiEPIC/install.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.793237 siepic-0.5.7/SiEPIC/lumerical/
+-rw-r--r--   0 lukasc     (501) staff       (20)     9113 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/lumerical/ApodizedContraDC.py
+-rwxr-xr-x   0 lukasc     (501) staff       (20)      364 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/lumerical/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    16928 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/lumerical/contraDirectionalCoupler.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    44944 2023-11-05 07:52:40.000000 siepic-0.5.7/SiEPIC/lumerical/fdtd.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    45741 2023-11-08 07:52:02.000000 siepic-0.5.7/SiEPIC/lumerical/interconnect.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7495 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/lumerical/load_lumapi.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    10177 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/lumerical/mode.py
+-rwxr-xr-x   0 lukasc     (501) staff       (20)    24849 2023-11-05 07:53:36.000000 siepic-0.5.7/SiEPIC/metal_menu_helper.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2644 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/netlist.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.795149 siepic-0.5.7/SiEPIC/opics/
+-rw-r--r--   0 lukasc     (501) staff       (20)     1601 2023-05-15 15:42:21.000000 siepic-0.5.7/SiEPIC/opics/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11422 2024-03-24 04:01:25.000000 siepic-0.5.7/SiEPIC/opics/components.py
+-rw-r--r--   0 lukasc     (501) staff       (20)       88 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/opics/globals.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.795874 siepic-0.5.7/SiEPIC/opics/libraries/
+-rw-r--r--   0 lukasc     (501) staff       (20)      928 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/opics/libraries/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4429 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/opics/libraries/catalogue_mgmt.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    16360 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/opics/network.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     8013 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/opics/sparam_ops.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    19845 2024-03-24 06:31:30.000000 siepic-0.5.7/SiEPIC/opics/utils.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4306 2024-03-24 05:40:25.000000 siepic-0.5.7/SiEPIC/opics_netlist_sim.py
+-rw-r--r--   0 lukasc     (501) staff       (20)   176124 2024-03-23 23:13:53.000000 siepic-0.5.7/SiEPIC/scripts.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     8091 2023-11-14 05:40:49.000000 siepic-0.5.7/SiEPIC/setup.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.796045 siepic-0.5.7/SiEPIC/simulation/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/__init__.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.796728 siepic-0.5.7/SiEPIC/simulation/contraDC/
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.797232 siepic-0.5.7/SiEPIC/simulation/contraDC/Tutorial/
+-rw-r--r--   0 lukasc     (501) staff       (20)     5979 2024-03-24 06:54:13.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/Tutorial/examples.py
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      607 2023-09-21 06:34:40.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contraDC_klayout_gui.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.798885 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/
+-rw-r--r--   0 lukasc     (501) staff       (20)    38987 2024-03-24 05:40:25.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/ContraDC.py
+-rw-r--r--   0 lukasc     (501) staff       (20)       16 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3981 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/lumerical_tools.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      226 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/modules.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2582 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/utils.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    23540 2024-03-24 05:40:25.000000 siepic-0.5.7/SiEPIC/simulation/contraDC/klayout_gui.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.799827 siepic-0.5.7/SiEPIC/tidy3d/
+-rw-r--r--   0 lukasc     (501) staff       (20)     1566 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/lint.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1914 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/make_script.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      276 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/schema.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2119 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/setup.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.800142 siepic-0.5.7/SiEPIC/tidy3d/tests/
+-rw-r--r--   0 lukasc     (501) staff       (20)       34 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/__init__.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.801490 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     9050 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4760 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2684 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1491 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7026 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_web.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.805733 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7912 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_IO.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1359 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_apodization.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3312 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_base.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7018 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_boundaries.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    10420 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_custom.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    10793 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_field_projection.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    17440 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_geometry.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11141 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_grid.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2438 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7926 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_medium.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    22200 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      837 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_mode.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    10667 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_monitor.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    19473 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_sidewall.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    34997 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_simulation.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7581 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_source.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      692 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_types.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      229 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_viz.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.806485 siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     9196 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    19312 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11662 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.807448 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1044 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_config.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1487 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_log.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      509 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_main.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1067 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_make_script.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1986 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_material_library.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.808831 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    24776 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11953 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2529 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     6094 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     6190 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7434 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_resonance_finder.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.810088 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      287 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/mock_web.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4168 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_auth.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      563 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_cli.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      133 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_task.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     5152 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_webapi.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    13532 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tests/utils.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.811768 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/
+-rw-r--r--   0 lukasc     (501) staff       (20)     5013 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2860 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/__main__.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.815990 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3113 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/apodization.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    22482 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/base.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    25014 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/boundary.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.817562 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    13000 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/data_array.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    13720 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/dataset.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    69817 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    19852 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    35105 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/field_projection.py
+-rw-r--r--   0 lukasc     (501) staff       (20)   129452 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/geometry.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.818266 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    14523 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/grid.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    22210 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    47226 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    37971 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/medium.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4988 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/mode.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    29696 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/monitor.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    90768 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/simulation.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    30929 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/source.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4737 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/structure.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     5135 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/types.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7626 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/validators.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7374 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/viz.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1091 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/config.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1258 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/constants.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3642 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/log.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.819087 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    57477 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/material_library.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7867 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/material_reference.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.819519 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/
+-rw-r--r--   0 lukasc     (501) staff       (20)      598 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.820221 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/
+-rw-r--r--   0 lukasc     (501) staff       (20)      878 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.821552 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 lukasc     (501) staff       (20)      507 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2244 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.822518 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     7349 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1005 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    12129 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4667 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    17964 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    12660 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    12597 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3508 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2900 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 lukasc     (501) staff       (20)      157 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/log.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11774 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.823011 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    23656 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    12374 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.823968 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/
+-rw-r--r--   0 lukasc     (501) staff       (20)      135 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     5726 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    22687 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    20820 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4370 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.824144 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/optimize/
+-rw-r--r--   0 lukasc     (501) staff       (20)      347 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/optimize/device_optimizer.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.824459 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/polyslab/
+-rw-r--r--   0 lukasc     (501) staff       (20)       63 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    11049 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.824757 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/resonance/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    17709 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.825068 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/smatrix/
+-rw-r--r--   0 lukasc     (501) staff       (20)        0 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    16023 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/smatrix/smatrix.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    10860 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/updater.py
+-rw-r--r--   0 lukasc     (501) staff       (20)       94 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/version.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.826756 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/
+-rw-r--r--   0 lukasc     (501) staff       (20)      406 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     5800 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/asynchronous.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     6333 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/auth.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.827194 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/cli/
+-rw-r--r--   0 lukasc     (501) staff       (20)       62 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1773 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/cli/app.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     2550 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/config.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    17294 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/container.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     3747 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/httputils.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     8201 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/s3utils.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     1860 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/task.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    23092 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/webapi.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.830725 siepic-0.5.7/SiEPIC/utils/
+-rw-r--r--   0 lukasc     (501) staff       (20)    54914 2024-05-03 05:29:01.000000 siepic-0.5.7/SiEPIC/utils/__init__.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     8844 2023-11-23 23:41:23.000000 siepic-0.5.7/SiEPIC/utils/components.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    16889 2023-11-05 08:53:36.000000 siepic-0.5.7/SiEPIC/utils/crossings.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    14965 2023-11-15 07:37:45.000000 siepic-0.5.7/SiEPIC/utils/geometry.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4024 2023-11-19 08:17:27.000000 siepic-0.5.7/SiEPIC/utils/klive.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    52209 2024-02-11 06:11:00.000000 siepic-0.5.7/SiEPIC/utils/layout.py
+-rw-r--r--   0 lukasc     (501) staff       (20)     4926 2023-03-31 03:57:33.000000 siepic-0.5.7/SiEPIC/utils/sampling.py
+-rw-r--r--   0 lukasc     (501) staff       (20)    38681 2024-05-03 05:29:01.000000 siepic-0.5.7/SiEPIC/verification.py
+drwxr-xr-x   0 lukasc     (501) staff       (20)        0 2024-05-03 05:30:51.831083 siepic-0.5.7/SiEPIC.egg-info/
+-rw-r--r--   0 lukasc     (501) staff       (20)     3228 2024-05-03 05:30:51.000000 siepic-0.5.7/SiEPIC.egg-info/PKG-INFO
+-rw-r--r--   0 lukasc     (501) staff       (20)     7762 2024-05-03 05:30:51.000000 siepic-0.5.7/SiEPIC.egg-info/SOURCES.txt
+-rw-r--r--   0 lukasc     (501) staff       (20)        1 2024-05-03 05:30:51.000000 siepic-0.5.7/SiEPIC.egg-info/dependency_links.txt
+-rw-r--r--   0 lukasc     (501) staff       (20)       19 2024-05-03 05:30:51.000000 siepic-0.5.7/SiEPIC.egg-info/requires.txt
+-rw-r--r--   0 lukasc     (501) staff       (20)        7 2024-05-03 05:30:51.000000 siepic-0.5.7/SiEPIC.egg-info/top_level.txt
+-rw-r--r--   0 lukasc     (501) staff       (20)      595 2024-05-03 05:29:23.000000 siepic-0.5.7/pyproject.toml
+-rw-r--r--   0 lukasc     (501) staff       (20)       38 2024-05-03 05:30:51.831672 siepic-0.5.7/setup.cfg
```

### Comparing `SiEPIC-0.5.5/PKG-INFO` & `siepic-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: SiEPIC
-Version: 0.5.5
+Version: 0.5.7
 Summary: SiEPIC-Tools: for silicon photonics layout, design, verification and circuit simulation
 Author-email: Lukas Chrostowski <lukasc@ece.ubc.ca>
 Project-URL: Homepage, https://github.com/SiEPIC/SiEPIC-Tools
 Project-URL: Issues, https://github.com/SiEPIC/SiEPIC-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: pandas
 
 # SiEPIC-Tools
 
 - SiEPIC-Tools - for silicon photonics layout, design, verification and circuit simulation
 - Developed within the <a href="http://www.siepic.ubc.ca">SiEPIC</a> program, by <a href="https://ca.linkedin.com/in/chrostowski">Lukas Chrostowski</a>, with contributions from many others.
 - This is a package implemented using Python in <a href="http://www.klayout.de">KLayout</a>.
 - Instruction on design, layout, fabrication, test, data analysis for silicon photonics provided in the edX course: <a href="http://edx.org/course/silicon-photonics-design-fabrication-ubcx-phot1x">Silicon Photonics Design, Fabrication and Data Analysis</a> and textbook <a href="http://www.cambridge.org/ca/academic/subjects/engineering/electronic-optoelectronic-devices-and-nanotechnology/silicon-photonics-design-devices-systems">Silicon Photonics Design: From Devices to Systems</a> by Lukas Chrostowski and Michael Hochberg.
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: SiEPIC Version: 0.5.5 Summary: SiEPIC-Tools: for
+Metadata-Version: 2.1 Name: SiEPIC Version: 0.5.7 Summary: SiEPIC-Tools: for
 silicon photonics layout, design, verification and circuit simulation Author-
 email: Lukas Chrostowski
 ece.ubc.ca> Project-URL: Homepage, https://github.com/SiEPIC/SiEPIC-Tools
 Project-URL: Issues, https://github.com/SiEPIC/SiEPIC-Tools/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: numpy Requires-Dist:
-scipy # SiEPIC-Tools - SiEPIC-Tools - for silicon photonics layout, design,
-verification and circuit simulation - Developed within the _S_i_E_P_I_C program, by
-_L_u_k_a_s_ _C_h_r_o_s_t_o_w_s_k_i, with contributions from many others. - This is a package
-implemented using Python in _K_L_a_y_o_u_t. - Instruction on design, layout,
-fabrication, test, data analysis for silicon photonics provided in the edX
-course: _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_,_ _F_a_b_r_i_c_a_t_i_o_n_ _a_n_d_ _D_a_t_a_ _A_n_a_l_y_s_i_s and textbook
-_S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_:_ _F_r_o_m_ _D_e_v_i_c_e_s_ _t_o_ _S_y_s_t_e_m_s by Lukas Chrostowski and
-Michael Hochberg. - Process Design Kits that use KLayout SiEPIC-Tools are
-available for multiple foundries including _A_M_F, _A_I_M_ _P_h_o_t_o_n_i_c_s, _T_o_w_e_r
-_S_e_m_i_c_o_n_d_u_c_t_o_r, _L_i_g_e_n_t_e_c, _A_p_p_l_i_e_d_ _N_a_n_o_t_o_o_l_s_ _I_n_c_., and _S_i_E_P_I_C_f_a_b. - Citing this
-work: - Lukas Chrostowski, Zeqin Lu, Jonas Flueckiger, Xu Wang, Jackson Klein,
-Amy Liu, Jaspreet Jhoja, James Pond, "_D_e_s_i_g_n_ _a_n_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_l_i_c_o_n_ _p_h_o_t_o_n_i_c
-_s_c_h_e_m_a_t_i_c_s_ _a_n_d_ _l_a_y_o_u_t_s," Proc. SPIE 9891, Silicon Photonics and Photonic
-Integrated Circuits V, 989114 (May 13, 2016); doi:10.1117/12.2230376. - Lukas
-Chrostowski, Hossam Shoman, Mustafa Hammood, Han Yun, Jaspreet Jhoja, Enxiao
-Luan, Stephen Lin, Ajay Mistry, Donald Witt, Nicolas A. F. Jaeger, Sudip
+scipy Requires-Dist: pandas # SiEPIC-Tools - SiEPIC-Tools - for silicon
+photonics layout, design, verification and circuit simulation - Developed
+within the _S_i_E_P_I_C program, by _L_u_k_a_s_ _C_h_r_o_s_t_o_w_s_k_i, with contributions from many
+others. - This is a package implemented using Python in _K_L_a_y_o_u_t. - Instruction
+on design, layout, fabrication, test, data analysis for silicon photonics
+provided in the edX course: _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_,_ _F_a_b_r_i_c_a_t_i_o_n_ _a_n_d_ _D_a_t_a
+_A_n_a_l_y_s_i_s and textbook _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_:_ _F_r_o_m_ _D_e_v_i_c_e_s_ _t_o_ _S_y_s_t_e_m_s by
+Lukas Chrostowski and Michael Hochberg. - Process Design Kits that use KLayout
+SiEPIC-Tools are available for multiple foundries including _A_M_F, _A_I_M_ _P_h_o_t_o_n_i_c_s,
+_T_o_w_e_r_ _S_e_m_i_c_o_n_d_u_c_t_o_r, _L_i_g_e_n_t_e_c, _A_p_p_l_i_e_d_ _N_a_n_o_t_o_o_l_s_ _I_n_c_., and _S_i_E_P_I_C_f_a_b. - Citing
+this work: - Lukas Chrostowski, Zeqin Lu, Jonas Flueckiger, Xu Wang, Jackson
+Klein, Amy Liu, Jaspreet Jhoja, James Pond, "_D_e_s_i_g_n_ _a_n_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_l_i_c_o_n
+_p_h_o_t_o_n_i_c_ _s_c_h_e_m_a_t_i_c_s_ _a_n_d_ _l_a_y_o_u_t_s," Proc. SPIE 9891, Silicon Photonics and
+Photonic Integrated Circuits V, 989114 (May 13, 2016); doi:10.1117/12.2230376.
+- Lukas Chrostowski, Hossam Shoman, Mustafa Hammood, Han Yun, Jaspreet Jhoja,
+Enxiao Luan, Stephen Lin, Ajay Mistry, Donald Witt, Nicolas A. F. Jaeger, Sudip
 Shekhar, Hasitha Jayatilleka, Philippe Jean, Simon B.-de Villers, Jonathan
 Cauchon, Wei Shi, Cameron Horvath, Jocelyn N. Westwood-Bachman, Kevin Setzer,
 Mirwais Aktary, N. Shane Patrick, Richard Bojko, Amin Khavasi, Xu Wang, Thomas
 Ferreira de Lima, Alexander N. Tait, Paul R. Prucnal, David E. Hagan, Doris
 Stevanovic, Andy P. Knights, "_S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_ _C_i_r_c_u_i_t_ _D_e_s_i_g_n_ _U_s_i_n_g_ _R_a_p_i_d
 _P_r_o_t_o_t_y_p_i_n_g_ _F_o_u_n_d_r_y_ _P_r_o_c_e_s_s_ _D_e_s_i_g_n_ _K_i_t_s" IEEE Journal of Selected Topics in
 Quantum Electronics, Volume: 25, Issue: 5, Sept.-Oct. 2019. (_P_D_F)
```

### Comparing `SiEPIC-0.5.5/README.md` & `siepic-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/__init__.py` & `siepic-0.5.7/SiEPIC/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 SiEPIC-Tools package for KLayout
 '''
 
-__version__ = '0.5.5'
+__version__ = '0.5.7'
 
 print("KLayout SiEPIC-Tools version %s" %__version__)
 
 import pya
 if '__version__' in dir(pya):
     # pya.__version__ was introduced in KLayout version 0.28.6
     KLAYOUT_VERSION = int(pya.__version__.split('.')[1])
```

### Comparing `SiEPIC-0.5.5/SiEPIC/_globals.py` & `siepic-0.5.7/SiEPIC/_globals.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/calibre_temp.py` & `siepic-0.5.7/SiEPIC/calibre_temp.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/core.py` & `siepic-0.5.7/SiEPIC/core.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/extend.py` & `siepic-0.5.7/SiEPIC/extend.py`

 * *Files 1% similar despite different names*

```diff
@@ -929,21 +929,31 @@
 
     Find all the pins for the component, save in components and also return pin list.
     Use the pin names on layer PinRec to sort the pins in alphabetical order
 
     cell_selected: only find components that match this specific cell.
     
     inst: return only the component that matches the instance inst
+    
+    limitation:
+     - flat components only. doesn't find the component if it is buried in a hierarchy
+     - no function for instance.find_components.  Instead we find based on cell, then try to match it to the requested instance.
 
     '''
+    
+    if cell_selected != None and type(cell_selected) != type([]):
+          cell_selected=[cell_selected]
+
     if verbose:
         print('*** Cell.find_components:')
+        if cell_selected[0]:
+          print('  - cell_selected=%s' % (cell_selected[0].name if cell_selected[0] else None))
+        if inst:
+          print('  - inst=%s' % (inst.cell.name))
 
-    if cell_selected != None and type(cell_selected) != type([]):
-          cell_selected=[cell_selected]
 
     components = []
 
     from .core import Component
     from . import _globals
     from .utils import get_technology_by_name
     if 'TECHNOLOGY' in dir(self.layout()):
@@ -964,16 +974,20 @@
         
     component_matched = []
 
     while not(iter1.at_end()):
         idx = len(components)  # component index value to be assigned to Component.idx
         component_ID = idx
         subcell = iter1.cell()  # cell (component) to which this shape belongs
+        if verbose:
+          print(' - looking at shape in cell %s. ' % subcell.name)
         if cell_selected and not subcell in cell_selected:
             # check if subcell is one of the arguments to this function: cell_selected
+            if verbose:
+              print(' - cell_selected and not subcell (%s) in cell_selected (%s). ' % (subcell.name, cell_selected[0].name))
             iter1.next()
             continue
         component = subcell.basic_name().replace(' ', '_')   # name library component
         instance = subcell.name
 
         found_component = False
         # DevRec must be either a Box or a Polygon:
@@ -1091,14 +1105,17 @@
 
         iter1.next()
     # end while iter1
     
     if component_matched:
         return component_matched
     
+    if components == []:
+        raise Exception ('SiEPIC.extend.find_components: No component found for cell_selected=%s' % (cell_selected[0].name if cell_selected else None))
+
     return components
 # end def find_components
 
 
 def identify_nets(self, verbose=False):
     # function to identify all the nets in the cell layout
     # use the data in Optical_pin, Optical_waveguide to find overlaps
```

### Comparing `SiEPIC-0.5.5/SiEPIC/github.py` & `siepic-0.5.7/SiEPIC/github.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/install.py` & `siepic-0.5.7/SiEPIC/install.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/ApodizedContraDC.py` & `siepic-0.5.7/SiEPIC/lumerical/ApodizedContraDC.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/contraDirectionalCoupler.py` & `siepic-0.5.7/SiEPIC/lumerical/contraDirectionalCoupler.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/fdtd.py` & `siepic-0.5.7/SiEPIC/lumerical/fdtd.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/interconnect.py` & `siepic-0.5.7/SiEPIC/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/load_lumapi.py` & `siepic-0.5.7/SiEPIC/lumerical/load_lumapi.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/lumerical/mode.py` & `siepic-0.5.7/SiEPIC/lumerical/mode.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/metal_menu_helper.py` & `siepic-0.5.7/SiEPIC/metal_menu_helper.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/netlist.py` & `siepic-0.5.7/SiEPIC/netlist.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/__init__.py` & `siepic-0.5.7/SiEPIC/opics/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/components.py` & `siepic-0.5.7/SiEPIC/opics/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,18 @@
         for _ in range(self.nports):
             self.port_references[_] = _
 
         self.sparam_attr = sparam_attr
         self.sparam_file = filename
 
         for key, value in kwargs.items():
-            self.componentParameters.append([key, str(value)])
+            self.componentParameters.append([key, value])
 
-    def load_sparameters(self, data_folder: PosixPath, filename: str) -> ndarray:
+    def load_sparameters(self, data_folder: PosixPath, filename: str, 
+            verbose: bool = True) -> ndarray:
         """
         Loads sparameters either from an npz file or from a raw sparam\
              file using a look-up table.
 
         Args:
             data_folder: Directory path of the data folder containing\
                  s-parameter data files and a look up table.
@@ -86,14 +87,15 @@
         else:
             componentData, self.sparam_file = LUT_processor(
                 data_folder,
                 filename,
                 self.componentParameters,
                 self.nports,
                 self.sparam_attr,
+                verbose = verbose
             )
             return self.interpolate_sparameters(
                 self.f, componentData[0], componentData[1]
             )
 
     def set_port_reference(self, port_number: int, port_name: str) -> None:
         """
```

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/libraries/__init__.py` & `siepic-0.5.7/SiEPIC/opics/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/libraries/catalogue_mgmt.py` & `siepic-0.5.7/SiEPIC/opics/libraries/catalogue_mgmt.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/network.py` & `siepic-0.5.7/SiEPIC/opics/network.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/sparam_ops.py` & `siepic-0.5.7/SiEPIC/opics/sparam_ops.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/opics/utils.py` & `siepic-0.5.7/SiEPIC/opics/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,16 +184,36 @@
         filedir: Directory of the XML look-up-table file.
         lutfilename: Look-up-table filename.
         lutdata: Look-up-table arguments.
     """
     xml = parse(filedir / lutfilename)
     root = xml.getroot()
 
+    if "contraDC" in lutfilename:
+        print(1)
+
     for node in root.iter("association"):
         sample = [[each.attrib["name"], each.text] for each in node.iter("value")]
+        '''
+        Look-up is not working. returns the last one each time.
+        Attempt to fix it.. gave up...
+        
+        sample = [[each.attrib["name"], float(each.text) if each.attrib["type"]=='double' else int(each.text) if each.attrib["type"]=='int' else bool(each.text) if each.attrib["type"]=='bool' else  each.text, each.attrib["type"]] for each in node.iter("value")]    
+
+        # Make sure the two data sets have the same datatypes
+        for q in lutdata:
+            w = [r for r in sample if r[0]==q[0]] [0]
+            if w[2] == 'double':
+                q[1] = float(q[1])
+            if w[2] == 'bool':
+                q[1] = bool(q[1])
+            if w[2] == 'int':
+                q[1] = int(q[1])
+        '''
+        
         if sorted(sample[0:-1]) == sorted(lutdata):
             break
     sparam_file = sample[-1][1].split(";")
     return (sparam_file, xml, node)
 
 
 def LUT_processor(
@@ -204,28 +224,30 @@
     sparam_attr: str,
     verbose: bool = False,
 ) -> Tuple[Tuple[ndarray, ndarray], str]:
     """process look up table data"""
     start = time.time()
     sparam_file, xml, node = LUT_reader(filedir, lutfilename, lutdata)
 
+    print(' - LUT_processor: file: %s' % sparam_file)
+
     # read data
     if ".npz" in sparam_file[0] or ".npz" in sparam_file[-1]:
         npzfile = [each for each in sparam_file if ".npz" in each][0]
         tempdata = np.load(filedir / npzfile)
         sdata = (tempdata["f"], tempdata["s"])
         npz_file = npzfile
 
     else:
         if verbose:
-            print("numpy datafile not found. reading sparam file instead..")
+            print("numpy datafile not found. reading sparam file instead.. %s " % sparam_file)
 
         sdata = universal_sparam_filereader(nports, sparam_file[-1], filedir, "auto")
         # create npz file name
-        npz_file = sparam_file[-1].split(".")[0]
+        npz_file = sparam_file[-1].split(".dat")[0]
 
         # save as npz file
         np.savez(filedir / npz_file, f=sdata[0], s=sdata[1])
 
         # update xml file
         sparam_file.append(npz_file + ".npz")
         sparam_file = list(set(sparam_file))
```

### Comparing `SiEPIC-0.5.5/SiEPIC/opics_netlist_sim.py` & `siepic-0.5.7/SiEPIC/opics_netlist_sim.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,140 @@
 import pya
 
-def circuit_simulation_opics(verbose=False,opt_in_selection_text=[], require_save=True):
-    ''' Simulate the circuit using OPICS
-    Using a netlist extracte from the layout'''
-    
+
+def circuit_simulation_opics(
+    verbose=False, opt_in_selection_text=[], require_save=True
+):
+    """Simulate the circuit using OPICS
+    Using a netlist extracte from the layout"""
+
     # Required packages
     from SiEPIC.install import install
-    if not install('plotly'):
+
+    if not install("plotly"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'plotly'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'plotly'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('pandas'):
+    if not install("pandas"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'pandas'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'pandas'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('packaging'):
+    if not install("packaging"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'packaging'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'packaging'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('defusedxml'):
+    if not install("defusedxml"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'defusedxml'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'defusedxml'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('numpy'):
+    if not install("numpy"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'numpy'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'numpy'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('yaml'):
+    if not install("yaml"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'yaml'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'yaml'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    if not install('scipy'):
+    if not install("scipy"):
         pya.MessageBox.warning(
-        "Missing package", "The OPICS circuit simulator does not function without the package 'scipy'.",  pya.MessageBox.Ok)    
+            "Missing package",
+            "The OPICS circuit simulator does not function without the package 'scipy'.",
+            pya.MessageBox.Ok,
+        )
         return None
-    
-    
+
     # obtain the spice file from the layout
     from SiEPIC.netlist import export_spice_layoutview
-    spice_filepath, _ = export_spice_layoutview(verbose=False,opt_in_selection_text=[], require_save=require_save)
-    
+
+    spice_filepath, _ = export_spice_layoutview(
+        verbose=False, opt_in_selection_text=[], require_save=require_save
+    )
+
     from SiEPIC.opics import libraries
     from SiEPIC.opics.network import Network
     from SiEPIC.opics.utils import netlistParser, NetlistProcessor
     from SiEPIC.opics.globals import C as c_
-        
+
     print(spice_filepath)
-    
+
     # get netlist data
     circuitData = netlistParser(spice_filepath).readfile()
-    
+
     print(circuitData)
-    
-    '''
+
+    """
     import numpy as np
     from SiEPIC.opics.globals import C
     freq = np.linspace(C * 1e6 / 1.5, C * 1e6 / 1.6, 2000)
     circuit = Network(network_id="circuit_name", f=freq)
-    '''
-    
+    """
+
     # process netlist data
-    subckt = NetlistProcessor(spice_filepath, Network, libraries, c_, circuitData, verbose=False)
-    
+    subckt = NetlistProcessor(
+        spice_filepath, Network, libraries, c_, circuitData, verbose=False
+    )
+
     print(subckt)
-    
+
     # simulate network
     subckt.simulate_network()
-    
+
     # get input and output net labels
     inp_idx = subckt.global_netlist[list(subckt.global_netlist.keys())[-1]].index(
         circuitData["inp_net"]
     )
     out_idx = [
         subckt.global_netlist[list(subckt.global_netlist.keys())[-1]].index(each)
         for each in circuitData["out_net"]
     ]
-    
+
     ports = [[each_output, inp_idx] for each_output in out_idx]
-    
-    
+
     # plot results
     # subckt.sim_result.plot_sparameters(ports=ports, interactive=False)
-    
-    
+
     # Plot using Plotly:
     import plotly.express as px
-    import pandas as pd # https://pandas.pydata.org/docs/user_guide/10min.html
+    import pandas as pd  # https://pandas.pydata.org/docs/user_guide/10min.html
+
     result = subckt.sim_result.get_data()
-    wavelengths = c_/subckt.f
+    wavelengths = c_ / subckt.f
 
     # collect all the results for each port:
     import numpy as np
+
     nports = subckt.sim_result.nports
-    out = result['S_1_0']
-    print(out.shape)       
-    columns = ['Output 1']
-    for i in range(1,nports-1):
-        print(out.shape)       
-        out = np.vstack((out, result['S_%s_0' %(i+1)]))
-        columns = columns + ['Output %s' % (i+1) ]
-    
+    out = result["S_1_0"]
+    print(out.shape)
+    columns = ["Output 1"]
+    for i in range(1, nports - 1):
+        print(out.shape)
+        out = np.vstack((out, result["S_%s_0" % (i + 1)]))
+        columns = columns + ["Output %s" % (i + 1)]
+
     # Single line:
-    #df = pd.DataFrame(transmission, index=wavelengths, columns=['Transmission'])
-    
+    # df = pd.DataFrame(transmission, index=wavelengths, columns=['Transmission'])
+
     # Two lines:
     df = pd.DataFrame(out.transpose(), index=wavelengths, columns=columns)
-    fig = px.line(df, labels={'index':'Wavelength', 'value':'Transmission (dB)'}, markers=True)
+    fig = px.line(
+        df, labels={"index": "Wavelength", "value": "Transmission (dB)"}, markers=True
+    )
     fig.show()
-    
-
```

### Comparing `SiEPIC-0.5.5/SiEPIC/scripts.py` & `siepic-0.5.7/SiEPIC/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1732,17 +1732,23 @@
   # check cells
   if type(cellB) != pya.Cell:
       raise Exception("cellB needs to be a cell, not a cell index")
   if type(instanceA) != pya.Instance:
       raise Exception("instanceA needs to be an Instance, not an index")
 
   # Find the two components:
-  componentA = instanceA.parent_cell.find_components(cell_selected=instanceA.cell, inst=instanceA)
+  componentA = instanceA.parent_cell.find_components(cell_selected=instanceA.cell, inst=instanceA, verbose=verbose)
   componentB = cellB.find_components()
   if componentA==[]:
+    if verbose:
+      print('*** WARNING: componentA not found, looking lower in the hierarchy')
+    componentA = instanceA.cell.find_components(inst=instanceA, verbose=verbose)
+  if componentA==[]:
+    if verbose:
+      print('*** WARNING: componentA not found, looking higher in the hierarchy which may not work correctly: instanceA.parent_cell.find_components(inst=instanceA)')
     componentA = instanceA.parent_cell.find_components(inst=instanceA)
     if componentA==[]:
       if _globals.Python_Env == "KLayout_GUI":
         question = pya.QMessageBox().setStandardButtons(pya.QMessageBox.Ok)
         question.setText("SiEPIC-Tools scripted layout, requested component not found")
         question.setInformativeText("Component instanceA not found: %s, %s" % (instanceA, instanceA.cell.name))
         pya.QMessageBox_StandardButton(question.exec_())
@@ -3531,55 +3537,72 @@
             splitter1.setSizes([400, 500])
             container = QWidget()
             hbox.addWidget(splitter1)
             selection(None)
             wdg.show()
 
 
-def replace_cell(layout, cell_x_name, cell_y_name, cell_y_file=None, cell_y_library=None, Exact = True, debug = False):
+def replace_cell(layout, cell_x_name, cell_y_name, cell_y_file=None, cell_y_library=None, Exact = True, RequiredCharacter = '$', debug = False):
     '''
     SiEPIC-Tools: scripts.replace_cell
     Search and replace: cell_x with cell_y
     useful for blackbox IP cell replacement
     - load layout containing cell_y_name from cell_y_file or cell_y_library
     - replace all cell_x_name* instances with cell_y
+    - Exact = True: the cell name must match exactly
+            = False: the cell_y_name appears at the beginning of the cells to be replaced
+                     and RequiredCharacter appears directly after, e.g,. '$' as KLayout appends during merging
+              (exact match is still included)
     
     Black box                   True geometry
     Basename_BB, Basename_BB*   YES: Basename
     Basename, Basename*         NO: Basename_extension
     Basename, Basename*         YES: DifferentName
     '''
     
     import os
     if debug:
         print(" - cell replacement for: %s, with cell %s (%s), "  % (cell_x_name, cell_y_name, os.path.basename(cell_y_file)))
     log = ''
     log += "- cell replacement for: %s, with cell %s (%s)\n"  % (cell_x_name, cell_y_name, os.path.basename(cell_y_file))
 
     # Find the cells that need replacement (cell_x)
-    if Exact:
-        # find cell name exactly matching cell_x_name
-        cells_x = [layout.cell(cell_x_name)]
-    else:
+    # find cell name exactly matching cell_x_name
+    cells_x = [layout.cell(cell_x_name)]
+    if not Exact:
         # replacement for all cells that:
         # 1) cell name exact matching cell_x_name, OR
         # 2) that begin with the cell name, i.e., xxx* is matched
         #    i.e., xxx and xxx* are matched
-        cells_x = [cell for cell in layout.each_cell() if cell.name.find(cell_x_name) == 0]
+        cells_x += [cell for cell in layout.each_cell() if cell.name.find(cell_x_name+RequiredCharacter) == 0]
 
         # replacement for all cells that:
         # 1) cell name exact matching cell_x_name, OR
         # 2) that begin with the cell name and have a $
         #    i.e., xxx and xxx$* are matched  (was used for the Phot1x 2022/06 tapeout)
         #cells_x = [cell for cell in layout.each_cell() if cell.name == cell_x_name or cell.name.find(cell_x_name) == 0 and '$' in cell.name]
 
+
+    if not cells_x or not cells_x[0]:
+        if debug:
+            print("  - none found: %s" % cell_x_name)
+        log += " - none found: %s" % cell_x_name
+        return
+
+    if Exact:
+        if debug:
+            print("  - exact match: %s" % cells_x[0].name)
+        log += "  - exact match: %s" % cells_x[0].name
+    else:
+        if debug:
+            print("  - non-exact match: %s" % ([c.name for c in cells_x]) )
+        log += "  - non-exact match: %s" % ([c.name for c in cells_x]) 
+    
     # Load the new cell:   
     if cell_y_file:
-        # find cell name CELL_Y
-#        print(layout.top_cell())
         cell_y = layout.cell(cell_y_name)
         if debug:
             print(" - checking for cell %s in current layout: %s" % (cell_y_name, cell_y))
         if not cell_y:
             # Load cell_y_name:
             if debug:
                 print(" - loading cell %s from file %s" % (cell_y_name, cell_y_file))
@@ -3596,54 +3619,48 @@
             raise Exception ('Cannot import cell %s from library %s' % (cell_y_name, cell_y_library))        
 
     if cells_x:
         log += "   - replacing cells: %s\n"  % ([c.name for c in cells_x])
         
     for cell_x in cells_x:
         if debug:
-            print(" - replace_cell: found cells to be replaced: %s"  % (cell_x.name))
+            print("   - replace_cell: found cells to be replaced: %s"  % (cell_x.name))
     
         # find caller cells
         caller_cells = cell_x.caller_cells()
         # loop through all caller cells:
         for c in caller_cells:
             cc = layout.cell(c)
 
             # find instances of CELL_X in caller cell
             itr = cc.each_inst()
             inst = next(itr)
             while inst:
-#                if debug:
-#                    print("   - found inst: %s, %s" % (inst, inst.cell.name))
                 if inst.cell.name == cell_x.name:
                     if cell_y.destroyed():
                         print('   - Warning: cell_y (%s) destroyed, skipping replacement' % (cell_y_name))
                         print("   - destroyed status: cell_y - %s, cell_x - %s, cc - %s" % (cell_y.destroyed(), cell_x.destroyed(), cc.destroyed()))
                         print('   - looking for cell. %s, %s, %s' % (cell_y_name, cell_y, layout.cell(cell_y_name)))
                         log += '   - Warning: cell destroyed, skipping replacement\n'
-#                        continue # skip this inst, continue to next; stays in an infinite loop
                         break  # skip this cell
                     # replace with CELL_Y
                     if inst.is_regular_array():
                         if debug:
                             print("    - replacing %s in %s, with cell array: %s" % (cell_x.name, cc.name, cell_y.name))
                         ci = inst.cell_inst
                         cc.replace(inst, pya.CellInstArray(cell_y.cell_index(),inst.trans, ci.a, ci.b, ci.na, ci.nb))
                     else:
                         if debug:
                             print("    - replacing %s in %s, with cell: %s" % (cell_x.name, cc.name, cell_y.name))
                         cc.replace(inst, pya.CellInstArray(cell_y.cell_index(),inst.trans))
                 inst = next(itr, None)
 
-
     return log
 
 
-
-
 def svg_from_cell(verbose=True):
   if verbose:
     print('SiEPIC.scripts: svg_from_cell()')
 
   # Get technology and layout details
   from .utils import get_layout_variables
   TECHNOLOGY, lv, ly, cell = get_layout_variables()
```

### Comparing `SiEPIC-0.5.5/SiEPIC/setup.py` & `siepic-0.5.7/SiEPIC/setup.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/Tutorial/examples.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/Tutorial/examples.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contraDC_klayout_gui.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/contraDC_klayout_gui.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/ContraDC.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/ContraDC.py`

 * *Files 5% similar despite different names*

```diff
@@ -517,16 +517,15 @@
         filename = "ContraDC_sparams.mat"
         import os
         path = os.path.join(filepath,filename)
         sio.savemat(path, S)
 
         # from lumerical_tools import generate_dat
         # generate_dat()
-        self.generate_dat(filepath=filepath, make_plot=make_plot)
-        return self
+        return self.generate_dat(filepath=filepath, make_plot=make_plot)
 
     def generate_dat(self, filepath='', make_plot=True):
         import numpy as np
         import plotly.graph_objects as go
 
         if self.pol == 'TM':
             mode_ID = '2'
@@ -652,16 +651,15 @@
         else:
             w1=self.w1
             w2=self.w2
         if type(self.period) == list:
             period=self.period[0]
         else:
             period=self.period
-        filename =  "w1=" + "%.0f"%(w1*1e9) + ",w2=" + "%.0f"%(w2*1e9) + ",dW1=" + "%.0f"%(self.dw1*1e9) + ",dW2=" + "%.0f"%(self.dw2*1e9) +  ",gap=" + "%.0f"%(self.gap*1e9) + ",p=" + "%.1f"%(period*1e9) + ",N=" + str(self.N) + ",s=" + str(1 if self.sinusoidal else 0) +  ",a=" + "%.2f"%self.a +  ",rib=" + str(1 if self.rib else 0) + ",pol=" + str(0 if self.pol=='TE' else 1) + ",l1=" + "%.0f"%(self.wvl_range[0]*1e9) + ",l2=" + "%.0f"%(self.wvl_range[1]*1e9) + ",ln=" + str(self.resolution) + '.dat';
-        
+        filename = f"w1={w1*1e9:.0f},w2={w2*1e9:.0f},dW1={self.dw1*1e9:.0f},dW2={self.dw2*1e9:.0f},gap={self.gap*1e9:.0f},p={period*1e9:.1f},N={int(self.N)},s={1 if self.sinusoidal else 0},a={self.a:.2f},rib={1 if self.rib else 0},pol={0 if self.pol=='TE' else 1},l1={self.wvl_range[0]*1e9:.0f},l2={self.wvl_range[1]*1e9:.0f},ln={self.resolution}.dat"
         import os
         path = os.path.join(filepath,filename)
 
         # Save the data to file
         with open(path, "w") as f:
             # Write header information
 
@@ -740,15 +738,15 @@
             f.write(f"({FREQ_PTS},3)\n")
             np.savetxt(f, S34_data, fmt="%.6e", delimiter=" ")
 
             # Write S44 data
             f.write(f"('port 4',{mode_label},{mode_ID},'port 4',{mode_ID},'transmission')\n")
             f.write(f"({FREQ_PTS},3)\n")
             np.savetxt(f, S44_data, fmt="%.6e", delimiter=" ")
-        return path
+        return filename
 
     def getGroupDelay(self):
         """Calculates the group delay of the device,
         using the phase derivative. Requires self.is_simulated=True.
         """
 
         if self.is_simulated:
```

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/lumerical_tools.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/lumerical_tools.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/contra_directional_coupler/utils.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/contra_directional_coupler/utils.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/simulation/contraDC/klayout_gui.py` & `siepic-0.5.7/SiEPIC/simulation/contraDC/klayout_gui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,240 +1,256 @@
-
 # Required packages
 from SiEPIC.install import install
-if not install('scipy', requested_by='Contra Directional Coupler design'):
-  pya.MessageBox.warning(
-  "Missing package", "The simulator does not function without the package 'scipy'.",  pya.MessageBox.Ok)    
-if not install('plotly', requested_by='Contra Directional Coupler design'):
-  pya.MessageBox.warning(
-  "Missing package", "The simulator does not function without the package 'plotly'.",  pya.MessageBox.Ok)    
 
+if not install("scipy", requested_by="Contra Directional Coupler design"):
+    pya.MessageBox.warning(
+        "Missing package",
+        "The simulator does not function without the package 'scipy'.",
+        pya.MessageBox.Ok,
+    )
+if not install("plotly", requested_by="Contra Directional Coupler design"):
+    pya.MessageBox.warning(
+        "Missing package",
+        "The simulator does not function without the package 'plotly'.",
+        pya.MessageBox.Ok,
+    )
 
 
 from SiEPIC.simulation.contraDC.contra_directional_coupler.ContraDC import *
 import sys
 import pya
 import plotly.graph_objs as go
 import plotly.offline as pyo
 import plotly.io as pio
+
 pio.renderers.default = "browser"
 
+
 class MyWindow(pya.QWidget):
 
     def __init__(self):
         super().__init__()
-        self.setWindowTitle('Contra-directional coupler simulator')
+        self.setWindowTitle("Contra-directional coupler simulator")
         self.setMinimumSize(200, 200)
 
         # fetch pcell parameters
         if self.load_pcell_params() == 0:
             self.close()
-        
+
         # fetch technology parameters
         self.load_DFT()
 
-        #******************************************************
+        # ******************************************************
         # Create the layout_pcell and add the UI elements to it
-        from pya import QVBoxLayout, QPushButton, QLabel, QLineEdit, QCheckBox, QComboBox, QHBoxLayout
+        from pya import (
+            QVBoxLayout,
+            QPushButton,
+            QLabel,
+            QLineEdit,
+            QCheckBox,
+            QComboBox,
+            QHBoxLayout,
+        )
+
         layout_pcell = QVBoxLayout()
-        self.button = QPushButton('Refresh PCell')
+        self.button = QPushButton("Refresh PCell")
         # Connect the button to a callback function
         self.button.clicked(self.on_refresh_clicked)
 
-        self.label_pcell = QLabel('Parameterized cell definitions:')
+        self.label_pcell = QLabel("Parameterized cell definitions:")
         layout_pcell.addWidget(self.label_pcell)
 
-        self.pcell_N_label = QLabel('Number of gratings (N) (µm): ')
-        self.pcell_N_fill = QLineEdit(str(self.params['number_of_periods']))
+        self.pcell_N_label = QLabel("Number of gratings (N) (µm): ")
+        self.pcell_N_fill = QLineEdit(str(self.params["number_of_periods"]))
         self.pcell_N_fill.setReadOnly(True)
-        self.pcell_N_fill.setStyleSheet('color: gray')
+        self.pcell_N_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_N_label)
         layout_pcell.addWidget(self.pcell_N_fill)
 
-        self.pcell_period_label = QLabel('Gratings period (Λ) (µm): ')
-        self.pcell_period_fill = QLineEdit(str(self.params['grating_period']))
+        self.pcell_period_label = QLabel("Gratings period (Λ) (µm): ")
+        self.pcell_period_fill = QLineEdit(str(self.params["grating_period"]))
         self.pcell_period_fill.setReadOnly(True)
-        self.pcell_period_fill.setStyleSheet('color: gray')
+        self.pcell_period_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_period_label)
         layout_pcell.addWidget(self.pcell_period_fill)
 
-        self.pcell_gap_label = QLabel('Waveguides gap (G) (µm): ')
-        self.pcell_gap_fill = QLineEdit(str(self.params['gap']))
+        self.pcell_gap_label = QLabel("Waveguides gap (G) (µm): ")
+        self.pcell_gap_fill = QLineEdit(str(self.params["gap"]))
         self.pcell_gap_fill.setReadOnly(True)
-        self.pcell_gap_fill.setStyleSheet('color: gray')
+        self.pcell_gap_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_gap_label)
         layout_pcell.addWidget(self.pcell_gap_fill)
 
-        self.pcell_w1_label = QLabel('Waveguide 1 width (W1) (µm): ')
-        self.pcell_w1_fill = QLineEdit(str(self.params['wg1_width']))
+        self.pcell_w1_label = QLabel("Waveguide 1 width (W1) (µm): ")
+        self.pcell_w1_fill = QLineEdit(str(self.params["wg1_width"]))
         self.pcell_w1_fill.setReadOnly(True)
-        self.pcell_w1_fill.setStyleSheet('color: gray')
+        self.pcell_w1_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_w1_label)
         layout_pcell.addWidget(self.pcell_w1_fill)
 
-        self.pcell_dw1_label = QLabel('Waveguide 1 Δwidth (ΔW1) (µm): ')
-        self.pcell_dw1_fill = QLineEdit(str(self.params['corrugation1_width']))
+        self.pcell_dw1_label = QLabel("Waveguide 1 Δwidth (ΔW1) (µm): ")
+        self.pcell_dw1_fill = QLineEdit(str(self.params["corrugation1_width"]))
         self.pcell_dw1_fill.setReadOnly(True)
-        self.pcell_dw1_fill.setStyleSheet('color: gray')
+        self.pcell_dw1_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_dw1_label)
         layout_pcell.addWidget(self.pcell_dw1_fill)
 
-        self.pcell_w2_label = QLabel('Waveguide 2 width (W2) (µm): ')
-        self.pcell_w2_fill = QLineEdit(str(self.params['wg2_width']))
+        self.pcell_w2_label = QLabel("Waveguide 2 width (W2) (µm): ")
+        self.pcell_w2_fill = QLineEdit(str(self.params["wg2_width"]))
         self.pcell_w2_fill.setReadOnly(True)
-        self.pcell_w2_fill.setStyleSheet('color: gray')
+        self.pcell_w2_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_w2_label)
         layout_pcell.addWidget(self.pcell_w2_fill)
 
-        self.pcell_dw2_label = QLabel('Waveguide 2 Δwidth (ΔW2) (µm): ')
-        self.pcell_dw2_fill = QLineEdit(str(self.params['corrugation2_width']))
+        self.pcell_dw2_label = QLabel("Waveguide 2 Δwidth (ΔW2) (µm): ")
+        self.pcell_dw2_fill = QLineEdit(str(self.params["corrugation2_width"]))
         self.pcell_dw2_fill.setReadOnly(True)
-        self.pcell_dw2_fill.setStyleSheet('color: gray')
+        self.pcell_dw2_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_dw2_label)
         layout_pcell.addWidget(self.pcell_dw2_fill)
 
-        self.pcell_apod_label = QLabel('Apodization index (a): ')
-        self.pcell_apod_fill = QLineEdit(str(self.params['apodization_index']))
+        self.pcell_apod_label = QLabel("Apodization index (a): ")
+        self.pcell_apod_fill = QLineEdit(str(self.params["apodization_index"]))
         self.pcell_apod_fill.setReadOnly(True)
-        self.pcell_apod_fill.setStyleSheet('color: gray')
+        self.pcell_apod_fill.setStyleSheet("color: gray")
         layout_pcell.addWidget(self.pcell_apod_label)
         layout_pcell.addWidget(self.pcell_apod_fill)
 
-        self.pcell_rib_label = QLabel('Rib waveguides? ')
+        self.pcell_rib_label = QLabel("Rib waveguides? ")
         self.pcell_rib_fill = QCheckBox()
-        self.pcell_rib_fill.setChecked(self.params['rib'])
+        self.pcell_rib_fill.setChecked(self.params["rib"])
         layout_pcell.addWidget(self.pcell_rib_label)
         layout_pcell.addWidget(self.pcell_rib_fill)
         self.pcell_rib_fill.clicked(self.on_rib_click)
 
         layout_pcell.addWidget(self.button)
 
-        #******************************************************
+        # ******************************************************
         # add simulation box and add the UI elements to it
         layout_sim = QVBoxLayout()
-        self.label_sim = QLabel('Simulation definitions:')
+        self.label_sim = QLabel("Simulation definitions:")
         layout_sim.addWidget(self.label_sim)
 
         # Create a dropdown menu to select simulation import type
-        self.sim_import_label = QLabel('Import simulation definitions from:')
+        self.sim_import_label = QLabel("Import simulation definitions from:")
         self.sim_import = QComboBox()
         self.sim_import.addItem("PDK definitions")
         self.sim_import.addItem("Custom")
         layout_sim.addWidget(self.sim_import_label)
         layout_sim.addWidget(self.sim_import)
 
         # Connect the dropdown menu to a slot function
         self.sim_import.currentIndexChanged(self.on_sim_import)
 
-        self.sim_wavlstart_label = QLabel('Start wavelength (µm): ')
+        self.sim_wavlstart_label = QLabel("Start wavelength (µm): ")
         self.sim_wavlstart_fill = QLineEdit(str(self.wavl_start))
         self.sim_wavlstart_fill.setReadOnly(True)
-        self.sim_wavlstart_fill.setStyleSheet('color: gray')
+        self.sim_wavlstart_fill.setStyleSheet("color: gray")
         layout_sim.addWidget(self.sim_wavlstart_label)
         layout_sim.addWidget(self.sim_wavlstart_fill)
 
-        self.sim_wavlstop_label = QLabel('Stop wavelength (µm): ')
+        self.sim_wavlstop_label = QLabel("Stop wavelength (µm): ")
         self.sim_wavlstop_fill = QLineEdit(str(self.wavl_stop))
         self.sim_wavlstop_fill.setReadOnly(True)
-        self.sim_wavlstop_fill.setStyleSheet('color: gray')
+        self.sim_wavlstop_fill.setStyleSheet("color: gray")
         layout_sim.addWidget(self.sim_wavlstop_label)
         layout_sim.addWidget(self.sim_wavlstop_fill)
 
-        self.sim_wavlpts_label = QLabel('Wavelength points: ')
+        self.sim_wavlpts_label = QLabel("Wavelength points: ")
         self.sim_wavlpts_fill = QLineEdit(str(self.wavl_pts))
         self.sim_wavlpts_fill.setReadOnly(True)
-        self.sim_wavlpts_fill.setStyleSheet('color: gray')
+        self.sim_wavlpts_fill.setStyleSheet("color: gray")
         layout_sim.addWidget(self.sim_wavlpts_label)
         layout_sim.addWidget(self.sim_wavlpts_fill)
 
         # Polarization
-        self.sim_pol_label = QLabel('Polarization: ')
+        self.sim_pol_label = QLabel("Polarization: ")
         self.sim_pol_dropdown = QComboBox()
         self.sim_pol_dropdown.addItem("TE")
         self.sim_pol_dropdown.addItem("TM")
         layout_sim.addWidget(self.sim_pol_label)
         layout_sim.addWidget(self.sim_pol_dropdown)
 
         # coupling coefficient
-        self.sim_kappa_label = QLabel('Coupling coefficient (κ, /m): ')
+        self.sim_kappa_label = QLabel("Coupling coefficient (κ, /m): ")
         self.sim_kappa_dropdown = QComboBox()
         self.sim_kappa_dropdown.addItem("User defined")
         self.sim_kappa_dropdown.addItem("Simulate")
-        self.sim_kappa_fill = QLineEdit('24000')
+        self.sim_kappa_fill = QLineEdit("24000")
         self.sim_kappa_fill.setReadOnly(True)
-        self.sim_kappa_fill.setStyleSheet('color: gray')
+        self.sim_kappa_fill.setStyleSheet("color: gray")
         layout_sim.addWidget(self.sim_kappa_label)
         layout_sim.addWidget(self.sim_kappa_dropdown)
         layout_sim.addWidget(self.sim_kappa_fill)
 
         # Connect the dropdown menu to a slot function
         self.sim_kappa_dropdown.currentIndexChanged(self.on_kappa_dropdown)
 
         # waveguide models
-        self.sim_wg_label = QLabel('Waveguide models: ')
+        self.sim_wg_label = QLabel("Waveguide models: ")
         self.sim_wg_dropdown = QComboBox()
         self.sim_wg_dropdown.addItem("Lookup table")
         self.sim_wg_dropdown.addItem("Simulate")
         layout_sim.addWidget(self.sim_wg_label)
         layout_sim.addWidget(self.sim_wg_dropdown)
 
         # Connect the dropdown menu to a slot function
         self.sim_wg_dropdown.currentIndexChanged(self.on_wg_dropdown)
 
-        #******************************************************
+        # ******************************************************
         # add technology box and add the UI elements to it
         layout_tech = QVBoxLayout()
-        
-        self.label_tech = QLabel('Technology definitions:')
+
+        self.label_tech = QLabel("Technology definitions:")
         layout_tech.addWidget(self.label_tech)
 
         # Create a dropdown menu to select simulation import type
-        self.tech_import_label = QLabel('Import techonology definitions from: ')
+        self.tech_import_label = QLabel("Import techonology definitions from: ")
         self.tech_import = QComboBox()
         self.tech_import.addItem("PDK definitions")
         self.tech_import.addItem("Custom")
         layout_tech.addWidget(self.tech_import_label)
         layout_tech.addWidget(self.tech_import)
 
-        self.tech_devthick_label = QLabel('Waveguide thickness (µm): ')
-        self.tech_devthick_fill = QLineEdit('0.22')
+        self.tech_devthick_label = QLabel("Waveguide thickness (µm): ")
+        self.tech_devthick_fill = QLineEdit("0.22")
         self.tech_devthick_fill.setReadOnly(False)
         layout_tech.addWidget(self.tech_devthick_label)
         layout_tech.addWidget(self.tech_devthick_fill)
 
-        self.tech_ribthick_label = QLabel('Rib thickness (µm): ')
+        self.tech_ribthick_label = QLabel("Rib thickness (µm): ")
         if self.pcell_rib_fill.isChecked():
-          self.tech_ribthick_fill = QLineEdit('0.09')
-          self.tech_ribthick_fill.setReadOnly(False)
+            self.tech_ribthick_fill = QLineEdit("0.09")
+            self.tech_ribthick_fill.setReadOnly(False)
         else:
-          self.tech_ribthick_fill = QLineEdit('0.0')
-          self.tech_ribthick_fill.setReadOnly(True)
-          self.tech_ribthick_fill.setStyleSheet('color: gray')
+            self.tech_ribthick_fill = QLineEdit("0.0")
+            self.tech_ribthick_fill.setReadOnly(True)
+            self.tech_ribthick_fill.setStyleSheet("color: gray")
         layout_tech.addWidget(self.tech_ribthick_label)
         layout_tech.addWidget(self.tech_ribthick_fill)
 
-        self.tech_plot_label = QLabel('Plot result? ')
+        self.tech_plot_label = QLabel("Plot result? ")
         self.tech_plot_fill = QCheckBox()
         self.tech_plot_fill.setChecked(True)
         layout_tech.addWidget(self.tech_plot_label)
         layout_tech.addWidget(self.tech_plot_fill)
 
-        self.tech_cm_label = QLabel('Generate compact model? ')
+        self.tech_cm_label = QLabel("Generate compact model? ")
         self.tech_cm_fill = QCheckBox()
         self.tech_cm_fill.setChecked(True)
         layout_tech.addWidget(self.tech_cm_label)
         layout_tech.addWidget(self.tech_cm_fill)
 
-        self.simulate = QPushButton('Run simulation')
+        self.simulate = QPushButton("Run simulation")
         layout_tech.addWidget(self.simulate)
 
         # Connect the button to a callback function
         self.simulate.clicked(self.on_simulate_clicked)
 
-        #******************************************************
+        # ******************************************************
         # assemble and order the menus
         layout_pcell.addStretch()
         layout_sim.addStretch()
         layout_tech.addStretch()
         hbox = QHBoxLayout(self)
         hbox.addLayout(layout_pcell)
         hbox.addSpacing(20)
@@ -243,217 +259,317 @@
         hbox.addLayout(layout_tech)
 
         vbox = QVBoxLayout(self)
         vbox.addLayout(hbox)
 
         self.setLayout(vbox)
 
+    def condition_xml(self, element, indent='    ', level=0):
+        """Recursively add indentation and line breaks to the XML tree."""
+        if element:  # checks if element is not None and not an empty string/list
+            if not element.text or not element.text.strip():
+                element.text = f"\n{indent * (level+1)}"
+            if not element.tail or not element.tail.strip():
+                element.tail = f"\n{indent * level}"
+            for elem in element:
+                self.condition_xml(elem, indent, level+1)
+        else:
+            if level and (not element.tail or not element.tail.strip()):
+                element.tail = f"\n{indent * (level-1)}"
 
     def on_simulate_clicked(self):
-        
-        
+        import glob
+        import xml.etree.ElementTree as ET
 
-        N = float(self.pcell_N_fill.text)        
-        period = float(self.pcell_period_fill.text)*1e-6
-        gap = float(self.pcell_gap_fill.text)*1e-6
-        w1 = float(self.pcell_w1_fill.text)*1e-6
-        w2 = float(self.pcell_w2_fill.text)*1e-6
-        dw1 = float(self.pcell_dw1_fill.text)*1e-6
-        dw2 = float(self.pcell_dw2_fill.text)*1e-6
+        N = float(self.pcell_N_fill.text)
+        period = float(self.pcell_period_fill.text) * 1e-6
+        gap = float(self.pcell_gap_fill.text) * 1e-6
+        w1 = float(self.pcell_w1_fill.text) * 1e-6
+        w2 = float(self.pcell_w2_fill.text) * 1e-6
+        dw1 = float(self.pcell_dw1_fill.text) * 1e-6
+        dw2 = float(self.pcell_dw2_fill.text) * 1e-6
         a = float(self.pcell_apod_fill.text)
         if self.sim_pol_dropdown.currentIndex == 0:
-            pol = 'TE'
+            pol = "TE"
         else:
-            pol = 'TM'
+            pol = "TM"
         if self.pcell_rib_fill.isChecked():
             rib = True
         else:
             rib = False
 
-        thickness_device = float(self.tech_devthick_fill.text)*1e-6
-        thickness_rib = float(self.tech_ribthick_fill.text)*1e-6
-        wvl_range = [float(self.sim_wavlstart_fill.text)*1e-9, float(self.sim_wavlstop_fill.text)*1e-9]
-
-        device = ContraDC(w1= w1, dw1=dw1, w2=w2, dw2=dw2, gap=gap, a=a, period=period, rib=rib,
-        pol=pol, thickness_device=thickness_device, thickness_rib=thickness_rib, wvl_range=wvl_range)
+        thickness_device = float(self.tech_devthick_fill.text) * 1e-6
+        thickness_rib = float(self.tech_ribthick_fill.text) * 1e-6
+        wvl_range = [
+            float(self.sim_wavlstart_fill.text) * 1e-9,
+            float(self.sim_wavlstop_fill.text) * 1e-9,
+        ]
+
+        device = ContraDC(
+            N=N,
+            w1=w1,
+            dw1=dw1,
+            w2=w2,
+            dw2=dw2,
+            gap=gap,
+            a=a,
+            period=period,
+            rib=rib,
+            pol=pol,
+            thickness_device=thickness_device,
+            thickness_rib=thickness_rib,
+            wvl_range=wvl_range,
+        )
 
         if self.sim_kappa_dropdown.currentIndex == 0:
             device.kappa = float(self.sim_kappa_fill.text)
         else:
             device.simulate_kappa()
 
-        self.simulate.setText('Simulating...')
+        self.simulate.setText("Simulating...")
         device.simulate()
 
         if self.tech_plot_fill.isChecked():
             import plotly.graph_objs as go
             import plotly.offline as pyo
             import plotly.io as pio
-            #pio.renderers.default = "browser"
-            
-            drop = go.Scatter(x=device.wavelength*1e9, y=device.drop, mode='lines', name='Through')
-            thru = go.Scatter(x=device.wavelength*1e9, y=device.thru, mode='lines', name='Drop')
-            layout = go.Layout(title='Contra-directional coupler device', xaxis=dict(title='X Axis'), yaxis=dict(title='Y Axis'))
+
+            # pio.renderers.default = "browser"
+
+            drop = go.Scatter(
+                x=device.wavelength * 1e9, y=device.drop, mode="lines", name="Through"
+            )
+            thru = go.Scatter(
+                x=device.wavelength * 1e9, y=device.thru, mode="lines", name="Drop"
+            )
+            layout = go.Layout(
+                title="Contra-directional coupler device",
+                xaxis=dict(title="X Axis"),
+                yaxis=dict(title="Y Axis"),
+            )
             fig = go.Figure(data=[thru, drop], layout=layout)
             fig.show()
-        
+
         if self.tech_cm_fill.isChecked():
             # Check if there is a layout open, so we know which technology to install
             lv = pya.Application.instance().main_window().current_view()
             if lv == None:
-                raise UserWarning("To save data to the Compact Model Library, first, please create a new layout and select the desired technology:\n  Menu: File > New Layout, and a Technology.\nThen repeat.")
-            
-            # Get the Technology 
+                raise UserWarning(
+                    "To save data to the Compact Model Library, first, please create a new layout and select the desired technology:\n  Menu: File > New Layout, and a Technology.\nThen repeat."
+                )
+
+            # Get the Technology
             from SiEPIC.utils import get_layout_variables
+
             TECHNOLOGY, lv, ly, top_cell = get_layout_variables()
-            
+
             # Check if there is a CML folder in the Technology folder
             import os
-            base_path = ly.technology().base_path()    
-            folder_CML = os.path.join(base_path,'CML/%s/source_data/contraDC' % ly.technology().name)
+
+            base_path = ly.technology().base_path()
+            folder_CML = os.path.join(
+                base_path, "CML/%s/source_data/contraDC" % ly.technology().name
+            )
             if not os.path.exists(folder_CML):
-                raise UserWarning("The folder %s does not exist. \nCannot save to the Compact Model Library." %folder_CML)
-            
+                raise UserWarning(
+                    "The folder %s does not exist. \nCannot save to the Compact Model Library."
+                    % folder_CML
+                )
+
             # Generate compact model for Lumerical INTERCONNECT
             # return self.path_dat, .dat file that was created
-            device.gen_sparams(filepath=folder_CML, make_plot=False) # this will create a ContraDC_sparams.dat file to import into INTC
+            filename = device.gen_sparams(
+                filepath=folder_CML, make_plot=False
+            )  # this will create a ContraDC_sparams.dat file to import into INTC
+
+            # append data to xml
+            # Search for an XML file in folder_CML
+            xml_files = glob.glob(os.path.join(folder_CML, '*.xml'))
+            if not xml_files:
+                raise UserWarning(
+                    f"No XML file found in the folder {folder_CML}. "
+                    "Cannot save to the Compact Model Library."
+                )
+            xml_file = xml_files[0]  # Take the first XML file found
+
+            # Load and parse the XML file
+            tree = ET.parse(xml_file)
+            root = tree.getroot()
+
+            # Use the same association details for the new entry
+            new_association = ET.fromstring(f'''
+                <association>
+                    <design>
+                        <value name="wg1_width" type="double">{w1}</value>
+                        <value name="wg2_width" type="double">{w2}</value>
+                        <value name="corrugation_width1" type="double">{dw1}</value>
+                        <value name="corrugation_width2" type="double">{dw2}</value>
+                        <value name="gap" type="double">{gap}</value>
+                        <value name="grating_period" type="double">{period}</value>
+                        <value name="number_of_periods" type="int">{int(N)}</value>
+                        <value name="sinusoidal" type="double">False</value>
+                        <value name="apodization_index" type="double">{a}</value>
+                        <value name="lambda_start" type="double">{float(self.sim_wavlstart_fill.text)}</value>
+                        <value name="lambda_end" type="double">{float(self.sim_wavlstop_fill.text)}</value>
+                        <value name="lambda_points" type="double">500</value>
+                    </design>
+                    <extracted>
+                        <value name="sparam" type="string">{filename}</value>
+                    </extracted>
+                </association>''')
+
+            # Add the new association to the root element
+            root.append(new_association)
+
+            # Prettify the entire XML tree
+            self.condition_xml(root)
+
+            # Write the updated and formatted XML back to the file
+            tree.write(xml_file, encoding='utf-8', xml_declaration=True)
+            print(xml_file)
 
 
-        self.device = device
-        self.simulate.setText('Done simulating.')
 
+        self.device = device
+        self.simulate.setText("Done simulating.")
 
     def on_refresh_clicked(self):
         # fetch pcell parameters
         if self.load_pcell_params() == 0:
             return
-        self.pcell_N_fill.setText(str(self.params['number_of_periods']))
-        self.pcell_period_fill.setText(str(self.params['grating_period']))
-        self.pcell_gap_fill.setText(str(self.params['gap']))
-        self.pcell_w1_fill.setText(str(self.params['wg1_width']))
-        self.pcell_dw1_fill.setText(str(self.params['corrugation1_width']))
-        self.pcell_w2_fill.setText(str(self.params['wg2_width']))
-        self.pcell_dw2_fill.setText(str(self.params['corrugation2_width']))
-        self.pcell_apod_fill.setText(str(self.params['apodization_index']))
-        self.pcell_rib_fill.setChecked(self.params['rib'])
+        self.pcell_N_fill.setText(str(self.params["number_of_periods"]))
+        self.pcell_period_fill.setText(str(self.params["grating_period"]))
+        self.pcell_gap_fill.setText(str(self.params["gap"]))
+        self.pcell_w1_fill.setText(str(self.params["wg1_width"]))
+        self.pcell_dw1_fill.setText(str(self.params["corrugation1_width"]))
+        self.pcell_w2_fill.setText(str(self.params["wg2_width"]))
+        self.pcell_dw2_fill.setText(str(self.params["corrugation2_width"]))
+        self.pcell_apod_fill.setText(str(self.params["apodization_index"]))
+        self.pcell_rib_fill.setChecked(self.params["rib"])
 
-        self.label_pcell.setText('Parameterized cell refreshed...')
-        self.simulate.setText('Simulate')
+        self.label_pcell.setText("Parameterized cell refreshed...")
+        self.simulate.setText("Simulate")
 
     def on_sim_import(self):
         if self.sim_import.currentIndex == 0:
             # import simulation parameters from DFT
             self.load_DFT()
-            self.sim_import_label.setText('Simulation definitions: PDK')
+            self.sim_import_label.setText("Simulation definitions: PDK")
             self.sim_wavlstart_fill.setText(str(self.wavl_start))
             self.sim_wavlstart_fill.setReadOnly(True)
-            self.sim_wavlstart_fill.setStyleSheet('color: gray')
+            self.sim_wavlstart_fill.setStyleSheet("color: gray")
 
             self.sim_wavlstop_fill.setText(str(self.wavl_stop))
             self.sim_wavlstop_fill.setReadOnly(True)
-            self.sim_wavlstop_fill.setStyleSheet('color: gray')
+            self.sim_wavlstop_fill.setStyleSheet("color: gray")
 
             self.sim_wavlpts_fill.setText(str(self.wavl_pts))
             self.sim_wavlpts_fill.setReadOnly(True)
-            self.sim_wavlpts_fill.setStyleSheet('color: gray')
+            self.sim_wavlpts_fill.setStyleSheet("color: gray")
         else:
             # let user pick and ungrey the boxes
-            self.sim_import_label.setText('Simulation definitions: Custom')
+            self.sim_import_label.setText("Simulation definitions: Custom")
             self.sim_wavlstart_fill.setReadOnly(False)
-            self.sim_wavlstart_fill.setStyleSheet('color: black')
+            self.sim_wavlstart_fill.setStyleSheet("color: black")
 
             self.sim_wavlstop_fill.setReadOnly(False)
-            self.sim_wavlstop_fill.setStyleSheet('color: black')
+            self.sim_wavlstop_fill.setStyleSheet("color: black")
 
             self.sim_wavlpts_fill.setReadOnly(False)
-            self.sim_wavlpts_fill.setStyleSheet('color: black')
+            self.sim_wavlpts_fill.setStyleSheet("color: black")
 
     def on_kappa_dropdown(self):
         if self.sim_kappa_dropdown.currentIndex == 0:
             # query user for input
-            self.sim_kappa_label.setText('Coupling coefficient (κ): Custom')
+            self.sim_kappa_label.setText("Coupling coefficient (κ): Custom")
             self.sim_kappa_fill.setReadOnly(False)
-            self.sim_kappa_fill.setStyleSheet('color: black')
-            self.sim_kappa_fill.setText('Kappa (/m)')
+            self.sim_kappa_fill.setStyleSheet("color: black")
+            self.sim_kappa_fill.setText("Kappa (/m)")
         else:
             # simulate kappa using Lumerical
-            self.sim_kappa_label.setText('Coupling coefficient (κ): Simulate')
+            self.sim_kappa_label.setText("Coupling coefficient (κ): Simulate")
             self.sim_kappa_fill.setReadOnly(True)
-            self.sim_kappa_fill.setStyleSheet('color: gray')
-            self.sim_kappa_fill.setText('simulation')
+            self.sim_kappa_fill.setStyleSheet("color: gray")
+            self.sim_kappa_fill.setText("simulation")
 
     def on_wg_dropdown(self):
         if self.sim_wg_dropdown.currentIndex == 0:
             # look up if value is within lookup table index
-            self.sim_wg_label.setText('Waveguide models: LUT')
+            self.sim_wg_label.setText("Waveguide models: LUT")
         else:
             # simulate modes using Lumerical
-            self.sim_wg_label.setText('Waveguide models: Simulate')
+            self.sim_wg_label.setText("Waveguide models: Simulate")
 
     def on_rib_click(self):
         if self.pcell_rib_fill.isChecked():
-            self.tech_ribthick_fill.setText('rib thickness (µm)')
-            self.tech_ribthick_fill.setStyleSheet('color: black')
+            self.tech_ribthick_fill.setText("rib thickness (µm)")
+            self.tech_ribthick_fill.setStyleSheet("color: black")
             self.tech_ribthick_fill.setReadOnly(False)
         else:
-            self.tech_ribthick_fill.setText('0 nm')
+            self.tech_ribthick_fill.setText("0 nm")
             self.tech_ribthick_fill.setReadOnly(True)
-            self.tech_ribthick_fill.setStyleSheet('color: gray')
+            self.tech_ribthick_fill.setStyleSheet("color: gray")
 
     def load_DFT(self):
         from SiEPIC.utils import load_DFT
+
         DFT = load_DFT()
-        self.wavl_start = DFT['design-for-test']['tunable-laser'][0]['wavelength-start']
-        self.wavl_stop = DFT['design-for-test']['tunable-laser'][0]['wavelength-stop']
-        self.wavl_pts = DFT['design-for-test']['tunable-laser'][0]['wavelength-points']
-        self.pol = DFT['design-for-test']['tunable-laser'][0]['polarization']
+        self.wavl_start = DFT["design-for-test"]["tunable-laser"][0]["wavelength-start"]
+        self.wavl_stop = DFT["design-for-test"]["tunable-laser"][0]["wavelength-stop"]
+        self.wavl_pts = DFT["design-for-test"]["tunable-laser"][0]["wavelength-points"]
+        self.pol = DFT["design-for-test"]["tunable-laser"][0]["polarization"]
 
     def load_pcell_params(self):
         # get selected instances; only one
         from SiEPIC.utils import select_instances, get_layout_variables
+
         TECHNOLOGY, lv, ly, cell = get_layout_variables()
-    
+
         # print error message if no or more than one component selected
         selected_instances = select_instances()
         error = pya.QMessageBox()
         error.setStandardButtons(pya.QMessageBox.Ok)
         if len(selected_instances) != 1:
             error.setText("Error: Need to have one component selected.")
             response = error.exec_()
             return 0
-    
+
         for obj in selected_instances:
             c = cell.find_components(cell_selected=[obj.inst().cell], verbose=True)
-    
+
         # check if selected PCell is a contra DC
         if c[0].cell.basic_name() != "contra_directional_coupler":
-            error.setText("Error: selected component must be a contra_directional_coupler PCell.")
+            error.setText(
+                "Error: selected component must be a contra_directional_coupler PCell."
+            )
             response = error.exec_()
             return 0
-    
+
         # parse PCell parameters into params array
         if c[0].cell.is_pcell_variant():
             self.params = c[0].cell.pcell_parameters_by_name()
         else:
             error.setText("Error: selected component must be a contra-DC PCell.")
             response = error.exec_()
             return 0
 
     # Define the exit function
     def exit(self):
         self.close()
 
+
 def cdc_gui():
     app = pya.QApplication.instance()
     if app is None:
         app = pya.QApplication([])
 
-#    import SiEPIC._globals
-#    SiEPIC._globals.GUI_cdc = MyWindow()
-#    print(SiEPIC._globals.GUI_cdc)
-#    SiEPIC._globals.GUI_cdc.show()
+    #    import SiEPIC._globals
+    #    SiEPIC._globals.GUI_cdc = MyWindow()
+    #    print(SiEPIC._globals.GUI_cdc)
+    #    SiEPIC._globals.GUI_cdc.show()
     GUI_cdc.show()
-    
+
     app.exec_()
 
+
 GUI_cdc = MyWindow()
-print('CDC Gui: %s' % GUI_cdc)
+print("CDC Gui: %s" % GUI_cdc)
```

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/lint.py` & `siepic-0.5.7/SiEPIC/tidy3d/lint.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/make_script.py` & `siepic-0.5.7/SiEPIC/tidy3d/make_script.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/setup.py` & `siepic-0.5.7/SiEPIC/tidy3d/setup.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_adjoint_performance.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_data_performance.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_fit_web.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_plugins_web.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/_test_local/_test_web.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_IO.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_apodization.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_base.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_boundaries.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_custom.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_field_projection.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_geometry.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_grid.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_grid_spec.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_medium.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_meshgenerate.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_mode.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_monitor.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_sidewall.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_simulation.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_simulation.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_source.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_components/test_types.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_data_arrays.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_monitor_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_data/test_sim_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_config.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_log.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_make_script.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_package/test_material_library.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_adjoint.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_component_modeler.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_dispersion_fitter.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_mode_solver.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_polyslab.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_plugins/test_resonance_finder.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_auth.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_cli.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/test_web/test_webapi.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tests/utils.py` & `siepic-0.5.7/SiEPIC/tidy3d/tests/utils.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/__init__.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/__main__.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/apodization.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/base.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/boundary.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/data_array.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/dataset.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/monitor_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/data/sim_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/field_projection.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/geometry.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/grid.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/grid_spec.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/grid/mesher.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/medium.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/mode.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/monitor.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/simulation.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/simulation.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/source.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/structure.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/types.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/validators.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/components/viz.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/config.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/constants.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/log.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/material_library.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/material_library/material_reference.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/__init__.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/__init__.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/base.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/data_array.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/dataset.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/sim_data.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/geometry.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/medium.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/simulation.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/structure.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/types.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/adjoint/web.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit_web.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/derivatives.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/mode_solver.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/solver.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/mode/transforms.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/polyslab/polyslab.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/resonance/resonance.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/plugins/smatrix/smatrix.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/updater.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/asynchronous.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/auth.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/cli/app.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/config.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/container.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/httputils.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/s3utils.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/task.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/tidy3d/tidy3d/web/webapi.py` & `siepic-0.5.7/SiEPIC/tidy3d/tidy3d/web/webapi.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/__init__.py` & `siepic-0.5.7/SiEPIC/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 get_library_names
 get_technology_by_name
 get_technology
 load_Waveguides
 load_Waveguides_by_Tech
 load_Calibre
 load_Monte_Carlo
+load_Verification
 load_DFT
 load_FDTD_settings
 load_GC_settings
 get_layout_variables
 enum
 find_paths
 selected_opt_in_text
```

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/components.py` & `siepic-0.5.7/SiEPIC/utils/components.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/crossings.py` & `siepic-0.5.7/SiEPIC/utils/crossings.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/geometry.py` & `siepic-0.5.7/SiEPIC/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/klive.py` & `siepic-0.5.7/SiEPIC/utils/klive.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/layout.py` & `siepic-0.5.7/SiEPIC/utils/layout.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/utils/sampling.py` & `siepic-0.5.7/SiEPIC/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/SiEPIC/verification.py` & `siepic-0.5.7/SiEPIC/verification.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,14 +235,20 @@
           dir1 = ' below '
           dir2 = ' above '
           dir3 = 'vertically'
         
         rdb_cat_id_GCarrayconfig.description = "Circuit must be connected such that there is at most %s Grating Coupler(s) %s the opt_in label (laser injection port) and at most %s Grating Coupler(s) %s the opt_in label. \nGrating couplers must be on a %s micron pitch, %s arranged." % (
             int(DFT['design-for-test']['grating-couplers']['detectors-above-laser']), dir1,int(DFT['design-for-test']['grating-couplers']['detectors-below-laser']), dir2,float(DFT['design-for-test']['grating-couplers']['gc-pitch']),dir3)
 
+        # minimum-gc-spacing        
+        if 'minimum-gc-spacing' in DFT['design-for-test']['grating-couplers'].keys():
+            rdb_cat_id_GC_min_spacing= rdb.create_category(rdb_cat_id, "Grating coupler: minimum spacing")
+            rdb_cat_id_GC_min_spacing.description = "The grating coupler spacing (pitch) must be at least %s microns." % float(DFT['design-for-test']['grating-couplers']['minimum-gc-spacing'])
+
+
     else:
         if verbose:
             print('  No DFT rules found.')
 
     if timing:
         print("*** layout_check(), timing; done DFT")
         print('    Time elapsed: %s' % (time() - time1))    
@@ -334,14 +340,17 @@
                 print( "   - %s, %s" % (e[0], e[1]) )
         # add shapes into the results database
         for e in extra_shapes:
             if e[0].dpolygon:
                 rdb_item = rdb.create_item(rdb_cell.rdb_id(), rdb_cat_id_comp_shapesoutside.rdb_id())
                 rdb_item.add_value(pya.RdbItemValue(e[0].dpolygon.transformed(e[1].to_trans().to_itrans(dbu))))
 
+
+
+
     if timing:
         print("*** layout_check(), timing; done shapes in component ")
         print('    Time elapsed: %s' % (time() - time1))    
 
 
     # Experimental, attempt to break up the circuit into regions connected by DevRec layers
     region = pya.Region()
@@ -437,14 +446,36 @@
                         if verbose:
                             print(" - Found DFT error, GC facing the wrong way: %s, %s" %
                                   (c.component, c.trans.angle))
                         rdb_item = rdb.create_item(rdb_cell.rdb_id(), rdb_cat_id_GCorient.rdb_id())
                         rdb_item.add_value(pya.RdbItemValue( "Cell %s should be %s degrees" % (ci,DFT_GC_angle) ))
                         rdb_item.add_value(pya.RdbItemValue(c.polygon.to_dtype(dbu)))
 
+                # minimum-gc-spacing        
+                #  grating couplers need to be far enough apart for the automated probe station so it doesn't get confused
+                # check if the component "c" in the loop is a grating coupler:
+                if 'minimum-gc-spacing' in DFT['design-for-test']['grating-couplers'].keys():
+                    test = [ci.startswith(k) for k in DFT['design-for-test']['grating-couplers']['gc-orientation'].keys()]
+                    if any(test):
+                        min_gc_spacing = float(DFT['design-for-test']['grating-couplers']['minimum-gc-spacing']) / dbu
+                        for i2 in range(i + 1, len(components)):
+                            c2 = components[i2]
+                            c2i = c2.basic_name
+                            # check if the 2nd component "c2" in the loop is a grating coupler:
+                            test = [c2i.startswith(k) for k in DFT['design-for-test']['grating-couplers']['gc-orientation'].keys()]
+                            if any(test):
+                                # compare two grating coupler distances, versus the rule
+                                dist = (c.trans.disp-c2.trans.disp).abs()
+                                # print('dist: %s, %s' % (dist, min_gc_spacing))
+                                if dist < min_gc_spacing:
+                                    rdb_item = rdb.create_item(rdb_cell.rdb_id(), rdb_cat_id_GC_min_spacing.rdb_id())
+                                    rdb_item.add_value(pya.RdbItemValue( "Grating couplers should be at least %s microns apart (center-to-center pitch)" % (min_gc_spacing) ))
+                                    rdb_item.add_value(pya.RdbItemValue(c.polygon.to_dtype(dbu)))
+                                    rdb_item.add_value(pya.RdbItemValue(c2.polygon.to_dtype(dbu)))
+
 
         # Pre-simulation check: do components have models?
         # disabled by lukasc, 2021/05
         if 0 and not c.has_model():
             if verbose:
                 print(" - Missing compact model, for component: %s" % (c.component))
             rdb_item = rdb.create_item(rdb_cell.rdb_id(), rdb_cat_id_sim_nomodel.rdb_id())
@@ -493,28 +524,31 @@
                     rdb_item = rdb.create_item(
                         rdb_cell.rdb_id(), rdb_cat_id_optin_polarization.rdb_id())
                     rdb_item.add_value(pya.RdbItemValue(pya.Polygon(box).to_dtype(dbu)))
     
                 # find the GC closest to the opt_in label.
                 components_sorted = sorted([c for c in components if [p for p in c.pins if p.type == _globals.PIN_TYPES.OPTICALIO]],
                                            key=lambda x: x.trans.disp.to_p().distance(pya.Point(t.x, t.y).to_dtype(1)))
-                # GC too far check:
+                # GC opt_in label too far check:
                 if components_sorted:
                     dist_optin_c = components_sorted[0].trans.disp.to_p(
                     ).distance(pya.Point(t.x, t.y).to_dtype(1))
                     if verbose:
                         print(" - Found opt_in: %s, nearest GC: %s.  Locations: %s, %s. distance: %s" % (opt_in[ti1][
                               'Text'], components_sorted[0].instance,  components_sorted[0].center, pya.Point(t.x, t.y), dist_optin_c * dbu))
                     if dist_optin_c > float(DFT['design-for-test']['opt_in']['max-distance-to-grating-coupler']) * 1000:
                         if verbose:
                             print(" - opt_in label too far from the nearest grating coupler: %s, %s" %
                                   (components_sorted[0].instance, opt_in[ti1]['opt_in']))
                         rdb_item = rdb.create_item(rdb_cell.rdb_id(), rdb_cat_id_optin_toofar.rdb_id())
                         rdb_item.add_value(pya.RdbItemValue(pya.Polygon(box).to_dtype(dbu)))
-    
+                        rdb_item.add_value(pya.RdbItemValue(components_sorted[0].polygon.to_dtype(dbu)))
+                        # it would be nice to highlight the entire text, but bbox returns a point https://www.klayout.de/doc-qt5/code/class_DText.html#method18
+                        # rdb_item.add_value(pya.RdbItemValue(t.bbox()))
+
                     # starting with each opt_in label, identify the sub-circuit, then GCs, and
                     # check for GC spacing
                     trimmed_nets, trimmed_components = trim_netlist(
                         nets, components, components_sorted[0])
                     components_connected_opt_in = components_connected_opt_in + trimmed_components
                     detector_GCs = [c for c in trimmed_components if [p for p in c.pins if p.type == _globals.PIN_TYPES.OPTICALIO] if (
                         c.trans.disp - components_sorted[0].trans.disp).to_p() != pya.DPoint(0, 0)]
```

### Comparing `SiEPIC-0.5.5/SiEPIC.egg-info/PKG-INFO` & `siepic-0.5.7/SiEPIC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: SiEPIC
-Version: 0.5.5
+Version: 0.5.7
 Summary: SiEPIC-Tools: for silicon photonics layout, design, verification and circuit simulation
 Author-email: Lukas Chrostowski <lukasc@ece.ubc.ca>
 Project-URL: Homepage, https://github.com/SiEPIC/SiEPIC-Tools
 Project-URL: Issues, https://github.com/SiEPIC/SiEPIC-Tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: pandas
 
 # SiEPIC-Tools
 
 - SiEPIC-Tools - for silicon photonics layout, design, verification and circuit simulation
 - Developed within the <a href="http://www.siepic.ubc.ca">SiEPIC</a> program, by <a href="https://ca.linkedin.com/in/chrostowski">Lukas Chrostowski</a>, with contributions from many others.
 - This is a package implemented using Python in <a href="http://www.klayout.de">KLayout</a>.
 - Instruction on design, layout, fabrication, test, data analysis for silicon photonics provided in the edX course: <a href="http://edx.org/course/silicon-photonics-design-fabrication-ubcx-phot1x">Silicon Photonics Design, Fabrication and Data Analysis</a> and textbook <a href="http://www.cambridge.org/ca/academic/subjects/engineering/electronic-optoelectronic-devices-and-nanotechnology/silicon-photonics-design-devices-systems">Silicon Photonics Design: From Devices to Systems</a> by Lukas Chrostowski and Michael Hochberg.
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: SiEPIC Version: 0.5.5 Summary: SiEPIC-Tools: for
+Metadata-Version: 2.1 Name: SiEPIC Version: 0.5.7 Summary: SiEPIC-Tools: for
 silicon photonics layout, design, verification and circuit simulation Author-
 email: Lukas Chrostowski
 ece.ubc.ca> Project-URL: Homepage, https://github.com/SiEPIC/SiEPIC-Tools
 Project-URL: Issues, https://github.com/SiEPIC/SiEPIC-Tools/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: numpy Requires-Dist:
-scipy # SiEPIC-Tools - SiEPIC-Tools - for silicon photonics layout, design,
-verification and circuit simulation - Developed within the _S_i_E_P_I_C program, by
-_L_u_k_a_s_ _C_h_r_o_s_t_o_w_s_k_i, with contributions from many others. - This is a package
-implemented using Python in _K_L_a_y_o_u_t. - Instruction on design, layout,
-fabrication, test, data analysis for silicon photonics provided in the edX
-course: _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_,_ _F_a_b_r_i_c_a_t_i_o_n_ _a_n_d_ _D_a_t_a_ _A_n_a_l_y_s_i_s and textbook
-_S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_:_ _F_r_o_m_ _D_e_v_i_c_e_s_ _t_o_ _S_y_s_t_e_m_s by Lukas Chrostowski and
-Michael Hochberg. - Process Design Kits that use KLayout SiEPIC-Tools are
-available for multiple foundries including _A_M_F, _A_I_M_ _P_h_o_t_o_n_i_c_s, _T_o_w_e_r
-_S_e_m_i_c_o_n_d_u_c_t_o_r, _L_i_g_e_n_t_e_c, _A_p_p_l_i_e_d_ _N_a_n_o_t_o_o_l_s_ _I_n_c_., and _S_i_E_P_I_C_f_a_b. - Citing this
-work: - Lukas Chrostowski, Zeqin Lu, Jonas Flueckiger, Xu Wang, Jackson Klein,
-Amy Liu, Jaspreet Jhoja, James Pond, "_D_e_s_i_g_n_ _a_n_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_l_i_c_o_n_ _p_h_o_t_o_n_i_c
-_s_c_h_e_m_a_t_i_c_s_ _a_n_d_ _l_a_y_o_u_t_s," Proc. SPIE 9891, Silicon Photonics and Photonic
-Integrated Circuits V, 989114 (May 13, 2016); doi:10.1117/12.2230376. - Lukas
-Chrostowski, Hossam Shoman, Mustafa Hammood, Han Yun, Jaspreet Jhoja, Enxiao
-Luan, Stephen Lin, Ajay Mistry, Donald Witt, Nicolas A. F. Jaeger, Sudip
+scipy Requires-Dist: pandas # SiEPIC-Tools - SiEPIC-Tools - for silicon
+photonics layout, design, verification and circuit simulation - Developed
+within the _S_i_E_P_I_C program, by _L_u_k_a_s_ _C_h_r_o_s_t_o_w_s_k_i, with contributions from many
+others. - This is a package implemented using Python in _K_L_a_y_o_u_t. - Instruction
+on design, layout, fabrication, test, data analysis for silicon photonics
+provided in the edX course: _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_,_ _F_a_b_r_i_c_a_t_i_o_n_ _a_n_d_ _D_a_t_a
+_A_n_a_l_y_s_i_s and textbook _S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_s_ _D_e_s_i_g_n_:_ _F_r_o_m_ _D_e_v_i_c_e_s_ _t_o_ _S_y_s_t_e_m_s by
+Lukas Chrostowski and Michael Hochberg. - Process Design Kits that use KLayout
+SiEPIC-Tools are available for multiple foundries including _A_M_F, _A_I_M_ _P_h_o_t_o_n_i_c_s,
+_T_o_w_e_r_ _S_e_m_i_c_o_n_d_u_c_t_o_r, _L_i_g_e_n_t_e_c, _A_p_p_l_i_e_d_ _N_a_n_o_t_o_o_l_s_ _I_n_c_., and _S_i_E_P_I_C_f_a_b. - Citing
+this work: - Lukas Chrostowski, Zeqin Lu, Jonas Flueckiger, Xu Wang, Jackson
+Klein, Amy Liu, Jaspreet Jhoja, James Pond, "_D_e_s_i_g_n_ _a_n_d_ _s_i_m_u_l_a_t_i_o_n_ _o_f_ _s_i_l_i_c_o_n
+_p_h_o_t_o_n_i_c_ _s_c_h_e_m_a_t_i_c_s_ _a_n_d_ _l_a_y_o_u_t_s," Proc. SPIE 9891, Silicon Photonics and
+Photonic Integrated Circuits V, 989114 (May 13, 2016); doi:10.1117/12.2230376.
+- Lukas Chrostowski, Hossam Shoman, Mustafa Hammood, Han Yun, Jaspreet Jhoja,
+Enxiao Luan, Stephen Lin, Ajay Mistry, Donald Witt, Nicolas A. F. Jaeger, Sudip
 Shekhar, Hasitha Jayatilleka, Philippe Jean, Simon B.-de Villers, Jonathan
 Cauchon, Wei Shi, Cameron Horvath, Jocelyn N. Westwood-Bachman, Kevin Setzer,
 Mirwais Aktary, N. Shane Patrick, Richard Bojko, Amin Khavasi, Xu Wang, Thomas
 Ferreira de Lima, Alexander N. Tait, Paul R. Prucnal, David E. Hagan, Doris
 Stevanovic, Andy P. Knights, "_S_i_l_i_c_o_n_ _P_h_o_t_o_n_i_c_ _C_i_r_c_u_i_t_ _D_e_s_i_g_n_ _U_s_i_n_g_ _R_a_p_i_d
 _P_r_o_t_o_t_y_p_i_n_g_ _F_o_u_n_d_r_y_ _P_r_o_c_e_s_s_ _D_e_s_i_g_n_ _K_i_t_s" IEEE Journal of Selected Topics in
 Quantum Electronics, Volume: 25, Issue: 5, Sept.-Oct. 2019. (_P_D_F)
```

### Comparing `SiEPIC-0.5.5/SiEPIC.egg-info/SOURCES.txt` & `siepic-0.5.7/SiEPIC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SiEPIC-0.5.5/pyproject.toml` & `siepic-0.5.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "SiEPIC"
-version = "0.5.5"
+version = "0.5.7"
 authors = [
   { name="Lukas Chrostowski", email="lukasc@ece.ubc.ca" },
 ]
 description = "SiEPIC-Tools: for silicon photonics layout, design, verification and circuit simulation"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy", 
-  "scipy"] 
+  "scipy",
+  "pandas"] 
 
 [project.urls]
 Homepage = "https://github.com/SiEPIC/SiEPIC-Tools"
 Issues = "https://github.com/SiEPIC/SiEPIC-Tools/issues"
```

