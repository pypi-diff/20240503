# Comparing `tmp/simpeg_drivers-0.1.0b3.tar.gz` & `tmp/simpeg_drivers-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpeg_drivers-0.1.0b3.tar", max compression
+gzip compressed data, was "simpeg_drivers-0.1.0b4.tar", max compression
```

## Comparing `simpeg_drivers-0.1.0b3.tar` & `simpeg_drivers-0.1.0b4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b3/LICENSE
--rw-r--r--   0        0        0     5121 2024-04-29 13:43:34.081354 simpeg_drivers-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b3/README.rst
--rw-r--r--   0        0        0     3604 2024-04-29 13:38:23.627819 simpeg_drivers-0.1.0b3/simpeg_drivers/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b3/simpeg_drivers/components/__init__.py
--rw-r--r--   0        0        0    20280 2024-04-26 14:45:23.742914 simpeg_drivers-0.1.0b3/simpeg_drivers/components/data.py
--rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/abstract_factory.py
--rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/directives_factory.py
--rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/entity_factory.py
--rw-r--r--   0        0        0     5003 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/misfit_factory.py
--rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/receiver_factory.py
--rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/simpeg_factory.py
--rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/simulation_factory.py
--rw-r--r--   0        0        0     6142 2024-04-26 14:45:23.748321 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/source_factory.py
--rw-r--r--   0        0        0    17787 2024-04-29 01:48:58.170502 simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/survey_factory.py
--rw-r--r--   0        0        0     6476 2024-04-26 14:45:23.750330 simpeg_drivers-0.1.0b3/simpeg_drivers/components/locations.py
--rw-r--r--   0        0        0     4799 2024-04-26 14:45:23.751485 simpeg_drivers-0.1.0b3/simpeg_drivers/components/meshes.py
--rw-r--r--   0        0        0    16897 2024-04-26 14:45:23.751584 simpeg_drivers-0.1.0b3/simpeg_drivers/components/models.py
--rw-r--r--   0        0        0     6135 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b3/simpeg_drivers/components/topography.py
--rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b3/simpeg_drivers/components/utils.py
--rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b3/simpeg_drivers/components/windows.py
--rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b3/simpeg_drivers/constants.py
--rw-r--r--   0        0        0    18654 2024-04-26 14:45:23.754889 simpeg_drivers-0.1.0b3/simpeg_drivers/driver.py
--rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/__init__.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/__init__.py
--rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
--rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
--rw-r--r--   0        0        0      911 2024-04-26 14:45:23.761252 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
--rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
--rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
--rw-r--r--   0        0        0     6721 2024-04-29 01:48:52.896367 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/driver.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/__init__.py
--rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
--rw-r--r--   0        0        0     3529 2024-04-26 14:45:23.768920 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
--rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
--rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
--rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/__init__.py
--rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/constants.py
--rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/driver.py
--rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/params.py
--rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/constants.py
--rw-r--r--   0        0        0     1300 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/driver.py
--rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/params.py
--rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/constants.py
--rw-r--r--   0        0        0     8448 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/driver.py
--rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/__init__.py
--rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/constants.py
--rw-r--r--   0        0        0     9514 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/driver.py
--rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/params.py
--rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/constants.py
--rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/driver.py
--rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/params.py
--rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b3/simpeg_drivers/joint/params.py
--rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b3/simpeg_drivers/line_sweep/driver.py
--rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/__init__.py
--rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
--rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/constants.py
--rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/driver.py
--rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/params.py
--rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/__init__.py
--rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/constants.py
--rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/driver.py
--rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/params.py
--rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b3/simpeg_drivers/params.py
--rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/__init__.py
--rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/constants.py
--rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/driver.py
--rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
--rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
--rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
--rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
--rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/constants.py
--rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/driver.py
--rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b3/simpeg_drivers/utils/__init__.py
--rw-r--r--   0        0        0     6760 2024-04-29 01:49:04.877716 simpeg_drivers-0.1.0b3/simpeg_drivers/utils/surveys.py
--rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b3/simpeg_drivers/utils/testing.py
--rw-r--r--   0        0        0    27897 2024-04-29 01:49:00.210738 simpeg_drivers-0.1.0b3/simpeg_drivers/utils/utils.py
--rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/__init__.py
--rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/colortable.csv
--rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/inversion_demo.geoh5
--rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/time_channels.txt
--rw-r--r--   0        0        0     6004 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
--rw-r--r--   0        0        0     4504 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
--rw-r--r--   0        0        0     6052 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14041 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
--rw-r--r--   0        0        0    13494 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
--rw-r--r--   0        0        0    14265 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0     3788 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/fem_forward.ui.json
--rw-r--r--   0        0        0    13429 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/fem_inversion.ui.json
--rw-r--r--   0        0        0     6267 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/gravity_forward.ui.json
--rw-r--r--   0        0        0    20665 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
--rw-r--r--   0        0        0     6083 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
--rw-r--r--   0        0        0     4915 2024-04-26 14:45:23.733154 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
--rw-r--r--   0        0        0     6370 2024-04-26 14:45:23.733921 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14301 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
--rw-r--r--   0        0        0    13912 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
--rw-r--r--   0        0        0    14596 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0    12638 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
--rw-r--r--   0        0        0    12715 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
--rw-r--r--   0        0        0     7075 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
--rw-r--r--   0        0        0    21473 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
--rw-r--r--   0        0        0     7896 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
--rw-r--r--   0        0        0    23135 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
--rw-r--r--   0        0        0     5966 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
--rw-r--r--   0        0        0    19475 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
--rw-r--r--   0        0        0     4262 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tdem_forward.ui.json
--rw-r--r--   0        0        0    14381 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
--rw-r--r--   0        0        0     5343 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tipper_forward.ui.json
--rw-r--r--   0        0        0    16280 2024-04-26 14:45:23.740599 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
--rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b3/simpeg_drivers-assets/waveform.txt
--rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b3/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b4/LICENSE
+-rw-r--r--   0        0        0     5304 2024-05-03 20:13:53.242114 simpeg_drivers-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b4/README.rst
+-rw-r--r--   0        0        0     3604 2024-05-03 19:13:21.827160 simpeg_drivers-0.1.0b4/simpeg_drivers/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b4/simpeg_drivers/components/__init__.py
+-rw-r--r--   0        0        0    20469 2024-05-03 20:13:32.764456 simpeg_drivers-0.1.0b4/simpeg_drivers/components/data.py
+-rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/abstract_factory.py
+-rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/directives_factory.py
+-rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/entity_factory.py
+-rw-r--r--   0        0        0     5003 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/misfit_factory.py
+-rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/receiver_factory.py
+-rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simpeg_factory.py
+-rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simulation_factory.py
+-rw-r--r--   0        0        0     6194 2024-05-03 18:35:52.953133 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/source_factory.py
+-rw-r--r--   0        0        0    17797 2024-05-03 18:35:52.953133 simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/survey_factory.py
+-rw-r--r--   0        0        0     6492 2024-05-03 18:35:52.954132 simpeg_drivers-0.1.0b4/simpeg_drivers/components/locations.py
+-rw-r--r--   0        0        0     4797 2024-05-03 20:13:32.766267 simpeg_drivers-0.1.0b4/simpeg_drivers/components/meshes.py
+-rw-r--r--   0        0        0    16890 2024-05-03 18:36:25.041051 simpeg_drivers-0.1.0b4/simpeg_drivers/components/models.py
+-rw-r--r--   0        0        0     6144 2024-05-03 18:35:52.955183 simpeg_drivers-0.1.0b4/simpeg_drivers/components/topography.py
+-rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b4/simpeg_drivers/components/utils.py
+-rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b4/simpeg_drivers/components/windows.py
+-rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b4/simpeg_drivers/constants.py
+-rw-r--r--   0        0        0    18418 2024-05-03 19:13:59.671778 simpeg_drivers-0.1.0b4/simpeg_drivers/driver.py
+-rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/__init__.py
+-rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
+-rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
+-rw-r--r--   0        0        0      948 2024-05-03 20:13:32.768270 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
+-rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
+-rw-r--r--   0        0        0     6677 2024-05-03 18:35:52.656394 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/driver.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/__init__.py
+-rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
+-rw-r--r--   0        0        0     3529 2024-04-26 14:45:23.768920 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
+-rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
+-rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/__init__.py
+-rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/constants.py
+-rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/driver.py
+-rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/params.py
+-rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/constants.py
+-rw-r--r--   0        0        0     1300 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/driver.py
+-rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/params.py
+-rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/constants.py
+-rw-r--r--   0        0        0     8452 2024-05-03 19:13:21.834695 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/driver.py
+-rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/__init__.py
+-rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/constants.py
+-rw-r--r--   0        0        0     9514 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/driver.py
+-rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/params.py
+-rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/constants.py
+-rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/driver.py
+-rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/params.py
+-rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b4/simpeg_drivers/joint/params.py
+-rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b4/simpeg_drivers/line_sweep/driver.py
+-rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
+-rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/constants.py
+-rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/driver.py
+-rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/params.py
+-rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/__init__.py
+-rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/constants.py
+-rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/driver.py
+-rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/params.py
+-rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b4/simpeg_drivers/params.py
+-rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/constants.py
+-rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/driver.py
+-rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
+-rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
+-rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
+-rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
+-rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/constants.py
+-rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/driver.py
+-rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/__init__.py
+-rw-r--r--   0        0        0     6694 2024-05-03 18:35:52.901412 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/surveys.py
+-rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/testing.py
+-rw-r--r--   0        0        0    27865 2024-05-03 19:15:10.720720 simpeg_drivers-0.1.0b4/simpeg_drivers/utils/utils.py
+-rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/colortable.csv
+-rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/inversion_demo.geoh5
+-rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/time_channels.txt
+-rw-r--r--   0        0        0     6006 2024-05-03 18:35:52.883963 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
+-rw-r--r--   0        0        0     4506 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
+-rw-r--r--   0        0        0     6054 2024-05-03 18:35:52.885035 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14043 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13496 2024-05-03 18:35:52.886092 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14267 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0     3790 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_forward.ui.json
+-rw-r--r--   0        0        0    13431 2024-05-03 18:35:52.887215 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_inversion.ui.json
+-rw-r--r--   0        0        0     6269 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_forward.ui.json
+-rw-r--r--   0        0        0    20667 2024-05-03 18:35:52.888305 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
+-rw-r--r--   0        0        0     6085 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
+-rw-r--r--   0        0        0     4917 2024-05-03 18:35:52.889361 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
+-rw-r--r--   0        0        0     6372 2024-05-03 18:35:52.890482 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14303 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13914 2024-05-03 18:35:52.891560 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14598 2024-05-03 18:35:52.892614 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0    12640 2024-05-03 18:35:52.892614 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
+-rw-r--r--   0        0        0    12717 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
+-rw-r--r--   0        0        0     7077 2024-05-03 18:35:52.893713 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
+-rw-r--r--   0        0        0    21475 2024-05-03 18:35:52.894827 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
+-rw-r--r--   0        0        0     7898 2024-05-03 18:35:52.894827 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
+-rw-r--r--   0        0        0    23137 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
+-rw-r--r--   0        0        0     5968 2024-05-03 18:35:52.895919 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
+-rw-r--r--   0        0        0    19477 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
+-rw-r--r--   0        0        0     4264 2024-05-03 18:35:52.897020 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_forward.ui.json
+-rw-r--r--   0        0        0    14383 2024-05-03 18:35:52.898158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
+-rw-r--r--   0        0        0     5345 2024-05-03 18:35:52.898158 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_forward.ui.json
+-rw-r--r--   0        0        0    16282 2024-05-03 18:35:52.899266 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
+-rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b4/simpeg_drivers-assets/waveform.txt
+-rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b4/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b4/PKG-INFO
```

### Comparing `simpeg_drivers-0.1.0b3/LICENSE` & `simpeg_drivers-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/pyproject.toml` & `simpeg_drivers-0.1.0b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simpeg-drivers"
-version = "0.1.0-beta.3"
+version = "0.1.0-beta.4"
 description = "Application to run SimPEG inversions with geoh5 files from Geoscience Analyst."
 license = "MIT"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = [
     "Benjamin Kary <benjamink@mirageoscience.com>",
     "Dominique Fournier <dominiquef@mirageoscience.com>",
 ]
