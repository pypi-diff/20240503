# Comparing `tmp/pyiron_atomistics-0.5.3.tar.gz` & `tmp/pyiron_atomistics-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_atomistics-0.5.3.tar", last modified: Fri Apr 26 15:54:44 2024, max compression
+gzip compressed data, was "pyiron_atomistics-0.5.4.tar", last modified: Fri May  3 14:35:53 2024, max compression
```

## Comparing `pyiron_atomistics-0.5.3.tar` & `pyiron_atomistics-0.5.4.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.779926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42892 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.779926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/elasticmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)   121522 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/atomsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/has_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyxtal.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/structurestorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/data/
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/data/periodic_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/bader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/quasi_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41067 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41928 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83168 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/input_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    16340 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)    51126 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/sxphonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   106070 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/metadyn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (127)    45802 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/outcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-26 15:54:39.000000 pyiron_atomistics-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.150296 pyiron_atomistics-0.5.4/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.150296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.150296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.150296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42892 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.154296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/elasticmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.154296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121522 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyxtal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/data/periodic_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.158296 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.162296 pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.162296 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.162296 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41067 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41928 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.166296 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83168 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/input_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16340 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.166296 pyiron_atomistics-0.5.4/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.166296 pyiron_atomistics-0.5.4/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.166296 pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51140 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106070 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/metadyn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45802 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-03 14:35:53.000000 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-03 14:35:53.000000 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:35:53.000000 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-03 14:35:53.000000 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 14:35:53.000000 pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-03 14:35:49.000000 pyiron_atomistics-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:35:53.170296 pyiron_atomistics-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 14:33:52.000000 pyiron_atomistics-0.5.4/tests/test_toolkit.py
```

### Comparing `pyiron_atomistics-0.5.3/LICENSE` & `pyiron_atomistics-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/PKG-INFO` & `pyiron_atomistics-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.5.3
+Version: 0.5.4
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -56,15 +56,15 @@
 Requires-Dist: matplotlib<=3.8.4,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.41.2,>=0.37.0
 Requires-Dist: numpy<=1.26.4,>=1.26.0
 Requires-Dist: pandas<=2.2.2,>=2.0.3
 Requires-Dist: phonopy<=2.22.1,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
-Requires-Dist: pyiron_base<=0.8.2,>=0.7.7
+Requires-Dist: pyiron_base<=0.8.3,>=0.7.7
 Requires-Dist: pylammpsmpi<=0.2.18,>=0.2.7
 Requires-Dist: scipy<=1.13.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.2,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
 Requires-Dist: spglib<=2.4.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.22,>=0.0.19
