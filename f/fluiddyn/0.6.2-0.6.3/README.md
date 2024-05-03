# Comparing `tmp/fluiddyn-0.6.2.tar.gz` & `tmp/fluiddyn-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluiddyn-0.6.2.tar", last modified: Tue Apr 16 08:16:57 2024, max compression
+gzip compressed data, was "fluiddyn-0.6.3.tar", last modified: Mon Apr 22 14:36:54 2024, max compression
```

## Comparing `fluiddyn-0.6.2.tar` & `fluiddyn-0.6.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0      314 2024-01-17 16:37:56.387718 fluiddyn-0.6.2/AUTHORS.md
--rw-r--r--   0        0        0    21394 2023-07-04 19:04:38.313096 fluiddyn-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     5322 2024-01-17 16:37:56.387718 fluiddyn-0.6.2/README.rst
--rw-r--r--   0        0        0     1136 2023-07-04 19:04:38.345096 fluiddyn-0.6.2/fluiddoc/__init__.py
--rw-r--r--   0        0        0     4408 2024-01-18 13:20:32.401745 fluiddyn-0.6.2/fluiddoc/fluiddocset.py
--rw-r--r--   0        0        0     2344 2023-07-04 19:04:38.349096 fluiddyn-0.6.2/fluiddoc/fluidnbstripout.py
--rw-r--r--   0        0        0     3096 2023-07-06 09:48:56.909088 fluiddyn-0.6.2/fluiddoc/ipynb_maker.py
--rw-r--r--   0        0        0     5174 2023-07-04 19:04:38.349096 fluiddyn-0.6.2/fluiddoc/mathmacro.py
--rw-r--r--   0        0        0     1127 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/__init__.py
--rw-r--r--   0        0        0      343 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/_version.py
--rw-r--r--   0        0        0      144 2023-07-04 19:04:38.353096 fluiddyn-0.6.2/fluiddyn/calcul/__init__.py
--rw-r--r--   0        0        0    18805 2023-07-04 19:04:38.353096 fluiddyn-0.6.2/fluiddyn/calcul/easypyfft.py
--rw-r--r--   0        0        0     4223 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/setofvariables.py
--rw-r--r--   0        0        0     5250 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/signal.py
--rw-r--r--   0        0        0    24798 2024-02-18 20:17:29.053325 fluiddyn-0.6.2/fluiddyn/calcul/sphericalharmo.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.357096 fluiddyn-0.6.2/fluiddyn/calcul/test/__init__.py
--rw-r--r--   0        0        0     5783 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/calcul/test/test_easypyfft.py
--rw-r--r--   0        0        0      330 2023-07-04 19:04:38.357096 fluiddyn-0.6.2/fluiddyn/calcul/test/test_setofvariables.py
--rw-r--r--   0        0        0      660 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/calcul/test/test_signal.py
--rw-r--r--   0        0        0      895 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/calcul/test/test_sphericalharmo.py
--rw-r--r--   0        0        0     2887 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/clusters/__init__.py
--rw-r--r--   0        0        0      875 2023-07-04 19:04:38.361096 fluiddyn-0.6.2/fluiddyn/clusters/azzurra.py
--rw-r--r--   0        0        0      995 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/ciment.py
--rw-r--r--   0        0        0     1274 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/clusters/cines.py
--rw-r--r--   0        0        0      834 2023-07-04 19:04:38.365096 fluiddyn-0.6.2/fluiddyn/clusters/idris.py
--rw-r--r--   0        0        0     1045 2024-03-26 14:06:06.131975 fluiddyn-0.6.2/fluiddyn/clusters/legi.py
--rw-r--r--   0        0        0      716 2023-07-04 19:04:38.365096 fluiddyn-0.6.2/fluiddyn/clusters/licallo.py
--rw-r--r--   0        0        0     8102 2023-07-06 09:48:56.913088 fluiddyn-0.6.2/fluiddyn/clusters/local.py
--rw-r--r--   0        0        0     9408 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/oar.py
--rw-r--r--   0        0        0     8351 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/pbs.py
--rw-r--r--   0        0        0    16542 2023-07-06 09:48:56.917088 fluiddyn-0.6.2/fluiddyn/clusters/slurm.py
--rw-r--r--   0        0        0     4178 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/snic.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.369096 fluiddyn-0.6.2/fluiddyn/clusters/test/__init__.py
--rw-r--r--   0        0        0     1026 2024-02-18 20:17:29.057325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_local.py
--rw-r--r--   0        0        0     2865 2024-03-26 14:06:06.131975 fluiddyn-0.6.2/fluiddyn/clusters/test/test_oar.py
--rw-r--r--   0        0        0     2797 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_pbs.py
--rw-r--r--   0        0        0     3479 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/clusters/test/test_slurm_snic.py
--rw-r--r--   0        0        0     2115 2024-03-26 14:06:06.135975 fluiddyn-0.6.2/fluiddyn/io/__init__.py
--rw-r--r--   0        0        0     5138 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/io/binary.py
--rw-r--r--   0        0        0     3822 2024-02-18 20:17:29.061325 fluiddyn-0.6.2/fluiddyn/io/dantec.py
--rw-r--r--   0        0        0     3779 2024-01-11 10:47:04.851740 fluiddyn-0.6.2/fluiddyn/io/davis.py
--rw-r--r--   0        0        0    19554 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/digiflow.py
--rw-r--r--   0        0        0     4052 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/dump.py
--rw-r--r--   0        0        0     4758 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/hdf5.py
--rw-r--r--   0        0        0     5683 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/image.py
--rw-r--r--   0        0        0     1378 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/in_py.py
--rw-r--r--   0        0        0    13149 2023-07-06 09:48:56.921088 fluiddyn-0.6.2/fluiddyn/io/multitiff.py
--rw-r--r--   0        0        0     1762 2023-07-04 19:04:38.381096 fluiddyn-0.6.2/fluiddyn/io/mycsv.py
--rw-r--r--   0        0        0    12165 2024-02-18 20:17:29.065325 fluiddyn-0.6.2/fluiddyn/io/ns3d.py
--rw-r--r--   0        0        0     2539 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/query.py
--rw-r--r--   0        0        0     2809 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/rdvision.py
--rw-r--r--   0        0        0     1142 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/io/redirect_stdout.py
--rw-r--r--   0        0        0      620 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/tee.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/test/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-04 19:04:38.385096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/PV.t=0000.000
--rw-r--r--   0        0        0      284 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
--rw-r--r--   0        0        0      284 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
--rw-r--r--   0        0        0      429 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.seq
--rw-r--r--   0        0        0       48 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
--rw-r--r--   0        0        0     1267 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.xml
--rw-r--r--   0        0        0     1137 2023-07-04 19:04:38.389096 fluiddyn-0.6.2/fluiddyn/io/test/test_binary.py
--rw-r--r--   0        0        0      525 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_dantec.py
--rw-r--r--   0        0        0      660 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_digiflow.py
--rw-r--r--   0        0        0     1456 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_dump.py
--rw-r--r--   0        0        0     2123 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_hdf5.py
--rw-r--r--   0        0        0     2909 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_image.py
--rw-r--r--   0        0        0     1224 2023-07-04 19:04:38.393096 fluiddyn-0.6.2/fluiddyn/io/test/test_in_py.py
--rw-r--r--   0        0        0     2411 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_multitiff.py
--rw-r--r--   0        0        0      746 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_mycsv.py
--rw-r--r--   0        0        0     1855 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_ns3d.py
--rw-r--r--   0        0        0     1232 2023-07-06 09:48:56.921088 fluiddyn-0.6.2/fluiddyn/io/test/test_query.py
--rw-r--r--   0        0        0     1027 2023-07-04 19:04:38.397096 fluiddyn-0.6.2/fluiddyn/io/test/test_rdvision.py
--rw-r--r--   0        0        0      739 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/io/test/test_tee.py
--rw-r--r--   0        0        0     1095 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/io/test/test_txt.py
--rw-r--r--   0        0        0     3342 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/io/txt.py
--rw-r--r--   0        0        0      533 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/output/__init__.py
--rw-r--r--   0        0        0     6098 2023-07-04 19:04:38.401096 fluiddyn-0.6.2/fluiddyn/output/colorchart.py
--rw-r--r--   0        0        0     5323 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/output/figs.py
--rw-r--r--   0        0        0     1177 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/rcparams.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/test/__init__.py
--rw-r--r--   0        0        0      307 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/test/test_colorchart.py
--rw-r--r--   0        0        0     1052 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/output/test/test_figs.py
--rw-r--r--   0        0        0      721 2023-07-04 19:04:38.405096 fluiddyn-0.6.2/fluiddyn/output/util.py
--rw-r--r--   0        0        0     1135 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/util/__init__.py
--rw-r--r--   0        0        0      133 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/compat.py
--rw-r--r--   0        0        0      304 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/constants.py
--rw-r--r--   0        0        0     1068 2024-02-18 20:17:29.069325 fluiddyn-0.6.2/fluiddyn/util/daemons.py
--rw-r--r--   0        0        0    15219 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/info.py
--rw-r--r--   0        0        0     4282 2023-07-04 19:04:38.409096 fluiddyn-0.6.2/fluiddyn/util/logger.py
--rw-r--r--   0        0        0     3513 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/mail.py
--rw-r--r--   0        0        0     1971 2023-07-06 09:48:56.925088 fluiddyn-0.6.2/fluiddyn/util/matlab2py/__init__.py
--rw-r--r--   0        0        0     5860 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/matlab2py/cleanmat.py
--rw-r--r--   0        0        0     3238 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/matlab2py/mat2wrongpy.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/__init__.py
--rw-r--r--   0        0        0      810 2023-07-04 19:04:38.413096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/courant.m
--rw-r--r--   0        0        0      519 2023-07-04 19:04:38.417096 fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/test_matlab2py.py
--rw-r--r--   0        0        0     3780 2023-07-04 19:04:38.417096 fluiddyn-0.6.2/fluiddyn/util/mpi.py
--rw-r--r--   0        0        0    23542 2024-02-18 20:17:29.073325 fluiddyn-0.6.2/fluiddyn/util/numpy_distutils_cpuinfo.py
--rw-r--r--   0        0        0      964 2024-02-18 20:17:29.077325 fluiddyn-0.6.2/fluiddyn/util/opencv.py
--rw-r--r--   0        0        0    23221 2024-01-18 13:20:32.405745 fluiddyn-0.6.2/fluiddyn/util/paramcontainer.py
--rw-r--r--   0        0        0     7281 2024-01-18 13:20:32.405745 fluiddyn-0.6.2/fluiddyn/util/paramcontainer_gui.py
--rw-r--r--   0        0        0    32191 2024-04-16 08:16:22.836543 fluiddyn-0.6.2/fluiddyn/util/serieofarrays.py
--rw-r--r--   0        0        0     4724 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/terminal_colors.py
--rw-r--r--   0        0        0        0 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/__init__.py
--rw-r--r--   0        0        0     1814 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/file.xml
--rw-r--r--   0        0        0      808 2023-07-04 19:04:38.421096 fluiddyn-0.6.2/fluiddyn/util/test/test_daemons.py
--rw-r--r--   0        0        0      974 2024-02-18 20:17:29.077325 fluiddyn-0.6.2/fluiddyn/util/test/test_info.py
--rw-r--r--   0        0        0      942 2024-01-18 13:20:32.409745 fluiddyn-0.6.2/fluiddyn/util/test/test_logger.py
--rw-r--r--   0        0        0     2194 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_mpi.py
--rw-r--r--   0        0        0     4725 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_paramcontainer.py
--rw-r--r--   0        0        0     7447 2024-04-16 08:16:22.840543 fluiddyn-0.6.2/fluiddyn/util/test/test_serieofarrays.py
--rw-r--r--   0        0        0      797 2023-07-04 19:04:38.425096 fluiddyn-0.6.2/fluiddyn/util/test/test_timer.py
--rw-r--r--   0        0        0     2734 2023-07-06 09:48:56.929088 fluiddyn-0.6.2/fluiddyn/util/test/test_util.py
--rw-r--r--   0        0        0     4522 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/timer.py
--rw-r--r--   0        0        0     1200 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/userconfig.py
--rw-r--r--   0        0        0     9277 2024-02-18 20:17:29.081325 fluiddyn-0.6.2/fluiddyn/util/util.py
--rw-r--r--   0        0        0     4443 2023-07-04 19:04:38.429096 fluiddyn-0.6.2/fluiddyn/util/xmltotext.py
--rw-r--r--   0        0        0     4238 2024-04-16 08:16:57.716501 fluiddyn-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 fluiddyn-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      314 2024-02-17 22:43:56.129004 fluiddyn-0.6.3/AUTHORS.md
+-rw-r--r--   0        0        0    21394 2024-02-17 22:43:56.129004 fluiddyn-0.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     5322 2024-02-17 22:43:56.133004 fluiddyn-0.6.3/README.rst
+-rw-r--r--   0        0        0     1136 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddoc/__init__.py
+-rw-r--r--   0        0        0     4408 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddoc/fluiddocset.py
+-rw-r--r--   0        0        0     2344 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddoc/fluidnbstripout.py
+-rw-r--r--   0        0        0     3096 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddoc/ipynb_maker.py
+-rw-r--r--   0        0        0     5174 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddoc/mathmacro.py
+-rw-r--r--   0        0        0     1127 2024-02-17 22:43:56.161004 fluiddyn-0.6.3/fluiddyn/__init__.py
+-rw-r--r--   0        0        0      343 2024-02-17 22:43:56.165003 fluiddyn-0.6.3/fluiddyn/_version.py
+-rw-r--r--   0        0        0      144 2024-02-17 22:43:56.165003 fluiddyn-0.6.3/fluiddyn/calcul/__init__.py
+-rw-r--r--   0        0        0    18805 2024-02-17 22:43:56.165003 fluiddyn-0.6.3/fluiddyn/calcul/easypyfft.py
+-rw-r--r--   0        0        0     4223 2024-02-17 22:43:56.165003 fluiddyn-0.6.3/fluiddyn/calcul/setofvariables.py
+-rw-r--r--   0        0        0     5250 2024-02-17 22:43:56.165003 fluiddyn-0.6.3/fluiddyn/calcul/signal.py
+-rw-r--r--   0        0        0    24798 2024-02-17 22:43:56.169003 fluiddyn-0.6.3/fluiddyn/calcul/sphericalharmo.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.169003 fluiddyn-0.6.3/fluiddyn/calcul/test/__init__.py
+-rw-r--r--   0        0        0     5783 2024-02-17 22:43:56.169003 fluiddyn-0.6.3/fluiddyn/calcul/test/test_easypyfft.py
+-rw-r--r--   0        0        0      330 2024-02-17 22:43:56.169003 fluiddyn-0.6.3/fluiddyn/calcul/test/test_setofvariables.py
+-rw-r--r--   0        0        0      660 2024-02-17 22:43:56.169003 fluiddyn-0.6.3/fluiddyn/calcul/test/test_signal.py
+-rw-r--r--   0        0        0      895 2024-02-17 22:43:56.173003 fluiddyn-0.6.3/fluiddyn/calcul/test/test_sphericalharmo.py
+-rw-r--r--   0        0        0     4818 2024-04-22 14:36:43.451957 fluiddyn-0.6.3/fluiddyn/clusters/__init__.py
+-rw-r--r--   0        0        0      875 2024-02-17 22:43:56.173003 fluiddyn-0.6.3/fluiddyn/clusters/azzurra.py
+-rw-r--r--   0        0        0      995 2024-02-17 22:43:56.173003 fluiddyn-0.6.3/fluiddyn/clusters/ciment.py
+-rw-r--r--   0        0        0     1274 2024-02-17 22:43:56.173003 fluiddyn-0.6.3/fluiddyn/clusters/cines.py
+-rw-r--r--   0        0        0      834 2024-02-17 22:43:56.173003 fluiddyn-0.6.3/fluiddyn/clusters/idris.py
+-rw-r--r--   0        0        0     1045 2024-03-26 14:13:20.514828 fluiddyn-0.6.3/fluiddyn/clusters/legi.py
+-rw-r--r--   0        0        0      716 2024-02-17 22:43:56.177003 fluiddyn-0.6.3/fluiddyn/clusters/licallo.py
+-rw-r--r--   0        0        0     7952 2024-04-22 14:36:43.455957 fluiddyn-0.6.3/fluiddyn/clusters/local.py
+-rw-r--r--   0        0        0     9091 2024-04-22 14:36:43.455957 fluiddyn-0.6.3/fluiddyn/clusters/oar.py
+-rw-r--r--   0        0        0     8357 2024-04-22 14:36:43.455957 fluiddyn-0.6.3/fluiddyn/clusters/pbs.py
+-rw-r--r--   0        0        0    16500 2024-04-22 14:36:43.455957 fluiddyn-0.6.3/fluiddyn/clusters/slurm.py
+-rw-r--r--   0        0        0     4009 2024-04-22 14:36:43.459957 fluiddyn-0.6.3/fluiddyn/clusters/snic.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.181003 fluiddyn-0.6.3/fluiddyn/clusters/test/__init__.py
+-rw-r--r--   0        0        0     1026 2024-02-17 22:43:56.181003 fluiddyn-0.6.3/fluiddyn/clusters/test/test_local.py
+-rw-r--r--   0        0        0     4354 2024-04-22 14:36:43.459957 fluiddyn-0.6.3/fluiddyn/clusters/test/test_oar.py
+-rw-r--r--   0        0        0     2797 2024-02-17 22:43:56.185003 fluiddyn-0.6.3/fluiddyn/clusters/test/test_pbs.py
+-rw-r--r--   0        0        0     3479 2024-02-17 22:43:56.185003 fluiddyn-0.6.3/fluiddyn/clusters/test/test_slurm_snic.py
+-rw-r--r--   0        0        0     2115 2024-03-20 15:24:08.394333 fluiddyn-0.6.3/fluiddyn/io/__init__.py
+-rw-r--r--   0        0        0     5138 2024-02-17 22:43:56.185003 fluiddyn-0.6.3/fluiddyn/io/binary.py
+-rw-r--r--   0        0        0     3822 2024-02-17 22:43:56.185003 fluiddyn-0.6.3/fluiddyn/io/dantec.py
+-rw-r--r--   0        0        0     3779 2024-02-17 22:43:56.189003 fluiddyn-0.6.3/fluiddyn/io/davis.py
+-rw-r--r--   0        0        0    19554 2024-02-17 22:43:56.189003 fluiddyn-0.6.3/fluiddyn/io/digiflow.py
+-rw-r--r--   0        0        0     4052 2024-02-17 22:43:56.189003 fluiddyn-0.6.3/fluiddyn/io/dump.py
+-rw-r--r--   0        0        0     4758 2024-02-17 22:43:56.189003 fluiddyn-0.6.3/fluiddyn/io/hdf5.py
+-rw-r--r--   0        0        0     5683 2024-02-17 22:43:56.189003 fluiddyn-0.6.3/fluiddyn/io/image.py
+-rw-r--r--   0        0        0     1378 2024-02-17 22:43:56.193003 fluiddyn-0.6.3/fluiddyn/io/in_py.py
+-rw-r--r--   0        0        0    13149 2024-02-17 22:43:56.193003 fluiddyn-0.6.3/fluiddyn/io/multitiff.py
+-rw-r--r--   0        0        0     1762 2024-02-17 22:43:56.193003 fluiddyn-0.6.3/fluiddyn/io/mycsv.py
+-rw-r--r--   0        0        0    12165 2024-02-17 22:43:56.193003 fluiddyn-0.6.3/fluiddyn/io/ns3d.py
+-rw-r--r--   0        0        0     2539 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/query.py
+-rw-r--r--   0        0        0     2809 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/rdvision.py
+-rw-r--r--   0        0        0     1142 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/redirect_stdout.py
+-rw-r--r--   0        0        0      620 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/tee.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/test/__init__.py
+-rw-r--r--   0        0        0     2460 2024-02-17 22:43:56.197003 fluiddyn-0.6.3/fluiddyn/io/test/ns3d_files/PV.t=0000.000
+-rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28
+-rw-r--r--   0        0        0      284 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/ns3d_files/forcing_2D_info.in_L=30x30_nh=48_expLO_b=1.8_Ti=7.0_nbgene=4_d=4_T=28_little-endian
+-rw-r--r--   0        0        0      429 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/rdvision_files/Dalsa2.seq
+-rw-r--r--   0        0        0       48 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/rdvision_files/Dalsa2.sqb
+-rw-r--r--   0        0        0     1267 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/rdvision_files/Dalsa2.xml
+-rw-r--r--   0        0        0     1137 2024-02-17 22:43:56.201003 fluiddyn-0.6.3/fluiddyn/io/test/test_binary.py
+-rw-r--r--   0        0        0      525 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_dantec.py
+-rw-r--r--   0        0        0      660 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_digiflow.py
+-rw-r--r--   0        0        0     1456 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_dump.py
+-rw-r--r--   0        0        0     2123 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_hdf5.py
+-rw-r--r--   0        0        0     2909 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_image.py
+-rw-r--r--   0        0        0     1224 2024-02-17 22:43:56.205003 fluiddyn-0.6.3/fluiddyn/io/test/test_in_py.py
+-rw-r--r--   0        0        0     2411 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_multitiff.py
+-rw-r--r--   0        0        0      746 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_mycsv.py
+-rw-r--r--   0        0        0     1855 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_ns3d.py
+-rw-r--r--   0        0        0     1232 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_query.py
+-rw-r--r--   0        0        0     1027 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_rdvision.py
+-rw-r--r--   0        0        0      739 2024-02-17 22:43:56.209003 fluiddyn-0.6.3/fluiddyn/io/test/test_tee.py
+-rw-r--r--   0        0        0     1095 2024-02-17 22:43:56.213003 fluiddyn-0.6.3/fluiddyn/io/test/test_txt.py
+-rw-r--r--   0        0        0     3342 2024-02-17 22:43:56.213003 fluiddyn-0.6.3/fluiddyn/io/txt.py
+-rw-r--r--   0        0        0      533 2024-02-17 22:43:56.213003 fluiddyn-0.6.3/fluiddyn/output/__init__.py
+-rw-r--r--   0        0        0     6098 2024-02-17 22:43:56.213003 fluiddyn-0.6.3/fluiddyn/output/colorchart.py
+-rw-r--r--   0        0        0     5323 2024-02-17 22:43:56.213003 fluiddyn-0.6.3/fluiddyn/output/figs.py
+-rw-r--r--   0        0        0     1177 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/output/rcparams.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/output/test/__init__.py
+-rw-r--r--   0        0        0      307 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/output/test/test_colorchart.py
+-rw-r--r--   0        0        0     1052 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/output/test/test_figs.py
+-rw-r--r--   0        0        0      721 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/output/util.py
+-rw-r--r--   0        0        0     1135 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/util/__init__.py
+-rw-r--r--   0        0        0      133 2024-02-17 22:43:56.217003 fluiddyn-0.6.3/fluiddyn/util/compat.py
+-rw-r--r--   0        0        0      304 2024-02-17 22:43:56.221003 fluiddyn-0.6.3/fluiddyn/util/constants.py
+-rw-r--r--   0        0        0     1068 2024-02-17 22:43:56.221003 fluiddyn-0.6.3/fluiddyn/util/daemons.py
+-rw-r--r--   0        0        0    15219 2024-02-17 22:43:56.221003 fluiddyn-0.6.3/fluiddyn/util/info.py
+-rw-r--r--   0        0        0     4282 2024-02-17 22:43:56.221003 fluiddyn-0.6.3/fluiddyn/util/logger.py
+-rw-r--r--   0        0        0     3513 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/mail.py
+-rw-r--r--   0        0        0     1971 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/__init__.py
+-rw-r--r--   0        0        0     5860 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/cleanmat.py
+-rw-r--r--   0        0        0     3238 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/mat2wrongpy.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/test/__init__.py
+-rw-r--r--   0        0        0      810 2024-02-17 22:43:56.225003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/test/courant.m
+-rw-r--r--   0        0        0      519 2024-02-17 22:43:56.229003 fluiddyn-0.6.3/fluiddyn/util/matlab2py/test/test_matlab2py.py
+-rw-r--r--   0        0        0     3780 2024-02-17 22:43:56.229003 fluiddyn-0.6.3/fluiddyn/util/mpi.py
+-rw-r--r--   0        0        0    23542 2024-02-17 22:43:56.229003 fluiddyn-0.6.3/fluiddyn/util/numpy_distutils_cpuinfo.py
+-rw-r--r--   0        0        0      964 2024-02-17 22:43:56.229003 fluiddyn-0.6.3/fluiddyn/util/opencv.py
+-rw-r--r--   0        0        0    23221 2024-02-17 22:43:56.233003 fluiddyn-0.6.3/fluiddyn/util/paramcontainer.py
+-rw-r--r--   0        0        0     7281 2024-02-17 22:43:56.233003 fluiddyn-0.6.3/fluiddyn/util/paramcontainer_gui.py
+-rw-r--r--   0        0        0    32191 2024-04-18 21:06:11.348621 fluiddyn-0.6.3/fluiddyn/util/serieofarrays.py
+-rw-r--r--   0        0        0     4724 2024-02-17 22:43:56.233003 fluiddyn-0.6.3/fluiddyn/util/terminal_colors.py
+-rw-r--r--   0        0        0        0 2024-02-17 22:43:56.233003 fluiddyn-0.6.3/fluiddyn/util/test/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-17 22:43:56.237002 fluiddyn-0.6.3/fluiddyn/util/test/file.xml
+-rw-r--r--   0        0        0      808 2024-02-17 22:43:56.237002 fluiddyn-0.6.3/fluiddyn/util/test/test_daemons.py
+-rw-r--r--   0        0        0      974 2024-02-17 22:43:56.237002 fluiddyn-0.6.3/fluiddyn/util/test/test_info.py
+-rw-r--r--   0        0        0      942 2024-02-17 22:43:56.237002 fluiddyn-0.6.3/fluiddyn/util/test/test_logger.py
+-rw-r--r--   0        0        0     2194 2024-02-17 22:43:56.237002 fluiddyn-0.6.3/fluiddyn/util/test/test_mpi.py
+-rw-r--r--   0        0        0     4725 2024-02-17 22:43:56.241002 fluiddyn-0.6.3/fluiddyn/util/test/test_paramcontainer.py
+-rw-r--r--   0        0        0     7447 2024-04-18 21:06:11.348621 fluiddyn-0.6.3/fluiddyn/util/test/test_serieofarrays.py
+-rw-r--r--   0        0        0      797 2024-02-17 22:43:56.241002 fluiddyn-0.6.3/fluiddyn/util/test/test_timer.py
+-rw-r--r--   0        0        0     2734 2024-02-17 22:43:56.241002 fluiddyn-0.6.3/fluiddyn/util/test/test_util.py
+-rw-r--r--   0        0        0     4522 2024-02-17 22:43:56.241002 fluiddyn-0.6.3/fluiddyn/util/timer.py
+-rw-r--r--   0        0        0     1200 2024-02-17 22:43:56.241002 fluiddyn-0.6.3/fluiddyn/util/userconfig.py
+-rw-r--r--   0        0        0     9277 2024-02-17 22:43:56.245002 fluiddyn-0.6.3/fluiddyn/util/util.py
+-rw-r--r--   0        0        0     4443 2024-02-17 22:43:56.245002 fluiddyn-0.6.3/fluiddyn/util/xmltotext.py
+-rw-r--r--   0        0        0     4238 2024-04-22 14:36:54.172024 fluiddyn-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     7114 1970-01-01 00:00:00.000000 fluiddyn-0.6.3/PKG-INFO
```

### Comparing `fluiddyn-0.6.2/LICENSE.txt` & `fluiddyn-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/README.rst` & `fluiddyn-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddoc/__init__.py` & `fluiddyn-0.6.3/fluiddoc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddoc/fluiddocset.py` & `fluiddyn-0.6.3/fluiddoc/fluiddocset.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddoc/fluidnbstripout.py` & `fluiddyn-0.6.3/fluiddoc/fluidnbstripout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddoc/ipynb_maker.py` & `fluiddyn-0.6.3/fluiddoc/ipynb_maker.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddoc/mathmacro.py` & `fluiddyn-0.6.3/fluiddoc/mathmacro.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/__init__.py` & `fluiddyn-0.6.3/fluiddyn/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/easypyfft.py` & `fluiddyn-0.6.3/fluiddyn/calcul/easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/setofvariables.py` & `fluiddyn-0.6.3/fluiddyn/calcul/setofvariables.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/signal.py` & `fluiddyn-0.6.3/fluiddyn/calcul/signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/sphericalharmo.py` & `fluiddyn-0.6.3/fluiddyn/calcul/sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/test/test_easypyfft.py` & `fluiddyn-0.6.3/fluiddyn/calcul/test/test_easypyfft.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/test/test_signal.py` & `fluiddyn-0.6.3/fluiddyn/calcul/test/test_signal.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/calcul/test/test_sphericalharmo.py` & `fluiddyn-0.6.3/fluiddyn/calcul/test/test_sphericalharmo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/azzurra.py` & `fluiddyn-0.6.3/fluiddyn/clusters/azzurra.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/ciment.py` & `fluiddyn-0.6.3/fluiddyn/clusters/ciment.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/cines.py` & `fluiddyn-0.6.3/fluiddyn/clusters/cines.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/idris.py` & `fluiddyn-0.6.3/fluiddyn/clusters/idris.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/legi.py` & `fluiddyn-0.6.3/fluiddyn/clusters/legi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/licallo.py` & `fluiddyn-0.6.3/fluiddyn/clusters/licallo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/local.py` & `fluiddyn-0.6.3/fluiddyn/clusters/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,21 +51,17 @@
     name_cluster = gethostname()
     nb_cores_per_node = psutil.cpu_count()
     cmd_run = "mpirun"
     cmd_launch = "nohup"
     max_walltime = "30-00:00:00"
 
     def __init__(self):
