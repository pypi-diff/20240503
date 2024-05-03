# Comparing `tmp/grid_data_models-0.2.0.tar.gz` & `tmp/grid_data_models-0.3.0.tar.gz`

## Comparing `grid_data_models-0.2.0.tar` & `grid_data_models-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,65 @@
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/bus.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/capacitor.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/constants.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/exceptions.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/load.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/quantities.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transformer.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/cost_model.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/dataset_system.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/__init__.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/curve.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_common.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_enum.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_graph.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_system.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/limitset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/sequence_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_branch.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_bus.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_capacitor.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_component.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_feeder.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_fuse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_load.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_recloser.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_regulator.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_solar.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_substation.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_switch.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_transformer.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_vsource.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/geometry_branch.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_branch.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_fuse.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_recloser.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_switch.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/sequence_impedance_branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/__init__.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_switch_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/capacitor_equipment.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/inverter_equipment.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/load_equipment.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_load_equipment.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/solar_equipment.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_branch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_bus.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_capacitor.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_component.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_load.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_substation.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/.gitignore
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/README.md
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/constants.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/exceptions.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/quantities.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/dataset/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/dataset/cost_model.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/dataset/dataset_system.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/curve.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/distribution_common.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/distribution_enum.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/distribution_graph.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/distribution_system.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/limitset.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/sequence_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/__init__.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_branch.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_bus.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_capacitor.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_component.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_feeder.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_fuse.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_load.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_recloser.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_regulator.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_solar.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_substation.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_switch.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_transformer.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/distribution_vsource.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/geometry_branch.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_branch.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_fuse.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_recloser.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_switch.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/components/sequence_impedance_branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/__init__.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_switch_controller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/capacitor_equipment.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/inverter_equipment.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/load_equipment.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/phase_load_equipment.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/src/gdm/distribution/equipment/solar_equipment.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/README.md
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 grid_data_models-0.3.0/PKG-INFO
```

### Comparing `grid_data_models-0.2.0/src/gdm/__init__.py` & `grid_data_models-0.3.0/src/gdm/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -159,14 +159,7 @@
     ConnectionType,
     VoltageTypes,
     LimitType,
 )
 from gdm.distribution.distribution_system import DistributionSystem
 from gdm.distribution.distribution_graph import build_graph_from_system
 from gdm.distribution.curve import Curve, TimeCurrentCurve
-
-from gdm.transmission.transmission_bus import TransmissionBus
-from gdm.transmission.transmission_component import TransmissionComponent
-from gdm.transmission.transmission_branch import TransmissionBranch
-from gdm.transmission.transmission_capacitor import TransmissionCapacitor
-from gdm.transmission.transmission_load import TransmissionLoad
-from gdm.transmission.transmission_substation import TransmissionSubstation
```

### Comparing `grid_data_models-0.2.0/src/gdm/quantities.py` & `grid_data_models-0.3.0/src/gdm/quantities.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/version.py` & `grid_data_models-0.3.0/src/gdm/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import subprocess
 import platform
 import sys
 
-VERSION = "0.2.0"
+VERSION = "0.3.0"
 
 
 def is_git_repo(dir: Path) -> bool:
     """Returns true if it is a git repo."""
     git_path = dir / ".git"
     return git_path.exists()
```

### Comparing `grid_data_models-0.2.0/src/gdm/dataset/cost_model.py` & `grid_data_models-0.3.0/src/gdm/dataset/cost_model.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/dataset/dataset_system.py` & `grid_data_models-0.3.0/src/gdm/dataset/dataset_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/curve.py` & `grid_data_models-0.3.0/src/gdm/distribution/curve.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/distribution_enum.py` & `grid_data_models-0.3.0/src/gdm/distribution/distribution_enum.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/distribution_graph.py` & `grid_data_models-0.3.0/src/gdm/distribution/distribution_graph.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/distribution_system.py` & `grid_data_models-0.3.0/src/gdm/distribution/distribution_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/limitset.py` & `grid_data_models-0.3.0/src/gdm/distribution/limitset.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_branch.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_branch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """ This module contains distribution branch. """
 
 from typing import Annotated
 from itertools import product
 
 from pydantic import model_validator, Field