```

### Comparing `pyiron_atomistics-0.5.3/README.rst` & `pyiron_atomistics-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/__init__.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/_tests.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/elasticmatrix.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/elasticmatrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,18 +73,15 @@
         (
             elastic_matrix,
             self._data["A2"],
             self._data["strain_energy"],
             self._data["e0"],
         ) = analyse_structures_helper(
             output_dict=output_dict,
-            Lag_strain_list=self._data["Lag_strain_list"],
-            epss=self._data["epss"],
-            v0=self._data["v0"],
-            LC=self._data["LC"],
+            sym_dict=self._data,
             fit_order=self.fit_order,
             zero_strain_job_name=self.zero_strain_job_name,
         )
         elastic = ElasticProperties(elastic_matrix=elastic_matrix)
         self._data.update(
             {
                 "C": elastic.elastic_matrix(),
```

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/structure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/atomsk.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/atomsk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/compound.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/compound.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/materialsproject.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factories/materialsproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/has_structure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/has_structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyxtal.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/pyxtal.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/structurestorage.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/structure/structurestorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/job.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/calphy/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/data/periodic_table.csv` & `pyiron_atomistics-0.5.4/pyiron_atomistics/data/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/bader.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/bader.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/generic.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/dos.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/dos.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/electronic.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/dft/waves/electronic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/gpaw.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/quasi_newton.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/base.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/control.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/interactive.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/lammps.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/output.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/potential.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/structure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/units.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/lammps/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/project.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/base.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/input_writer.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/input_writer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/interactive.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             self._logger.debug("restarting; interactive run - start ...")
             self._interactive_pipe_write("run restart")
             self.interactive_fetch()
 
     def _output_interactive_to_generic(self):
         with self.project_hdf5.open("output") as h5:
             if "interactive" in h5.list_groups():
-                for key in ["positions", "cells", "indices", "cells", "forces"]:
+                for key in ["positions", "indices", "cells", "forces"]:
                     self.output.generic[key] = h5["interactive/" + key]
                 if "atom_spin_constraints" in h5["interactive"].list_nodes():
                     self.output.generic.dft.atom_spin_constraints = h5[
                         "interactive/atom_spin_constraints"
                     ]
                 self.output.generic.to_hdf(hdf=self.project_hdf5)
```

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/output_parser.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/potential.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/sphinx.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/structure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/util.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/table/datamining.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/table/funct.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/testing/executable.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/testing/randomatomistic.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/testing/randomatomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Args:
         basis (pyiron_atomistics.structure.atoms.Atoms): Atomistic structure object
 
     Returns:
         pyiron_atomistics.structure.atoms.Atoms: Atomistic structure object with half of the atoms fixed
     """
-    basis.add_tag(selective_dynamics=None)
+    basis.add_tag(selective_dynamics=[True, True, True])
     _, _, z = basis.scaled_pos_xyz()
     for selector, ind in zip(z < 0.5, range(len(basis))):
         if selector:
             basis.selective_dynamics[ind] = [True, True, True]
         else:
             basis.selective_dynamics[ind] = [False, False, False]
     return basis
```

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/toolkit.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/base.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/interactive.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/metadyn.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/oszicar.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/outcar.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/outcar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/report.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/parser/report.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/potential.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/procar.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/structure.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasp.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasprun.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vaspsol.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron_atomistics-0.5.4/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.5.3
+Version: 0.5.4
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -56,15 +56,15 @@
 Requires-Dist: matplotlib<=3.8.4,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.41.2,>=0.37.0
 Requires-Dist: numpy<=1.26.4,>=1.26.0
 Requires-Dist: pandas<=2.2.2,>=2.0.3
 Requires-Dist: phonopy<=2.22.1,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
-Requires-Dist: pyiron_base<=0.8.2,>=0.7.7
+Requires-Dist: pyiron_base<=0.8.3,>=0.7.7
 Requires-Dist: pylammpsmpi<=0.2.18,>=0.2.7
 Requires-Dist: scipy<=1.13.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.2,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
 Requires-Dist: spglib<=2.4.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.22,>=0.0.19
```

### Comparing `pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron_atomistics-0.5.4/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/pyproject.toml` & `pyiron_atomistics-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "matplotlib>=3.5.3,<=3.8.4",
     "mendeleev>=0.12.0,<=0.15.0",
     "mp-api>=0.37.0,<=0.41.2",
     "numpy>=1.26.0,<=1.26.4",
     "pandas>=2.0.3,<=2.2.2",
     "phonopy>=2.20.0,<=2.22.1",
     "pint>=0.18,<=0.23",
-    "pyiron_base>=0.7.7,<=0.8.2",
+    "pyiron_base>=0.7.7,<=0.8.3",
     "pylammpsmpi>=0.2.7,<=0.2.18",
     "scipy>=1.11.1,<=1.13.0",
     "scikit-learn>=1.2.1,<=1.4.2",
     "seekpath>=1.9.5,<=2.1.0",
     "spglib>=2.0.2,<=2.4.0",
     "structuretoolkit>=0.0.19,<=0.0.22",
 ]
```

### Comparing `pyiron_atomistics-0.5.3/tests/test_project.py` & `pyiron_atomistics-0.5.4/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.3/tests/test_toolkit.py` & `pyiron_atomistics-0.5.4/tests/test_toolkit.py`

 * *Files identical despite different names*