-        self.commands_setting_env = []
         self.commands_unsetting_env = []
         virtualenv = os.getenv("VIRTUAL_ENV")
         if virtualenv is not None:
-            self.commands_setting_env.append(
-                "source " + virtualenv + "/bin/activate"
-            )
             self.commands_unsetting_env.append("deactivate")
 
     def submit_script(self, path, *args, **kwargs):
         """Submit a script. See `submit_command` for all possible arguments"""
         path = os.path.expandvars(path)
         script = path.split()[0]
         if not os.path.exists(script):
@@ -203,15 +199,15 @@
         txt += self._log_job(
             nb_mpi_processes,
             path_launching_script,
             logfile_stdout,
             command,
             "LOCAL_JOB.md",
         )
-        txt += "\n".join(self.commands_setting_env) + "\n\n"
+        txt += "\n".join(self.get_commands_setting_env()) + "\n\n"
 
         if omp_num_threads is not None:
             txt += f"export OMP_NUM_THREADS={omp_num_threads}\n\n"
 
         cmd = command
         if nb_mpi_processes is not None and nb_mpi_processes > 1:
             cmd = f"{self.cmd_run} -n {nb_mpi_processes} {cmd}"
```

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/oar.py` & `fluiddyn-0.6.3/fluiddyn/clusters/oar.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,31 +90,20 @@
 Useful commands
 ---------------
 oarsub -S script.sh
 oarstat -u
 oardel $JOB_ID
 oarsub -C $JOB_ID"""
 
-    def __init__(self):
-        self.commands_setting_env = [
-            "source /etc/profile",
-            "module load python/{}.{}.{}".format(
-                version.major, version.minor, version.micro
-            ),
-            "source /home/users/$USER/opt/mypy{}.{}/bin/activate".format(
-                version.major, version.minor
-            ),
-        ]
-
     def check_oar(self):
         """check if this script is run on a frontal with oar installed"""
         try:
             subprocess.check_call(["oarsub", "--version"], stdout=subprocess.PIPE)
-        except OSError:
-            raise OSError("oar does not seem to be installed.")
+        except OSError as error:
+            raise OSError("oar does not seem to be installed.") from error
 
     def submit_script(
         self,
         path,
         name_run="fluiddyn",
         nb_nodes=1,
         nb_cores_per_node=None,
@@ -203,16 +192,16 @@
             omp_num_threads=omp_num_threads,
             network_address=network_address,
             run_with_exec=run_with_exec,
             resource_conditions=resource_conditions,
             use_oar_envsh=use_oar_envsh,
         )
 
-        with open(path_launching_script, "w") as f:
-            f.write(txt)
+        with open(path_launching_script, "w", encoding="utf-8") as file:
+            file.write(txt)
 
         os.chmod(
             path_launching_script, stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR
         )
 
         launching_command = "oarsub"
 
@@ -276,15 +265,15 @@
 
         txt += "/nodes={}/core={},walltime={}\n\n".format(
             nb_nodes, nb_cores_per_node, walltime
         )
 
         txt += 'echo "hostname: "$HOSTNAME\n\n'
 
-        txt += "\n".join(self.commands_setting_env) + "\n\n"
+        txt += "\n".join(self.get_commands_setting_env()) + "\n\n"
 
         if omp_num_threads is not None:
             txt += f"export OMP_NUM_THREADS={omp_num_threads}\n\n"
 
         if use_oar_envsh is None:
             use_oar_envsh = nb_mpi_processes is not None and nb_nodes > 1
```

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/pbs.py` & `fluiddyn-0.6.3/fluiddyn/clusters/pbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             nb_cores,
             path_launching_script,
             logfile_stdout,
             command,
             "PBS_JOB.md",
         )
 