-from infrasys import Component
 
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.distribution.distribution_enum import Phase
+from gdm.distribution.components.distribution_component import DistributionComponent
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.quantities import (
     PositiveDistance,
     PositiveVoltage,
 )
 from gdm.constants import PINT_SCHEMA
 
 
-class DistributionBranch(Component):
+class DistributionBranch(DistributionComponent):
     """Interface for distribution branch."""
 
-    belongs_to: BELONG_TO_TYPE
     buses: Annotated[
         list[DistributionBus],
         Field(..., description="List of buses connecting a branch."),
     ]
     length: Annotated[
         PositiveDistance, PINT_SCHEMA, Field(..., description="Length of the branch.")
     ]
@@ -67,27 +67,33 @@
     @classmethod
     def example(cls) -> "DistributionBranch":
         """Example for base distribution branch."""
         bus1 = DistributionBus(
             voltage_type="line-to-ground",
             phases=[Phase.A, Phase.B, Phase.C],
             nominal_voltage=PositiveVoltage(400, "volt"),
-            name="DistBus1",
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
+            name="Branch-DistBus1",
         )
         bus2 = DistributionBus(
             voltage_type="line-to-ground",
             phases=[Phase.A, Phase.B, Phase.C],
             nominal_voltage=PositiveVoltage(400, "volt"),
-            name="DistBus2",
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
+            name="Branch-DistBus2",
         )
         return DistributionBranch(
             buses=[bus1, bus2],
             length=PositiveDistance(130.2, "meter"),
             phases=[Phase.A, Phase.B, Phase.C],
-            name="p14u405",
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
+            name="DistBranch1",
         )
 
 
 class SwitchedDistributionBranch(DistributionBranch):
     """Interface for distribution branch that can be toggled."""
 
     is_closed: Annotated[list[bool], Field(description="Status of branch for each phase.")]
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_bus.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_bus.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 """ This module contains interface for Distribution Bus."""
 
-from typing import Annotated
+from typing import Annotated, Optional
 
 from infrasys import Location
 from pydantic import Field
 
 from gdm.distribution.distribution_enum import LimitType, Phase, VoltageTypes
 from gdm.distribution.components.distribution_component import DistributionComponent
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.distribution.limitset import VoltageLimitSet
 from gdm.quantities import PositiveVoltage
-from gdm.bus import PowerSystemBus
+from gdm.constants import PINT_SCHEMA
 
 
-class DistributionBus(PowerSystemBus):
+class DistributionBus(DistributionComponent):
     """Interface for distribution bus.
 
     Examples:
         >>> from gdm import DistributionBus
         >>> DistributionBus.example()
     """
 
     voltage_type: Annotated[VoltageTypes, Field(..., description="Voltage types for buses.")]
-    belongs_to: BELONG_TO_TYPE
     phases: Annotated[list[Phase], Field(..., description="List of phases for this bus.")]
     voltagelimits: Annotated[
         list[VoltageLimitSet],
         Field([], description="List of voltage limit sets for this bus."),
     ]