@@ -24,19 +24,20 @@
     "README.rst",
     "THIRD_PARTY_SOFTWARE.rst",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10, <3.11"
 
-dask = {version = "2022.10.*", extras = ["distributed"]}
-discretize = "~0.10.0"
+dask = {version = "2022.10.*", extras = ["distributed"]}  # also in simpeg[dask]
+discretize = "~0.10.0"  # also in simpeg, octree-creation-app
 distributed = "2022.10.*"  # because conda-lock doesn't take dask extras into account
 numpy = "~1.23.5" # also in geoh5py, simpeg
 scipy = "~1.10.1"
+zarr = "~2.14.2"  # also in simpeg[dask]
 
 ## Pip dependencies from Git repositories
 #----------------------------------------
 geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}
 #geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 #geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
@@ -44,37 +45,38 @@
 #octree-creation-app = {url = "https://github.com/MiraGeoscience/octree-creation-app/archive/refs/heads/release/0.1.0.zip#sha256="}
 #octree-creation-app = {url = "http://localhost:8888/octree-creation-app.tar.gz#sha256="}
 
 geoapps-utils = {version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
 #geoapps-utils = {url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256="}
 #geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
-mira-simpeg = {version = ">=0.19.0.8a3,<0.19.0.8.post999", source = "pypi", allow-prereleases = true}
+mira-simpeg = {version = ">=0.19.0.8rc1,<0.19.0.8.post999", source = "pypi", allow-prereleases = true}
 #mira-simpeg = {url = "https://github.com/MiraGeoscience/simpeg/archive/refs/heads/release/0.19.0.8.zip#sha256="}
 #mira-simpeg = {url = "http://localhost:8888/mira-simpeg.tar.gz#sha256="}
 
 param-sweeps = {version = "~0.1.7rc1", source = "pypi", allow-prereleases = true}
 #param-sweeps = {url = "https://github.com/MiraGeoscience/param-sweeps/archive/refs/heads/release/0.1.7.zip#sha256="}
 #param-sweeps = {url = "http://localhost:8888/param-sweeps.tar.gz#sha256="}
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
 #---------------------------------------------------------------------------------
 Pillow = "~10.1.0"  # from geoh5py
+fsspec = "2022.*"  # from simpeg[dask]
 geoana = "~0.4.0"  # from simpeg
 h5py = "^3.2.1"  # from geoh5py
 mkl = "2022.1.*"  # from simpeg
 pandas = "~2.2.1"  # from SimPEG, also used by targeting-workflow, petro-lingo
 pydantic = "~2.5.2"  # from geoapps-utils
 pydiso = "~0.0.3"  # from simpeg
 pymatsolver = "~0.2.0"  # from simpeg
 scikit-learn = "~1.4.0"  # from SimPEG, also used by geo-unsup-mapper, petro-lingo
 tqdm = "^4.66.1"  # from simpeg
-zarr = "~2.14.2"  # from simpeg using Dask
 
 # force some versions to resolve incompatible resolution between PyPI and Conda
+#------------------------------------------------------------------------------
 tzdata = "2023.4"  # through pandas from SimPEG
 
 ## about pip dependencies
 # to be specified to work with conda-lock
 # - from PyPI: my_package = { version = "1.2.3", source = "pypi" }
 # - from URL:
 #   - for a tags:   my_package = { url = "https://github.com/ORGANISATION/REPO/archive/refs/tags/VERSION_TAG.zip#sha256=" }
```

### Comparing `simpeg_drivers-0.1.0b3/README.rst` & `simpeg_drivers-0.1.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 # pylint: disable=unused-import
 # flake8: noqa
 
 from __future__ import annotations
 
-__version__ = "0.1.0-beta.3"
+__version__ = "0.1.0-beta.4"
 
 from pathlib import Path
 
 from SimPEG import dask
 
 from simpeg_drivers.constants import default_ui_json
 from simpeg_drivers.params import InversionBaseParams
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/data.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from geoh5py.workspace import Workspace
     from simpeg_drivers.params import InversionBaseParams
 
 from copy import deepcopy
+from re import findall
 
 import numpy as np
 from discretize import TreeMesh
 from scipy.spatial import cKDTree
 from SimPEG import maps
 from SimPEG.electromagnetics.static.utils.static_utils import geometric_factor
 
@@ -167,22 +168,25 @@
                 rad[:, ii] + 1e-8
             )
 
         distance_interp /= ((rad + 1e-8) ** -1.0).sum(axis=1)
 
         return np.c_[distance_interp, locations[:, 2:]]
 