-        txt += "\n".join(self.commands_setting_env) + "\n\n"
+        txt += "\n".join(self.get_commands_setting_env()) + "\n\n"
 
         if omp_num_threads is not None:
             txt += f"export OMP_NUM_THREADS={omp_num_threads}\n\n"
 
         if is_resume_script:
             jobid = dependencies[0]
             main_logfile = f"PBS.{name_run}.{jobid}.stdout"
```

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/slurm.py` & `fluiddyn-0.6.3/fluiddyn/clusters/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     dependency = None  #: Dependency option
     mem = None  #: Minimum amount of real memory allocation for the job
     account = None  #: Name of the project for jobs' submission (mandatory on some clusters)
     exclusive = False  #: Reserve nodes when submitting jobs
 
     def __init__(self):
         self.check_slurm()
-        self.commands_setting_env = []
         self.commands_unsetting_env = []
 
     def check_slurm(self):
         """Check if this script is run on a frontal with slurm installed."""
         try:
             subprocess.check_call(["sbatch", "--version"], stdout=PIPE)
             slurm_installed = True
@@ -361,18 +360,18 @@
 
         if mem is not None:
             txt += f"#SBATCH --mem={mem}\n"
 
         if account is not None:
             txt += f"#SBATCH --account={account}\n"
 
-        if exclusive == True:
-            txt += f"#SBATCH --exclusive\n"
+        if exclusive:
+            txt += "#SBATCH --exclusive\n"
 
-        txt += "\n".join(self.commands_setting_env) + "\n\n"
+        txt += "\n".join(self.get_commands_setting_env()) + "\n\n"
 
         txt += 'echo "hostname: "$HOSTNAME\n\n'
         txt += self._log_job(
             nb_cores,
             path_launching_script,
             logfile_stdout,
             command,
```

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/snic.py` & `fluiddyn-0.6.3/fluiddyn/clusters/snic.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,27 +82,24 @@
     cmd_run = "mpprun"
     cmd_run_interactive = "mpirun"
     max_walltime = "7-00:00:00"
 
     def __init__(self):
         super().__init__()
         self.check_name_cluster("SNIC_RESOURCE")