+    nominal_voltage: Annotated[
+        PositiveVoltage,
+        PINT_SCHEMA,
+        Field(..., description="Nominal voltage for this bus."),
+    ]
+    coordinate: Annotated[
+        Optional[Location],
+        Field(None, description="Coordinate for the power system bus."),
+    ]
 
     @classmethod
     def example(cls) -> "DistributionBus":
         return DistributionBus(
             voltage_type=VoltageTypes.LINE_TO_LINE,
-            belongs_to=DistributionComponent.example(),
             phases=[Phase.A, Phase.B, Phase.C],
             nominal_voltage=PositiveVoltage(400, "volt"),
             name="DistBus1",
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
             voltagelimits=[
                 VoltageLimitSet(
                     limit_type=LimitType.MIN, value=PositiveVoltage(400 * 0.9, "volt")
                 ),
                 VoltageLimitSet(
                     limit_type=LimitType.MAX, value=PositiveVoltage(400 * 1.1, "volt")
                 ),
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_capacitor.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_capacitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """ This module contains interface for distribution system capacitor."""
 
 from typing import Annotated
 
-from infrasys import Component
 from pydantic import Field, model_validator
 
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.distribution.equipment.capacitor_equipment import CapacitorEquipment
+from gdm.distribution.components.distribution_component import DistributionComponent
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.quantities import PositiveVoltage
 from gdm.distribution.distribution_enum import Phase
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.controllers.distribution_capacitor_controller import (
     CapacitorController,
     VoltageCapacitorController,
 )
 
 
-class DistributionCapacitor(Component):
+class DistributionCapacitor(DistributionComponent):
     """Interface for capacitor present in distribution system models."""
 
     bus: Annotated[
         DistributionBus,
         Field(
             ...,
             description="Distribution bus to which this capacitor is connected to.",
         ),
     ]
-    belongs_to: BELONG_TO_TYPE
     phases: Annotated[
         list[Phase],
         Field(
             ...,
             description=(
                 "List of phases at which this phase capacitors"
                 "are connected to in the same order."
@@ -71,18 +71,22 @@
     @classmethod
     def example(cls) -> "DistributionCapacitor":
         """Example for distribution capacitor."""
         return DistributionCapacitor(
             name="Capacitor1",
             bus=DistributionBus(
                 voltage_type="line-to-ground",
-                name="Bus1",
+                name="Capacitor-DistBus1",
                 nominal_voltage=PositiveVoltage(400, "volt"),
                 phases=[Phase.A, Phase.B, Phase.C],
+                substation=DistributionSubstation.example(),
+                feeder=DistributionFeeder.example(),
             ),
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
             phases=[Phase.A, Phase.B, Phase.C],
             equipment=CapacitorEquipment.example(),
             controllers=[
                 VoltageCapacitorController.example(),
                 VoltageCapacitorController.example(),
                 VoltageCapacitorController.example(),
             ],
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_component.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from gdm.distribution.components.distribution_feeder import DistributionFeeder
 from gdm.distribution.components.distribution_substation import DistributionSubstation
 
 
 class DistributionComponent(Component):
     """Interface for simple distribution component."""
 
-    name: Annotated[str, Field("", description="Name of the component.")]
     substation: Annotated[
         Optional[DistributionSubstation], Field(None, description="Name of the substation.")
     ]
     feeder: Annotated[Optional[DistributionFeeder], Field(None, description="Name of the feeder.")]
 
     @classmethod
     def example(cls) -> "DistributionComponent":
         return DistributionComponent(
-            substation=DistributionSubstation.example(), feeder=DistributionFeeder.example()
+            name="BaseComponent",
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example()
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_load.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_load.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """ This module contains interface for distribution load."""
 
 from typing import Annotated
 
 from pydantic import model_validator, Field
-from infrasys import Component
 
 from gdm.distribution.distribution_enum import Phase
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.components.distribution_bus import DistributionBus
+from gdm.distribution.components.distribution_component import DistributionComponent
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.quantities import PositiveVoltage
 from gdm.distribution.equipment.load_equipment import LoadEquipment
 
 
-class DistributionLoad(Component):
+class DistributionLoad(DistributionComponent):
     """Interface for distribution load."""
 
     bus: Annotated[
         DistributionBus,
         Field(
             ...,
             description="Distribution bus to which this load is connected to.",
         ),
     ]
-    belongs_to: BELONG_TO_TYPE
     phases: Annotated[
         list[Phase],
         Field(..., description="Phases to which this load is connected to."),
     ]
     equipment: Annotated[LoadEquipment, Field(..., description="Load model.")]
 
     @model_validator(mode="after")
@@ -47,14 +47,18 @@
     @classmethod
     def example(cls) -> "DistributionLoad":
         """Example for distribution load."""
         return DistributionLoad(
             name="DistributionLoad1",
             bus=DistributionBus(
                 voltage_type="line-to-ground",
-                name="Bus1",
+                name="Load-DistBus1",
                 phases=[Phase.A, Phase.B, Phase.C],
+                substation=DistributionSubstation.example(),
+                feeder=DistributionFeeder.example(),
                 nominal_voltage=PositiveVoltage(0.4, "kilovolt"),
             ),
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
             phases=[Phase.A, Phase.B, Phase.C],
             equipment=LoadEquipment.example(),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_regulator.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_regulator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """This module contains distribution regulator."""
 
 from typing import Annotated
 
 from pydantic import Field, model_validator
 
 from gdm.distribution.components.distribution_transformer import DistributionTransformer
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.distribution.controllers.distribution_regulator_controller import RegulatorController
 from gdm.distribution.equipment.distribution_transformer_equipment import (
     TapWindingEquipment,
     DistributionTransformerEquipment,
 )
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.distribution.distribution_enum import Phase
@@ -61,22 +63,26 @@
     def example(cls) -> "DistributionRegulator":
         """Example for Voltage Regulator"""
         return DistributionRegulator(
             name="DistributionRegulator1",
             buses=[
                 DistributionBus(
                     voltage_type="line-to-ground",
-                    name="Bus1",
+                    name="Regulator-DistBus1",
                     nominal_voltage=PositiveVoltage(12.47, "kilovolt"),
+                    substation=DistributionSubstation.example(),
+                    feeder=DistributionFeeder.example(),
                     phases=[Phase.A, Phase.B, Phase.C],
                 ),
                 DistributionBus(
                     voltage_type="line-to-ground",
-                    name="Bus2",
+                    name="Regulator-DistBus2",
                     nominal_voltage=PositiveVoltage(12.47, "kilovolt"),
+                    substation=DistributionSubstation.example(),
+                    feeder=DistributionFeeder.example(),
                     phases=[Phase.A, Phase.B, Phase.C],
                 ),
             ],
             winding_phases=[[Phase.A, Phase.B, Phase.C], [Phase.A, Phase.B, Phase.C]],
             equipment=DistributionTransformerEquipment.example_with_taps(),
             controllers=[
                 RegulatorController.example(),
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_substation.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_substation.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_transformer.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """ This module contains interface for distribution transformer."""
 
 import math
 from typing import Annotated
 
-from infrasys import Component
 from infrasys.quantities import Voltage
 from pydantic import Field, model_validator
 
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.distribution_enum import Phase, VoltageTypes
 from gdm.quantities import PositiveVoltage
 from gdm.distribution.components.distribution_bus import DistributionBus
+from gdm.distribution.components.distribution_component import DistributionComponent
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 from gdm.distribution.equipment.distribution_transformer_equipment import (
     DistributionTransformerEquipment,
 )
 
 
 def get_phase_voltage_in_kv(
     voltage: Voltage, voltage_type: VoltageTypes, split_phase_secondary: bool = False
 ) -> Voltage:
     """Function to return phase voltage"""
     kv_voltage = voltage.to("kilovolt")
     factor = math.sqrt(3) if not split_phase_secondary else 2
     return kv_voltage / factor if voltage_type == VoltageTypes.LINE_TO_LINE else kv_voltage
 
 
-class DistributionTransformer(Component):
+class DistributionTransformer(DistributionComponent):
     """Interface for distribution transformer."""
 
-    belongs_to: BELONG_TO_TYPE
-
     buses: Annotated[
         list[DistributionBus],
         Field(
             ...,
             description="List of distribution buses in the same order as windings. ",
         ),
     ]
@@ -118,21 +117,25 @@
     def example(cls) -> "DistributionTransformer":
         """Example for distribution transformer."""
         return DistributionTransformer(
             name="DistributionTransformer1",
             buses=[
                 DistributionBus(
                     voltage_type=VoltageTypes.LINE_TO_LINE,
-                    name="Bus1",
+                    name="Transformer-DistBus1",
                     nominal_voltage=PositiveVoltage(12.47, "kilovolt"),
+                    substation=DistributionSubstation.example(),
+                    feeder=DistributionFeeder.example(),
                     phases=[Phase.A, Phase.B, Phase.C],
                 ),
                 DistributionBus(
                     voltage_type=VoltageTypes.LINE_TO_LINE,
-                    name="Bus2",
+                    name="Transformer-DistBus2",
                     nominal_voltage=PositiveVoltage(0.4, "kilovolt"),
+                    substation=DistributionSubstation.example(),
+                    feeder=DistributionFeeder.example(),
                     phases=[Phase.A, Phase.B, Phase.C],
                 ),
             ],
             winding_phases=[[Phase.A, Phase.B, Phase.C], [Phase.A, Phase.B, Phase.C]],
             equipment=DistributionTransformerEquipment.example(),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_vsource.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/distribution_vsource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """This module contains interface for distribution substation."""
 
 from typing import Annotated
 
-from infrasys import Component
 from infrasys.quantities import Angle, Resistance, Voltage
 from pydantic import Field
 
-from gdm.distribution.distribution_common import BELONG_TO_TYPE
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.quantities import Reactance, PositiveVoltage
 from gdm.distribution.distribution_enum import Phase
 from gdm.constants import PINT_SCHEMA
+from gdm.distribution.components.distribution_component import DistributionComponent
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
 
 
-class PhaseVoltageSourceEquipment(Component):
+class PhaseVoltageSourceEquipment(DistributionComponent):
     """Interface for phase voltage source."""
 
     r0: Annotated[Resistance, PINT_SCHEMA, Field(..., description="Zero sequence resistance.")]
     r1: Annotated[Resistance, PINT_SCHEMA, Field(..., description="Positive sequence resistance.")]
     x0: Annotated[Reactance, PINT_SCHEMA, Field(..., description="Zero sequence reactance.")]
     x1: Annotated[Reactance, PINT_SCHEMA, Field(..., description="Positive sequence reactane.")]
     voltage: Annotated[
@@ -32,18 +33,20 @@
             name="phase-source-1",
             r0=Resistance(0.001, "ohm"),
             r1=Resistance(0.001, "ohm"),
             x0=Reactance(0.001, "ohm"),
             x1=Reactance(0.001, "ohm"),
             voltage=PositiveVoltage(132.0, "kilovolt"),
             angle=Angle(180, "degree"),
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
         )
 
 
-class VoltageSourceEquipment(Component):
+class VoltageSourceEquipment(DistributionComponent):
     """Interface for voltage source model."""
 
     sources: Annotated[
         list[PhaseVoltageSourceEquipment],
         Field(
             ...,
             description="list of single phase voltage sources",
@@ -54,18 +57,17 @@
     def example(cls) -> "VoltageSourceEquipment":
         """Example for voltage source model."""
         return VoltageSourceEquipment(
             name="Voltage Source 1", sources=[PhaseVoltageSourceEquipment.example()] * 3
         )
 
 
-class DistributionVoltageSource(Component):
+class DistributionVoltageSource(DistributionComponent):
     """Interface for distribution substation."""
 
-    belongs_to: BELONG_TO_TYPE
     bus: Annotated[
         DistributionBus,
         Field(
             ...,
             description="Distribution bus to which this voltage source is connected to.",
         ),
     ]
@@ -75,9 +77,11 @@
     @classmethod
     def example(cls) -> "DistributionVoltageSource":
         """Example for distribution voltage source."""
         return DistributionVoltageSource(
             name="DistributionVoltageSource1",
             bus=DistributionBus.example(),
             phases=[Phase.A, Phase.B, Phase.C],
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
             equipment=VoltageSourceEquipment.example(),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/geometry_branch.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/sequence_impedance_branch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-"""This module contains geometry branch."""
+"""This module contains sequence impedance branch."""
 
 from typing import Annotated
 
-from pydantic import Field
+from pydantic import Field, model_validator
 
 from gdm.distribution.components.distribution_branch import DistributionBranch
-from gdm.distribution.equipment.geometry_branch_equipment import GeometryBranchEquipment
+from gdm.distribution.components.distribution_feeder import DistributionFeeder
+from gdm.distribution.components.distribution_substation import DistributionSubstation
+from gdm.distribution.equipment.sequence_impedance_branch_equipment import (
+    SequenceImpedanceBranchEquipment,
+)
 
 
-class GeometryBranch(DistributionBranch):
-    """Interface for geometry based lines."""
+class SequenceImpedanceBranch(DistributionBranch):
+    """Interface for sequence impedance branch."""
 
     equipment: Annotated[
-        GeometryBranchEquipment, Field(..., description="Geometry branch equipment.")
+        SequenceImpedanceBranchEquipment, Field(..., description="Sequence impedance branch.")
     ]
 
-    def validate_fields(self) -> "GeometryBranch":
-        """Custom validator for geometry branch fields."""
-        if len(self.phases) != len(self.equipment.conductors):
-            msg = "Number of phases is not equal to number of wires."
+    @model_validator(mode="after")
+    def validate_fields(self) -> "SequenceImpedanceBranch":
+        """Custom validator for sequence impedance branch."""
+        if len(self.phases) == 1:
+            msg = f"Sequence impedance assigned to single phase {self.phases=}"
             raise ValueError(msg)
         return self
 
     @classmethod
-    def example(cls) -> "GeometryBranch":
-        """Example for geometry branch."""
+    def example(cls) -> "SequenceImpedanceBranch":
+        """Example for sequence impedance branch."""
         base_branch = DistributionBranch.example()
-        return GeometryBranch(
+        return SequenceImpedanceBranch(
             buses=base_branch.buses,
             length=base_branch.length,
             phases=base_branch.phases,
             name=base_branch.name,
-            equipment=GeometryBranchEquipment.example(),
+            substation=DistributionSubstation.example(),
+            feeder=DistributionFeeder.example(),
+            equipment=SequenceImpedanceBranchEquipment.example(),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_branch.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_switch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-"""This module contains matrix impedance branch."""
+"""This module contains matrix impedance switch."""
 
 from typing import Annotated
 
 from pydantic import Field, model_validator
 
-from gdm.distribution.components.distribution_branch import DistributionBranch
-from gdm.distribution.equipment.matrix_impedance_branch_equipment import (
-    MatrixImpedanceBranchEquipment,
+from gdm.distribution.equipment.matrix_impedance_switch_equipment import (
+    MatrixImpedanceSwitchEquipment,
 )
+from gdm.distribution.components.distribution_switch import DistributionSwitch
 
 
-class MatrixImpedanceBranch(DistributionBranch):
-    """Interface for matrix impedance branch."""
+class MatrixImpedanceSwitch(DistributionSwitch):
+    """Interface for matrix impedance switch."""
 
     equipment: Annotated[
-        MatrixImpedanceBranchEquipment,
+        MatrixImpedanceSwitchEquipment,
         Field(..., description="Matrix impedance branch equipment."),
     ]
 
     @model_validator(mode="after")
-    def validate_fields(self) -> "MatrixImpedanceBranch":
+    def validate_fields(self) -> "MatrixImpedanceSwitch":
         """Custom validator for matrix impedance branch."""
         for mat in [
             self.equipment.r_matrix,
             self.equipment.x_matrix,
             self.equipment.c_matrix,
         ]:
             if set(mat.shape) != {len(self.phases)}:
                 msg = f"Length of matrix {mat=} did not match number of phases {self.phases=}"
                 raise ValueError(msg)
 
         return self
 
     @classmethod
-    def example(cls) -> "MatrixImpedanceBranch":
+    def example(cls) -> "MatrixImpedanceSwitch":
         """Example for matrix impedance branch."""
-        base_branch = DistributionBranch.example()
-        return MatrixImpedanceBranch(
-            buses=base_branch.buses,
-            length=base_branch.length,
-            phases=base_branch.phases,
-            name=base_branch.name,
-            equipment=MatrixImpedanceBranchEquipment.example(),
+        return MatrixImpedanceSwitch(
+            **DistributionSwitch.example().model_dump(exclude_none=True),
+            equipment=MatrixImpedanceSwitchEquipment.example(),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_fuse.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_fuse.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_recloser.py` & `grid_data_models-0.3.0/src/gdm/distribution/components/matrix_impedance_recloser.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py` & `grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_inverter_controller.py` & `grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_inverter_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_recloser_controller.py` & `grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_recloser_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_regulator_controller.py` & `grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_regulator_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_switch_controller.py` & `grid_data_models-0.3.0/src/gdm/distribution/controllers/distribution_switch_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/bare_conductor_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/bare_conductor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/capacitor_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/concentric_cable_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/concentric_cable_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             strict=True,
             ge=0,
             le=100,
             description="Percentage no load losses for this transformer.",
         ),
     ]
     windings: Annotated[
-        list[WindingEquipment],
+        list[TapWindingEquipment | WindingEquipment],
         Field(..., description="List of windings for this transformer."),
     ]
 
     coupling_sequences: Annotated[
         list[SequencePair],
         Field(
             ...,
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/geometry_branch_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/geometry_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/inverter_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/inverter_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/load_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,12 +51,13 @@
         raise ValueError(msg)
 
     @classmethod
     def example(cls) -> "MatrixImpedanceBranchEquipment":
         """Example for matrix impedance model."""
         return MatrixImpedanceBranchEquipment(
             name="matrix-impedance-branch-1",
-            r_matrix=ResistancePULength([[1, 2, 3] for _ in range(3)], "ohm/mi"),
-            x_matrix=ReactancePULength([[1, 2, 3] for _ in range(3)], "ohm/mi"),
-            c_matrix=CapacitancePULength([[1, 2, 3] for _ in range(3)], "farad/mi"),
+            r_matrix=ResistancePULength([[0.08820, 0.0312137, 0.0306264], [0.0312137, 0.0901946, 0.0316143 ], [0.0306264, 0.0316143, 0.0889665]], "ohm/mi"),
+            x_matrix=ReactancePULength([[0.20744, 0.0935314, 0.0760312], [0.0935314, 0.200783, 0.0855879], [0.0760312, 0.0855879, 0.204877]], "ohm/mi"),
+            c_matrix=CapacitancePULength([[2.90301, -0.679335, -0.22313], [-0.679335, 3.15896, -0.481416], [-0.22313, -0.481416, 2.8965]], "nanofarad/mi"),
+
             ampacity=PositiveCurrent(90, "ampere"),
         )
```

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/src/gdm/distribution/equipment/solar_equipment.py` & `grid_data_models-0.3.0/src/gdm/distribution/equipment/solar_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/.gitignore` & `grid_data_models-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/LICENSE.txt` & `grid_data_models-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/README.md` & `grid_data_models-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/pyproject.toml` & `grid_data_models-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.2.0/PKG-INFO` & `grid_data_models-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: grid-data-models
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/NREL-Distribution-Suites/grid-data-models#readme
 Project-URL: Issues, https://github.com/NREL-Distribution-Suites/grid-data-models/issues
 Project-URL: Source, https://github.com/NREL-Distribution-Suites/grid-data-models
 Author-email: Kapil Duwadi <Kapil.Duwadi@nrel.gov>, Aadil Latif <Aadil.Latif@nrel.gov>, Tarek Elgindy <tarek.elgindy@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: BSD License
```