-    def filter(self, a):
+    def filter(self, obj: dict[str, np.ndarray] | np.ndarray, mask=None):
         """Remove vertices based on mask property."""
+        if mask is None:
+            mask = self.mask
+
         if self.indices is None:
-            self.indices = np.where(self.mask)[0]
+            self.indices = np.where(mask)[0]
 
-        a = super().filter(a, mask=self.indices)
+        obj = super().filter(obj, mask=self.indices)
 
-        return a
+        return obj
 
     def get_data(self) -> tuple[list, dict, dict]:
         """
         Get all data and uncertainty components and possibly set infinite uncertainties.
 
         :return: components: list of data components sorted in the
             order of self.observed.keys().
@@ -486,17 +490,23 @@
         """
         Stored data types
         """
         return self._observed_data_types
 
     @staticmethod
     def check_tensor(channels):
-        tensor_components = ["xx", "xy", "xz", "yx", "zx", "yy", "zz", "zy", "yz"]
-        has_tensor = lambda c: any(k in c for k in tensor_components)
-        return any(has_tensor(c) for c in channels)
+        tensor_components = "|".join(
+            ["xx", "xy", "xz", "yx", "zx", "yy", "zz", "zy", "yz"]
+        )
+
+        for channel in channels:
+            if any(findall(tensor_components, channel)):
+                return True
+
+        return False
 
     def update_params(self, data_dict, uncert_dict):
         """
         Update pointers to newly created object and data.
         """
 
         components = self.params.components()
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/abstract_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/directives_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/directives_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/entity_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/entity_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/misfit_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/misfit_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/receiver_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/receiver_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/simpeg_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simpeg_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/simulation_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/simulation_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/source_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/source_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             kwargs["location"] = locations
         if self.factory_type in ["tdem"]:
             kwargs["location"] = locations
             kwargs["waveform"] = waveform
 
         return kwargs
 
-    def build(self, receivers=None, locations=None, frequency=None, waveform=None):
+    def build(  # pylint: disable=arguments-differ
+        self, receivers=None, locations=None, frequency=None, waveform=None
+    ):
         return super().build(
             receivers=receivers,
             locations=locations,
             frequency=frequency,
             waveform=waveform,
         )
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/factories/survey_factory.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/factories/survey_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             return self._fem_arguments(data=data, mesh=mesh, channel=channel)
         else:
             receivers = ReceiversFactory(self.params).build(
                 locations=data.locations,
                 data=data.observed,
                 local_index=self.local_index,
             )
-            sources = SourcesFactory(self.params).build(receivers)
+            sources = SourcesFactory(self.params).build(receivers=receivers)
             return [sources]
 
     def assemble_keyword_arguments(self, **_):
         """Implementation of abstract method from SimPEGFactory."""
         return {}
 
     def build(
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/locations.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,38 +138,38 @@
         is_none = []
         for v in a.values():
             if isinstance(v, dict):
                 v = None if self._none_dict(v) else 1
             is_none.append(v is None)
         return all(is_none)
 
-    def filter(self, a: dict[str, np.ndarray] | np.ndarray, mask=None):
+    def filter(self, obj: dict[str, np.ndarray] | np.ndarray, mask=None):
         """
         Apply accumulated self.mask to array, or dict of arrays.
 
         If argument a is a dictionary filter will be applied to all key/values.
 