-        self.commands_setting_env = []
 
         # NOTE: Typically load the following modules and save them
         # Python/3.6.3-anaconda-5.0.1-nsc1 intel/2018a
         # buildtool-easybuild/3.5.3-nsc17d8ce4 buildenv-intel/2018a-eb
         # FFTW/3.3.6-nsc1
-        self.commands_setting_env.extend(
-            [
-                "ml restore",
-                f"source activate {_venv}",
-                'export LD_LIBRARY_PATH="$LD_LIBRARY_PATH":"$LIBRARY_PATH"',
-            ]
-        )
+        self.commands_setting_env = [
+            "ml restore",
+            f"source activate {_venv}",
+            'export LD_LIBRARY_PATH="$LD_LIBRARY_PATH":"$LIBRARY_PATH"',
+        ]
 
         self.commands_unsetting_env = ["source deactivate"]
 
 
 class Abisko(SNIC):
     name_cluster = "abisko"
     nb_cores_per_node = 24
@@ -129,27 +126,24 @@
     nb_cores_per_node = 28
     cmd_run_interactive = "mpirun"
     max_walltime = "7-00:00:00"
 
     def __init__(self):
         super().__init__()
         self.check_name_cluster("SNIC_RESOURCE")
-        self.commands_setting_env = ["source /etc/profile"]
-
-        self.commands_setting_env.extend(
-            [
-                "module load foss/2017a",
-                # also loads GCC/6.3.0-2.27  OpenMPI/2.0.2
-                # OpenBLAS/0.2.19-LAPACK-3.7.0 FFTW/3.3.6
-                "module rm FFTW/3.3.6",
-                "module load HDF5/1.10.0-patch1",
-                "module load Python/3.6.1",
-                f"source {_venv}/bin/activate",
-            ]
-        )
+        self.commands_setting_env = [
+            "source /etc/profile",
+            "module load foss/2017a",
+            # also loads GCC/6.3.0-2.27  OpenMPI/2.0.2
+            # OpenBLAS/0.2.19-LAPACK-3.7.0 FFTW/3.3.6
+            "module rm FFTW/3.3.6",
+            "module load HDF5/1.10.0-patch1",
+            "module load Python/3.6.1",
+            f"source {_venv}/bin/activate",
+        ]
 
         self.commands_unsetting_env = []
 
 
 _host = getenv("SNIC_RESOURCE")
 if _host == "beskow":
     ClusterSNIC = Beskow