-        :param a: Object containing data to filter.
+        :param obj: Object containing data to filter.
 
         :return: Filtered data.
 
         """
 
         mask = self.mask if mask is None else mask
 
-        if isinstance(a, dict):
-            if self._none_dict(a):
-                return a
+        if isinstance(obj, dict):
+            if self._none_dict(obj):
+                return obj
             else:
-                return self._filter(a, mask)
+                return self._filter(obj, mask)
         else:
-            if a is None:
+            if obj is None:
                 return None
             else:
-                return a[mask]
+                return obj[mask]
 
     def set_z_from_topo(self, locs: np.ndarray):
         """interpolate locations z data from topography."""
 
         if locs is None:
             return None
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/meshes.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/meshes.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,27 @@
 
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
+from discretize import TensorMesh, TreeMesh
 from geoh5py.objects import DrapeModel, Octree
 from octree_creation_app.params import OctreeParams
 from octree_creation_app.utils import octree_2_treemesh
 
 from simpeg_drivers.utils.utils import drape_2_tensor
 
 if TYPE_CHECKING:
     from geoh5py.workspace import Workspace
 
     from simpeg_drivers.components.data import InversionData
     from simpeg_drivers.components.topography import InversionTopography
 
-from discretize import TensorMesh, TreeMesh
-
 
 class InversionMesh:
     """
     Retrieve octree mesh data from workspace and convert to Treemesh.
 
     Attributes
     ----------
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/models.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
         return mstart
 
     def _model_method_wrapper(self, method, name=None, **kwargs):
         """wraps individual model's specific method and applies in loop over model types."""
         returned_items = {}
         for mtype in self.model_types:
-            model = self.__getattribute__(f"_{mtype}")
+            model = getattr(self, f"_{mtype}")
             if model.model is not None:
                 f = getattr(model, method)
                 returned_items[mtype] = f(**kwargs)
 
         if name is not None:
             return returned_items[name]
 
@@ -481,10 +481,10 @@
     @property
     def model_type(self):
         return self._model_type
 
     @model_type.setter
     def model_type(self, v):
         if v not in self.model_types:
-            msg = f"Invalid 'model_type'. Must be one of {*self.model_types,}."
+            msg = f"Invalid 'model_type'. Must be one of {*self.model_types, }."
             raise ValueError(msg)
         self._model_type = v
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/topography.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/topography.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,26 +107,26 @@
                 warnings.warn(
                     "Active cell adjustment has created a patch of active cells in the air, "
                     "likely due to a faulty survey location."
                 )
 
         return active_cells
 
-    def get_locations(self, obj: Entity) -> np.ndarray:
+    def get_locations(self, entity: Entity) -> np.ndarray:
         """
         Returns locations of data object centroids or vertices.
 
-        :param obj: geoh5py object containing centroid or
+        :param entity: geoh5py object containing centroid or
             vertex location data
 
         :return: Array shape(*, 3) of x, y, z location data
 
         """
 
-        locs = super().get_locations(obj)
+        locs = super().get_locations(entity)
 
         if self.params.topography is not None:
             if isinstance(self.params.topography, Entity):
                 elev = self.params.topography.values
             elif isinstance(self.params.topography, (int, float)):
                 elev = np.ones_like(locs[:, 2]) * self.params.topography
             else:
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/utils.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/utils.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/components/windows.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/components/windows.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from simpeg_drivers import InversionBaseParams
-
 import multiprocessing
 import sys
 from datetime import datetime, timedelta
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from time import time
 
@@ -348,26 +343,20 @@
             data_count = np.sum(
                 [len(d.inversion_data.survey.std) for d in getattr(self, "drivers")]
             )
         else:
             data_count = len(self.inversion_data.survey.std)
 
         print(
-            "Target Misfit: {:.2e} ({} data with chifact = {}) / 2".format(
-                0.5 * self.params.chi_factor * data_count,
-                data_count,
-                self.params.chi_factor,
-            )
+            f"Target Misfit: {0.5 * self.params.chi_factor * data_count:.2e} ({data_count} data "
+            f"with chifact = {self.params.chi_factor}) / 2"
         )
         print(
-            "IRLS Start Misfit: {:.2e} ({} data with chifact = {}) / 2".format(
-                0.5 * chi_start * data_count,
-                data_count,
-                chi_start,
-            )
+            f"IRLS Start Misfit: {0.5 * chi_start * data_count:.2e} ({data_count} data "
+            f"with chifact = {chi_start}) / 2"
         )
 
     @property
     def mapping(self) -> list[maps.IdentityMap] | None:
         """Model mapping for the inversion."""
         if self._mapping is None:
             self.mapping = maps.IdentityMap(nP=self.n_values)