```

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/test/test_local.py` & `fluiddyn-0.6.3/fluiddyn/clusters/test/test_local.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/test/test_pbs.py` & `fluiddyn-0.6.3/fluiddyn/clusters/test/test_pbs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/clusters/test/test_slurm_snic.py` & `fluiddyn-0.6.3/fluiddyn/clusters/test/test_slurm_snic.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/__init__.py` & `fluiddyn-0.6.3/fluiddyn/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/binary.py` & `fluiddyn-0.6.3/fluiddyn/io/binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/dantec.py` & `fluiddyn-0.6.3/fluiddyn/io/dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/davis.py` & `fluiddyn-0.6.3/fluiddyn/io/davis.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/digiflow.py` & `fluiddyn-0.6.3/fluiddyn/io/digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/dump.py` & `fluiddyn-0.6.3/fluiddyn/io/dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/hdf5.py` & `fluiddyn-0.6.3/fluiddyn/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/image.py` & `fluiddyn-0.6.3/fluiddyn/io/image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/in_py.py` & `fluiddyn-0.6.3/fluiddyn/io/in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/multitiff.py` & `fluiddyn-0.6.3/fluiddyn/io/multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/mycsv.py` & `fluiddyn-0.6.3/fluiddyn/io/mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/ns3d.py` & `fluiddyn-0.6.3/fluiddyn/io/ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/query.py` & `fluiddyn-0.6.3/fluiddyn/io/query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/rdvision.py` & `fluiddyn-0.6.3/fluiddyn/io/rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/redirect_stdout.py` & `fluiddyn-0.6.3/fluiddyn/io/redirect_stdout.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/tee.py` & `fluiddyn-0.6.3/fluiddyn/io/tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/ns3d_files/PV.t=0000.000` & `fluiddyn-0.6.3/fluiddyn/io/test/ns3d_files/PV.t=0000.000`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/rdvision_files/Dalsa2.xml` & `fluiddyn-0.6.3/fluiddyn/io/test/rdvision_files/Dalsa2.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_binary.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_binary.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_dantec.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_dantec.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_digiflow.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_digiflow.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_dump.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_dump.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_hdf5.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_image.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_image.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_in_py.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_in_py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_multitiff.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_multitiff.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_mycsv.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_mycsv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_ns3d.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_ns3d.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_query.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_query.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_rdvision.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_rdvision.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_tee.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_tee.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/test/test_txt.py` & `fluiddyn-0.6.3/fluiddyn/io/test/test_txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/io/txt.py` & `fluiddyn-0.6.3/fluiddyn/io/txt.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/__init__.py` & `fluiddyn-0.6.3/fluiddyn/output/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/colorchart.py` & `fluiddyn-0.6.3/fluiddyn/output/colorchart.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/figs.py` & `fluiddyn-0.6.3/fluiddyn/output/figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/rcparams.py` & `fluiddyn-0.6.3/fluiddyn/output/rcparams.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/test/test_figs.py` & `fluiddyn-0.6.3/fluiddyn/output/test/test_figs.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/output/util.py` & `fluiddyn-0.6.3/fluiddyn/output/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/__init__.py` & `fluiddyn-0.6.3/fluiddyn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/daemons.py` & `fluiddyn-0.6.3/fluiddyn/util/daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/info.py` & `fluiddyn-0.6.3/fluiddyn/util/info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/logger.py` & `fluiddyn-0.6.3/fluiddyn/util/logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/mail.py` & `fluiddyn-0.6.3/fluiddyn/util/mail.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/matlab2py/__init__.py` & `fluiddyn-0.6.3/fluiddyn/util/matlab2py/__init__.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/matlab2py/cleanmat.py` & `fluiddyn-0.6.3/fluiddyn/util/matlab2py/cleanmat.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/matlab2py/mat2wrongpy.py` & `fluiddyn-0.6.3/fluiddyn/util/matlab2py/mat2wrongpy.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/courant.m` & `fluiddyn-0.6.3/fluiddyn/util/matlab2py/test/courant.m`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/matlab2py/test/test_matlab2py.py` & `fluiddyn-0.6.3/fluiddyn/util/matlab2py/test/test_matlab2py.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/mpi.py` & `fluiddyn-0.6.3/fluiddyn/util/mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/numpy_distutils_cpuinfo.py` & `fluiddyn-0.6.3/fluiddyn/util/numpy_distutils_cpuinfo.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/opencv.py` & `fluiddyn-0.6.3/fluiddyn/util/opencv.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/paramcontainer.py` & `fluiddyn-0.6.3/fluiddyn/util/paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/paramcontainer_gui.py` & `fluiddyn-0.6.3/fluiddyn/util/paramcontainer_gui.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/serieofarrays.py` & `fluiddyn-0.6.3/fluiddyn/util/serieofarrays.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/terminal_colors.py` & `fluiddyn-0.6.3/fluiddyn/util/terminal_colors.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/file.xml` & `fluiddyn-0.6.3/fluiddyn/util/test/file.xml`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_daemons.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_daemons.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_info.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_info.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_logger.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_mpi.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_mpi.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_paramcontainer.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_paramcontainer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_serieofarrays.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_serieofarrays.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_timer.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/test/test_util.py` & `fluiddyn-0.6.3/fluiddyn/util/test/test_util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/timer.py` & `fluiddyn-0.6.3/fluiddyn/util/timer.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/userconfig.py` & `fluiddyn-0.6.3/fluiddyn/util/userconfig.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/util.py` & `fluiddyn-0.6.3/fluiddyn/util/util.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/fluiddyn/util/xmltotext.py` & `fluiddyn-0.6.3/fluiddyn/util/xmltotext.py`

 * *Files identical despite different names*

### Comparing `fluiddyn-0.6.2/pyproject.toml` & `fluiddyn-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "fluiddyn"
-version = "0.6.2"
+version = "0.6.3"
 description = "Framework for studying fluid dynamics."
 keywords = [
     "Fluid dynamics",
     "research",
 ]
 authors = [
     { name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr" },
```

### Comparing `fluiddyn-0.6.2/PKG-INFO` & `fluiddyn-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluiddyn
-Version: 0.6.2
+Version: 0.6.3
 Summary: Framework for studying fluid dynamics.
 Keywords: Fluid dynamics,research
 Home-page: https://foss.heptapod.net/fluiddyn/fluiddyn
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL-B License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