@@ -444,28 +433,28 @@
         return tiles
 
     def configure_dask(self):
         """Sets Dask config settings."""
 
         if self.params.parallelized:
             if self.params.n_cpu is None:
-                self.params.n_cpu = int(multiprocessing.cpu_count() / 2)
+                self.params.n_cpu = int(multiprocessing.cpu_count())
 
             dconf.set({"array.chunk-size": str(self.params.max_chunk_size) + "MiB"})
             dconf.set(scheduler="threads", pool=ThreadPool(self.params.n_cpu))
 
     @classmethod
     def start(cls, filepath: str | Path, driver_class=None):
         _ = driver_class
 
         ifile = InputFile.read_ui_json(filepath)
         inversion_type = ifile.data["inversion_type"]
         if inversion_type not in DRIVER_MAP:
             msg = f"Inversion type {inversion_type} is not supported."
-            msg += f" Valid inversions are: {*list(DRIVER_MAP),}."
+            msg += f" Valid inversions are: {*list(DRIVER_MAP), }."
             raise NotImplementedError(msg)
 
         mod_name, class_name = DRIVER_MAP.get(inversion_type)
         module = __import__(mod_name, fromlist=[class_name])
         inversion_driver = getattr(module, class_name)
         driver = BaseDriver.start(filepath, driver_class=inversion_driver)
         return driver
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/three_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 #  may be used, copied, transmitted, and stored only in accordance with
 #  the terms of such license and with the inclusion of the above copyright
 #  notice.  This software and information or any other copies thereof may
 #  not be provided or otherwise made available to any other person.
 #
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
-
 from .params import DirectCurrent2DParams
+
+__all__ = ["DirectCurrent2DParams"]
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/direct_current/two_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/direct_current/two_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 class BasePseudo3DDriver(LineSweepDriver):
     _params_class: type(BaseParams)
     _params_2d_class: type(BaseParams)
     _validations: dict
     _model_list: list[str] = []
 
-    def __init__(self, params):  # pylint: disable=useless_super_delegation
+    def __init__(self, params):
         super().__init__(params)
         if params.files_only:
             sys.exit("Files written")
 
     def transfer_models(self, mesh: DrapeModel) -> dict[str, uuid.UUID | float]:
         """
         Transfer models from the input parameters to the output drape mesh.
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electricals/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electricals/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/frequency_domain/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/frequency_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/electromagnetics/time_domain/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/electromagnetics/time_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def drivers(self) -> list[InversionDriver] | None:
         """List of inversion drivers."""
         if self._drivers is None:
             drivers = []
             physical_property = []
             # Create sub-drivers
             for group in self.params.groups:
-                group.options  # Triggers something... otherwise ui_json is empty
+                _ = group.options  # Triggers something... otherwise ui_json is empty
                 group = group.copy(parent=self.params.out_group)
 
                 ui_json = group.options
                 ui_json["geoh5"] = self.workspace
 
                 ifile = InputFile(ui_json=ui_json)
                 mod_name, class_name = DRIVER_MAP.get(ui_json["inversion_type"])
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_cross_gradient/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_cross_gradient/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/joint_surveys/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/joint_surveys/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/joint/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/joint/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/line_sweep/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/line_sweep/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/magnetotellurics/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/magnetotellurics/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/natural_sources/tipper/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/natural_sources/tipper/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/gravity/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/gravity/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_scalar/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_scalar/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/constants.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/driver.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/potential_fields/magnetic_vector/params.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/potential_fields/magnetic_vector/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/utils/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/utils/surveys.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/surveys.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 from __future__ import annotations
 
 from collections.abc import Callable
 
 import numpy as np
-from discretize import TensorMesh, TreeMesh
+from discretize import TreeMesh
 from geoapps_utils.numerical import traveling_salesman
 from geoh5py import Workspace
-from geoh5py.data import FloatData
-from geoh5py.objects import CurrentElectrode, PotentialElectrode
+from geoh5py.objects import PotentialElectrode
 from scipy.spatial import cKDTree
 from SimPEG.survey import BaseSurvey
 
 
 def compute_alongline_distance(points: np.ndarray, ordered: bool = True):
     """
     Convert from cartesian (x, y, values) points to (distance, values) locations.
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/utils/testing.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/testing.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers/utils/utils.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     values = values[ind_nan]
 
     if method == "perimeter":
         hull = ConvexHull(loc_xy[:, :2])
         # Extract only those points that make the ConvexHull
         loc_xy = loc_xy[hull.vertices, :2]
         values = values[hull.vertices]
-    elif not method == "all":
+    elif method != "all":
         raise ValueError(
             "'method' must be either 'all', or 'perimeter'. " f"Value {method} provided"
         )
 
     # Compute center of mass
     center_x = np.sum(loc_xy[:, 0] * np.abs(values)) / np.sum(np.abs(values))
     center_y = np.sum(loc_xy[:, 1] * np.abs(values)) / np.sum(np.abs(values))
@@ -265,16 +265,14 @@
                         model.centroids
                     )
                 )
                 octree_model[lookup_inds] = datum[0].values
 
         if method == "nearest":
             octree_model = np.hstack(octree_model)[lookup_inds]
-        else:
-            octree_model = octree_model
 
         if np.issubdtype(octree_model.dtype, np.integer):
             octree_model[~active] = INTEGER_NDV
         else:
             octree_model[~active] = np.nan  # apply active cells
 
         octree.add_data({label: {"values": octree_model}})
@@ -454,17 +452,19 @@
         group = workspace.get_entity(inversion_group)[0]
     except IndexError as exc:
         raise IndexError(
             f"BaseInversion group {inversion_group} could not be found in the target geoh5 {h5file}"
         ) from exc
 
     outfile = group.get_entity("SimPEG.out")[0]
-    out = [l for l in outfile.values.decode("utf-8").replace("\r", "").split("\n")][:-1]
+    out = [
+        elem for elem in outfile.values.decode("utf-8").replace("\r", "").split("\n")
+    ][:-1]
     cols = out.pop(0).split(" ")
-    out = [[string_to_numeric(k) for k in l.split(" ")] for l in out]
+    out = [[string_to_numeric(k) for k in elem.split(" ")] for elem in out]
     out = dict(zip(cols, list(map(list, zip(*out)))))
 
     return out
 
 
 def tile_locations(
     locations,
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/__init__.py` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/inversion_demo.geoh5` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/inversion_demo.geoh5`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 2D Forward",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current 2d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current 2d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -198,18 +202,14 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "gradient_type": {
         "choiceList": [
             "total",
             "components"
         ],
         "group": "Regularization",
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 3D Forward",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current 3d",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current 3d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -148,13 +152,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 2D Batch Forward",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current pseudo 3d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current pseudo 3d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -204,14 +208,10 @@
     },
     "cleanup": {
         "main": true,
         "group": "Python run preferences",
         "label": "Clean directory",
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
     "run_command_boolean": false,
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 2D Inversion",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current 2d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current 2d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -491,14 +495,10 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "potential_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 3D Inversion",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current 3d",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current 3d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -473,14 +477,10 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "potential_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Direct Current (DC) 2D Batch Inversion",
     "icon": "PotentialElectrode",
-    "inversion_type": "direct current pseudo 3d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "direct current pseudo 3d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -496,15 +500,11 @@
     },
     "cleanup": {
         "main": true,
         "group": "Python run preferences",
         "label": "Clean directory",
         "value": true
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
     "run_command_boolean": false,
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "potential_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/fem_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Frequency-domain EM (FEM) Forward",
     "icon": "surveyairborneem",
-    "inversion_type": "fem",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "fem",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -129,13 +133,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/fem_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/fem_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Frequency-domain EM (FEM) Inversion",
     "icon": "surveyairborneem",
-    "inversion_type": "fem",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "fem",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -477,13 +481,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/gravity_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Gravity Forward",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornegravity",
-    "inversion_type": "gravity",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "gravity",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -216,13 +220,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/gravity_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/gravity_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Gravity Inversion",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornegravity",
-    "inversion_type": "gravity",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "gravity",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -758,13 +762,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 2D Forward",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization 2d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization 2d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -209,13 +213,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 3D Forward",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization 3d",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization 3d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -164,13 +168,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 2D Batch Forward",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization pseudo 3d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization pseudo 3d",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -215,14 +219,10 @@
     },
     "cleanup": {
         "main": true,
         "group": "Python run preferences",
         "label": "Clean directory",
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
     "run_command_boolean": false,
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 2D Inversion",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization 2d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization 2d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -501,14 +505,10 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "chargeability_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 3D Inversion",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization 3d",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization 3d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -489,14 +493,10 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "chargeability_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Induced Polarization (IP) 2D Batch Inversion",
     "icon": "PotentialElectrode",
-    "inversion_type": "induced polarization pseudo 3d",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "induced polarization pseudo 3d",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -507,15 +511,11 @@
     },
     "cleanup": {
         "main": true,
         "group": "Python run preferences",
         "label": "Clean directory",
         "value": true
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
     "run_command_boolean": false,
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": "",
     "chargeability_channel_bool": true
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,12 +1,16 @@
 {
-    "title": "SimPEG Joint Cross Gradient Inversion",
-    "inversion_type": "joint cross gradient",
     "version": "0.1.0-alpha.1",
+    "title": "SimPEG Joint Cross Gradient Inversion",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "joint cross gradient",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -420,13 +424,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,12 +1,16 @@
 {
-    "title": "SimPEG Joint Surveys Inversion",
-    "inversion_type": "joint surveys",
     "version": "0.1.0-alpha.1",
+    "title": "SimPEG Joint Surveys Inversion",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "joint surveys",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -439,13 +443,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetic Forward",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornegravity",
-    "inversion_type": "magnetic scalar",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetic scalar",
     "forward_only": true,
     "inducing_field_strength": {
         "min": 0.0,
         "max": 100000.0,
         "precision": 2,
         "lineEdit": false,
         "main": true,
@@ -246,13 +250,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetic Inversion",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornemagnetics",
-    "inversion_type": "magnetic scalar",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetic scalar",
     "forward_only": false,
     "inducing_field_strength": {
         "min": 0.0,
         "max": 100000.0,
         "precision": 2,
         "lineEdit": false,
         "main": true,
@@ -788,13 +792,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetic Vector (MVI) Forward",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornemagnetics",
-    "inversion_type": "magnetic vector",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetic vector",
     "forward_only": true,
     "inducing_field_strength": {
         "min": 0.1,
         "max": 100000.0,
         "precision": 2,
         "lineEdit": false,
         "main": true,
@@ -278,13 +282,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,14 +1,18 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetic Vector (MVI) Inversion",
-    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
     "icon": "surveyairbornegravity",
-    "inversion_type": "magnetic vector",
+    "documentation": "https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetic vector",
     "forward_only": false,
     "inducing_field_strength": {
         "min": 0.1,
         "max": 100000.0,
         "precision": 2,
         "lineEdit": false,
         "main": true,
@@ -852,13 +856,9 @@
     "ga_group": "",
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetotellurics (MT) Forward",
     "icon": "surveymagnetotellurics",
-    "inversion_type": "magnetotellurics",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetotellurics",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -208,13 +212,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Magnetotellurics (MT) Inversion",
     "icon": "surveymagnetotellurics",
-    "inversion_type": "magnetotellurics",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "magnetotellurics",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -700,13 +704,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tdem_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Time-domain EM (TEM) Forward",
     "icon": "surveyairborneem",
-    "inversion_type": "tdem",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "tdem",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -148,13 +152,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tdem_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tdem_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Time-domain EM (TEM) Inversion",
     "icon": "surveyairborneem",
-    "inversion_type": "tdem",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "tdem",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -513,13 +517,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tipper_forward.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_forward.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Tipper Forward",
     "icon": "surveyztem",
-    "inversion_type": "tipper",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "tipper",
     "forward_only": true,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -184,13 +188,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/simpeg_drivers-assets/uijson/tipper_inversion.ui.json` & `simpeg_drivers-0.1.0b4/simpeg_drivers-assets/uijson/tipper_inversion.ui.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,13 +1,17 @@
 {
     "version": "0.1.0-alpha.1",
     "title": "Tipper Inversion",
     "icon": "surveyztem",
-    "inversion_type": "tipper",
+    "conda_environment": "simpeg_drivers",
+    "run_command": "simpeg_drivers.driver",
     "geoh5": "",
+    "monitoring_directory": "",
+    "workspace_geoh5": "",
+    "inversion_type": "tipper",
     "forward_only": false,
     "topography_object": {
         "main": true,
         "group": "Topography",
         "label": "Topography",
         "meshType": [
             "{202c5db1-a56d-4004-9cad-baafd8899406}",
@@ -580,13 +584,9 @@
     },
     "generate_sweep": {
         "label": "Generate sweep file",
         "group": "Python run preferences",
         "main": true,
         "value": false
     },
-    "monitoring_directory": "",
-    "workspace_geoh5": "",
-    "run_command": "simpeg_drivers.driver",
-    "conda_environment": "simpeg_drivers",
     "distributed_workers": ""
 }
```

### Comparing `simpeg_drivers-0.1.0b3/THIRD_PARTY_SOFTWARE.rst` & `simpeg_drivers-0.1.0b4/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b3/PKG-INFO` & `simpeg_drivers-0.1.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpeg-drivers
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: Application to run SimPEG inversions with geoh5 files from Geoscience Analyst.
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
 Maintainer-email: benjamink@mirageoscience.com
@@ -12,19 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=10.1.0,<10.2.0)
 Requires-Dist: dask[distributed] (==2022.10.*)
 Requires-Dist: discretize (>=0.10.0,<0.11.0)
 Requires-Dist: distributed (==2022.10.*)
+Requires-Dist: fsspec (==2022.*)
 Requires-Dist: geoana (>=0.4.0,<0.5.0)
 Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
-Requires-Dist: mira-simpeg (>=0.19.0.8a3,<0.19.0.8.post999)
+Requires-Dist: mira-simpeg (>=0.19.0.8rc1,<0.19.0.8.post999)
 Requires-Dist: mkl (==2022.1.*)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: octree-creation-app (>=0.1.0rc2,<0.2.0)
 Requires-Dist: pandas (>=2.2.1,<2.3.0)
 Requires-Dist: param-sweeps (>=0.1.7rc1,<0.2.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: pydiso (>=0.0.3,<0.1.0)
```

